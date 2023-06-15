# Comparing `tmp/localstack-core-2.1.1.dev20230615143138.tar.gz` & `tmp/localstack-core-2.1.1.dev20230615150942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.1.1.dev20230615143138.tar", last modified: Thu Jun 15 14:31:46 2023, max compression
+gzip compressed data, was "localstack-core-2.1.1.dev20230615150942.tar", last modified: Thu Jun 15 15:09:54 2023, max compression
```

## Comparing `localstack-core-2.1.1.dev20230615143138.tar` & `localstack-core-2.1.1.dev20230615150942.tar`

### file list

```diff
@@ -1,851 +1,851 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.164439 localstack-core-2.1.1.dev20230615143138/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-15 14:31:46.164439 localstack-core-2.1.1.dev20230615143138/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.012442 localstack-core-2.1.1.dev20230615143138/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-15 14:31:38.000000 localstack-core-2.1.1.dev20230615143138/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    86119 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.016442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   755634 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48826 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71940 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38087 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.020442 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.024442 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.024442 localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.024442 localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.024442 localstack-core-2.1.1.dev20230615143138/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.024442 localstack-core-2.1.1.dev20230615143138/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.024442 localstack-core-2.1.1.dev20230615143138/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.024442 localstack-core-2.1.1.dev20230615143138/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.028442 localstack-core-2.1.1.dev20230615143138/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.028442 localstack-core-2.1.1.dev20230615143138/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.028442 localstack-core-2.1.1.dev20230615143138/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.028442 localstack-core-2.1.1.dev20230615143138/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.028442 localstack-core-2.1.1.dev20230615143138/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.028442 localstack-core-2.1.1.dev20230615143138/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.032442 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    61609 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14059 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.032442 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.076441 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.080441 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17831 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19612 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.080441 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.080441 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.080441 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    64921 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.084441 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33075 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20991 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2489 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7518 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2190 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21966 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2991 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3188 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9202 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28763 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3327 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2640 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13881 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6708 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8735 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5112 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3927 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5754 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3768 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5732 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.084441 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.084441 localstack-core-2.1.1.dev20230615143138/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.084441 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.088441 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.088441 localstack-core-2.1.1.dev20230615143138/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.088441 localstack-core-2.1.1.dev20230615143138/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.088441 localstack-core-2.1.1.dev20230615143138/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23351 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.088441 localstack-core-2.1.1.dev20230615143138/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.088441 localstack-core-2.1.1.dev20230615143138/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19690 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/iam/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.088441 localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.092440 localstack-core-2.1.1.dev20230615143138/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35960 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52700 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.092440 localstack-core-2.1.1.dev20230615143138/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.092440 localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.092440 localstack-core-2.1.1.dev20230615143138/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.092440 localstack-core-2.1.1.dev20230615143138/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.092440 localstack-core-2.1.1.dev20230615143138/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.092440 localstack-core-2.1.1.dev20230615143138/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.092440 localstack-core-2.1.1.dev20230615143138/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.092440 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43470 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.096440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.100440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.100440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.104440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.104440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.104440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.104440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.104440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.104440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.104440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.104440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.116440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.116440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.116440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.116440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.116440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.120440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.120440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.120440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.120440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.120440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.120440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.120440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.124440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.124440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.124440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.124440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.124440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.124440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.128440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.132440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.132440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.132440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.132440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.132440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.132440 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.140439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.140439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.140439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.140439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.140439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.140439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.144439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.144439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.144439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.144439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.144439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.144439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.144439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.152439 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.152439 localstack-core-2.1.1.dev20230615143138/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.152439 localstack-core-2.1.1.dev20230615143138/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.152439 localstack-core-2.1.1.dev20230615143138/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.152439 localstack-core-2.1.1.dev20230615143138/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.152439 localstack-core-2.1.1.dev20230615143138/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.152439 localstack-core-2.1.1.dev20230615143138/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.152439 localstack-core-2.1.1.dev20230615143138/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.152439 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69752 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.152439 localstack-core-2.1.1.dev20230615143138/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.156439 localstack-core-2.1.1.dev20230615143138/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.160439 localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.160439 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.160439 localstack-core-2.1.1.dev20230615143138/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.160439 localstack-core-2.1.1.dev20230615143138/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45834 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.164439 localstack-core-2.1.1.dev20230615143138/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.164439 localstack-core-2.1.1.dev20230615143138/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23579 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:31:46.164439 localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-15 14:31:45.000000 localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37808 2023-06-15 14:31:45.000000 localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-15 14:31:45.000000 localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-15 14:31:45.000000 localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-15 14:31:42.000000 localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-15 14:31:42.000000 localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2855 2023-06-15 14:31:45.000000 localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-15 14:31:45.000000 localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3186 2023-06-15 14:31:46.164439 localstack-core-2.1.1.dev20230615143138/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-15 12:07:39.000000 localstack-core-2.1.1.dev20230615143138/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:54.243802 localstack-core-2.1.1.dev20230615150942/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-15 15:09:54.243802 localstack-core-2.1.1.dev20230615150942/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.795829 localstack-core-2.1.1.dev20230615150942/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.795829 localstack-core-2.1.1.dev20230615150942/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-15 15:09:42.000000 localstack-core-2.1.1.dev20230615150942/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    86119 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   755634 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48826 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71940 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38087 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.799829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.803829 localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.807829 localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.807829 localstack-core-2.1.1.dev20230615150942/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.807829 localstack-core-2.1.1.dev20230615150942/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:49.807829 localstack-core-2.1.1.dev20230615150942/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.279826 localstack-core-2.1.1.dev20230615150942/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.279826 localstack-core-2.1.1.dev20230615150942/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.279826 localstack-core-2.1.1.dev20230615150942/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.279826 localstack-core-2.1.1.dev20230615150942/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.283826 localstack-core-2.1.1.dev20230615150942/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.283826 localstack-core-2.1.1.dev20230615150942/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.283826 localstack-core-2.1.1.dev20230615150942/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.283826 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    61609 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14059 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.287826 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.287826 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.287826 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17831 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19612 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.287826 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.359825 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.359825 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65114 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.359825 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33005 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20991 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2489 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7434 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2190 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21942 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2949 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3188 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9196 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28231 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3327 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4787 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2640 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13639 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6708 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8678 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5134 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3927 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5754 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3768 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5732 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.359825 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.359825 localstack-core-2.1.1.dev20230615150942/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.359825 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:50.363825 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:51.951816 localstack-core-2.1.1.dev20230615150942/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:51.951816 localstack-core-2.1.1.dev20230615150942/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:51.951816 localstack-core-2.1.1.dev20230615150942/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23351 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:51.951816 localstack-core-2.1.1.dev20230615150942/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:51.951816 localstack-core-2.1.1.dev20230615150942/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19690 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/iam/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:51.955816 localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:51.955816 localstack-core-2.1.1.dev20230615150942/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35960 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52700 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:51.955816 localstack-core-2.1.1.dev20230615150942/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.095815 localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.095815 localstack-core-2.1.1.dev20230615150942/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.095815 localstack-core-2.1.1.dev20230615150942/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.095815 localstack-core-2.1.1.dev20230615150942/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.095815 localstack-core-2.1.1.dev20230615150942/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.095815 localstack-core-2.1.1.dev20230615150942/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43470 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.099815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.103815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.103815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.103815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.103815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.103815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.103815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.103815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.103815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.103815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.103815 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.759811 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.759811 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.803810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.803810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.803810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.803810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.803810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.803810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.803810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.803810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.807811 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.807811 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.807811 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.807811 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.807811 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.807811 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.867810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.867810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.867810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.867810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.867810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.867810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:52.871810 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.591806 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.591806 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.591806 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.591806 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.591806 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.591806 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.679805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.679805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.679805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.679805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.679805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.683805 localstack-core-2.1.1.dev20230615150942/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.687805 localstack-core-2.1.1.dev20230615150942/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.687805 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69752 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:53.687805 localstack-core-2.1.1.dev20230615150942/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:54.239802 localstack-core-2.1.1.dev20230615150942/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:54.239802 localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:54.239802 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:54.239802 localstack-core-2.1.1.dev20230615150942/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:54.239802 localstack-core-2.1.1.dev20230615150942/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45834 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:54.239802 localstack-core-2.1.1.dev20230615150942/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:54.239802 localstack-core-2.1.1.dev20230615150942/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23579 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 15:09:54.243802 localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-15 15:09:49.000000 localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37808 2023-06-15 15:09:49.000000 localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-15 15:09:49.000000 localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-15 15:09:49.000000 localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-15 15:09:46.000000 localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-15 15:09:46.000000 localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2855 2023-06-15 15:09:49.000000 localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-15 15:09:49.000000 localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3186 2023-06-15 15:09:54.243802 localstack-core-2.1.1.dev20230615150942/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-15 14:34:16.000000 localstack-core-2.1.1.dev20230615150942/setup.py
```

### Comparing `localstack-core-2.1.1.dev20230615143138/LICENSE.txt` & `localstack-core-2.1.1.dev20230615150942/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/Makefile` & `localstack-core-2.1.1.dev20230615150942/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/PKG-INFO` & `localstack-core-2.1.1.dev20230615150942/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230615143138
+Version: 2.1.1.dev20230615150942
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230615143138/README.md` & `localstack-core-2.1.1.dev20230615150942/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/bin/localstack` & `localstack-core-2.1.1.dev20230615150942/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/bin/localstack-supervisor` & `localstack-core-2.1.1.dev20230615150942/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/accounts.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/acm/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/config/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/core.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/es/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/events/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/iam/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/kms/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/logs/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/route53/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/s3/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/ses/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/sns/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/sts/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/support/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/swf/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/app.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/chain.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/client.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/connect.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/forwarder.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/gateway.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/analytics.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/auth.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/codec.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/cors.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/fallback.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/internal.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/legacy.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/logging.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/proxy.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/region.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/routes.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/service.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/mocking.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/op_router.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/parser.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/serializer.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/service_router.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/protocol/validate.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/proxy.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/scaffold.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/asgi.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/edge.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/hypercorn.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/werkzeug.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/serving/wsgi.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/skeleton.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/spec-patches.json` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/spec.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/aws/trace.py` & `localstack-core-2.1.1.dev20230615150942/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/cli/localstack.py` & `localstack-core-2.1.1.dev20230615150942/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/cli/lpm.py` & `localstack-core-2.1.1.dev20230615150942/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/cli/plugin.py` & `localstack-core-2.1.1.dev20230615150942/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/cli/plugins.py` & `localstack-core-2.1.1.dev20230615150942/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/cli/profiles.py` & `localstack-core-2.1.1.dev20230615150942/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/config.py` & `localstack-core-2.1.1.dev20230615150942/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/constants.py` & `localstack-core-2.1.1.dev20230615150942/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/deprecations.py` & `localstack-core-2.1.1.dev20230615150942/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/extensions/api/aws.py` & `localstack-core-2.1.1.dev20230615150942/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/extensions/api/extension.py` & `localstack-core-2.1.1.dev20230615150942/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/http/adapters.py` & `localstack-core-2.1.1.dev20230615150942/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/http/asgi.py` & `localstack-core-2.1.1.dev20230615150942/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/http/client.py` & `localstack-core-2.1.1.dev20230615150942/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/http/dispatcher.py` & `localstack-core-2.1.1.dev20230615150942/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/http/hypercorn.py` & `localstack-core-2.1.1.dev20230615150942/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/http/proxy.py` & `localstack-core-2.1.1.dev20230615150942/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/http/request.py` & `localstack-core-2.1.1.dev20230615150942/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/http/resource.py` & `localstack-core-2.1.1.dev20230615150942/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/http/response.py` & `localstack-core-2.1.1.dev20230615150942/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/http/router.py` & `localstack-core-2.1.1.dev20230615150942/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/logging/format.py` & `localstack-core-2.1.1.dev20230615150942/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/logging/setup.py` & `localstack-core-2.1.1.dev20230615150942/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/packages/__init__.py` & `localstack-core-2.1.1.dev20230615150942/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/packages/api.py` & `localstack-core-2.1.1.dev20230615150942/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/packages/core.py` & `localstack-core-2.1.1.dev20230615150942/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/packages/debugpy.py` & `localstack-core-2.1.1.dev20230615150942/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/packages/ffmpeg.py` & `localstack-core-2.1.1.dev20230615150942/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/packages/terraform.py` & `localstack-core-2.1.1.dev20230615150942/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/plugins.py` & `localstack-core-2.1.1.dev20230615150942/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/runtime/analytics.py` & `localstack-core-2.1.1.dev20230615150942/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/runtime/hooks.py` & `localstack-core-2.1.1.dev20230615150942/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/runtime/init.py` & `localstack-core-2.1.1.dev20230615150942/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/runtime/main.py` & `localstack-core-2.1.1.dev20230615150942/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/runtime/shutdown.py` & `localstack-core-2.1.1.dev20230615150942/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/acm/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/context.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/helpers.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/integration.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/invocations.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/patches.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/router_asf.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/apigateway/templates.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/api_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/hooks.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/packages.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/plugins.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/deploy.html` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import base64
+import inspect
 import json
 import logging
 import re
 import traceback
 from typing import Any, Callable, Optional, Type, TypedDict
 
 import botocore
