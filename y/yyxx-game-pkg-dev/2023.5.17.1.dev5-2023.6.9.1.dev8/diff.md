# Comparing `tmp/yyxx_game_pkg_dev-2023.5.17.1.dev5.tar.gz` & `tmp/yyxx_game_pkg_dev-2023.6.9.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyxx_game_pkg_dev-2023.5.17.1.dev5.tar", max compression
+gzip compressed data, was "yyxx_game_pkg_dev-2023.6.9.1.dev8.tar", max compression
```

## Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5.tar` & `yyxx_game_pkg_dev-2023.6.9.1.dev8.tar`

### file list

```diff
@@ -1,114 +1,116 @@
--rw-r--r--   0        0        0     4895 2023-05-22 01:43:16.075163 yyxx_game_pkg_dev-2023.5.17.1.dev5/README.md
--rw-r--r--   0        0        0     1799 2023-05-22 01:43:31.907184 yyxx_game_pkg_dev-2023.5.17.1.dev5/pyproject.toml
--rw-r--r--   0        0        0       68 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/__init__.py
--rw-r--r--   0        0        0       83 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dbops/__init__.py
--rw-r--r--   0        0        0     1341 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dbops/mysql_op.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/config/__init__.py
--rw-r--r--   0        0        0     1228 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/config/celery_local_config.py
--rw-r--r--   0        0        0      660 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/rules/__init__.py
--rw-r--r--   0        0        0     1348 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/rules/rule_temp.py
--rw-r--r--   0        0        0      580 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/test_dispatch.py
--rw-r--r--   0        0        0       84 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/helpers/__init__.py
--rw-r--r--   0        0        0      522 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/helpers/test_mysql_helper.py
--rw-r--r--   0        0        0      455 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/helpers/test_pika_helper.py
--rw-r--r--   0        0        0      481 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/helpers/test_redis_helper.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/__init__.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/__init__.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
--rw-r--r--   0        0        0      431 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
--rw-r--r--   0        0        0      413 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/work_flow/__init__.py
--rw-r--r--   0        0        0     1217 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
--rw-r--r--   0        0        0      305 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/submit.json
--rw-r--r--   0        0        0     1250 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/test_submit.py
--rw-r--r--   0        0        0      235 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/test_ip2region.py
--rw-r--r--   0        0        0      513 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/test_logger.py
--rw-r--r--   0        0        0      960 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/test_xtrace.py
--rw-r--r--   0        0        0       81 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/utils/__init__.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/__init__.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/config/__init__.py
--rw-r--r--   0        0        0     1226 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/config/celery_local_config.py
--rw-r--r--   0        0        0      747 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/task_register.py
--rw-r--r--   0        0        0      299 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/test_celery.py
--rw-r--r--   0        0        0       69 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/__init__.py
--rw-r--r--   0        0        0      125 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/__init__.py
--rw-r--r--   0        0        0     5089 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/Operator.py
--rw-r--r--   0        0        0     1505 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/OperatorServer.py
--rw-r--r--   0        0        0     2572 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/RechargeConfig.py
--rw-r--r--   0        0        0     2600 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/TableFieldConf.py
--rw-r--r--   0        0        0      125 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/__init__.py
--rw-r--r--   0        0        0      125 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/sdk/__init__.py
--rw-r--r--   0        0        0     4379 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/sdk/check_token.py
--rw-r--r--   0        0        0     5887 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/sdk/map_core.py
--rw-r--r--   0        0        0     2957 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/sdk/recharge.py
--rw-r--r--   0        0        0     6895 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/conf/__init__.py
--rw-r--r--   0        0        0     2054 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/conf/global_settings.py
--rw-r--r--   0        0        0      129 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/aes.py
--rw-r--r--   0        0        0     1114 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/basic.py
--rw-r--r--   0        0        0     1312 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/make_sign.py
--rw-r--r--   0        0        0     2653 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/rsa.py
--rw-r--r--   0        0        0       83 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/__init__.py
--rw-r--r--   0        0        0     1331 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/base.py
--rw-r--r--   0        0        0     1295 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/ch_op.py
--rw-r--r--   0        0        0     5597 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/das_api.py
--rw-r--r--   0        0        0     1911 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/es_op.py
--rw-r--r--   0        0        0     1678 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/hdfs_op.py
--rw-r--r--   0        0        0      979 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/mongo_op.py
--rw-r--r--   0        0        0     3955 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/mysql_op.py
--rw-r--r--   0        0        0       81 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/__init__.py
--rw-r--r--   0        0        0     2512 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/mysql_helper.py
--rw-r--r--   0        0        0     2959 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/op_helper.py
--rw-r--r--   0        0        0     1266 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/pika_helper.py
--rw-r--r--   0        0        0     2966 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/redis_helper.py
--rw-r--r--   0        0        0       79 2023-05-22 01:43:16.079163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/__init__.py
--rw-r--r--   0        0        0 11070130 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/ip2region.xdb
--rw-r--r--   0        0        0      604 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/ip_x.py
--rw-r--r--   0        0        0     5735 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/xdbSearcher.py
--rw-r--r--   0        0        0       81 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/__init__.py
--rw-r--r--   0        0        0     2326 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/config.py
--rw-r--r--   0        0        0     3467 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/handlers.py
--rw-r--r--   0        0        0     2154 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/log.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/__init__.py
--rw-r--r--   0        0        0       68 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/common/__init__.py
--rw-r--r--   0        0        0     1514 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/common/common.py
--rw-r--r--   0        0        0       69 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/__init__.py
--rw-r--r--   0        0        0      805 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/manager.py
--rw-r--r--   0        0        0     1042 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/structs.py
--rw-r--r--   0        0        0     5533 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/workflows.py
--rw-r--r--   0        0        0      604 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/dispatch.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/logic/__init__.py
--rw-r--r--   0        0        0     4402 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
--rw-r--r--   0        0        0      809 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/route.py
--rw-r--r--   0        0        0      677 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/__init__.py
--rw-r--r--   0        0        0      689 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
--rw-r--r--   0        0        0     4270 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
--rw-r--r--   0        0        0      667 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/log.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/logic/__init__.py
--rw-r--r--   0        0        0     5961 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/logic/submit_logic.py
--rw-r--r--   0        0        0      987 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/submit.py
--rw-r--r--   0        0        0       70 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/xcelery/__init__.py
--rw-r--r--   0        0        0     2206 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/xcelery/instance.py
--rw-r--r--   0        0        0     1183 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/xcelery/task_base.py
--rw-r--r--   0        0        0      427 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/__init__.py
--rw-r--r--   0        0        0      132 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/cookiecutter.json
--rw-r--r--   0        0        0     3410 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
--rw-r--r--   0        0        0      624 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
--rw-r--r--   0        0        0     4208 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
--rw-r--r--   0        0        0       83 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/__init__.py
--rw-r--r--   0        0        0     5652 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/decorator.py
--rw-r--r--   0        0        0     3136 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/error_code.py
--rw-r--r--   0        0        0     2845 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/profiler.py
--rw-r--r--   0        0        0     3068 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xListStr.py
--rw-r--r--   0        0        0     8255 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xdataframe.py
--rw-r--r--   0        0        0     6238 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xdate.py
--rw-r--r--   0        0        0     3091 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xhttp.py
--rw-r--r--   0        0        0      971 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xmath.py
--rw-r--r--   0        0        0      574 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xstring.py
--rw-r--r--   0        0        0       69 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/xtrace/__init__.py
--rw-r--r--   0        0        0     2858 2023-05-22 01:43:16.143163 yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/xtrace/helper.py
--rw-r--r--   0        0        0     6881 1970-01-01 00:00:00.000000 yyxx_game_pkg_dev-2023.5.17.1.dev5/PKG-INFO
+-rw-r--r--   0        0        0     4895 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/README.md
+-rw-r--r--   0        0        0     1846 2023-06-15 09:27:35.619731 yyxx_game_pkg_dev-2023.6.9.1.dev8/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dbops/__init__.py
+-rw-r--r--   0        0        0     1341 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dbops/mysql_op.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/config/__init__.py
+-rw-r--r--   0        0        0     1228 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/config/celery_local_config.py
+-rw-r--r--   0        0        0      660 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0     1348 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/rules/rule_temp.py
+-rw-r--r--   0        0        0      580 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/test_dispatch.py
+-rw-r--r--   0        0        0       84 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/helpers/test_mysql_helper.py
+-rw-r--r--   0        0        0      455 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/helpers/test_pika_helper.py
+-rw-r--r--   0        0        0      481 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/helpers/test_redis_helper.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
+-rw-r--r--   0        0        0      431 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
+-rw-r--r--   0        0        0      413 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/work_flow/__init__.py
+-rw-r--r--   0        0        0     1217 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
+-rw-r--r--   0        0        0      305 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/submit.json
+-rw-r--r--   0        0        0     1250 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/test_submit.py
+-rw-r--r--   0        0        0      235 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/test_ip2region.py
+-rw-r--r--   0        0        0      513 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/test_logger.py
+-rw-r--r--   0        0        0      960 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/test_xtrace.py
+-rw-r--r--   0        0        0       81 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/utils/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/config/__init__.py
+-rw-r--r--   0        0        0     1226 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/config/celery_local_config.py
+-rw-r--r--   0        0        0      747 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/task_register.py
+-rw-r--r--   0        0        0      299 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/test_celery.py
+-rw-r--r--   0        0        0       69 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/__init__.py
+-rw-r--r--   0        0        0     5166 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/Operator.py
+-rw-r--r--   0        0        0     1505 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/OperatorServer.py
+-rw-r--r--   0        0        0     2572 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/RechargeConfig.py
+-rw-r--r--   0        0        0     2600 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/TableFieldConf.py
+-rw-r--r--   0        0        0      124 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/__init__.py
+-rw-r--r--   0        0        0     4353 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/check_token.py
+-rw-r--r--   0        0        0     5805 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/map_core.py
+-rw-r--r--   0        0        0     3506 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/recharge.py
+-rw-r--r--   0        0        0     6894 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/conf/__init__.py
+-rw-r--r--   0        0        0     2053 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/conf/global_settings.py
+-rw-r--r--   0        0        0      128 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/__init__.py
+-rw-r--r--   0        0        0     1164 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/aes.py
+-rw-r--r--   0        0        0     1113 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/basic.py
+-rw-r--r--   0        0        0     1351 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/make_sign.py
+-rw-r--r--   0        0        0     2652 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/rsa.py
+-rw-r--r--   0        0        0       83 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/__init__.py
+-rw-r--r--   0        0        0     1331 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/base.py
+-rw-r--r--   0        0        0     1304 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/ch_op.py
+-rw-r--r--   0        0        0     5596 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/das_api.py
+-rw-r--r--   0        0        0     1911 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/es_op.py
+-rw-r--r--   0        0        0     1678 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/hdfs_op.py
+-rw-r--r--   0        0        0      979 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/mongo_op.py
+-rw-r--r--   0        0        0     3955 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/mysql_op.py
+-rw-r--r--   0        0        0       81 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/__init__.py
+-rw-r--r--   0        0        0     2686 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/mysql_helper.py
+-rw-r--r--   0        0        0     3215 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/op_helper.py
+-rw-r--r--   0        0        0     1266 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/pika_helper.py
+-rw-r--r--   0        0        0     2966 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/redis_helper.py
+-rw-r--r--   0        0        0       79 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/__init__.py
+-rw-r--r--   0        0        0 11070130 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/ip2region.xdb
+-rw-r--r--   0        0        0      604 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/ip_x.py
+-rw-r--r--   0        0        0     5735 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/xdbSearcher.py
+-rw-r--r--   0        0        0       81 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/__init__.py
+-rw-r--r--   0        0        0     2326 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/config.py
+-rw-r--r--   0        0        0     3467 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/handlers.py
+-rw-r--r--   0        0        0     2154 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/log.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/common/__init__.py
+-rw-r--r--   0        0        0     1514 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/common/common.py
+-rw-r--r--   0        0        0       69 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/__init__.py
+-rw-r--r--   0        0        0      805 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/manager.py
+-rw-r--r--   0        0        0     1042 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/structs.py
+-rw-r--r--   0        0        0     5533 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/workflows.py
+-rw-r--r--   0        0        0      604 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/dispatch.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/logic/__init__.py
+-rw-r--r--   0        0        0     4402 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
+-rw-r--r--   0        0        0      809 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/route.py
+-rw-r--r--   0        0        0      677 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0      689 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
+-rw-r--r--   0        0        0     4270 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
+-rw-r--r--   0        0        0      667 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/log.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/logic/__init__.py
+-rw-r--r--   0        0        0     5961 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/logic/submit_logic.py
+-rw-r--r--   0        0        0      987 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/submit.py
+-rw-r--r--   0        0        0       70 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/xcelery/__init__.py
+-rw-r--r--   0        0        0     2206 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/xcelery/instance.py
+-rw-r--r--   0        0        0     1183 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/xcelery/task_base.py
+-rw-r--r--   0        0        0      428 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/__init__.py
+-rw-r--r--   0        0        0      132 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/cookiecutter.json
+-rw-r--r--   0        0        0     4023 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
+-rw-r--r--   0        0        0      624 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
+-rw-r--r--   0        0        0     4077 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
+-rw-r--r--   0        0        0       83 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/__init__.py
+-rw-r--r--   0        0        0     5652 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/decorator.py
+-rw-r--r--   0        0        0     3135 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/error_code.py
+-rw-r--r--   0        0        0     2845 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/profiler.py
+-rw-r--r--   0        0        0     3068 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xListStr.py
+-rw-r--r--   0        0        0     8845 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xdataframe.py
+-rw-r--r--   0        0        0     7441 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xdate.py
+-rw-r--r--   0        0        0     2092 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xfutures.py
+-rw-r--r--   0        0        0     3653 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xhttp.py
+-rw-r--r--   0        0        0      971 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xmath.py
+-rw-r--r--   0        0        0      573 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xstring.py
+-rw-r--r--   0        0        0       69 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/xtrace/__init__.py
+-rw-r--r--   0        0        0     1895 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/xtrace/flask/__init__.py
+-rw-r--r--   0        0        0     2858 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/xtrace/helper.py
+-rw-r--r--   0        0        0     6934 1970-01-01 00:00:00.000000 yyxx_game_pkg_dev-2023.6.9.1.dev8/PKG-INFO
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/README.md` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/pyproject.toml` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-equires = [ "poetry-core",]
+requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "yyxx-game-pkg-dev"
-version = "v2023.05.17.001dev5"
+version = "v2023.06.09.001dev8"
 description = "yyxx game custom module"
 authors = [ "yyxx-game",]
 license = "MIT"
 homepage = "https://github.com/yyxxgame/yyxxgame-pkg"
 repository = "https://github.com/yyxxgame/yyxxgame-pkg"
 readme = "README.md"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
@@ -23,22 +23,23 @@
 toml = "^0.10.2"
 opentelemetry-api = "^1.16.0"
 opentelemetry-sdk = "^1.16.0"
 opentelemetry-exporter-jaeger = "^1.16.0"
 opentelemetry-instrumentation-requests = "^0.37b0"
 opentelemetry-instrumentation-fastapi = "0.37b.0"
 opentelemetry-instrumentation-celery = "0.37b0"
+opentelemetry-instrumentation-flask = "^0.37b0"
 line-profiler = "^4.0.3"
 redis = "^4.5.1"
 pymysql = "^1.0.2"
 pika = "^1.3.1"
 dbutils = "^3.0.2"
 ujson = "^5.7.0"
-requests = "^2.28.2"
-celery = "^5.2.7"
+requests = "2.27.1"
+celery = "5.2.7"
 uvicorn = "^0.21.0"
 pandas = "^1.5.3"
 pycryptodome = "^3.17"
 
 [tool.poetry.extras]
 stat = [ "fastapi",]
 server_center = [ "django", "pillow", "filetype",]
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dbops/mysql_op.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/config/celery_local_config.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/rules/__init__.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/rules/rule_temp.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/rules/rule_temp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/dispatch/test_dispatch.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/helpers/test_mysql_helper.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/helpers/test_mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/submit/test_submit.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/test_submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/test_logger.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/test_xtrace.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/test_xtrace.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/config/celery_local_config.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/tests/xcelery/task_register.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/task_register.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/Operator.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/Operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,25 @@
     """
     注意：需要先设置 connection 和 redis_handle
     """
 
     @classmethod
     def get_key(cls, operator, game_channel_id):
         try:
-            cache_key = "api_operator_channel_%s_%s_key" % (operator, game_channel_id)
+            cache_key = "api_operator_channel_%s_%s_key" % (
+                operator,
+                game_channel_id,
+            )
             package = {}
             subpackage = {}
 
             sdk_data = redis.get_data(cache_key)
 
             if not sdk_data:
+                sdk_data = {}
                 sql = """
                     SELECT
                         t1.alias as operator, t2.game_channel_id, t2.group_id, t2.iw_id, t2.sdk_config, t3.alias as iw_alias
                     FROM
                         svr_operator t1, svr_channel t2 left join svr_inter_working_group t3 on t2.iw_id = t3.id
                     WHERE
                         ((t1.alias = '%s' AND t2.game_channel_id = '%s') OR (t1.alias = '%s' AND t2.game_channel_id='0'))
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/OperatorServer.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/OperatorServer.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/RechargeConfig.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/RechargeConfig.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/model/TableFieldConf.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/TableFieldConf.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/sdk/check_token.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/check_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # -*- coding: utf-8 -*-
 # @Author   : pmz
 # @Time     : 2023/04/18 16:17:00
 # @Software : python3.11
 # @Desc     : 二次认证
 import time
 from abc import ABC, abstractmethod
@@ -26,73 +25,72 @@
     @func sdk_check_token: 验证token方法
     @func sdk_helper: sdk 参数处理
     @func channel_make_sign: 默认 sorted(params) md5
 
     根据渠道需求填写以下参数
     @param is_https: 请求是否为https；默认 True
     @param method: 请求方式 POST GET；默认 POST
-    @param params: 发送和收到 参数的字段名
-    @param time_param: 时间戳字段 time / timestamp，十位时间戳（秒） / 十三位时间戳（毫秒）
-    @param sign_param: 签名字段 sign / signature
+    @param params: (key)发送和(value)接收 参数的字段名
     """
 
     is_https = True  # True False
     method = "POST"
     # params = {}
-    time_param = None  # ("time", int(time.time()))
-    sign_param = "sign"
+    sdk_exclude = ()
 
     def run_check_token(self, *args, **kwargs) -> dict:
         """
         run check token
         """
         sdk_helper, response_helper = self.sdk_version_choice(**kwargs)
         if sdk_helper is None:
             return self.sdk_rechfeed(ErrorCode.ERROR_INVALID_PARAM)
 
-        channel_data, post_data = sdk_helper(**kwargs)
+        channel_data, post_data = sdk_helper(self.sdk_exclude, **kwargs)
         response = self.sdk_check_token(channel_data, post_data)
 
         return response_helper(response, **kwargs)
 
     @abstractmethod
     def response_helper(self, response: dict | None, **kwargs) -> dict:
         """
         根据需求 return 相应的数据
         :return: {"ret": 1, "user_id": "any_user_id"}
         """
-        return self.sdk_rechfeed(ErrorCode.ERROR_SERVER_API_URL_ERROR)
+        return self.sdk_rechfeed(ErrorCode.ERROR_INVALID_PARAM, "验证失败")
 
     @property
     def _params(self):
         """
         params = {
             "appId": "sdk_appId",
             "accountId": "sdk_accountId",
             "token": "sdk_token",
         }
         """
         if self.params is None:
-            raise ValueError("params must be specified")
+            raise ValueError("params must be specified as a dict")
 
         return self.params
 
-    def sdk_helper(self, **kwargs) -> (dict, dict):
+    def sdk_helper(self, sdk_exclude=(), **kwargs) -> (dict, dict):
         """
         处理 sdk 数据
+        :param sdk_exclude: sdk_helper 处理数据，要排除的key
+            可选值: time(self.Time) sign(self.Flag)
         """
         channel_data = kwargs.get("channel_data", {})
 
         post_data = {}
         for k, v in self._params.items():
             post_data[k] = kwargs.get(v)
-        if self.time_param:
-            post_data[self.time_param[0]] = self.time_param[1]
-        if self.sign_param:
-            post_data[self.sign_param] = self.channel_make_sign(
+        if self.Time not in sdk_exclude:
+            post_data[self.Time] = int(time.time())
+        if self.Flag not in sdk_exclude:
+            post_data[self.Flag] = self.channel_make_sign(
                 post_data, channel_data.get("app_key", "")
             )
 
         return channel_data, post_data
 
     def sdk_check_token(self, channel_data, post_data) -> dict | None:
         """
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/center_api/sdk/map_core.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/map_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,34 @@
-
 # -*- coding: utf-8 -*-
 # @Author   : pmz
 # @Time     : 2023/04/18 15:42:33
 # @Software : python3.11
 # @Desc     : map_core
 import json
 import time
 from abc import abstractmethod
 
 from flask import request
 from yyxx_game_pkg.center_api.model.Operator import Operator
 from yyxx_game_pkg.center_api.model.OperatorServer import OperatorServer
 from yyxx_game_pkg.conf import settings
-from yyxx_game_pkg.crypto.basic import (RANDOM_STRING_CHARS_LOWER,
-                                        get_random_string, md5)
+from yyxx_game_pkg.crypto.basic import RANDOM_STRING_CHARS_LOWER, get_random_string, md5
 from yyxx_game_pkg.crypto.make_sign import make_sign
 from yyxx_game_pkg.helpers.op_helper import OPHelper
 
 
 class MapCore(OPHelper):
     Flag = "sign"
     Time = "time"
     Gmip = None
     Imei = None
     Callback = None
     OutTime = 0
 
-    make_sign_exclude = [
-        "sign",
-        "signature",
-        "time",
-        "timestamp",
-        "gmip",
-        "cp_platform",
-        "ch_conter",
-        "opts",
-    ]
+    make_sign_exclude = {"gmip", "cp_platform", "ch_conter", "opts"}
     API_KEY = settings.API_KEY
     params = None
     _plat_code = None
     _operator = None
     _game_channel_id = None
 
     # 大额充值限制
@@ -64,28 +53,32 @@
         if sign is None:
             return False
         _sign = self.make_sign(values)
         if sign != _sign:
             return False
         return True
 
-    def make_sign(self, values, sign_key=None) -> str:
-        return make_sign(values, self.api_key, self.make_sign_exclude, self.Time)
+    def make_sign(self, values) -> str:
+        return make_sign(
+            values, self.api_key, exclude=self.make_sign_exclude, time_key=self.Time
+        )
 
     def channel_make_sign(self, values, sign_key) -> str:
-        return make_sign(values, sign_key, self.make_sign_exclude, self.Time)
+        return make_sign(
+            values, sign_key, exclude=self.make_sign_exclude, time_key=None
+        )
 
     def check_time_out(self, values):
         _time = int(values.get(self.Time, 0))
         t = time.time()
         if self.OutTime != 0 and int(t) - _time > self.OutTime:
             return False
         return True
 
-    def check_public(self):
+    def check_public(self, values) -> bool:
         return True
 
     def sdk_rechfeed(self, error_code, msg="") -> dict:
         if not msg:
             msg = str(error_code.get("msg", ""))
         code = int(error_code.get("code", 0))
         return {"ret": code, "msg": msg}
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/conf/__init__.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/conf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # -*- coding: utf-8 -*-
 # @Author   : pmz
 # @Time     : 2023/05/05 09:57:27
 # @Software : python3.11
 # @Desc     : 设置项目配置, 配置文件懒加载
 import copy
 import operator
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/conf/global_settings.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/conf/global_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # -*- coding: utf-8 -*-
 # @Author   : pmz
 # @Time     : 2023/05/05 09:57:27
 # @Software : python3.11
 # @Desc     : global_settings
 
 # DEBUG
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/aes.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/aes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # -*- coding: utf-8 -*-
 # @Author   : pmz
 # @Time     : 2023/03/28 10:44:11
 # @Software : python3.11
 # @Desc     : AES encryption AES 加密
 from base64 import b64decode, b64encode
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/basic.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # -*- coding: utf-8 -*-
 # @Author   : pmz
 # @Time     : 2023/03/22 16:51:15
 # @Software : python3.11
 # @Desc     : 内置加密模块 -> 加密
 import hashlib
 import hmac
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/make_sign.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/make_sign.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-
 # -*- coding: utf-8 -*-
 # @Author   : pmz
 # @Time     : 2023/04/18 16:36:36
 # @Software : python3.11
 # @Desc     : make_sign
+from typing import Iterable
+
 from yyxx_game_pkg.crypto.basic import md5
 
 
 def make_sign(
     values: dict,
     secret_key: str,
-    exclude: list = None,
     *,
+    exclude: Iterable = None,
     time_key="time",
     make_sign_func=md5,
     make_sign_key: str = None,
     digest_mod=None,
-):
+) -> str:
     """
     签名方法
     :param values: 需要加密的数据（字典）
     :param secret_key: 加密秘钥
     :param exclude: 字段名可选列表，如果提供，加密时会排除其中字段，然后进行加密
     :param time_key: 获取时间戳的字段名；默认为 time
     :param make_sign_func: 进行加密的方法
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/crypto/rsa.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/rsa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # -*- coding: utf-8 -*-
 # @Author   : pmz
 # @Time     : 2023/04/20 20:02:59
 # @Software : python3.11
 # @Desc     : rsa
 import base64
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/base.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/ch_op.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/ch_op.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         获取单条数据
         :param sql:
         :return:
         """
         res_df = self.get_all_df(sql)
         if not res_df.empty:
             return res_df.iloc[0]
-        return pd.Series()
+        return pd.Series(dtype=str)
 
     def get_all_df(self, sql):
         """
         获取所有数据 dataframe
         :param sql:
         :return:
         """
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/das_api.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/das_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         clickhouse 执行 sql (数据插入)
         :param das_url: das_http_url
         :param post_data: {
             "sql": sql,                     # sql语句
         }
         :return:
         """
-        b_ok, res = DasApi._post(das_url, "/das/ch/query", post_data=post_data)
+        b_ok, res = DasApi._post(das_url, "/das/ch/exec", post_data=post_data)
         if not b_ok:
             raise Exception(res)
         return b_ok
 
 
 # if __name__ == '__main__':
 # post_type = "das/mgo/query"
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/es_op.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/es_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/hdfs_op.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/hdfs_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/mongo_op.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/mongo_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/dbops/mysql_op.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/mysql_helper.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/mysql_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,43 +2,47 @@
 """
 @File: mysql_helper.py
 @Author: ltw
 @Time: 2023/3/22
 """
 import pymysql
 from dbutils.pooled_db import PooledDB
+from pymysql.cursors import Cursor
+
+from yyxx_game_pkg.logger.log import root_log
 from yyxx_game_pkg.utils.decorator import (
     except_monitor,
     log_execute_time_monitor,
     singleton_unique_obj_args,
 )
-from yyxx_game_pkg.logger.log import root_log
 
 
 # ####################################################
 class MysqlConfig:
     HOST = None
     PORT = None
     USER = None
     PASSWD = None
     DB = None
     USE_UNICODE = None
     CHARSET = None
     MAX_CACHED = None
     MAX_CONNECTIONS = None
+    CURSOR = None
 
     def __str__(self):
-        return "host:{},port:{},db:{},use_unicode:{},charset:{},max_cache:{},max_connections:{}".format(
+        return "host:{},port:{},db:{},use_unicode:{},charset:{},max_cache:{},max_connections:{},cursor:{}".format(
             self.HOST,
             self.PORT,
             self.DB,
             self.USE_UNICODE,
             self.CHARSET,
             self.MAX_CACHED,
             self.MAX_CONNECTIONS,
+            self.CURSOR,
         )
 
 
 @singleton_unique_obj_args
 class MysqlDbPool(object):
     def __init__(self, config: MysqlConfig):
         self.DB_POOL = PooledDB(
@@ -48,14 +52,15 @@
             host=config.HOST,
             port=config.PORT,
             user=config.USER,
             passwd=config.PASSWD,
             db=config.DB,
             use_unicode=config.USE_UNICODE,
             charset=config.CHARSET,
+            cursorclass=config.CURSOR,
         )
         root_log(f"<MysqlDbPool> init, info:{config}")
 
     @except_monitor
     @log_execute_time_monitor()
     def get_connection(self):
         return self.DB_POOL.connection()
@@ -77,9 +82,10 @@
         USER = config["user"]
         PASSWD = config["password"]
         DB = config["db"]
         USE_UNICODE = config.get("use_unicode", True)
         CHARSET = config.get("charset", "utf8")
         MAX_CACHED = config.get("maxcached", 0)
         MAX_CONNECTIONS = config.get("maxconnections", 0)
+        CURSOR = config.get("cursor", Cursor)
 
     return MysqlDbPool(Config())
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/op_helper.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/op_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 # @Author   : pmz
 # @Time     : 2023/04/23 09:57:04
 # @Software : python3.11
 # @Desc     : 操作数据库的类, 继承使用（mysql, redis）
 import datetime
 import json
 
+from pymysql.cursors import Cursor, DictCursor
 from yyxx_game_pkg.conf import settings
 from yyxx_game_pkg.dbops.mysql_op import MysqlOperation
 from yyxx_game_pkg.helpers.mysql_helper import get_dbpool
 from yyxx_game_pkg.helpers.redis_helper import get_redis
 
 
 class OPHelper:
     # --------------- mysql start ---------------
     @classmethod
-    def connection(cls, mysql_alias="default"):
+    def connection(cls, mysql_alias="default", dict_cursor=True):
         db_settings = {}
         for k, v in settings.DATABASES[mysql_alias].items():
-            if v.isdigit():  # PORT 必须为数字
+            if k == "PORT" and isinstance(v, str) and v.isdigit():  # PORT 必须为数字
                 v = int(v)
             db_settings[k.lower()] = v
             if k == "NAME":
                 db_settings["db"] = db_settings.pop("name")
+        db_settings["cursor"] = DictCursor if dict_cursor else Cursor
         return get_dbpool(db_settings).get_connection()
 
     @classmethod
     def mp(cls):
         return MysqlOperation()
 
     @classmethod
@@ -75,22 +77,32 @@
         if isinstance(data, bytes):
             data = eval(json.loads(data))
 
         return data
 
     @classmethod
     def cache_sql_one(
-        cls, sql, redis_key, ex=None, redis_alias="default", mysql_alias="default"
+        cls,
+        sql,
+        redis_key,
+        ex=None,
+        redis_alias="default",
+        mysql_alias="default",
     ):
         sql_func = cls.mp().get_one
         return cls.cache(sql, sql_func, redis_key, ex, redis_alias, mysql_alias)
 
     @classmethod
     def cache_sql_all(
-        cls, sql, redis_key, ex=None, redis_alias="default", mysql_alias="default"
+        cls,
+        sql,
+        redis_key,
+        ex=None,
+        redis_alias="default",
+        mysql_alias="default",
     ):
         sql_func = cls.mp().get_all
         return cls.cache(sql, sql_func, redis_key, ex, redis_alias, mysql_alias)
 
     # --------------- redis cache end ---------------
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/pika_helper.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/pika_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/helpers/redis_helper.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/redis_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/ip2region.xdb` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/ip2region.xdb`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/ip_x.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/ip_x.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/ip2region/xdbSearcher.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/xdbSearcher.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/config.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/handlers.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/logger/log.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/common/common.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/common/common.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/manager.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/manager.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/structs.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/structs.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/core/workflows.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/workflows.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/dispatch.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/logic/task_logic.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/logic/task_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/route.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/route.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/__init__.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/rule_base.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/rule_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/log.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/logic/submit_logic.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/logic/submit_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/submit/submit.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/xcelery/instance.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/xcelery/instance.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/stat/xcelery/task_base.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/xcelery/task_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     # time_param = ("time", int(time.time())
 
     # 根据接口文档填写 params 的键值
     # params key: post_data的键
     # params value: kwargs的键
     # --> post_data[key] = kwargs[value]
     params = {}
+    sdk_exclude = ()
 
     # 父类中核心代码，此处可删除
     # def run_check_token(self, *args, **kwargs) -> dict:
     #     """
     #     run check token
     #     """
     #     sdk_helper, response_helper = self.sdk_version_choice(**kwargs)
@@ -32,30 +33,31 @@
     #         return self.sdk_rechfeed(ErrorCode.ERROR_INVALID_PARAM)
     #
     #     channel_data, post_data = sdk_helper(**kwargs)
     #     response = self.sdk_check_token(channel_data, post_data)
     #
     #     return response_helper(response, **kwargs)
 
-    def sdk_helper(self, **kwargs) -> (dict, dict):
+    def sdk_helper(self, sdk_exclude=(), **kwargs) -> (dict, dict):
         """
         channel_data = kwargs.get("channel_data", {})
 
         post_data = {}
         for k, v in self._params.items():
             post_data[k] = kwargs.get(v)
-        if self.time_param:
-            post_data[self.time_param[0]] = self.time_param[1]
-        if self.sign_param:
-            post_data[self.sign_param] = self.channel_make_sign(
+        if self.Time not in sdk_exclude:
+            post_data[self.Time] = int(time.time())
+        if self.Flag not in sdk_exclude:
+            post_data[self.Flag] = self.channel_make_sign(
                 post_data, channel_data.get("app_key", "")
             )
 
         return channel_data, post_data
 
+        :param sdk_exclude: exclude parameters
         :param kwargs: 参数
         :return: channel_data, post_data
 
         --------------------------------
         如果 post_data 有修改或者补充，可以在此方法中添加
         channel_data, post_data = super().sdk_helper(**kwargs)
         post_data["需要修改或添加的键"] = "需要修改或添加的值"
@@ -70,25 +72,39 @@
         可以在此方法中重写
         :param values: sdk_helper 中的 post_data
         :param sign_key: sdk_helper 中的 channel_data.get("app_key", "")
         :return: 签名字符串
         """
         return super().channel_make_sign(values, sign_key)
 
+    def sdk_check_token(self, channel_data, post_data):
+        """
+        默认使用 登录验证URL进行二次验证
+
+        如果不是使用登录验证URL的方式进行二次验证
+        重写此方法进行验证
+        同时，可以删除 sdk_helper 和 channel_make_sign
+
+        return 的值在 response_helper 中使用
+        具体返回什么视情况而定
+        """
+        return super().sdk_check_token(channel_data, post_data)
+
     def response_helper(self, response: dict, **kwargs) -> dict:
         """
         返回数据
         根据渠道文档，设置返回数据
         """
         if response and response["code"] == 0:
             data = {
                 # ----- ret,user_id为必传参数 ------
                 "ret": 1,
                 "user_id": kwargs["?"],  # ? 值根据具体参数填写
                 # --------------------------------
+                # 如果还有其他参数, 按需添加
             }
             return data
 
         return super().response_helper(response, **kwargs)
 
     # sdk 版本映射，一般不需要改变，此处可删除
     # @property
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,75 +5,74 @@
 # @Desc     : TODO
 from yyxx_game_pkg.center_api.sdk.recharge import BaseRecharge
 
 from .map_factor import MapRecharge
 
 
 class Recharge(MapRecharge, BaseRecharge):
-    """
-    类属性默认值
-    @param extra_key = "extra"
-    @param cp_order_id_key = None
-    @param order_id_key = "orderId"
-    @param platform_order_id_key = "orderId"
-    @param product_type = "coin"
-
-    按需修改
-    """
-
     # 父类中核心代码，此处可删除
     # def get_params(self, data) -> dict:
-    #     extra = data.get(self.extra_key, "")
+    #     self.modify_params()
+    #     extra = data.get(self.params.extra, "")
     #     if not extra:
     #         return {}
     #
     #     ext_ary = extra.split(",")
     #     data_ary = {"extra": extra}
     #     self.get_params_core(data, data_ary, ext_ary)
     #     self.get_params_helper(data, data_ary)
     #
     #     return data_ary
 
+    def modify_params(self):
+        """
+        修改 self.params 属性
+        默认值:
+            extra: str = "extra"
+            cp_order_id: str = "billno"
+            channel_order_id: str = "order_id"
+            player_id: str = "role_id"
+            channel_username: str = "openid"
+            is_check_username: int = 1
+            is_test: int = 0
+
+        self.params.cp_order_id = "xxx"
+        """
+        pass
+
     # 项目通用方法，一般不需要修改，直接使用父类方法，此处可删除
     def get_params_core(self, data, data_ary, ext_ary) -> None:
         """
         --------------------------------
         默认获取以下数据
-        data_ary["cp_platform"] = data.get("cp_platform", "")
-        data_ary["platCode"] = ext_ary[0]  # 渠道商
-        data_ary["game_channel_id"] = ext_ary[1]  # 渠道ID
-        data_ary["serverID"] = ext_ary[2]  # 服ID
-        data_ary["roleID"] = ext_ary[3]  # 角色ID
-        data_ary["cpOrderID"] = (
-            ext_ary[4]
-            if self.cp_order_id_key is None
-            else data.get(self.cp_order_id_key, "")
-        )  # 厂商订单ID，由厂商生成
-        data_ary["orderID"] = data.get(self.order_id_key, "")  # 渠道方订单ID
-        data_ary["platformOrderId"] = data.get(self.platform_order_id_key, "")  # 渠道方订单ID（C表要用）
+        data_ary["cp_order_id"] = data.get(self.params.cp_order_id, "")
+        data_ary["channel_order_id"] = data.get(self.params.channel_order_id, "")
+        data_ary["player_id"] = data.get(self.params.player_id)
+        data_ary["is_check_username"] = self.params.is_check_username
+        data_ary["channel_username"] = data.get(self.params.channel_username, "")
         if len(ext_ary) > 6:
             data_ary["recharge_id"] = int(ext_ary[5])
-        data_ary["productType"] = self.product_type
-        data_ary["productID"] = ""
         --------------------------------
         """
         super().get_params_core(data, data_ary, ext_ary)
 
     def get_params_helper(self, data, data_ary) -> None:
         """
+        补充数据, 添加额外参数
         对 get_params 中 data_ary 数据的补充
         无法在 get_params_core 中通过通用方式获得的参数，在此处进行处理
         --------------------------------
-        e.g. currency promotion extraGoldBindProportion extraGoldBind
-        data_ary["currency"] = data.get("currency", "")
-        data_ary["promotion"] = ""
-        data_ary["extraGoldBindProportion"] = ""
-        data_ary["extraGoldBind"] = ""
+        money  金额
+        real_money  实付金额
+        extra_gold  赠送元宝（渠道返利）
+        extra_gold_bind  赠送绑元（渠道返利）
+        pay_dt 充值时间（秒）
         --------------------------------
         """
+        super().get_params_helper(data, data_ary)
 
     def make_sign_helper(self, values) -> (dict, str):
         """
         ext_ary = values[self.extra_key].split(",")
         plat_code = ext_ary[0]
         game_channel_id = ext_ary[1]
         sdk_data = self.operator.get_key(plat_code, game_channel_id)
@@ -91,17 +90,17 @@
         --------------------------------
         """
         return super().make_sign_helper(values)
 
     # 签名核心方法，此处可删除
     # def make_sign(self, values, sign_key=None) -> str:
     #     values, pay_key = self.make_sign_helper(values)
-    #     return self.channel_make_sign(values, sign_key)
+    #     return self.channel_make_sign(values, pay_key)
 
-    def channel_make_sign(self, values, sign_key=None) -> str:
+    def channel_make_sign(self, values, sign_key) -> str:
         """
         默认签名方式为  md5(yyxx_game_pkg.crypto.basic.md5)
             post_data 中的键按照首字母升序排列
 
         也可继承或重新 MapRecharge MapFactor 中的方法
 
         :return: 签名字符串
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/decorator.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/error_code.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/error_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # -*- coding: utf-8 -*-
 # @Author   : pmz
 # @Time     : 2023/04/19 15:27:41
 # @Software : python3.11
 # @Desc     : TODO
 class ErrorCode:
     # 基本错误码
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/profiler.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xListStr.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xListStr.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xdataframe.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xdataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,19 +93,20 @@
     :return:
     """
     if isinstance(data, pd.DataFrame):
         return data.apply(cal_round_rate, args=(precision, suffix), axis=0)
     if isinstance(data, pd.Series):
         if str(invalid_value).isdigit():
             data = data.fillna(invalid_value)
+        data = data.astype(float).round(precision)
         if precision == 0:
             data = data.astype(int)
-        else:
-            data = data.astype(float).round(precision)
-        return data.apply(lambda d: invalid_value if (d == np.inf or np.isnan(d)) else f"{d}{suffix}")
+        return data.apply(
+            lambda d: invalid_value if (d == np.inf or np.isnan(d)) else f"{d}{suffix}"
+        )
     if isinstance(data, (int, float)):
         if np.isnan(data) or data == np.inf:
             return invalid_value
         if precision == 0:
             return str(int(data)) + suffix
         return str(round(data, precision)) + suffix
     return invalid_value
@@ -268,27 +269,44 @@
         return labels, bins[position]
 
     return _df.apply(cut_bins, axis=1, result_type="expand")
 
 
 def div_rate(data_df: pd.DataFrame, top_key, bottom_key, precision=2) -> pd.Series:
     """
-    dataframe div函数计算百分比
+    dataframe div函数计算百分比 top_key / bottom_key
     example:
         data_df["pay_rate"] = div_rate(data_df, "pid_cnt", "act_player_cnt")
     :return:
     """
+    if isinstance(top_key, list):
+        return (
+            data_df[top_key]
+            .div(data_df[bottom_key], axis=0)
+            .round(precision + 2)
+            .applymap(lambda x: f"{round(x * 100, precision) }%")
+        )
     return (
         data_df[top_key]
         .div(data_df[bottom_key], axis=0)
         .round(precision + 2)
         .apply(lambda x: f"{round(x * 100, precision) }%")
     )
 
 
+def div_round(data_df: pd.DataFrame, top_key, bottom_key, precision=2) -> pd.Series:
+    """
+    dataframe div函数 top_key / bottom_key
+    example:
+        data_df["pay_rate"] = div_round(data_df, "pid_cnt", "act_player_cnt")
+    :return:
+    """
+    return data_df[top_key].div(data_df[bottom_key], axis=0).round(precision)
+
+
 def concat_cols(data_df: pd.DataFrame, cols: list, concat_by="|") -> pd.Series:
     """
     合将列，汇总后的列为：recharge_cnt|recharge_type_id
     example:
         data_df["show_pid_cnt"] = concat_cols(data_df, ["pid_cnt", "pid_rate"]) -> 98|10.0%
     """
     res = None
@@ -297,8 +315,7 @@
             res = data_df[col].astype(str)
         else:
             res = res + data_df[col].astype(str)
         if col == cols[-1]:
             continue
         res = res + concat_by
     return res
-
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xdate.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xdate.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import time
 import datetime
 from enum import Enum
 
 DAY = 1
 WEEK = 2
 MONTH = 3
+VERSION = 4
 
 
 # 时间转换
 def str2date(date_str):
     """
     时间字符串转datetime obj
     """
@@ -77,31 +78,59 @@
     "2021-05-31 12:23:40" to "2021-05-31 23:59:59"
     :param date: datetime obj
     :return: datetime obj
     """
     return date2dt_day(date, 23, 59, 59)
 
 
-def day2date(day, fmt="%Y%m%d") -> datetime.datetime:
+def day2date(day, fmt="%Y%m%d", end=0) -> datetime.datetime:
     """
     "20210531" to "2021-05-31 00:00:00"
     :param day: 时间字符串
     :param fmt: 时间字符串格式 默认 "%Y%m%d"
+    :param end: 0: 00:00:00; 1: 23:59:59
     :return: datetime obj
     """
-    return datetime.datetime.strptime(str(day), fmt)
+    date = datetime.datetime.strptime(str(day), fmt)
+    if end:
+        return datetime.datetime(date.year, date.month, date.day, 23, 59, 59)
+    return date
+
+
+def day2str_date(day) -> str:
+    """
+    '20220301' -> '2022-03-01'
+    效率更高
+    """
+    day_s = str(day)
+    return day_s[:4] + '-' + day_s[4:6] + '-' + day_s[6:]
 
 
 def date2day(date):
     """
     "2021-05-31 12:23:40" to "20210531"
     """
     return date.strftime("%Y%m%d")
 
 
+def date2date(date, _h=0, _m=0, _s=0, end=0):
+    """
+    "2021-05-31 12:23:40" to "2021-05-31 00:00:00"
+    :param date: datetime obj
+    :param _h: hour
+    :param _m: minute
+    :param _s: second
+    :param end: 0: 00:00:00; 1: 23:59:59
+    :return: datetime obj
+    """
+    if end:
+        return datetime.datetime(date.year, date.month, date.day, 23, 59, 59)
+    return datetime.datetime(date.year, date.month, date.day, int(_h), int(_m), int(_s))
+
+
 def day_diff(day1, day2):
     """
     day_diff(20210531, 20210529) -> 2
     """
     return (day2date(day2) - day2date(day1)).days
 
 
@@ -113,15 +142,19 @@
     :param end: 0: 00:00:00 / 1: 23:59:59
     :return:
     """
     if end:
         return date2dt_day_end(date) + datetime.timedelta(days=delta)
     return date2dt_day(date) + datetime.timedelta(days=delta)
 
+
 def add_days(date, delta, end=0):
+    """
+    易读接口
+    """
     return delta_dt_day(date, delta, end)
 
 
 def date2stamp(dt_date):
     """
     datetime转时间戳
     """
@@ -152,29 +185,37 @@
     sdate = datetime.datetime.strptime(str(date), fmt)
     _, _, s_week_day = sdate.isocalendar()
     sday = (sdate - datetime.timedelta(days=s_week_day - 1)).strftime("%Y-%m-%d")
     eday = (sdate - datetime.timedelta(days=s_week_day - 7)).strftime("%Y-%m-%d")
     return f"{sday}~{eday}"
 
 
-def date_type_trans(date, date_type=DAY, fmt="%Y%m%d"):
+def date_type_trans(day, date_type=DAY, fmt="%Y%m%d", version_configs=None):
     """
     周期时间格式化
-    :param date: 时间字符串
+    :param day: 时间字符串 20230201
     :param date_type: 周期类型(1: 天 2: 周 3: 月)
     :param fmt: 时间字符串格式 默认 "%Y%m%d"
+    :param version_configs: 版本配置list [[版本号, 开始day, 结束day]]
     :return: 周期字符串
     """
     if date_type == DAY:
-        return datetime.datetime.strptime(str(date), fmt).strftime("%Y-%m-%d")
+        return datetime.datetime.strptime(str(day), fmt).strftime("%Y-%m-%d")
     if date_type == WEEK:
-        return get_week_str(date, fmt)
+        return get_week_str(day, fmt)
     if date_type == MONTH:
-        return datetime.datetime.strptime(str(date), fmt).strftime("%Y年%m月")
-    return date
+        return datetime.datetime.strptime(str(day), fmt).strftime("%Y年%m月")
+    if date_type == VERSION:
+        if version_configs is None:
+            return day
+        for version, start_day, end_day in version_configs:
+            if start_day <= day <= end_day:
+                return f"{version}版本"
+        return "未配置版本"
+    return day
 
 
 def to_start_of_interval(_t: datetime.datetime, unit="minute", interval=5):
     """
     to_start_of_interval("2023-03-09 11:16:20", 'minute', interval=5) -> datetime(2023-03-09 11:15:00)
     to_start_of_interval("2023-03-09 11:16:20", 'hour', interval=1) -> datetime(2023-03-09 11:00:00)
     """
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xhttp.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xhttp.py`

 * *Files 15% similar despite different names*

