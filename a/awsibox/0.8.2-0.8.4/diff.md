# Comparing `tmp/awsibox-0.8.2.tar.gz` & `tmp/awsibox-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsibox-0.8.2.tar", last modified: Tue Jun  6 14:36:27 2023, max compression
+gzip compressed data, was "awsibox-0.8.4.tar", last modified: Thu Jun 15 07:40:26 2023, max compression
```

## Comparing `awsibox-0.8.2.tar` & `awsibox-0.8.4.tar`

### file list

```diff
@@ -1,280 +1,276 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.244610 awsibox-0.8.2/
--rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.2/.gitignore
--rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.2/MANIFEST.in
--rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-06 14:36:27.244610 awsibox-0.8.2/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.2/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.152608 awsibox-0.8.2/awsibox/
--rw-r--r--   0 mello     (1000) mello     (1000)    19179 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/RP.py
--rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-06-06 14:34:45.000000 awsibox-0.8.2/awsibox/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.2/awsibox/args.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3755 2023-02-20 15:00:23.000000 awsibox-0.8.2/awsibox/autoscaling.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.152608 awsibox-0.8.2/awsibox/aws/
--rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/aws/CloudFormationResourceSpecification.json
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.132608 awsibox-0.8.2/awsibox/cfg/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.140608 awsibox-0.8.2/awsibox/cfg/ibox/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.188609 awsibox-0.8.2/awsibox/cfg/ibox/com/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/capacity.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1253 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudformation/
--rw-r--r--   0 mello     (1000) mello     (1000)      658 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     1521 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1687 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/for-services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      121 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1811 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/common.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/dynamodb/
--rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/securitygroup.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.196609 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1441 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3140 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6945 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      931 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.196609 awsibox-0.8.2/awsibox/cfg/ibox/com/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.200609 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      365 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      251 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.200609 awsibox-0.8.2/awsibox/cfg/ibox/com/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     2892 2023-05-01 13:36:02.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6914 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1570 2023-05-01 13:33:03.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1203 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/spot_advisor.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.200609 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      939 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.200609 awsibox-0.8.2/awsibox/cfg/ibox/com/kms/
--rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      165 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/layers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/py-packager.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)      513 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/s3/bucket-log.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/servicediscovery/
--rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/ssm/
--rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.140608 awsibox-0.8.2/awsibox/cfg/ibox/res/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/
--rw-r--r--   0 mello     (1000) mello     (1000)      147 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/accounts.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/deployments.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/domain-names.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1764 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)      706 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2937 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)     2442 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3101 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5137 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     4759 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      243 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/origin-access-identities.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/
--rw-r--r--   0 mello     (1000) mello     (1000)     7727 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      955 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      426 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1018 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.212609 awsibox-0.8.2/awsibox/cfg/ibox/res/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)      160 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ec2/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.212609 awsibox-0.8.2/awsibox/cfg/ibox/res/ecr/
--rw-r--r--   0 mello     (1000) mello     (1000)      136 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ecr/accounts.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ecr/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.212609 awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     9845 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1021 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.212609 awsibox-0.8.2/awsibox/cfg/ibox/res/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/efs/filesystems.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      561 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/efs/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.212609 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticache/
--rw-r--r--   0 mello     (1000) mello     (1000)     5327 2023-05-31 09:04:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.216609 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     3972 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4552 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2962 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.216609 awsibox-0.8.2/awsibox/cfg/ibox/res/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/events/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.216609 awsibox-0.8.2/awsibox/cfg/ibox/res/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     2287 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/iam/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/iam/instance-profiles.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3687 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.220610 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/functions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2444 2023-05-20 09:12:43.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/versions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.220610 awsibox-0.8.2/awsibox/cfg/ibox/res/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     8105 2023-05-10 15:52:15.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/rds/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.220610 awsibox-0.8.2/awsibox/cfg/ibox/res/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)     1427 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/route53/hostedzones.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      357 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/route53/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     7683 2023-05-02 08:15:00.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/route53/recordsets.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.220610 awsibox-0.8.2/awsibox/cfg/ibox/res/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)     2808 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/s3/bucket-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     8101 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/s3/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.220610 awsibox-0.8.2/awsibox/cfg/ibox/res/scheduler/
--rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/res/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      397 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/sns/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/sns/subscriptions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/res/sqs/
--rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/sqs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/sqs/queue-policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.144608 awsibox-0.8.2/awsibox/cfg/ibox/stacks/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/stacks/agw/
--rw-r--r--   0 mello     (1000) mello     (1000)     1751 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/agw/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/agw/infra-info.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/stacks/cch/
--rw-r--r--   0 mello     (1000) mello     (1000)      311 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/cch/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/stacks/clf/
--rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/clf/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     4594 2023-05-11 09:07:31.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3433 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ec2/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)      839 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2510 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.228610 awsibox-0.8.2/awsibox/cfg/ibox/stacks/lbd/
--rw-r--r--   0 mello     (1000) mello     (1000)      144 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/lbd/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1291 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.228610 awsibox-0.8.2/awsibox/cfg/ibox/stacks/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      240 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/rds/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.232610 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/
--rw-r--r--   0 mello     (1000) mello     (1000)      144 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1543 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3527 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-event-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      595 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      910 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4700 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       67 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-lambda-layer-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2157 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/vpc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.232610 awsibox-0.8.2/awsibox/cfg/ibox/stacks/tsk/
--rw-r--r--   0 mello     (1000) mello     (1000)     2490 2023-06-05 15:35:41.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/tsk/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)    16593 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1661 2023-03-20 14:25:03.000000 awsibox-0.8.2/awsibox/cloudformation.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2332 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cloudfront.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1685 2023-04-17 10:03:18.000000 awsibox-0.8.2/awsibox/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/discover.py
--rw-r--r--   0 mello     (1000) mello     (1000)    13278 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/ec2.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/ecr.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2878 2022-07-16 08:44:32.000000 awsibox-0.8.2/awsibox/efs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5303 2023-02-08 17:22:02.000000 awsibox-0.8.2/awsibox/elasticloadbalancing.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2409 2023-06-06 14:34:34.000000 awsibox-0.8.2/awsibox/generate.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3369 2023-04-14 07:54:55.000000 awsibox-0.8.2/awsibox/iam.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2942 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/joker.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.240610 awsibox-0.8.2/awsibox/lambdas/
--rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/ASGSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/AtEdgeAddHeaders.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4293 2023-04-11 07:34:58.000000 awsibox-0.8.2/awsibox/lambdas/CCRFargateSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.2/awsibox/lambdas/CCRLightHouse.code
--rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.2/awsibox/lambdas/CCRStackReplicator.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.2/awsibox/lambdas/CloudWatchAlarmStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.2/awsibox/lambdas/CloudWatchRepeatedNotify.code
--rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/EC2StartStopTagged.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.2/awsibox/lambdas/ECSClusterAutoscale.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.2/awsibox/lambdas/ECSDrainInstance.code
--rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.2/awsibox/lambdas/ECSDrainTasks.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.2/awsibox/lambdas/ECSEventTaskStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.2/awsibox/lambdas/ECSEventsSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.2/awsibox/lambdas/ECSRaiseASGAlarm.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.2/awsibox/lambdas/ECSRunTask.code
--rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/ECSUpdateDesiredCount.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/ElasticSearchSnapShot.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5327 2023-05-18 13:11:03.000000 awsibox-0.8.2/awsibox/lambdas/InfraInfo.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.2/awsibox/lambdas/ManageService.code
--rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/PaidApi.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.2/awsibox/lambdas/PyPackager.code
--rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/Python37SSM.layer
--rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.2/awsibox/lambdas/R53RecordInstanceId.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.2/awsibox/lambdas/ServiceDiscovery.code
--rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.2/awsibox/lambdas/ServiceUnavailable.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.8.2/awsibox/lambdas/StacksOps.code
--rw-r--r--   0 mello     (1000) mello     (1000)     3383 2022-03-18 08:09:10.000000 awsibox-0.8.2/awsibox/mappings.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5917 2022-06-21 15:07:51.000000 awsibox-0.8.2/awsibox/rds.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2760 2023-02-13 17:05:21.000000 awsibox-0.8.2/awsibox/s3.py
--rw-r--r--   0 mello     (1000) mello     (1000)    45530 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/shared.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.240610 awsibox-0.8.2/awsibox/user-data/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.240610 awsibox-0.8.2/awsibox/user-data/SCRIPTS/
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/ELBCHECK.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/END.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/INIT.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/PACKAGE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/SERVICE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/SETUP.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.2/awsibox/user-data/ecs-cluster.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     7975 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/waf.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.132608 awsibox-0.8.2/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.132608 awsibox-0.8.2/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.148608 awsibox-0.8.2/build/lib/awsibox.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-06 14:36:26.000000 awsibox-0.8.2/build/lib/awsibox.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)     8959 2023-06-06 14:36:26.000000 awsibox-0.8.2/build/lib/awsibox.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-06-06 14:36:26.000000 awsibox-0.8.2/build/lib/awsibox.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-06-06 14:36:26.000000 awsibox-0.8.2/build/lib/awsibox.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-06-06 14:36:26.000000 awsibox-0.8.2/build/lib/awsibox.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.240610 awsibox-0.8.2/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)     3177 2023-04-27 09:19:18.000000 awsibox-0.8.2/scripts/ibox_generate_templates.py
--rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-06-06 14:36:27.244610 awsibox-0.8.2/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      506 2023-04-27 09:19:18.000000 awsibox-0.8.2/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.245040 awsibox-0.8.4/
+-rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.4/.gitignore
+-rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.4/MANIFEST.in
+-rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-15 07:40:26.245040 awsibox-0.8.4/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.4/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.129038 awsibox-0.8.4/awsibox/
+-rw-r--r--   0 mello     (1000) mello     (1000)    19179 2023-06-06 14:25:53.000000 awsibox-0.8.4/awsibox/RP.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-06-15 07:37:31.000000 awsibox-0.8.4/awsibox/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.4/awsibox/args.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4155 2023-06-09 13:02:33.000000 awsibox-0.8.4/awsibox/autoscaling.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.129038 awsibox-0.8.4/awsibox/aws/
+-rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/aws/CloudFormationResourceSpecification.json
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.109038 awsibox-0.8.4/awsibox/cfg/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.113038 awsibox-0.8.4/awsibox/cfg/ibox/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.165039 awsibox-0.8.4/awsibox/cfg/ibox/com/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.169039 awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/capacity.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1253 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.169039 awsibox-0.8.4/awsibox/cfg/ibox/com/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.173039 awsibox-0.8.4/awsibox/cfg/ibox/com/cloudformation/
+-rw-r--r--   0 mello     (1000) mello     (1000)      658 2023-06-06 14:25:53.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.173039 awsibox-0.8.4/awsibox/cfg/ibox/com/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1521 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1656 2023-06-14 15:23:58.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/cloudfront/for-services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      121 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/cloudfront/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.173039 awsibox-0.8.4/awsibox/cfg/ibox/com/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1811 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/common.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.173039 awsibox-0.8.4/awsibox/cfg/ibox/com/dynamodb/
+-rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.177039 awsibox-0.8.4/awsibox/cfg/ibox/com/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ec2/securitygroup.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.177039 awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1414 2023-06-14 16:05:45.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3140 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6894 2023-06-14 16:14:09.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      899 2023-06-14 16:05:02.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.181039 awsibox-0.8.4/awsibox/cfg/ibox/com/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.181039 awsibox-0.8.4/awsibox/cfg/ibox/com/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      242 2023-06-14 15:18:04.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      201 2023-06-14 16:13:04.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.185039 awsibox-0.8.4/awsibox/cfg/ibox/com/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2892 2023-05-01 13:36:02.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6914 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/events/ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/events/ecs-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1570 2023-05-01 13:33:03.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/events/ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1203 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/events/spot_advisor.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.189039 awsibox-0.8.4/awsibox/cfg/ibox/com/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      939 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.189039 awsibox-0.8.4/awsibox/cfg/ibox/com/kms/
+-rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.193040 awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/layers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/py-packager.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.193040 awsibox-0.8.4/awsibox/cfg/ibox/com/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.193040 awsibox-0.8.4/awsibox/cfg/ibox/com/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)      513 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/s3/bucket-log.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.193040 awsibox-0.8.4/awsibox/cfg/ibox/com/servicediscovery/
+-rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.197039 awsibox-0.8.4/awsibox/cfg/ibox/com/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.197039 awsibox-0.8.4/awsibox/cfg/ibox/com/ssm/
+-rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.113038 awsibox-0.8.4/awsibox/cfg/ibox/res/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.197039 awsibox-0.8.4/awsibox/cfg/ibox/res/apigateway/
+-rw-r--r--   0 mello     (1000) mello     (1000)      147 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/apigateway/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/apigateway/deployments.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/apigateway/domain-names.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1821 2023-06-14 15:29:04.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.197039 awsibox-0.8.4/awsibox/cfg/ibox/res/application-autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      832 2023-06-14 15:40:34.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2965 2023-06-14 15:41:11.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.201040 awsibox-0.8.4/awsibox/cfg/ibox/res/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-06-14 15:45:22.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3163 2023-06-14 15:45:28.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5137 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.201040 awsibox-0.8.4/awsibox/cfg/ibox/res/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.201040 awsibox-0.8.4/awsibox/cfg/ibox/res/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4829 2023-06-14 15:51:31.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      243 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/cloudfront/origin-access-identities.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/cloudfront/policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.201040 awsibox-0.8.4/awsibox/cfg/ibox/res/cloudwatch/
+-rw-r--r--   0 mello     (1000) mello     (1000)     7727 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1041 2023-06-14 15:57:15.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.205040 awsibox-0.8.4/awsibox/cfg/ibox/res/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      364 2023-06-14 16:02:37.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1081 2023-06-14 16:01:55.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.205040 awsibox-0.8.4/awsibox/cfg/ibox/res/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)      160 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/ec2/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.205040 awsibox-0.8.4/awsibox/cfg/ibox/res/ecr/
+-rw-r--r--   0 mello     (1000) mello     (1000)      136 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/ecr/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/ecr/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.205040 awsibox-0.8.4/awsibox/cfg/ibox/res/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     9924 2023-06-14 16:06:44.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/ecs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/ecs/services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1021 2023-06-06 14:25:53.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.209040 awsibox-0.8.4/awsibox/cfg/ibox/res/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/efs/filesystems.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      561 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/efs/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.209040 awsibox-0.8.4/awsibox/cfg/ibox/res/elasticache/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5327 2023-05-31 09:04:53.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.213040 awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4187 2023-06-14 16:14:27.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4552 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2962 2023-06-06 14:25:53.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.213040 awsibox-0.8.4/awsibox/cfg/ibox/res/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/events/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.213040 awsibox-0.8.4/awsibox/cfg/ibox/res/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2364 2023-06-14 16:17:13.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/iam/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/iam/instance-profiles.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3687 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.217040 awsibox-0.8.4/awsibox/cfg/ibox/res/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/lambda/functions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2591 2023-06-14 16:23:01.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/lambda/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/lambda/permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/lambda/versions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.217040 awsibox-0.8.4/awsibox/cfg/ibox/res/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     8105 2023-05-10 15:52:15.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/rds/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.217040 awsibox-0.8.4/awsibox/cfg/ibox/res/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1427 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/route53/hostedzones.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      410 2023-06-14 15:15:46.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/route53/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     7638 2023-06-14 15:16:13.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/route53/recordsets.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.221040 awsibox-0.8.4/awsibox/cfg/ibox/res/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2808 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/s3/bucket-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     8101 2023-06-14 16:17:34.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/s3/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.221040 awsibox-0.8.4/awsibox/cfg/ibox/res/scheduler/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.221040 awsibox-0.8.4/awsibox/cfg/ibox/res/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      449 2023-06-14 16:29:21.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/sns/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/sns/subscriptions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.221040 awsibox-0.8.4/awsibox/cfg/ibox/res/sqs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/sqs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/res/sqs/queue-policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.117038 awsibox-0.8.4/awsibox/cfg/ibox/stacks/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.221040 awsibox-0.8.4/awsibox/cfg/ibox/stacks/agw/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1690 2023-06-14 15:29:08.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/agw/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/agw/infra-info.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.221040 awsibox-0.8.4/awsibox/cfg/ibox/stacks/cch/
+-rw-r--r--   0 mello     (1000) mello     (1000)      280 2023-06-14 15:24:02.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/cch/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.225040 awsibox-0.8.4/awsibox/cfg/ibox/stacks/clf/
+-rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/clf/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.225040 awsibox-0.8.4/awsibox/cfg/ibox/stacks/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4594 2023-05-11 09:07:31.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3294 2023-06-14 16:32:13.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/ec2/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.225040 awsibox-0.8.4/awsibox/cfg/ibox/stacks/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      839 2023-06-06 14:25:53.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2378 2023-06-14 16:05:52.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/ecs/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-14 15:54:35.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.225040 awsibox-0.8.4/awsibox/cfg/ibox/stacks/lbd/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1291 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.225040 awsibox-0.8.4/awsibox/cfg/ibox/stacks/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      209 2023-06-14 15:24:08.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/rds/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.229040 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/
+-rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1543 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3497 2023-06-14 15:55:04.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-event-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      564 2023-06-14 15:24:17.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      910 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4645 2023-06-14 16:16:30.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2157 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/vpc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.229040 awsibox-0.8.4/awsibox/cfg/ibox/stacks/tsk/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2459 2023-06-14 16:36:55.000000 awsibox-0.8.4/awsibox/cfg/ibox/stacks/tsk/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)    16625 2023-06-08 07:25:26.000000 awsibox-0.8.4/awsibox/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1661 2023-03-20 14:25:03.000000 awsibox-0.8.4/awsibox/cloudformation.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2332 2023-06-06 14:25:53.000000 awsibox-0.8.4/awsibox/cloudfront.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1685 2023-04-17 10:03:18.000000 awsibox-0.8.4/awsibox/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/discover.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    13278 2023-06-06 14:25:53.000000 awsibox-0.8.4/awsibox/ec2.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-04-27 09:19:18.000000 awsibox-0.8.4/awsibox/ecr.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2878 2022-07-16 08:44:32.000000 awsibox-0.8.4/awsibox/efs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5303 2023-02-08 17:22:02.000000 awsibox-0.8.4/awsibox/elasticloadbalancing.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2409 2023-06-06 14:34:34.000000 awsibox-0.8.4/awsibox/generate.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3369 2023-04-14 07:54:55.000000 awsibox-0.8.4/awsibox/iam.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2942 2023-06-06 14:25:53.000000 awsibox-0.8.4/awsibox/joker.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.241040 awsibox-0.8.4/awsibox/lambdas/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.4/awsibox/lambdas/ASGSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.4/awsibox/lambdas/AtEdgeAddHeaders.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4293 2023-04-11 07:34:58.000000 awsibox-0.8.4/awsibox/lambdas/CCRFargateSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.4/awsibox/lambdas/CCRLightHouse.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.4/awsibox/lambdas/CCRStackReplicator.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.4/awsibox/lambdas/CloudWatchAlarmStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.4/awsibox/lambdas/CloudWatchRepeatedNotify.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.4/awsibox/lambdas/EC2StartStopTagged.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.4/awsibox/lambdas/ECSClusterAutoscale.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.4/awsibox/lambdas/ECSDrainInstance.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.4/awsibox/lambdas/ECSDrainTasks.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.4/awsibox/lambdas/ECSEventTaskStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.4/awsibox/lambdas/ECSEventsSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.4/awsibox/lambdas/ECSRaiseASGAlarm.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.4/awsibox/lambdas/ECSRunTask.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.4/awsibox/lambdas/ECSUpdateDesiredCount.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.4/awsibox/lambdas/ElasticSearchSnapShot.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5370 2023-06-07 12:49:30.000000 awsibox-0.8.4/awsibox/lambdas/InfraInfo.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.4/awsibox/lambdas/ManageService.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.4/awsibox/lambdas/PaidApi.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.4/awsibox/lambdas/PyPackager.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.4/awsibox/lambdas/Python37SSM.layer
+-rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.4/awsibox/lambdas/R53RecordInstanceId.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.4/awsibox/lambdas/ServiceDiscovery.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.4/awsibox/lambdas/ServiceUnavailable.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.8.4/awsibox/lambdas/StacksOps.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     3383 2022-03-18 08:09:10.000000 awsibox-0.8.4/awsibox/mappings.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5917 2022-06-21 15:07:51.000000 awsibox-0.8.4/awsibox/rds.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2760 2023-02-13 17:05:21.000000 awsibox-0.8.4/awsibox/s3.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    46030 2023-06-09 13:02:41.000000 awsibox-0.8.4/awsibox/shared.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.241040 awsibox-0.8.4/awsibox/user-data/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.241040 awsibox-0.8.4/awsibox/user-data/SCRIPTS/
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.4/awsibox/user-data/SCRIPTS/ELBCHECK.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.4/awsibox/user-data/SCRIPTS/END.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.4/awsibox/user-data/SCRIPTS/INIT.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.4/awsibox/user-data/SCRIPTS/PACKAGE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.4/awsibox/user-data/SCRIPTS/SERVICE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.4/awsibox/user-data/SCRIPTS/SETUP.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.4/awsibox/user-data/ecs-cluster.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     7975 2022-03-14 08:29:15.000000 awsibox-0.8.4/awsibox/waf.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.105038 awsibox-0.8.4/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.105038 awsibox-0.8.4/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.121038 awsibox-0.8.4/build/lib/awsibox.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-15 07:40:25.000000 awsibox-0.8.4/build/lib/awsibox.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)     8790 2023-06-15 07:40:25.000000 awsibox-0.8.4/build/lib/awsibox.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-06-15 07:40:25.000000 awsibox-0.8.4/build/lib/awsibox.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-06-15 07:40:25.000000 awsibox-0.8.4/build/lib/awsibox.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-06-15 07:40:25.000000 awsibox-0.8.4/build/lib/awsibox.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-15 07:40:26.241040 awsibox-0.8.4/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     3177 2023-04-27 09:19:18.000000 awsibox-0.8.4/scripts/ibox_generate_templates.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-06-15 07:40:26.245040 awsibox-0.8.4/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      506 2023-04-27 09:19:18.000000 awsibox-0.8.4/setup.py
```

### Comparing `awsibox-0.8.2/.gitignore` & `awsibox-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/PKG-INFO` & `awsibox-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.2
+Version: 0.8.4
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBox
         AwsIBox - **AWS** **I**nfrastructure in a **Box**