@@ -68,20 +69,18 @@
 # - resource_id
 ResourceProp = str | Callable[[dict, str, dict, str], dict]
 ResourceDefinition = dict[str, ResourceProp]
 
 
 class FuncDetailsValue(TypedDict):
     # Callable here takes the arguments:
-    # - resource_id
-    # - resources
-    # - resource_type
-    # - func
+    # - logical_resource_id
+    # - resource
     # - stack_name
-    function: str | Callable[[str, list[dict], str, Any, str], Any]
+    function: str | Callable[[str, dict, str], Any]
     """Either an api method to call directly with `parameters` or a callable to directly invoke"""
     # Callable here takes the arguments:
     # - resource_props
     # - stack_name
     # - resources
     # - resource_id
     parameters: Optional[ResourceDefinition | Callable[[dict, str, list[dict], str], dict]]
@@ -168,15 +167,14 @@
         return None
 
 
 # TODO(ds): remove next
 def retrieve_resource_details(
     resource_id, resource_status, resources: dict[str, Type[GenericBaseModel]], stack_name
 ):
-
     resource = resources.get(resource_id)
     resource_id = resource_status.get("PhysicalResourceId") or resource_id
     if not resource:
         resource = {}
     resource_type = get_resource_type(resource)
     resource_props = resource.get("Properties")
     if resource_props is None:
@@ -808,15 +806,19 @@
     func_details = func_details if isinstance(func_details, list) else [func_details]
     results = []
     for func in func_details:
         result = None
         executed = False
         # TODO(srw) 3 - callable function
         if callable(func.get("function")):
-            result = func["function"](resource_id, resources, resource_type, func, stack_name)
+            sig = inspect.signature(func["function"])
+            if "logical_resource_id" in sig.parameters:
+                result = func["function"](resource_id, resources[resource_id], stack_name)
+            else:
+                result = func["function"](resource_id, resources, resource_type, func, stack_name)
             results.append(result)
             executed = True
 
         elif not executed and get_client(resource):
             # get the service client to invoke
             client = get_client(resource)
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/apigateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,16 @@
 
     @classmethod
     def get_deploy_templates(cls):
         def _api_id(params, resources, resource_id, **kwargs):
             resource = cls(resources[resource_id])
             return resource.physical_resource_id
 
-        def _create(resource_id, resources, resource_type, func, stack_name):
+        def _create(logical_resource_id: str, resource: dict, stack_name: str):
             client = connect_to().apigateway
-            resource = resources[resource_id]
             props = resource["Properties"]
 
             kwargs = select_attributes(
                 props,
                 [
                     "Name",
                     "Description",
@@ -147,15 +146,15 @@
             kwargs = keys_to_lower(kwargs, skip_children_of=["policy"])
             kwargs["tags"] = {tag["key"]: tag["value"] for tag in kwargs.get("tags", [])}
 
             cfn_client = connect_to().cloudformation
             stack_id = cfn_client.describe_stacks(StackName=stack_name)["Stacks"][0]["StackId"]
             kwargs["tags"].update(
                 {
-                    "aws:cloudformation:logical-id": resource_id,
+                    "aws:cloudformation:logical-id": logical_resource_id,
                     "aws:cloudformation:stack-name": stack_name,
                     "aws:cloudformation:stack-id": stack_id,
                 }
             )
             if isinstance(kwargs.get("policy"), dict):
                 kwargs["policy"] = json.dumps(kwargs["policy"])
 
@@ -397,27 +396,26 @@
                 "requestValidatorId",
             ]
             result = select_attributes(result, param_names)
             result["requestModels"] = result.get("requestModels") or {}
             result["requestParameters"] = result.get("requestParameters") or {}
             return result
 
-        def _subresources(resource_id, resources, resource_type, func, stack_name):
+        def _subresources(logical_resource_id: str, resource: dict, stack_name: str):
             apigateway = connect_to().apigateway
-            resource = cls(resources[resource_id])
-            props = resource.props
+            provider = cls(resource)
+            props = provider.props
 
             integration = props.get("Integration")
             if integration:
                 api_id = props["RestApiId"]
                 res_id = props["ResourceId"]
 
                 kwargs = keys_to_lower(integration)
                 if uri := integration.get("Uri"):
-
                     # Moto has a validate method on Uri for integration_type "HTTP" | "HTTP_PROXY" that does not accept
                     # Uri value without path, we need to add path ("/") if not exists
                     if integration.get("Type") in ["HTTP", "HTTP_PROXY"]:
                         rs = urlparse(uri)
                         if not rs.path:
                             uri = "{}/".format(uri)
 
@@ -769,17 +767,17 @@
             [self.props.get("BasePath")] if self.props.get("BasePath") else [None, "", "(none)"]
         )
 
         return next(iter(res for res in resources if res.get("basePath") in comparable))
 
     @classmethod
     def get_deploy_templates(cls):
-        def _create_base_path_mapping(resource_id, resources, *args, **kwargs):
-            resource = cls(resources[resource_id])
-            props = resource.props
+        def _create_base_path_mapping(logical_resource_id: str, resource: dict, stack_name: str):
+            provider = cls(resource)
+            props = provider.props
 
             kwargs = {
                 "domainName": props.get("DomainName"),
                 "restApiId": props.get("RestApiId"),
                 **({"basePath": props.get("BasePath")} if props.get("BasePath") else {}),
                 **({"stage": props.get("Stage")} if props.get("Stage") else {}),
             }
@@ -857,26 +855,25 @@
         if not self.physical_resource_id:
             return None
         client = connect_to().apigateway
         return client.get_account()
 
     @classmethod
     def get_deploy_templates(cls):