```diff
@@ -103,7 +103,28 @@
 
     post_data_log = json.dumps(post_data, ensure_ascii=False)
     local_log(f"http_push_server url:{url} post_data: {post_data_log}")
 
     result = http_request(url, post_data, False, "get")
     local_log(f"http_push_server url:{url} res: {result}")
     return result
+
+
+def make_post_data(ex_params, api_key):
+    """
+    生成post_data
+    """
+    _t = int(time.time())
+    values = {"time": _t, "params": json.dumps(ex_params)}
+    keys = values.keys()
+    keys = sorted(keys)
+    params = []
+    for key in keys:
+        params.append(f"{key}={values[key]}")
+    params = "&".join(params)
+    timestamp = str(_t + (_t % 38975))
+    _tmp = md5(f"{params}{api_key}")
+    sign = md5(f"{timestamp}{_tmp}")
+
+    post_data = {"time": _t, "params": ex_params, "sign": sign}
+    post_data = set_params(post_data)
+    return post_data
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xmath.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xmath.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/utils/xstring.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xstring.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # -*- coding: utf-8 -*-
 # @Author   : pmz
 # @Time     : 2023/04/13 17:28:50
 # @Software : python3.11
 # @Desc     : string
 import json
```

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/yyxx_game_pkg/xtrace/helper.py` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/xtrace/helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.5.17.1.dev5/PKG-INFO` & `yyxx_game_pkg_dev-2023.6.9.1.dev8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yyxx-game-pkg-dev
-Version: 2023.5.17.1.dev5
+Version: 2023.6.9.1.dev8
 Summary: yyxx game custom module
 Home-page: https://github.com/yyxxgame/yyxxgame-pkg
 License: MIT
 Author: yyxx-game
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,35 +12,36 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: center-api
 Provides-Extra: server-center
 Provides-Extra: stat
-Requires-Dist: celery (>=5.2.7,<6.0.0)
+Requires-Dist: celery (==5.2.7)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0) ; extra == "center-api"
 Requires-Dist: dbutils (>=3.0.2,<4.0.0)
 Requires-Dist: django (>=4.2.1,<5.0.0) ; extra == "server-center"
 Requires-Dist: fastapi (>=0.94.0,<0.95.0) ; extra == "stat"
 Requires-Dist: filetype (>=1.2.0,<2.0.0) ; extra == "server-center"
 Requires-Dist: flask (>=2.3.2,<3.0.0) ; extra == "center-api"
 Requires-Dist: line-profiler (>=4.0.3,<5.0.0)
 Requires-Dist: opentelemetry-api (>=1.16.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-jaeger (>=1.16.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation-celery (==0.37b0)
 Requires-Dist: opentelemetry-instrumentation-fastapi (==0.37b.0)
+Requires-Dist: opentelemetry-instrumentation-flask (>=0.37b0,<0.38)
 Requires-Dist: opentelemetry-instrumentation-requests (>=0.37b0,<0.38)
 Requires-Dist: opentelemetry-sdk (>=1.16.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0) ; extra == "server-center"
 Requires-Dist: pycryptodome (>=3.17,<4.0)
 Requires-Dist: pymysql (>=1.0.2,<2.0.0)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (==2.27.1)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
 Project-URL: Repository, https://github.com/yyxxgame/yyxxgame-pkg
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,38 +1,39 @@
-Metadata-Version: 2.1 Name: yyxx-game-pkg-dev Version: 2023.5.17.1.dev5
-Summary: yyxx game custom module Home-page: https://github.com/yyxxgame/
-yyxxgame-pkg License: MIT Author: yyxx-game Requires-Python: >=3.8,<4
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Provides-Extra: center-api Provides-
-Extra: server-center Provides-Extra: stat Requires-Dist: celery
-(>=5.2.7,<6.0.0) Requires-Dist: cookiecutter (>=2.1.1,<3.0.0) ; extra ==
-"center-api" Requires-Dist: dbutils (>=3.0.2,<4.0.0) Requires-Dist: django
-(>=4.2.1,<5.0.0) ; extra == "server-center" Requires-Dist: fastapi
-(>=0.94.0,<0.95.0) ; extra == "stat" Requires-Dist: filetype (>=1.2.0,<2.0.0) ;
-extra == "server-center" Requires-Dist: flask (>=2.3.2,<3.0.0) ; extra ==
-"center-api" Requires-Dist: line-profiler (>=4.0.3,<5.0.0) Requires-Dist:
-opentelemetry-api (>=1.16.0,<2.0.0) Requires-Dist: opentelemetry-exporter-
-jaeger (>=1.16.0,<2.0.0) Requires-Dist: opentelemetry-instrumentation-celery
-(==0.37b0) Requires-Dist: opentelemetry-instrumentation-fastapi (==0.37b.0)
-Requires-Dist: opentelemetry-instrumentation-requests (>=0.37b0,<0.38)
-Requires-Dist: opentelemetry-sdk (>=1.16.0,<2.0.0) Requires-Dist: pandas
-(>=1.5.3,<2.0.0) Requires-Dist: pika (>=1.3.1,<2.0.0) Requires-Dist: pillow
-(>=9.5.0,<10.0.0) ; extra == "server-center" Requires-Dist: pycryptodome
-(>=3.17,<4.0) Requires-Dist: pymysql (>=1.0.2,<2.0.0) Requires-Dist: redis
-(>=4.5.1,<5.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: toml
-(>=0.10.2,<0.11.0) Requires-Dist: ujson (>=5.7.0,<6.0.0) Requires-Dist: uvicorn
-(>=0.21.0,<0.22.0) Project-URL: Repository, https://github.com/yyxxgame/
-yyxxgame-pkg Description-Content-Type: text/markdown # YYXXGAME-PKG `yyxx-game-
-pkg` æ¯ä¸ä¸ªä¸é¨ä¸ºåæ¸¸å¬å¸åå°å¼åç Python åé¨æ¥å£éåã
-[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![MIT License][license-shield]][license-url]
+Metadata-Version: 2.1 Name: yyxx-game-pkg-dev Version: 2023.6.9.1.dev8 Summary:
+yyxx game custom module Home-page: https://github.com/yyxxgame/yyxxgame-pkg
+License: MIT Author: yyxx-game Requires-Python: >=3.8,<4 Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Provides-Extra: center-api Provides-Extra: server-
+center Provides-Extra: stat Requires-Dist: celery (==5.2.7) Requires-Dist:
+cookiecutter (>=2.1.1,<3.0.0) ; extra == "center-api" Requires-Dist: dbutils
+(>=3.0.2,<4.0.0) Requires-Dist: django (>=4.2.1,<5.0.0) ; extra == "server-
+center" Requires-Dist: fastapi (>=0.94.0,<0.95.0) ; extra == "stat" Requires-
+Dist: filetype (>=1.2.0,<2.0.0) ; extra == "server-center" Requires-Dist: flask
+(>=2.3.2,<3.0.0) ; extra == "center-api" Requires-Dist: line-profiler
+(>=4.0.3,<5.0.0) Requires-Dist: opentelemetry-api (>=1.16.0,<2.0.0) Requires-
+Dist: opentelemetry-exporter-jaeger (>=1.16.0,<2.0.0) Requires-Dist:
+opentelemetry-instrumentation-celery (==0.37b0) Requires-Dist: opentelemetry-
+instrumentation-fastapi (==0.37b.0) Requires-Dist: opentelemetry-
+instrumentation-flask (>=0.37b0,<0.38) Requires-Dist: opentelemetry-
+instrumentation-requests (>=0.37b0,<0.38) Requires-Dist: opentelemetry-sdk
+(>=1.16.0,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: pika
+(>=1.3.1,<2.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) ; extra == "server-
+center" Requires-Dist: pycryptodome (>=3.17,<4.0) Requires-Dist: pymysql
+(>=1.0.2,<2.0.0) Requires-Dist: redis (>=4.5.1,<5.0.0) Requires-Dist: requests
+(==2.27.1) Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: ujson
+(>=5.7.0,<6.0.0) Requires-Dist: uvicorn (>=0.21.0,<0.22.0) Project-URL:
+Repository, https://github.com/yyxxgame/yyxxgame-pkg Description-Content-Type:
+text/markdown # YYXXGAME-PKG `yyxx-game-pkg`
+æ¯ä¸ä¸ªä¸é¨ä¸ºåæ¸¸å¬å¸åå°å¼åç Python åé¨æ¥å£éåã  [!
+[Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
+[forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
+[issues-url] [![MIT License][license-shield]][license-url]
                                 [åæ¸¸ä¿¡æ¯]
                             **** åæ¸¸ä¿¡æ¯ ****
 ## ç®å½ - [ä¸ææå](#ä¸ææå) - [ç¯å¢éç½®](#ç¯å¢éç½®) -
 [å®è£æ­¥éª¤](#å®è£æ­¥éª¤) - [æä»¶ç®å½è¯´æ](#æä»¶ç®å½è¯´æ) -
 [é¨ç½²](#é¨ç½²) - [develop](#develop) - [release](#release) - [æ¨¡åä»ç»]
 (#æ¨¡åä»ç») - [xtrace](#xtrace) - [stat](#stat) - [ä»£ç ç¤ºä¾]
 (#ä»£ç ç¤ºä¾) - [çæ¬æ§å¶](#çæ¬æ§å¶) ### ä¸ææå ######
```