```

### Comparing `awsibox-0.8.2/awsibox/RP.py` & `awsibox-0.8.4/awsibox/RP.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/args.py` & `awsibox-0.8.4/awsibox/args.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/autoscaling.py` & `awsibox-0.8.4/awsibox/autoscaling.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,19 @@
     get_endvalue,
     get_expvalue,
     get_subvalue,
     auto_get_props,
     get_condition,
     add_obj,
     import_user_data,
+    get_dictvalue,
 )
 
 
 def AS_LaunchTemplate():
-    Tags_List = []
-
     # Resources
     R_LaunchTemplate = ec2.LaunchTemplate(
         "LaunchTemplate",
         LaunchTemplateName=Sub("${AWS::StackName}-${EnvRole}"),
     )
 
     LaunchTemplateData = ec2.LaunchTemplateData("LaunchTemplateData")
@@ -76,17 +75,26 @@
                 ),
                 user_data,
             ),
         )
 
     add_obj(R_LaunchTemplate)
 
-    Tags = asg.Tags()
-    Tags.tags = Tags_List
-    return Tags
+    # add Medata Tags to LaunchTemplate TagSpecifications
+    if hasattr(cfg, "MetadataTags"):
+        for n in R_LaunchTemplate.LaunchTemplateData.TagSpecifications:
+            if n.ResourceType in ["instance", "volume"]:
+                n.Tags.tags.extend(
+                    [
+                        {"Key": n, "Value": v}
+                        for n, v in get_dictvalue(
+                            cfg.MetadataTags, mapname="MetadataTags"
+                        ).items()
+                    ],
+                )
 
 
 def AS_Autoscaling(key):
     LoadBalancers = []
     TargetGroups = []
     if cfg.LoadBalancerType == "Classic":
         for n in cfg.LoadBalancer:
@@ -106,15 +114,15 @@
                 setattr(
                     cfg,
                     "EC2InstanceUserDataELBV2CheckTargetGroupArn",
                     Ref(f"ElasticLoadBalancingV2TargetGroupTargetGroupLoadBalancer{n}"),
                 )
 
     # Resources
-    LaunchTemplateTags = AS_LaunchTemplate()
+    AS_LaunchTemplate()
 
     R_ASG = asg.AutoScalingGroup(
         "AutoScalingGroupBase",
         LoadBalancerNames=LoadBalancers,
     )
 
     auto_get_props(R_ASG)
@@ -122,10 +130,8 @@
     try:
         R_ASG.TargetGroupARNs
     except Exception:
         R_ASG.TargetGroupARNs = TargetGroups
     else:
         R_ASG.TargetGroupARNs.extend(TargetGroups)
 
-    R_ASG.Tags += LaunchTemplateTags
-
     add_obj([R_ASG])
```

### Comparing `awsibox-0.8.2/awsibox/aws/CloudFormationResourceSpecification.json` & `awsibox-0.8.4/awsibox/aws/CloudFormationResourceSpecification.json`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/capacity.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/capacity.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/for-services.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/cloudfront/for-services.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 IBoxLoader: !include
   - com/cloudfront/i_base.yml
-  - res/route53/recordsets.yml
 
 global:
   CloudFrontDistribution:
     - IBOX_BASE:
         IBOX_LINKED_OBJ:
           Route53RecordSet:
             Key: Route53RecordSet
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/common.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/common.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/bottlerocket.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/ec2/bottlerocket.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/capacityprovider.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/capacityprovider.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 IBoxLoader:
   - !exclude
     - com/iam/policy-ecs-exec.yml
   - !include
     - com/ecs/task.yml
-    - res/ecs/services.yml
 
 global:
   Parameter:
     - DaemonReserveCpu:
         Description: 'Empty for mapped value'
         AllowedValues: ['', 'yes', 'no']
   Condition:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/fargate-spot.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 IBoxLoader: !include
   - com/elasticloadbalancing/i_base.yml
-  - res/elasticloadbalancing/v2-listener-rules.yml
   - com/cloudfront/for-services.yml
   - com/elasticloadbalancing/v2-listener.yml
 
 global:
   Parameter:
     - LoadBalancer:
         Description: "Comma delimited list of enabled LoadBalancerApplication - empty for mapped value - none to disable"
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/task.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/ecs/task.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 IBoxLoader: !include
-  - res/ecs/taskdefinitions.yml
   - com/iam/policy-parameterstore.yml
   - com/iam/policy-ecs-exec.yml
   - com/ec2/securitygroup.yml
 
 
 global:
   Parameter:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/events/cluster-autoscale.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/events/cluster-autoscale.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/events/ec2.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/events/ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs-spot.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/events/ecs-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/events/ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/events/spot_advisor.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/events/spot_advisor.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/managed-policies.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-update_stack.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/iam/policy-update_stack.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/roles.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/py-packager.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/py-packager.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/service-unavailable.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/lambda/service-unavailable.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/s3/bucket-log.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/s3/bucket-log.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/apigateway/ibox_base.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+IBoxLoader: !include
+  - res/apigateway/deployments.yml
+
 global:
   ApiGatewayDomainName:
     - IBOX_BASE:
         IBOX_ENABLED: False
         IBOX_LINKED_OBJ:
           Key: Route53RecordSet
           Type: ApiGatewayDomainName.IBOX_INDEXNAME
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+IBoxLoader: !include
+  - res/application-autoscaling/scalingpolicies.yml
+  - res/application-autoscaling/scalabletargets.yml
+
 global:
   ApplicationAutoScalingScalingPolicy:
     - IBOX_BASE:
         PolicyName: IBOX_RESNAME
         ScalingTargetId: Ref('ApplicationAutoScalingScalableTargetECSService')
         TargetTrackingScalingPolicyConfiguration:
           PredefinedMetricSpecification.IBOX_PCO:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 global:
   ApplicationAutoScalingScalableTarget:
     - ECSService:
+        IBOX_ENABLED: False
         MaxCapacity: get_endvalue('CapacityMax')
         MinCapacity: get_endvalue('CapacityMin')
         ResourceId: get_subvalue('service/${1E}/${Service.Name}', 'Cluster', 'ClusterStack')
         RoleARN: get_expvalue('RoleEC2ContainerServiceAutoscale', '')
         ScalableDimension: 'ecs:service:DesiredCount'
         ServiceNamespace: ecs
         ScheduledActions:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 IBoxLoader: !include
   - com/autoscaling/capacity.yml
   #- com/autoscaling/imageid-ec2.yml
   - res/autoscaling/launchtemplates.yml
-  - res/autoscaling/scalingpolicies.yml
 
 global:
   AutoScalingGroup:
     - Base:
         IBOX_TITLE: AutoScalingGroup
         AvailabilityZones: GetAZs()
         DesiredCapacity: get_endvalue('CapacityDesired')
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+IBoxLoader: !include
+  - res/autoscaling/scalingpolicies.yml
+
 global:
   AutoScalingScalingPolicy:
     - IBOX_BASE:
         AutoScalingGroupName: Ref('AutoScalingGroup')
         TargetTrackingConfiguration:
           PredefinedMetricSpecification.IBOX_PCO:
             IBOX_OUTPUT:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+IBoxLoader: !include
+  - res/cloudfront/origin-access-identities.yml
+
 global:
   CloudFrontDistribution:
     - IBOX_BASE:
         IBOX_TITLE: CloudFrontDistribution
         Condition: IBOX_RESNAME.Create
         AcmCertificate.IBOX_PCO:
           IBOX_CONDITION:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/policies.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/cloudfront/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/alarms.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/cloudwatch/alarms.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+IBoxLoader: !include
+  - res/codedeploy/deployment-groups.yml
+
 global:
   CodeDeployDeploymentGroup:
     - IBOX_BASE:
         Ec2TagFilters:
           - IBOX_IF:
             - DeployRevision
             - IBOX_IFVALUE
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/ecr/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/ecr/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/ecs/ibox_base.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+IBoxLoader: !include
+  - res/ecs/taskdefinitions.yml
+  - res/ecs/services.yml
+
 global:
   ECSTaskDefinition:
     - IBOX_BASE:
         IBOX_ENABLED: False
         # Need to define Parameters, Conditions and Outputs here because they need to be used/evaluated also in ContainerDefinitions
         # and ContainerDefinitions is processed before ECSTaskDefinition keys Cpu, Memory and NetworkMode (alphabetical order).
         IBOX_PARAMETER:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/services.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/ecs/services.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/efs/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/efs/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticache/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/elasticache/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+IBoxLoader: !include
+  - res/elasticloadbalancing/listeners.yml
+  - res/elasticloadbalancing/v2-targetgroups.yml
+  - res/elasticloadbalancing/v2-listener-rules.yml
+  - res/elasticloadbalancing/v2-loadbalancers.yml
+
 global:
   ElasticLoadBalancingLoadBalancer:
     - IBOX_BASE:
         IBOX_OUTPUT:
           - _HealthCheck:
               Value:
                 get_subvalue(
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/events/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/events/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/iam/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/iam/ibox_base.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+IBoxLoader: !include
+  - res/iam/managed-policies.yml
+  - res/iam/roles.yml
+
 global:
   IAMManagedPolicy:
     - IBOX_BASE:
         IBOX_RESNAME: IAMPolicy.IBOX_INDEXNAME
         IBOX_OUTPUT:
           - _:
               IBOX_ENABLED_IF: get_endvalue(f"{IBOX_MAPNAME}Export") == True
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/iam/managed-policies.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/iam/roles.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/functions.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/lambda/functions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/lambda/ibox_base.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+IBoxLoader: !include
+  - res/lambda/permissions.yml
+  - res/lambda/functions.yml
+  - res/lambda/versions.yml
+  - res/lambda/layer_permissions.yml
+
 global:
   LambdaPermission:
     - IBOX_BASE:
         Action: "lambda:InvokeFunction"
 
   Lambda:
     - IBOX_BASE:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/permissions.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/lambda/permissions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/versions.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/lambda/versions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/rds/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/rds/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/route53/hostedzones.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/route53/hostedzones.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/route53/recordsets.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/route53/recordsets.yml`

 * *Files 2% similar despite different names*