-        def _create(resource_id, resources, *args, **kwargs):
-            resource = resources[resource_id]
+        def _create(logical_resource_id: str, resource: dict, stack_name: str):
             props = cls(resource).props
 
             role_arn = props["CloudWatchRoleArn"]
 
             connect_to().apigateway.update_account(
                 patchOperations=[{"op": "replace", "path": "/cloudwatchRoleArn", "value": role_arn}]
             )
 
             resource["PhysicalResourceId"] = generate_default_name(
-                args[2], resource["LogicalResourceId"]
+                stack_name, resource["LogicalResourceId"]
             )
 
         def _delete(*_, **__):
             # note: deletion of accounts is currently a no-op
             pass
 
         return {"create": {"function": _create}, "delete": {"function": _delete}}
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/cloudformation.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,22 +97,20 @@
         return "AWS::CloudFormation::Macro"
 
     def fetch_state(self, stack_name, resources):
         return get_cloudformation_store().macros.get(self.props.get("Name"))
 
     @classmethod
     def get_deploy_templates(cls):
-        def _store_macro(resource_id, resources, resource_type, func, stack_name):
-            resource = resources[resource_id]
+        def _store_macro(logical_resource_id: str, resource: dict, stack_name: str):
             properties = resource["Properties"]
             name = properties["Name"]
             get_cloudformation_store().macros[name] = properties
 
-        def _delete_macro(resource_id, resources, resource_type, func, stack_name):
-            resource = resources[resource_id]
+        def _delete_macro(logical_resource_id: str, resource: dict, stack_name: str):
             properties = resource["Properties"]
             name = properties["Name"]
             get_cloudformation_store().macros.pop(name)
 
         def _set_physical_resource_id(
             result: dict, resource_id: str, resources: dict, resource_type: str
         ):
@@ -149,15 +147,15 @@
 
     def fetch_state(self, stack_name, resources):
         if self.physical_resource_id is not None:
             return {"deployed": True}
 
     @staticmethod
     def get_deploy_templates():
-        def _create(resource_id, resources, resource_type, func, stack_name) -> dict:
+        def _create(logical_resource_id: str, resource: dict, stack_name: str) -> dict:
             # no resources to create as such, but the physical resource id needs the stack name
             return {"stack_name": stack_name}
 
         def _set_physical_resource_id(result, resource_id, resources, resource_type):
             waitcondition_url = generate_waitcondition_url(
                 stack_name=result["stack_name"],
             )
@@ -181,15 +179,15 @@
 
     def fetch_state(self, stack_name, resources):
         if self.physical_resource_id is not None:
             return {"deployed": True}
 
     @staticmethod
     def get_deploy_templates():
-        def _create(resource_id, resources, resource_type, func, stack_name) -> dict:
+        def _create(logical_resource_id: str, resource: dict, stack_name: str) -> dict:
             # no resources to create, but the physical resource id requires the stack name
             return {"stack_name": stack_name}
 
         def _set_physical_resource_id(result, resource_id, resources, resource_type):
             stack_arn = arns.cloudformation_stack_arn(result["stack_name"])
             resources[resource_id][
                 "PhysicalResourceId"
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,18 +193,18 @@
         attachments = gateway.get("Attachments") or gateway.get("VpcAttachments") or []
         result = [a for a in attachments if a.get("State") in ("attached", "available")]
         if result:
             return gateway
 
     @classmethod
     def get_deploy_templates(cls):
-        def _attach_gateway(resource_id, resources, *args, **kwargs):
+        def _attach_gateway(logical_resource_id: str, resource: dict, stack_name: str):
             client = aws_stack.connect_to_service("ec2")
-            resource = cls(resources[resource_id])
-            props = resource.props
+            resource_provider = cls(resource)
+            props = resource_provider.props
             igw_id = props.get("InternetGatewayId")
             vpngw_id = props.get("VpnGatewayId")
             vpc_id = props.get("VpcId")
             if igw_id:
                 return client.attach_internet_gateway(VpcId=vpc_id, InternetGatewayId=igw_id)
             elif vpngw_id:
                 return client.attach_vpn_gateway(VpcId=vpc_id, VpnGatewayId=vpngw_id)
@@ -277,15 +277,15 @@
 
 
 class EC2Subnet(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::Subnet"
 
-    def fetch_state(self, stack_name, resources):
+    def fetch_state(self, stack_name, resources) -> dict:
         if not self.physical_resource_id:
             return None
         client = aws_stack.connect_to_service("ec2")
         props = self.props
         filters = [
             {"Name": "cidr-block", "Values": [props["CidrBlock"]]},
             {"Name": "vpc-id", "Values": [props["VpcId"]]},
@@ -296,30 +296,29 @@
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "SubnetId":
             return self.props.get("SubnetId")
         return super(EC2Subnet, self).get_cfn_attribute(attribute_name)
 
     @classmethod
     def get_deploy_templates(cls):
-        def _post_create(resource_id, resources, resource_type, func, stack_name):
+        def _post_create(logical_resource_id: str, resource: dict, stack_name: str):
             client = aws_stack.connect_to_service("ec2")
-            resource = cls(resources[resource_id])
-            props = resource.props
+            resource_provider = cls(resource)
+            props = resource_provider.props
 
             bool_attrs = [
                 "AssignIpv6AddressOnCreation",
                 "EnableDns64",
                 "MapPublicIpOnLaunch",
             ]
             custom_attrs = bool_attrs + ["PrivateDnsNameOptionsOnLaunch"]
             if not any(attr in props for attr in custom_attrs):
                 return
 
-            state = resource.fetch_state(stack_name, resources)
-            subnet_id = state.get("SubnetId")
+            subnet_id = props.get("SubnetId")
 
             # update boolean attributes
             for attr in bool_attrs:
                 if attr in props:
                     kwargs = {attr: {"Value": str_to_bool(props[attr])}}
                     client.modify_subnet_attribute(SubnetId=subnet_id, **kwargs)
 
@@ -400,16 +399,16 @@
                 )
             return acls[0]["NetworkAclId"]
         else:
             return super(EC2VPC, self).get_cfn_attribute(attribute_name)
 
     @classmethod
     def get_deploy_templates(cls):
-        def _pre_delete(resource_id, resources, *args, **kwargs):
-            res = cls(resources[resource_id])
+        def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
+            res = cls(resource)
             vpc_id = res.state.get("VpcId")
             if vpc_id:
                 ec2_client = aws_stack.connect_to_service("ec2")
                 resp = ec2_client.describe_route_tables(
                     Filters=[
                         {"Name": "vpc-id", "Values": [vpc_id]},
                         {"Name": "association.main", "Values": ["false"]},
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/ecr.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,22 +41,21 @@
                 "imageScanningConfiguration": {"scanOnPush": True},
             }
         else:
             return None
 
     @staticmethod
     def get_deploy_templates():
-        def _create_repo(resource_id, resources, resource_type, func, stack_name):
-            resource = resources[resource_id]
+        def _create_repo(logical_resource_id: str, resource: dict, stack_name: str):
             default_repos_per_stack[stack_name] = resource["Properties"]["RepositoryName"]
             LOG.warning(
                 "Creating a Mock ECR Repository for CloudFormation. This is only intended to be used for allowing a successful CDK bootstrap and does not provision any underlying ECR repository."
             )
 
-        def _delete_repo(resource_id, resources, resource_type, func, stack_name):
+        def _delete_repo(logical_resource_id: str, resource: dict, stack_name: str):
             if default_repos_per_stack.get(stack_name):
                 del default_repos_per_stack[stack_name]
 
         def _set_physical_resource_id(result, resource_id, resources, resource_type):
             resource = resources[resource_id]
             repo_name = resource["Properties"]["RepositoryName"]
             resource["PhysicalResourceId"] = arns.get_ecr_repository_arn(repo_name)
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/events.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 
+from botocore.exceptions import ClientError
+
 from localstack.services.cloudformation.deployment_utils import (
     generate_default_name,
     select_parameters,
 )
 from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.utils import common
 from localstack.utils.aws import arns, aws_stack
@@ -128,28 +130,26 @@
 
             pattern = result.get("EventPattern")
             if isinstance(pattern, dict):
                 wrapped = common.recurse_object(pattern, wrap_in_lists)
                 result["EventPattern"] = json.dumps(wrapped)
             return result
 
-        def _delete_rule(resource_id, resources, *args, **kwargs):
+        def _delete_rule(logical_resource_id: str, resource: dict, stack_name: str):
             events = aws_stack.connect_to_service("events")
-            resource = resources[resource_id]
             props = resource["Properties"]
             rule_name = props["Name"]
             targets = events.list_targets_by_rule(Rule=rule_name)["Targets"]
             target_ids = [tgt["Id"] for tgt in targets]
             if targets:
                 events.remove_targets(Rule=rule_name, Ids=target_ids, Force=True)
             events.delete_rule(Name=rule_name)
 
-        def _put_targets(resource_id, resources, *args, **kwargs):
+        def _put_targets(logical_resource_id: str, resource: dict, stack_name: str):
             events = aws_stack.connect_to_service("events")
-            resource = resources[resource_id]
             props = resource["Properties"]
             rule_name = props["Name"]
             event_bus_name = props.get("EventBusName")
             targets = props.get("Targets") or []
             if len(targets) > 0 and event_bus_name:
                 events.put_targets(Rule=rule_name, EventBusName=event_bus_name, Targets=targets)
             elif len(targets) > 0:
@@ -176,17 +176,16 @@
 class EventBusPolicy(GenericBaseModel):
     @classmethod
     def cloudformation_type(cls):
         return "AWS::Events::EventBusPolicy"
 
     @classmethod
     def get_deploy_templates(cls):
-        def _create(resource_id, resources, resource_type, func, stack_name):
+        def _create(logical_resource_id: str, resource: dict, stack_name: str):
             events = aws_stack.connect_to_service("events")
-            resource = resources[resource_id]
             props = resource["Properties"]
 
             resource["PhysicalResourceId"] = f"EventBusPolicy-{short_uid()}"
 
             statement_id = props["StatementId"]  # required
             event_bus_name = props.get("EventBusName")  # optional
             statement = props.get(
@@ -213,27 +212,29 @@
                     StatementId=statement_id,
                     Action=props["Action"],
                     Principal=props["Principal"],
                     **optional_event_bus_name,
                     **optional_condition,
                 )
 
-        def _delete(resource_id, resources, resource_type, func, stack_name):
+        def _delete(logical_resource_id: str, resource: dict, stack_name: str):
             events = aws_stack.connect_to_service("events")
-            resource = resources[resource_id]
             props = resource["Properties"]
             statement_id = props["StatementId"]
             event_bus_name = props.get("EventBusName")
             optional_event_bus_name = {"EventBusName": event_bus_name} if event_bus_name else {}
             try:
                 events.remove_permission(
                     StatementId=statement_id, RemoveAllPermissions=False, **optional_event_bus_name
                 )
             except Exception as err:
-                if err.response["Error"]["Code"] == "ResourceNotFoundException":
+                if (
+                    isinstance(err, ClientError)
+                    and err.response["Error"]["Code"] == "ResourceNotFoundException"
+                ):
                     pass  # expected behavior ("parent" resource event bus already deleted)
                 else:
                     raise err
 
         return {
             "create": {"function": _create},
             "delete": {"function": _delete},
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/iam.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,17 +38,16 @@
         if not role_name:
             resource["Properties"]["ManagedPolicyName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def get_deploy_templates(cls):
-        def _create(resource_id, resources, resource_type, func, stack_name, *args, **kwargs):
+        def _create(logical_resource_id: str, resource: dict, stack_name: str):
             iam = aws_stack.connect_to_service("iam")
-            resource = resources[resource_id]
             props = resource["Properties"]
 
             policy_doc = json.dumps(remove_none_values(props["PolicyDocument"]))
             policy = iam.create_policy(
                 PolicyName=props["ManagedPolicyName"], PolicyDocument=policy_doc
             )
             policy_arn = policy["Policy"]["Arn"]
@@ -83,17 +82,16 @@
         if not role_name:
             resource["Properties"]["UserName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
     def get_deploy_templates():
-        def _post_create(resource_id, resources, resource_type, func, stack_name):
+        def _post_create(logical_resource_id: str, resource: dict, stack_name: str):
             client = aws_stack.connect_to_service("iam")
-            resource = resources[resource_id]
             props = resource["Properties"]
             username = props["UserName"]
 
             for group in props.get("Groups", []):
                 client.add_user_to_group(UserName=username, GroupName=group)
             for managed_policy in props.get("ManagedPolicyArns", []):
                 client.attach_user_policy(UserName=username, PolicyArn=managed_policy)
@@ -108,17 +106,16 @@
             if login_profile:
                 client.create_login_profile(
                     UserName=username,
                     Password=login_profile.get("Password"),
                     PasswordResetRequired=login_profile.get("PasswordResetRequired"),
                 )
 
-        def _pre_delete(resource_id, resources, resource_type, func, stack_name):
+        def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
             client = aws_stack.connect_to_service("iam")
-            resource = resources[resource_id]
             props = resource["Properties"]
             user_name = props["UserName"]
 
             for managed_policy in props.get("ManagedPolicyArns", []):
                 client.detach_user_policy(UserName=user_name, PolicyArn=managed_policy)
 
             for inline_policy in props.get("Policies", []):
@@ -187,17 +184,16 @@
 
         aws_stack.connect_to_service("iam").update_access_key(
             UserName=user_name, AccessKeyId=access_key_id, Status=status
         )
 
     @staticmethod
     def get_deploy_templates():
-        def _delete(resource_id, resources, resource_type, func, stack_name):
+        def _delete(logical_resource_id: str, resource: dict, stack_name: str):
             iam_client = aws_stack.connect_to_service("iam")
-            resource = resources[resource_id]
             props = resource["Properties"]
             user_name = props["UserName"]
             access_key_id = resource["PhysicalResourceId"]
 
             try:
                 iam_client.delete_access_key(UserName=user_name, AccessKeyId=access_key_id)
             except ClientError as err:
@@ -252,24 +248,22 @@
             props_policy = props.get("AssumeRolePolicyDocument")
             name_changed = props.get("RoleName") != _states.get("RoleName")
             policy_changed = props_policy and props_policy != _states.get(
                 "AssumeRolePolicyDocument", ""
             )
             if name_changed or policy_changed:
                 resource_id = new_resource.get("LogicalResourceId")
-                dummy_resources = {
-                    resource_id: {"Properties": {"RoleName": _states.get("RoleName")}}
-                }
-                IAMRole._pre_delete(resource_id, dummy_resources, None, None, None)
+                dummy_resource = {"Properties": {"RoleName": _states.get("RoleName")}}
+                IAMRole._pre_delete(resource_id, dummy_resource, stack_name)
                 client.delete_role(RoleName=_states.get("RoleName"))
                 role = client.create_role(
                     RoleName=props.get("RoleName"),
                     AssumeRolePolicyDocument=json.dumps(props_policy),
                 )
-                IAMRole._post_create(resource_id, resources, None, None, None)
+                IAMRole._post_create(resource_id, resources[resource_id], stack_name)
                 return role["Role"]
 
         return client.update_role(
             RoleName=props.get("RoleName"), Description=props.get("Description") or ""
         )
 
     @staticmethod
@@ -277,19 +271,18 @@
         role_name = resource.get("Properties", {}).get("RoleName")
         if not role_name:
             resource["Properties"]["RoleName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
-    def _post_create(cls, resource_id, resources, resource_type, func, stack_name):
+    def _post_create(cls, logical_resource_id: str, resource: dict, stack_name: str):
         """attaches managed policies from the template to the role"""
 
         iam = aws_stack.connect_to_service("iam")
-        resource = resources[resource_id]
         props = resource["Properties"]
         role_name = props["RoleName"]
 
         # attach managed policies
         policy_arns = props.get("ManagedPolicyArns", [])
         for arn in policy_arns:
             iam.attach_role_policy(RoleName=role_name, PolicyArn=arn)
@@ -323,18 +316,17 @@
             iam.put_role_policy(
                 RoleName=props["RoleName"],
                 PolicyName=pol_name,
                 PolicyDocument=doc,
             )
 
     @staticmethod
-    def _pre_delete(resource_id, resources, resource_type, func, stack_name):
+    def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
         """detach managed policies from role before deleting"""
         iam_client = aws_stack.connect_to_service("iam")
-        resource = resources[resource_id]
         props = resource["Properties"]
         role_name = props["RoleName"]
 
         try:
             # TODO: this should probably only remove the policies that are specified in the stack (verify with AWS)
             # detach managed policies
             for policy in iam_client.list_attached_role_policies(RoleName=role_name).get(
@@ -470,17 +462,17 @@
         def _store_physical_id(result, resource_id, resources, resource_type):
             resource = resources[resource_id]
             # the physical resource ID here has a bit of a weird format
             # e.g. 'stack-fnSe-1OKWZIBB89193' where fnSe are the first 4 characters of the LogicalResourceId (or name?)
             suffix = "".join(random.choices(string.ascii_uppercase + string.digits, k=13))
             resource["PhysicalResourceId"] = f"stack-{resource.get('PolicyName', '')[:4]}-{suffix}"
 
-        def _create(resource_id, resources, resource_type, func, stack_name, *args, **kwargs):
+        def _create(logical_resource_id: str, resource: dict, stack_name: str):
             iam = aws_stack.connect_to_service("iam")
-            props = resources[resource_id]["Properties"]
+            props = resource["Properties"]
             policy_doc = json.dumps(remove_none_values(props["PolicyDocument"]))
             policy_name = props["PolicyName"]
             for role in props.get("Roles", []):
                 iam.put_role_policy(
                     RoleName=role, PolicyName=policy_name, PolicyDocument=policy_doc
                 )
             for user in props.get("Users", []):
@@ -562,30 +554,28 @@
         if not role_name:
             resource["Properties"]["InstanceProfileName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
     def get_deploy_templates():
-        def _add_roles(resource_id, resources, resource_type, func, stack_name):
+        def _add_roles(logical_resource_id: str, resource: dict, stack_name: str):
             client = aws_stack.connect_to_service("iam")
-            resource = resources[resource_id]
             props = resource["Properties"]
             roles = props.get("Roles")
             if roles:
                 if len(roles) > 1:
                     raise Exception("Roles has too many elements. The limit is 1.")
                 client.add_role_to_instance_profile(
                     InstanceProfileName=props["InstanceProfileName"],
                     RoleName=roles[0],
                 )
 
-        def _pre_delete(resource_id, resources, resource_type, func, stack_name):
+        def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
             iam_client = aws_stack.connect_to_service("iam")
-            resource = resources[resource_id]
             props = resource["Properties"]
             roles = props.get("Roles")
             assert len(roles) == 1
             try:
                 iam_client.remove_role_from_instance_profile(
                     InstanceProfileName=props["InstanceProfileName"],
                     RoleName=roles[0],
@@ -636,34 +626,32 @@
             GroupName=props.get("GroupName"),
             NewPath=props.get("NewPath") or "",
             NewGroupName=props.get("NewGroupName") or "",
         )
 
     @staticmethod
     def get_deploy_templates():
-        def _post_create(resource_id, resources, resource_type, func, stack_name):
+        def _post_create(logical_resource_id: str, resource: dict, stack_name: str):
             client = aws_stack.connect_to_service("iam")
-            resource = resources[resource_id]
             props = resource["Properties"]
             group_name = props["GroupName"]
 
             for managed_policy in props.get("ManagedPolicyArns", []):
                 client.attach_group_policy(GroupName=group_name, PolicyArn=managed_policy)
 
             for inline_policy in props.get("Policies", []):
                 doc = json.dumps(inline_policy.get("PolicyDocument"))
                 client.put_group_policy(
                     GroupName=group_name,
                     PolicyName=inline_policy.get("PolicyName"),
                     PolicyDocument=doc,
                 )
 
-        def _pre_delete(resource_id, resources, resource_type, func, stack_name):
+        def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
             client = aws_stack.connect_to_service("iam")
-            resource = resources[resource_id]
             props = resource["Properties"]
             group_name = props["GroupName"]
 
             for managed_policy in props.get("ManagedPolicyArns", []):
                 client.detach_group_policy(GroupName=group_name, PolicyArn=managed_policy)
 
             for inline_policy in props.get("Policies", []):
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/kms.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,18 @@
                     break
         if not physical_res_id:
             return
         return client.describe_key(KeyId=physical_res_id)
 
     @classmethod
     def get_deploy_templates(cls):
-        def _create(resource_id, resources, resource_type, func, stack_name):
+        def _create(logical_resource_id: str, resource: dict, stack_name: str):
             kms_client = aws_stack.connect_to_service("kms")
-            resource = cls(resources[resource_id])
-            props = resource.props
+            resource_provider = cls(resource)
+            props = resource_provider.props
             params = {}
             if props.get("KeyPolicy"):
                 params["Policy"] = json.dumps(props["KeyPolicy"])
 
             if props.get("Tags"):
                 params["Tags"] = [
                     {"TagKey": tag["Key"], "TagValue": tag["Value"]}
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/s3.py`

 * *Files 5% similar despite different names*

```diff
@@ -168,83 +168,79 @@
 
         def _set_physical_resource_id(
             result: dict, resource_id: str, resources: dict, resource_type: str
         ):
             resource = resources[resource_id]
             resource["PhysicalResourceId"] = resource["Properties"]["BucketName"]
 
-        def _pre_delete(resource_id, resources, resource_type, func, stack_name):
+        def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
             s3 = aws_stack.connect_to_service("s3")
-            resource = resources[resource_id]
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             try:
                 s3.delete_bucket_policy(Bucket=bucket_name)
             except Exception:
                 pass
             s3_listener.remove_bucket_notification(resource["PhysicalResourceId"])
             # TODO: divergence from how AWS deals with bucket deletes (should throw an error)
             try:
                 delete_all_s3_objects(bucket_name)
             except Exception as e:
                 if "NoSuchBucket" not in str(e):
                     raise
 
-        def _add_bucket_tags(resource_id, resources, resource_type, func, stack_name):
+        def _add_bucket_tags(logical_resource_id: str, resource: dict, stack_name: str):
             s3 = aws_stack.connect_to_service("s3")
-            resource = resources[resource_id]
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             tags = props.get("Tags", [])
             if len(tags) > 0:
                 s3.put_bucket_tagging(Bucket=bucket_name, Tagging={"TagSet": tags})
 
-        def _put_bucket_versioning(resource_id, resources, resource_type, func, stack_name):
+        def _put_bucket_versioning(logical_resource_id: str, resource: dict, stack_name: str):
             s3_client = aws_stack.connect_to_service("s3")
-            resource = resources[resource_id]
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             versioning_config = props.get("VersioningConfiguration")
             if versioning_config:
                 s3_client.put_bucket_versioning(
                     Bucket=bucket_name,
                     VersioningConfiguration={
                         "Status": versioning_config.get("Status", "Disabled"),
                     },
                 )
 
-        def _put_bucket_cors_configuration(resource_id, resources, resource_type, func, stack_name):
+        def _put_bucket_cors_configuration(
+            logical_resource_id: str, resource: dict, stack_name: str
+        ):
             s3_client = aws_stack.connect_to_service("s3")
-            resource = resources[resource_id]
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             cors_configuration = transform_cfn_cors(props.get("CorsConfiguration"))
             if cors_configuration:
                 s3_client.put_bucket_cors(
                     Bucket=bucket_name,
                     CORSConfiguration=cors_configuration,
                 )
 
         def _put_bucket_website_configuration(
-            resource_id, resources, resource_type, func, stack_name
+            logical_resource_id: str, resource: dict, stack_name: str
         ):
             s3_client = aws_stack.connect_to_service("s3")
-            resource = resources[resource_id]
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             website_config = transform_website_configuration(props.get("WebsiteConfiguration"))
             if website_config:
                 s3_client.put_bucket_website(
                     Bucket=bucket_name,
                     WebsiteConfiguration=website_config,
                 )
 
-        def _create_bucket(resource_id, resources, resource_type, func, stack_name):
+        def _create_bucket(logical_resource_id: str, resource: dict, stack_name: str):
             s3_client = aws_stack.connect_to_service("s3")
-            resource = resources[resource_id]
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             try:
                 s3_client.head_bucket(Bucket=bucket_name)
             except ClientError as e:
                 if e.response["Error"]["Message"] == "Not Found":
                     bucket_name = props.get("BucketName")
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/sns.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,21 +68,21 @@
             while key and key != "":
                 rs = sns_client.list_topics(NextToken=key)
                 topics.extend(rs.get("Topics", []))
                 key = rs.get("NextToken")
 
             return topics
 
-        def _add_topics(resource_id, resources, resource_type, func, stack_name):
+        def _add_topics(logical_resource_id: str, resource: str, stack_name: str):
             sns_client = aws_stack.connect_to_service("sns")
             topics = _list_all_topics(sns_client)
             topics_by_name = {t["TopicArn"].split(":")[-1]: t for t in topics}
 
-            resource = cls(resources[resource_id])
-            props = resource.props
+            provider = cls(resource)
+            props = provider.props
 
             subscriptions = props.get("Subscription", [])
             for subscription in subscriptions:
                 if is_none_or_empty_value(subscription):
                     continue
                 endpoint = subscription["Endpoint"]
                 topic_arn = topics_by_name[props["TopicName"]]["TopicArn"]
@@ -193,33 +193,31 @@
         if not all(list(result.values())):
             # return None if not all policies for all topics are properly deployed yet
             return None
         return result
 
     @classmethod
     def get_deploy_templates(cls):
-        def _create(resource_id, resources, resource_type, func, stack_name):
+        def _create(logical_resource_id: str, resource: dict, stack_name: str):
             sns_client = aws_stack.connect_to_service("sns")
-            resource = cls(resources[resource_id])
-            props = resource.props
+            provider = cls(resource)
+            props = provider.props
 
-            resources[resource_id]["PhysicalResourceId"] = generate_default_name(
-                stack_name, resource_id
-            )
+            resource["PhysicalResourceId"] = generate_default_name(stack_name, logical_resource_id)
 
             policy = json.dumps(props["PolicyDocument"])
             for topic_arn in props["Topics"]:
                 sns_client.set_topic_attributes(
                     TopicArn=topic_arn, AttributeName="Policy", AttributeValue=policy
                 )
 
-        def _delete(resource_id, resources, *args, **kwargs):
+        def _delete(logical_resource_id: str, resource: dict, stack_name: str):
             sns_client = aws_stack.connect_to_service("sns")
-            resource = cls(resources[resource_id])
-            props = resource.props
+            provider = cls(resource)
+            props = provider.props
 
             for topic_arn in props["Topics"]:
                 try:
                     sns_client.set_topic_attributes(
                         TopicArn=topic_arn, AttributeName="Policy", AttributeValue=""
                     )
                 except ClientError as err:
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/sqs.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,33 +22,33 @@
 
     def fetch_state(self, stack_name, resources):
         if self.resource_json.get("PhysicalResourceId"):
             return {"something": "something"}  # gotta return <something> since {} is falsey :)
 
     @classmethod
     def get_deploy_templates(cls):
-        def _create(resource_id, resources, resource_type, func, stack_name):
+        def _create(logical_resource_id: str, resource: dict, stack_name: str):
             sqs_client = aws_stack.connect_to_service("sqs")
-            resource = cls(resources[resource_id])
-            props = resource.props
+            resource_provider = cls(resource)
+            props = resource_provider.props
 
-            resources[resource_id]["PhysicalResourceId"] = "%s-%s-%s" % (
+            resource["PhysicalResourceId"] = "%s-%s-%s" % (
                 stack_name,
-                resource_id,
+                logical_resource_id,
                 short_uid(),
             )
 
             policy = json.dumps(props["PolicyDocument"])
             for queue in props["Queues"]:
                 sqs_client.set_queue_attributes(QueueUrl=queue, Attributes={"Policy": policy})
 
-        def _delete(resource_id, resources, *args, **kwargs):
+        def _delete(logical_resource_id: str, resource: dict, stack_name: str):
             sqs_client = aws_stack.connect_to_service("sqs")
-            resource = cls(resources[resource_id])
-            props = resource.props
+            resource_provider = cls(resource)
+            props = resource_provider.props
 
             for queue in props["Queues"]:
                 try:
                     sqs_client.set_queue_attributes(QueueUrl=queue, Attributes={"Policy": ""})
                 except ClientError as err:
                     if "AWS.SimpleQueueService.NonExistentQueue" != err.response["Error"]["Code"]:
                         raise
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/packages.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/service_models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudformation/stores.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/cloudwatch/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/packages.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/server.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodb/utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/ec2/exceptions.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/ec2/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/ec2/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/edge.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/es/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/events/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/events/scheduler.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/firehose/mappers.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/firehose/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/firehose/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/generic_proxy.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/iam/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/infra.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/internal.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/packages.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/kinesis/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/kms/local_kms_server.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/kms/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/kms/packages.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/kms/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/kms/utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/logs/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/logs/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/messages.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/moto.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/motoserver.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/cluster.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/packages.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/opensearch/versions.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/plugins.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/providers.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/redshift/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/route53/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/route53resolver/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/route53resolver/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/route53resolver/utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/constants.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/cors.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/multipart_content.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/notifications.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/presigned_url.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/s3_listener.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/s3_starter.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/s3_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/virtual_host.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/s3/website_hosting.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/secretsmanager/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/ses/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sns/constants.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sns/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sns/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sns/publisher.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/constants.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/exceptions.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/query_api.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sqs/utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/ssm/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/packages.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/stores.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/sts/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/services/transcribe/provider.py` & `localstack-core-2.1.1.dev20230615150942/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/state/core.py` & `localstack-core-2.1.1.dev20230615150942/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/state/inspect.py` & `localstack-core-2.1.1.dev20230615150942/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/state/pickle.py` & `localstack-core-2.1.1.dev20230615150942/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/state/snapshot.py` & `localstack-core-2.1.1.dev20230615150942/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/aws/asf_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/aws/util.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/filters.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/fixtures.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/snapshot.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/pytest/util.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/snapshots/prototype.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/snapshots/report.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/snapshots/transformer.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.1.1.dev20230615150942/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/cli.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/client.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/events.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/logger.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/metadata.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/publisher.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/analytics/usage.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/archives.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/asyncio.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/auth.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/arns.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/aws_models.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/aws_responses.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/aws_stack.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/client.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/client_types.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/queries.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/request_context.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/resources.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/aws/templating.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/bootstrap.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/collections.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/common.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/config_listener.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/container_networking.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/container_utils/container_client.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/coverage_docs.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/crypto.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/diagnose.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/docker_utils.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/files.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/functions.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/http.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/json.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/net.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/numbers.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/objects.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/patch.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/platform.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/run.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/scheduler.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/server/http2_server.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/server/proxy_server.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/serving.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/ssl.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/strings.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/sync.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/tagging.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/tail.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/testutil.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/threads.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/time.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/urls.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/venv.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack/utils/xml.py` & `localstack-core-2.1.1.dev20230615150942/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230615143138
+Version: 2.1.1.dev20230615150942
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/plux.json` & `localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9208333333333334%*

 * *Differences: {"'localstack.hooks.on_infra_start'": '{insert: [(3, '*

 * *                                      "'_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start'), "*

 * *                                      '(5, '*

 * *                                      "'deprecation_warnings=localstack.plugins:deprecation_warnings'), "*

 * *                                      '(6, '*

 * *                                      "'register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_ […]*

```diff
@@ -54,35 +54,35 @@
     ],
     "localstack.hooks.on_infra_shutdown": [
         "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
         "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
-        "deprecation_warnings=localstack.plugins:deprecation_warnings",
-        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration"
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
+        "deprecation_warnings=localstack.plugins:deprecation_warnings",
+        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
-        "terraform/community=localstack.packages.plugins:terraform_package",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
         "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
         "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
+        "terraform/community=localstack.packages.plugins:terraform_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package"
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package"
     ]
 }
```

### Comparing `localstack-core-2.1.1.dev20230615143138/localstack_core.egg-info/requires.txt` & `localstack-core-2.1.1.dev20230615150942/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/pyproject.toml` & `localstack-core-2.1.1.dev20230615150942/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230615143138/setup.cfg` & `localstack-core-2.1.1.dev20230615150942/setup.cfg`

 * *Files identical despite different names*