```diff
@@ -139,16 +139,14 @@
   AliasTarget:
     DNSName: GetAtt(IBOX_INDEXNAME, 'RegionalDomainName')
     HostedZoneId: GetAtt(IBOX_INDEXNAME, 'RegionalHostedZoneId')
 
 
 global:
   Route53RecordSet:
-    - IBOX_BASE:
-        IBOX_ENABLED: False
     - EC2ExternalLoadBalancerExternal:
         <<: [*zone_external, *ec2_loadbalancer_target_external, *loadbalancer, *base_external]
     - EC2ExternalLoadBalancerInternal:
         <<: [*zone_external, *ec2_loadbalancer_target_internal, *loadbalancer, *base_external]
     - EC2InternalLoadBalancerInternal:
         <<: [*zone_internal, *ec2_loadbalancer_target_internal, *loadbalancer, *base_internal]
     - EC2InternalLoadBalancerExternal:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/s3/bucket-policies.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/s3/bucket-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/s3/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/s3/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/scheduler/ibox_base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/scheduler/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/sns/subscriptions.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/sns/subscriptions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/res/sqs/queue-policies.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/res/sqs/queue-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/agw/i_type.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/agw/i_type.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 IBoxLoader: !include
-  - res/apigateway/deployments.yml
   - com/cloudfront/for-services.yml
-  - com/lambda/i_base.yml
 
 global:
   Output:
     - InvokeUrl:
         Value: Sub('https://${ApiGatewayRestApi}.execute-api.${AWS::Region}.amazonaws.com/%s' % cfg.ApiGatewayRestApi['Base']['Stage'])
   ApiGatewayRestApi:
     - Base:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/agw/infra-info.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/agw/infra-info.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/ec2/i_type.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/ec2/i_type.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 IBoxLoader: !include
   - res/autoscaling/autoscalinggroups.yml
   - com/elasticloadbalancing/loadbalancer.yml
   - com/ec2/securitygroup.yml
-  - res/cloudwatch/alarms.yml
   - com/cloudfront/for-services.yml
   - com/iam/policy-parameterstore.yml
   - res/iam/instance-profiles.yml
-  - res/sns/subscriptions.yml
-  - res/sqs/queue-policies.yml
-  - com/lambda/i_base.yml
-  - res/iam/roles.yml
 
 global:
   Parameter:
     - UpdateMode:
         Description: 'How to update Instances'
         AllowedValues: ['none', 'Replace', 'Rolling']
         Default: 'none'
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/buildkite.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/ecs/buildkite.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/i_type.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/ecs/i_type.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 IBoxLoader: !include
   - com/autoscaling/capacity.yml
-  - res/application-autoscaling/scalingpolicies.yml
-  - res/application-autoscaling/scalabletargets.yml
-  - res/cloudwatch/alarms.yml
   - com/ecs/task.yml
-  - res/ecs/services.yml
   - com/ecs/service-elasticloadbalancing.yml
 
 global:
   ApplicationAutoScalingScalableTarget:
     - ECSService:
+        IBOX_ENABLED: True
         ScheduledActions:
           - Down:
               Enabled: 'no'
               CapacityMax: k
               CapacityMin: CapacityMin
               Schedule: 'cron(00 22 * * ? *)'
           - Up:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-base.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 IBoxLoader: !include
   - com/elasticloadbalancing/loadbalancer.yml
-  - res/cloudwatch/alarms.yml
 
 global:
   StackName: alb
   Parameter:
     - LoadBalancer:
         Description: 'Application Load Balancer to conditionally create - empty for default based on role - need to be already defined'
         AllowedValues: ['External', 'Internal', '']
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-extra-01.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-extra-01.yml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
   - com/certificatemanager/certificate-global.yml
   - com/certificatemanager/certificate-regional.yml
   - res/cloudfront/policies.yml
   - com/iam/roles-cloudformation-stackset.yml
   - res/elasticache/subnet-groups.yml
   - res/rds/db-subnet-groups.yml
   - res/apigateway/accounts.yml
-  - res/route53/recordsets.yml
   - res/efs/filesystems.yml
 
 
 global:
   StackName: r-extra-01
   MappingClass:
     - AZones:
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-IBoxLoader: !include
-  - res/iam/managed-policies.yml
-
 global:
   StackName: iam-p-01
   IAMManagedPolicy:
     - SSMParameterStoreBase:
         IBOX_ENABLED: True
     - LogRead:
         IBOX_ENABLED: True
```

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/vpc.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/res/vpc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cfg/ibox/stacks/tsk/i_type.yml` & `awsibox-0.8.4/awsibox/cfg/ibox/stacks/tsk/i_type.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 IBoxLoader: !include
   - com/ecs/task.yml
-  - res/lambda/permissions.yml
 
 global:
   Condition:
     - EnableExecuteCommand: Equals(True, False)
       # Need to create a "dummy" Condition for tasks that do not use EventsRuleECSRunTask, where there is the "right" one
     - ECSTasksLaunchOnFargate: Equals(True, True)
   ECSTaskDefinition:
```

### Comparing `awsibox-0.8.2/awsibox/cfg.py` & `awsibox-0.8.4/awsibox/cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 no_override = False
 
 Parameters = {}
 Conditions = {}
 Mappings = {}
 Resources = {}
 Outputs = {}
+Metadata = {}
 
 OBJS = {}
 
 APP_DIR = os.path.dirname(os.path.realpath(__file__))
 
 PATH_INT = os.path.join(APP_DIR, "cfg")
 PATH_INT = os.path.normpath(PATH_INT)
@@ -94,14 +95,15 @@
     "Join(",
     "Base64(",
     "If(",
     "Equals(",
     "Not(",
     "GetAZs(",
     "Tags(",
+    "FindInMap(",
 )
 
 EVAL_PYTHON_FUNCTIONS_IN_CFG = (
     "cfg.",
     "get_expvalue(",
     "get_subvalue(",
     "get_endvalue(",
```

### Comparing `awsibox-0.8.2/awsibox/cloudformation.py` & `awsibox-0.8.4/awsibox/cloudformation.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/cloudfront.py` & `awsibox-0.8.4/awsibox/cloudfront.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/common.py` & `awsibox-0.8.4/awsibox/common.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/discover.py` & `awsibox-0.8.4/awsibox/discover.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/ec2.py` & `awsibox-0.8.4/awsibox/ec2.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/ecr.py` & `awsibox-0.8.4/awsibox/ecr.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/efs.py` & `awsibox-0.8.4/awsibox/efs.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/elasticloadbalancing.py` & `awsibox-0.8.4/awsibox/elasticloadbalancing.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/generate.py` & `awsibox-0.8.4/awsibox/generate.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/iam.py` & `awsibox-0.8.4/awsibox/iam.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/joker.py` & `awsibox-0.8.4/awsibox/joker.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ASGSpot.code` & `awsibox-0.8.4/awsibox/lambdas/ASGSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/AtEdgeAddHeaders.code` & `awsibox-0.8.4/awsibox/lambdas/AtEdgeAddHeaders.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/CCRFargateSpot.code` & `awsibox-0.8.4/awsibox/lambdas/CCRFargateSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/CCRLightHouse.code` & `awsibox-0.8.4/awsibox/lambdas/CCRLightHouse.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/CCRStackReplicator.code` & `awsibox-0.8.4/awsibox/lambdas/CCRStackReplicator.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/CloudWatchAlarmStateChange.code` & `awsibox-0.8.4/awsibox/lambdas/CloudWatchAlarmStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/CloudWatchRepeatedNotify.code` & `awsibox-0.8.4/awsibox/lambdas/CloudWatchRepeatedNotify.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/EC2StartStopTagged.code` & `awsibox-0.8.4/awsibox/lambdas/EC2StartStopTagged.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ECSClusterAutoscale.code` & `awsibox-0.8.4/awsibox/lambdas/ECSClusterAutoscale.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ECSDrainInstance.code` & `awsibox-0.8.4/awsibox/lambdas/ECSDrainInstance.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ECSDrainTasks.code` & `awsibox-0.8.4/awsibox/lambdas/ECSDrainTasks.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ECSEventTaskStateChange.code` & `awsibox-0.8.4/awsibox/lambdas/ECSEventTaskStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ECSEventsSpot.code` & `awsibox-0.8.4/awsibox/lambdas/ECSEventsSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ECSRaiseASGAlarm.code` & `awsibox-0.8.4/awsibox/lambdas/ECSRaiseASGAlarm.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ECSRunTask.code` & `awsibox-0.8.4/awsibox/lambdas/ECSRunTask.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ECSUpdateDesiredCount.code` & `awsibox-0.8.4/awsibox/lambdas/ECSUpdateDesiredCount.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ElasticSearchSnapShot.code` & `awsibox-0.8.4/awsibox/lambdas/ElasticSearchSnapShot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/InfraInfo.code` & `awsibox-0.8.4/awsibox/lambdas/InfraInfo.code`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     i_cfg.output = "text"
     i_cfg.fields = [
         "LastUpdatedTime",
         "StackName",
         "EnvRole",
         "StackType",
         "EnvApp1Version",
-        "ContainerDefinitions1Constraints",
+        "ECSTaskDefinitionBaseContainerDefinitions1Constraints=Container1Constraints",
         "Capacity",
         "StackStatus",
     ]
 
     table = i_commands.show_table()
 
     headers["Content-Type"] = "text/plain"
```

### Comparing `awsibox-0.8.2/awsibox/lambdas/ManageService.code` & `awsibox-0.8.4/awsibox/lambdas/ManageService.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/PaidApi.code` & `awsibox-0.8.4/awsibox/lambdas/PaidApi.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/PyPackager.code` & `awsibox-0.8.4/awsibox/lambdas/PyPackager.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/Python37SSM.layer` & `awsibox-0.8.4/awsibox/lambdas/Python37SSM.layer`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/R53RecordInstanceId.code` & `awsibox-0.8.4/awsibox/lambdas/R53RecordInstanceId.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ServiceDiscovery.code` & `awsibox-0.8.4/awsibox/lambdas/ServiceDiscovery.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/ServiceUnavailable.code` & `awsibox-0.8.4/awsibox/lambdas/ServiceUnavailable.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/lambdas/StacksOps.code` & `awsibox-0.8.4/awsibox/lambdas/StacksOps.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/mappings.py` & `awsibox-0.8.4/awsibox/mappings.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/rds.py` & `awsibox-0.8.4/awsibox/rds.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/s3.py` & `awsibox-0.8.4/awsibox/s3.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/shared.py` & `awsibox-0.8.4/awsibox/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,17 @@
     cfg.Resources.clear()
 
     for n, v in cfg.Outputs.items():
         add_objoutput(v)
         cfg.template.add_output(v)
     cfg.Outputs.clear()
 
+    cfg.template.set_metadata(get_dictvalue(cfg.Metadata, mapname="Metadata"))
+    cfg.Metadata.clear()
+
 
 def add_obj(obj):
     if isinstance(obj, list):
         for n in obj:
             add_obj(n)
     elif isinstance(obj, Parameter):
         cfg.Parameters[obj.title] = obj
@@ -344,15 +347,15 @@
         value = If(condname, value, condvalues[1])
     else:
         value = If(condname, condvalues[0], value)
 
     return value
 
 
-def get_dictvalue(key):
+def get_dictvalue(key, mapname=""):
     if isinstance(key, list):
         value = [get_dictvalue(k) for k in key]
     elif isinstance(key, dict) and "IBOX_LIST" in key:
         # Usefull for KMS policy and other generic dict properties
         value = []
         for i, k in copy.deepcopy(key).items():
             if i == "IBOX_LIST":
@@ -361,17 +364,25 @@
             if_wrapper = k.pop("IBOX_IF", [])
             prop_obj = {j: get_dictvalue(w) for j, w in k.items()}
             if if_wrapper:
                 value.append(iboxif(if_wrapper, "", prop_obj))
             else:
                 value.append(prop_obj)
     elif isinstance(key, dict):
-        value = {i: get_dictvalue(k) for i, k in key.items()}
+        value = {
+            i: get_dictvalue(k, mapname=f"{mapname}{i}" if mapname else "")
+            for i, k in key.items()
+        }
     elif isinstance(key, str):
-        value = eval(key) if key.startswith(cfg.EVAL_FUNCTIONS_IN_CFG) else key
+        if key.startswith(cfg.EVAL_FUNCTIONS_IN_CFG):
+            value = eval(key)
+        elif mapname and mapname in cfg.mappedvalues:
+            value = get_endvalue(mapname)
+        else:
+            value = key
     else:
         value = key
 
     return value
 
 
 def get_condition(
@@ -965,18 +976,20 @@
 
                 # update it with config from IBOX_LINKED_OBJ Conf
                 linked_obj.update(lo_conf)
 
                 lo_resname = lo_conf.get("IBOX_RESNAME", f"{lo_key}{lo_name}")
                 linked_obj["IBOX_RESNAME"] = f"{lo_resname}{lo_for_index}"
 
-                condition = key.get("Condition", getattr(obj, "Condition", None))
-                if condition and not "Condition" in linked_obj:
-                    # automatically add Condition if source obj have it and target not
-                    linked_obj["Condition"] = parse_ibox_key(condition)
+                # automatically add Meta Properties like Condition and UpdateReplacePolicy..
+                for meta_prop in ["Condition", "UpdateReplacePolicy"]:
+                    source_meta_prop = key.get(meta_prop, getattr(obj, meta_prop, None))
+                    if source_meta_prop and not meta_prop in linked_obj:
+                        # ..if source obj have it and target not
+                        linked_obj[meta_prop] = parse_ibox_key(source_meta_prop)
 
                 # assign to louc_cfg lo_key
                 louc_cfg[target_name] = linked_obj
 
             if cfg.debug:
                 pprint(louc_cfg)
             # update cfg and fixedvalues, need to do it this way to avoid overwriting the lo_key and removing all objects
```

### Comparing `awsibox-0.8.2/awsibox/user-data/SCRIPTS/ELBCHECK.sh` & `awsibox-0.8.4/awsibox/user-data/SCRIPTS/ELBCHECK.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/user-data/SCRIPTS/END.sh` & `awsibox-0.8.4/awsibox/user-data/SCRIPTS/END.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/user-data/SCRIPTS/INIT.sh` & `awsibox-0.8.4/awsibox/user-data/SCRIPTS/INIT.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/user-data/SCRIPTS/PACKAGE.sh` & `awsibox-0.8.4/awsibox/user-data/SCRIPTS/PACKAGE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/user-data/SCRIPTS/SERVICE.sh` & `awsibox-0.8.4/awsibox/user-data/SCRIPTS/SERVICE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/user-data/SCRIPTS/SETUP.sh` & `awsibox-0.8.4/awsibox/user-data/SCRIPTS/SETUP.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/user-data/ecs-cluster.sh` & `awsibox-0.8.4/awsibox/user-data/ecs-cluster.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/awsibox/waf.py` & `awsibox-0.8.4/awsibox/waf.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/build/lib/awsibox.egg-info/PKG-INFO` & `awsibox-0.8.4/build/lib/awsibox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.2
+Version: 0.8.4
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBox
         AwsIBox - **AWS** **I**nfrastructure in a **Box**
```

### Comparing `awsibox-0.8.2/build/lib/awsibox.egg-info/SOURCES.txt` & `awsibox-0.8.4/build/lib/awsibox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 awsibox/cfg/ibox/com/iam/policy-update_stack.yml
 awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
 awsibox/cfg/ibox/com/iam/roles.yml
 awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
 awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
 awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
 awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
-awsibox/cfg/ibox/com/lambda/i_base.yml
 awsibox/cfg/ibox/com/lambda/layers.yml
 awsibox/cfg/ibox/com/lambda/py-packager.yml
 awsibox/cfg/ibox/com/lambda/service-unavailable.yml
 awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
 awsibox/cfg/ibox/com/s3/bucket-log.yml
 awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
 awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
@@ -156,28 +155,25 @@
 awsibox/cfg/ibox/stacks/cch/i_type.yml
 awsibox/cfg/ibox/stacks/clf/i_type.yml
 awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
 awsibox/cfg/ibox/stacks/ec2/i_type.yml
 awsibox/cfg/ibox/stacks/ecs/buildkite.yml
 awsibox/cfg/ibox/stacks/ecs/i_type.yml
 awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
-awsibox/cfg/ibox/stacks/lbd/i_type.yml
 awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
 awsibox/cfg/ibox/stacks/rds/i_type.yml
-awsibox/cfg/ibox/stacks/res/i_type.yml
 awsibox/cfg/ibox/stacks/res/res-base.yml
 awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
 awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
 awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
 awsibox/cfg/ibox/stacks/res/res-event-01.yml
 awsibox/cfg/ibox/stacks/res/res-extra-01.yml
 awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
 awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
 awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
-awsibox/cfg/ibox/stacks/res/res-lambda-layer-01.yml
 awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
 awsibox/cfg/ibox/stacks/res/res-s3-01.yml
 awsibox/cfg/ibox/stacks/res/vpc.yml
 awsibox/cfg/ibox/stacks/tsk/i_type.yml
 awsibox/lambdas/ASGSpot.code
 awsibox/lambdas/AtEdgeAddHeaders.code
 awsibox/lambdas/CCRFargateSpot.code
```

### Comparing `awsibox-0.8.2/scripts/ibox_generate_templates.py` & `awsibox-0.8.4/scripts/ibox_generate_templates.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.2/setup.cfg` & `awsibox-0.8.4/setup.cfg`

 * *Files identical despite different names*

