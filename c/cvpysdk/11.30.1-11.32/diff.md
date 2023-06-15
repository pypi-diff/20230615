# Comparing `tmp/cvpysdk-11.30.1.tar.gz` & `tmp/cvpysdk-11.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvpysdk-11.30.1.tar", last modified: Thu Feb 23 10:25:19 2023, max compression
+gzip compressed data, was "cvpysdk-11.32.tar", last modified: Thu Jun 15 08:11:27 2023, max compression
```

## Comparing `cvpysdk-11.30.1.tar` & `cvpysdk-11.32.tar`

### file list

```diff
@@ -1,279 +1,280 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.921885 cvpysdk-11.30.1/
--rw-rw-rw-   0        0        0    11531 2021-08-25 13:01:50.000000 cvpysdk-11.30.1/LICENSE.txt
--rw-rw-rw-   0        0        0       71 2021-08-25 13:01:50.000000 cvpysdk-11.30.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7312 2023-02-23 10:25:19.921885 cvpysdk-11.30.1/PKG-INFO
--rw-rw-rw-   0        0        0     6743 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:18.835152 cvpysdk-11.30.1/cvpysdk/
--rw-rw-rw-   0        0        0     1349 2023-02-23 10:05:44.000000 cvpysdk-11.30.1/cvpysdk/__init__.py
--rw-rw-rw-   0        0        0     6845 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/activate.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:18.915922 cvpysdk-11.30.1/cvpysdk/activateapps/
--rw-rw-rw-   0        0        0      866 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/activateapps/__init__.py
--rw-rw-rw-   0        0        0    34155 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/activateapps/constants.py
--rw-rw-rw-   0        0        0   136983 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/activateapps/ediscovery_utils.py
--rw-rw-rw-   0        0        0   101465 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/activateapps/entity_manager.py
--rw-rw-rw-   0        0        0    36915 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/activateapps/file_storage_optimization.py
--rw-rw-rw-   0        0        0    45578 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/activateapps/inventory_manager.py
--rw-rw-rw-   0        0        0    34226 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/activateapps/request_manager.py
--rw-rw-rw-   0        0        0    20756 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/activateapps/sensitive_data_governance.py
--rw-rw-rw-   0        0        0    10277 2021-08-25 13:01:50.000000 cvpysdk-11.30.1/cvpysdk/activitycontrol.py
--rw-rw-rw-   0        0        0    34248 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/agent.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:18.915922 cvpysdk-11.30.1/cvpysdk/agents/
--rw-rw-rw-   0        0        0      863 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/agents/__init__.py
--rw-rw-rw-   0        0        0     7472 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/agents/exchange_database_agent.py
--rw-rw-rw-   0        0        0    45679 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/alert.py
--rw-rw-rw-   0        0        0    26387 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/array_management.py
--rw-rw-rw-   0        0        0    10120 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backup_network_pairs.py
--rw-rw-rw-   0        0        0    91115 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/backupset.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:18.994046 cvpysdk-11.30.1/cvpysdk/backupsets/
--rw-rw-rw-   0        0        0      863 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.009676 cvpysdk-11.30.1/cvpysdk/backupsets/_virtual_server/
--rw-rw-rw-   0        0        0      876 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/_virtual_server/__init__.py
--rw-rw-rw-   0        0        0     2501 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/_virtual_server/kubernetes.py
--rw-rw-rw-   0        0        0    10718 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/_virtual_server/vmware.py
--rw-rw-rw-   0        0        0    18407 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/aadbackupset.py
--rw-rw-rw-   0        0        0     3275 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/adbackupset.py
--rw-rw-rw-   0        0        0     2695 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/cabackupset.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.009676 cvpysdk-11.30.1/cvpysdk/backupsets/cloudapps/
--rw-rw-rw-   0        0        0      874 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/cloudapps/__init__.py
--rw-rw-rw-   0        0        0     9083 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/cloudapps/salesforce_backupset.py
--rw-rw-rw-   0        0        0    11908 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/backupsets/db2backupset.py
--rw-rw-rw-   0        0        0    70921 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/backupsets/fsbackupset.py
--rw-rw-rw-   0        0        0     4615 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/backupsets/hanabackupset.py
--rw-rw-rw-   0        0        0     3639 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/nasbackupset.py
--rw-rw-rw-   0        0        0    11438 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/backupsets/postgresbackupset.py
--rw-rw-rw-   0        0        0     3721 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/backupsets/sharepointbackupset.py
--rw-rw-rw-   0        0        0    12986 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/backupsets/vsbackupset.py
--rw-rw-rw-   0        0        0     6246 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/certificates.py
--rw-rw-rw-   0        0        0   263502 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/client.py
--rw-rw-rw-   0        0        0    74888 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/clientgroup.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.025295 cvpysdk-11.30.1/cvpysdk/clients/
--rw-rw-rw-   0        0        0      860 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/clients/__init__.py
--rw-rw-rw-   0        0        0     6864 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/clients/onedrive_client.py
--rw-rw-rw-   0        0        0     9029 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/clients/vmclient.py
--rw-rw-rw-   0        0        0   126125 2023-02-23 10:08:17.000000 cvpysdk-11.30.1/cvpysdk/commcell.py
--rw-rw-rw-   0        0        0    24381 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/commcell_migration.py
--rw-rw-rw-   0        0        0    26730 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/constants.py
--rw-rw-rw-   0        0        0    16567 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/content_analyzer.py
--rw-rw-rw-   0        0        0    23902 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/credential_manager.py
--rw-rw-rw-   0        0        0    17286 2023-02-23 10:09:56.000000 cvpysdk-11.30.1/cvpysdk/cvpysdk.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.062507 cvpysdk-11.30.1/cvpysdk/datacube/
--rw-rw-rw-   0        0        0      879 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/datacube/__init__.py
--rw-rw-rw-   0        0        0     3294 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/datacube/constants.py
--rw-rw-rw-   0        0        0     6634 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/datacube/datacube.py
--rw-rw-rw-   0        0        0    36258 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/datacube/datasource.py
--rw-rw-rw-   0        0        0    18093 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/datacube/handler.py
--rw-rw-rw-   0        0        0     1997 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/datacube/sedstype.py
--rw-rw-rw-   0        0        0    54429 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/deduplication_engines.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.078133 cvpysdk-11.30.1/cvpysdk/deployment/
--rw-rw-rw-   0        0        0      863 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/deployment/__init__.py
--rw-rw-rw-   0        0        0    16603 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/deployment/cache_config.py
--rw-rw-rw-   0        0        0     3543 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/deployment/deploymentconstants.py
--rw-rw-rw-   0        0        0    14304 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/deployment/download.py
--rw-rw-rw-   0        0        0    26684 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/deployment/install.py
--rw-rw-rw-   0        0        0     6862 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/deployment/uninstall.py
--rw-rw-rw-   0        0        0     6091 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/dev_test_group.py
--rw-rw-rw-   0        0        0    42515 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/disasterrecovery.py
--rw-rw-rw-   0        0        0    21603 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/domains.py
--rw-rw-rw-   0        0        0    51805 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/download_center.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.140633 cvpysdk-11.30.1/cvpysdk/drorchestration/
--rw-rw-rw-   0        0        0      882 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/drorchestration/__init__.py
--rw-rw-rw-   0        0        0    48119 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/drorchestration/blr_pairs.py
--rw-rw-rw-   0        0        0     3808 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/drorchestration/dr_orchestration_job_phase.py
--rw-rw-rw-   0        0        0     6911 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/drorchestration/drjob.py
--rw-rw-rw-   0        0        0    33410 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/drorchestration/drorchestrationoperations.py
--rw-rw-rw-   0        0        0    18194 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/drorchestration/failovergroups.py
--rw-rw-rw-   0        0        0    29317 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/drorchestration/replication_groups.py
--rw-rw-rw-   0        0        0     5707 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/drorchestration/replication_pairs.py
--rw-rw-rw-   0        0        0    13215 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/drorchestration/replicationmonitor.py
--rw-rw-rw-   0        0        0     8905 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/eventviewer.py
--rw-rw-rw-   0        0        0    24322 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/exception.py
--rw-rw-rw-   0        0        0     9765 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/globalfilter.py
--rw-rw-rw-   0        0        0    19921 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/hac_clusters.py
--rw-rw-rw-   0        0        0    38514 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/identity_management.py
--rw-rw-rw-   0        0        0    19706 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/index_pools.py
--rw-rw-rw-   0        0        0    53990 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/index_server.py
--rw-rw-rw-   0        0        0   128360 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instance.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.234389 cvpysdk-11.30.1/cvpysdk/instances/
--rw-rw-rw-   0        0        0      862 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/__init__.py
--rw-rw-rw-   0        0        0     2399 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/aadinstance.py
--rw-rw-rw-   0        0        0     2827 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/bigdataappsinstance.py
--rw-rw-rw-   0        0        0     4702 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/cainstance.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.281256 cvpysdk-11.30.1/cvpysdk/instances/cloudapps/
--rw-rw-rw-   0        0        0      873 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/cloudapps/__init__.py
--rw-rw-rw-   0        0        0    23441 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/cloudapps/amazon_instance.py
--rw-rw-rw-   0        0        0     8534 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/cloudapps/cloud_database_instance.py
--rw-rw-rw-   0        0        0    32465 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/cloudapps/cloud_storage_instance.py
--rw-rw-rw-   0        0        0     6414 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/cloudapps/dynamics365_instance.py
--rw-rw-rw-   0        0        0    17755 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/cloudapps/google_instance.py
--rw-rw-rw-   0        0        0    33100 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/cloudapps/salesforce_instance.py
--rw-rw-rw-   0        0        0     5195 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/cloudapps/spanner_instance.py
--rw-rw-rw-   0        0        0    13394 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/cloudapps/teams_instance.py
--rw-rw-rw-   0        0        0    24158 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/db2instance.py
--rw-rw-rw-   0        0        0     4930 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/dbinstance.py
--rw-rw-rw-   0        0        0    18464 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/hanainstance.py
--rw-rw-rw-   0        0        0    15761 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/informixinstance.py
--rw-rw-rw-   0        0        0    16033 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/lndbinstance.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.312512 cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/
--rw-rw-rw-   0        0        0      874 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/__init__.py
--rw-rw-rw-   0        0        0    15182 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/lndbinstance.py
--rw-rw-rw-   0        0        0     8851 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/lndminstance.py
--rw-rw-rw-   0        0        0     9268 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/lndocinstance.py
--rw-rw-rw-   0        0        0     7983 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/lninstance.py
--rw-rw-rw-   0        0        0    22834 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/mysqlinstance.py
--rw-rw-rw-   0        0        0    53422 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/oracleinstance.py
--rw-rw-rw-   0        0        0    24700 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/postgresinstance.py
--rw-rw-rw-   0        0        0    18937 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/saporacleinstance.py
--rw-rw-rw-   0        0        0     9192 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/sharepointinstance.py
--rw-rw-rw-   0        0        0     4584 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/splunkinstance.py
--rw-rw-rw-   0        0        0    61965 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/sqlinstance.py
--rw-rw-rw-   0        0        0    43205 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/sybaseinstance.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.406261 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/
--rw-rw-rw-   0        0        0      862 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/__init__.py
--rw-rw-rw-   0        0        0     5325 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/alibaba_cloud.py
--rw-rw-rw-   0        0        0     5419 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/amazon_web_services.py
--rw-rw-rw-   0        0        0     4316 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/azure.py
--rw-rw-rw-   0        0        0     4810 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/azure_resource_manager.py
--rw-rw-rw-   0        0        0     4861 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/azure_stack.py
--rw-rw-rw-   0        0        0     4183 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/fusioncompute.py
--rw-rw-rw-   0        0        0     3647 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/google_cloud_platform.py
--rw-rw-rw-   0        0        0     4645 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/hyperv.py
--rw-rw-rw-   0        0        0     4422 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/kubernetes.py
--rw-rw-rw-   0        0        0     1177 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/null.py
--rw-rw-rw-   0        0        0     4943 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/nutanix_ahv.py
--rw-rw-rw-   0        0        0     4554 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/openstack.py
--rw-rw-rw-   0        0        0     5320 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/oracle_cloud.py
--rw-rw-rw-   0        0        0     4125 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/oracle_cloud_infrastructure.py
--rw-rw-rw-   0        0        0     4225 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/oraclevm.py
--rw-rw-rw-   0        0        0     4333 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/red_hat_virtualization.py
--rw-rw-rw-   0        0        0     4488 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/vcloud_director.py
--rw-rw-rw-   0        0        0     4401 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/vmware.py
--rw-rw-rw-   0        0        0     4371 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/virtualserver/xen.py
--rw-rw-rw-   0        0        0     2007 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/instances/vminstance.py
--rw-rw-rw-   0        0        0    12871 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/instances/vsinstance.py
--rw-rw-rw-   0        0        0     7827 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/internetoptions.py
--rw-rw-rw-   0        0        0   119031 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/job.py
--rw-rw-rw-   0        0        0    14494 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/key_management_server.py
--rw-rw-rw-   0        0        0    13533 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/license.py
--rw-rw-rw-   0        0        0    20426 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/metallic.py
--rw-rw-rw-   0        0        0    26237 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/metricsreport.py
--rw-rw-rw-   0        0        0    28226 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/monitoring.py
--rw-rw-rw-   0        0        0    23387 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/name_change.py
--rw-rw-rw-   0        0        0    34060 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/network.py
--rw-rw-rw-   0        0        0    13795 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/network_throttle.py
--rw-rw-rw-   0        0        0    36142 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/network_topology.py
--rw-rw-rw-   0        0        0    42158 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/operation_window.py
--rw-rw-rw-   0        0        0   101436 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/organization.py
--rw-rw-rw-   0        0        0   101567 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/plan.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.453136 cvpysdk-11.30.1/cvpysdk/policies/
--rw-rw-rw-   0        0        0      879 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/policies/__init__.py
--rw-rw-rw-   0        0        0    74032 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/policies/configuration_policies.py
--rw-rw-rw-   0        0        0     8072 2021-08-25 13:01:51.000000 cvpysdk-11.30.1/cvpysdk/policies/schedule_options.py
--rw-rw-rw-   0        0        0    44091 2023-02-23 10:00:42.000000 cvpysdk-11.30.1/cvpysdk/policies/schedule_policies.py
--rw-rw-rw-   0        0        0   177102 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/policies/storage_policies.py
--rw-rw-rw-   0        0        0     3033 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/policy.py
--rw-rw-rw-   0        0        0    25265 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/recovery_targets.py
--rw-rw-rw-   0        0        0     7414 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/regions.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.468765 cvpysdk-11.30.1/cvpysdk/reports/
--rw-rw-rw-   0        0        0      860 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/reports/__init__.py
--rw-rw-rw-   0        0        0    19808 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/reports/report.py
--rw-rw-rw-   0        0        0   108687 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/schedules.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.484452 cvpysdk-11.30.1/cvpysdk/security/
--rw-rw-rw-   0        0        0      869 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/security/__init__.py
--rw-rw-rw-   0        0        0    29798 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/security/role.py
--rw-rw-rw-   0        0        0    15983 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/security/security_association.py
--rw-rw-rw-   0        0        0     8966 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/security/two_factor_authentication.py
--rw-rw-rw-   0        0        0    39664 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/security/user.py
--rw-rw-rw-   0        0        0    38056 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/security/usergroup.py
--rw-rw-rw-   0        0        0    28214 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/services.py
--rw-rw-rw-   0        0        0   101928 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/storage.py
--rw-rw-rw-   0        0        0    32786 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/storage_pool.py
--rw-rw-rw-   0        0        0   122709 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclient.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.671890 cvpysdk-11.30.1/cvpysdk/subclients/
--rw-rw-rw-   0        0        0      863 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/__init__.py
--rw-rw-rw-   0        0        0     1952 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/aadsubclient.py
--rw-rw-rw-   0        0        0     4182 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/adsubclient.py
--rw-rw-rw-   0        0        0     4110 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/bigdataappssubclient.py
--rw-rw-rw-   0        0        0    11760 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/casesubclient.py
--rw-rw-rw-   0        0        0     3615 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/casubclient.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.718763 cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/
--rw-rw-rw-   0        0        0      874 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/__init__.py
--rw-rw-rw-   0        0        0     7660 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/cloud_database_subclient.py
--rw-rw-rw-   0        0        0    15228 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/cloud_storage_subclient.py
--rw-rw-rw-   0        0        0    42053 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/dynamics365_subclient.py
--rw-rw-rw-   0        0        0    29846 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/google_subclient.py
--rw-rw-rw-   0        0        0    51907 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/salesforce_subclient.py
--rw-rw-rw-   0        0        0     3329 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/spanner_subclient.py
--rw-rw-rw-   0        0        0     3704 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/teams_constants.py
--rw-rw-rw-   0        0        0    34397 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/teams_subclient.py
--rw-rw-rw-   0        0        0    13162 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/db2subclient.py
--rw-rw-rw-   0        0        0     3424 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/dbsubclient.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.750009 cvpysdk-11.30.1/cvpysdk/subclients/exchange/
--rw-rw-rw-   0        0        0      872 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/exchange/__init__.py
--rw-rw-rw-   0        0        0    13470 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/exchange/contentstoremailbox_subclient.py
--rw-rw-rw-   0        0        0    16906 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/exchange/exchange_database_subclient.py
--rw-rw-rw-   0        0        0    17764 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/exchange/journalmailbox_subclient.py
--rw-rw-rw-   0        0        0    71672 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/exchange/usermailbox_subclient.py
--rw-rw-rw-   0        0        0    32624 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/exchsubclient.py
--rw-rw-rw-   0        0        0    98208 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/fssubclient.py
--rw-rw-rw-   0        0        0     6083 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/hanasubclient.py
--rw-rw-rw-   0        0        0    15206 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/index_server_subclient.py
--rw-rw-rw-   0        0        0     4834 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/informixsubclient.py
--rw-rw-rw-   0        0        0    16884 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/lndbsubclient.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.765635 cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/
--rw-rw-rw-   0        0        0      875 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/__init__.py
--rw-rw-rw-   0        0        0    13018 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/lndbsubclient.py
--rw-rw-rw-   0        0        0     7184 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/lndmsubclient.py
--rw-rw-rw-   0        0        0     7947 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/lndocsubclient.py
--rw-rw-rw-   0        0        0     9183 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/lnsubclient.py
--rw-rw-rw-   0        0        0    19522 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/mysqlsubclient.py
--rw-rw-rw-   0        0        0     9193 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/nassubclient.py
--rw-rw-rw-   0        0        0    20278 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/oraclesubclient.py
--rw-rw-rw-   0        0        0    15895 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/postgressubclient.py
--rw-rw-rw-   0        0        0     5244 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/saporaclesubclient.py
--rw-rw-rw-   0        0        0    56653 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/sharepointsubclient.py
--rw-rw-rw-   0        0        0     4493 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/splunksubclient.py
--rw-rw-rw-   0        0        0    15757 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/sqlsubclient.py
--rw-rw-rw-   0        0        0    21028 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/sybasesubclient.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.890637 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/
--rw-rw-rw-   0        0        0      877 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/__init__.py
--rw-rw-rw-   0        0        0     6624 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/alibaba_cloud.py
--rw-rw-rw-   0        0        0    23395 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/amazon_web_services.py
--rw-rw-rw-   0        0        0     7627 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/azure.py
--rw-rw-rw-   0        0        0    27948 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/azure_resource_manager.py
--rw-rw-rw-   0        0        0     7319 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/azure_stack.py
--rw-rw-rw-   0        0        0    10508 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/fusioncompute.py
--rw-rw-rw-   0        0        0     9552 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/google_cloud_platform.py
--rw-rw-rw-   0        0        0    29397 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/hyperv.py
--rw-rw-rw-   0        0        0    72691 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/kubernetes.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:19.921885 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/
--rw-rw-rw-   0        0        0      819 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/__init__.py
--rw-rw-rw-   0        0        0     8233 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/amazon_live_sync.py
--rw-rw-rw-   0        0        0     8315 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/azure_live_sync.py
--rw-rw-rw-   0        0        0     6974 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/hyperv_live_sync.py
--rw-rw-rw-   0        0        0     6628 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/vmware_live_sync.py
--rw-rw-rw-   0        0        0    30597 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/vsa_live_sync.py
--rw-rw-rw-   0        0        0     1231 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/null.py
--rw-rw-rw-   0        0        0    14517 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/nutanix_ahv.py
--rw-rw-rw-   0        0        0    22011 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/openstack.py
--rw-rw-rw-   0        0        0     5112 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/oracle_cloud.py
--rw-rw-rw-   0        0        0    13895 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/oracle_cloud_infrastructure.py
--rw-rw-rw-   0        0        0    11967 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/oraclevm.py
--rw-rw-rw-   0        0        0     1812 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/red_hat_openshift.py
--rw-rw-rw-   0        0        0    11336 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/red_hat_virtualization.py
--rw-rw-rw-   0        0        0     2606 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/vcloud_director.py
--rw-rw-rw-   0        0        0    42604 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/vmware.py
--rw-rw-rw-   0        0        0     8907 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/xen.py
--rw-rw-rw-   0        0        0     8460 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/vminstancesubclient.py
--rw-rw-rw-   0        0        0   126793 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/subclients/vssubclient.py
--rw-rw-rw-   0        0        0     1933 2021-08-25 13:01:52.000000 cvpysdk-11.30.1/cvpysdk/system.py
--rw-rw-rw-   0        0        0    72522 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/virtualmachinepolicies.py
--rw-rw-rw-   0        0        0    57578 2023-02-23 10:00:43.000000 cvpysdk-11.30.1/cvpysdk/workflow.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:25:18.869047 cvpysdk-11.30.1/cvpysdk.egg-info/
--rw-rw-rw-   0        0        0     7312 2023-02-23 10:25:16.000000 cvpysdk-11.30.1/cvpysdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9402 2023-02-23 10:25:16.000000 cvpysdk-11.30.1/cvpysdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 10:25:16.000000 cvpysdk-11.30.1/cvpysdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-23 10:11:37.000000 cvpysdk-11.30.1/cvpysdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-02-23 10:25:16.000000 cvpysdk-11.30.1/cvpysdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-23 10:25:16.000000 cvpysdk-11.30.1/cvpysdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-23 10:25:19.921885 cvpysdk-11.30.1/setup.cfg
--rw-rw-rw-   0        0        0     2301 2023-02-23 10:00:44.000000 cvpysdk-11.30.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.220131 cvpysdk-11.32/
+-rw-rw-rw-   0        0        0    11531 2023-06-15 06:13:11.000000 cvpysdk-11.32/LICENSE.txt
+-rw-rw-rw-   0        0        0       71 2023-06-15 06:13:11.000000 cvpysdk-11.32/MANIFEST.in
+-rw-rw-rw-   0        0        0     7649 2023-06-15 08:11:27.204508 cvpysdk-11.32/PKG-INFO
+-rw-rw-rw-   0        0        0     7082 2023-06-15 08:11:08.000000 cvpysdk-11.32/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:25.980871 cvpysdk-11.32/cvpysdk/
+-rw-rw-rw-   0        0        0     1347 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/__init__.py
+-rw-rw-rw-   0        0        0     6845 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activate.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.090238 cvpysdk-11.32/cvpysdk/activateapps/
+-rw-rw-rw-   0        0        0      866 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/__init__.py
+-rw-rw-rw-   0        0        0    33458 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/constants.py
+-rw-rw-rw-   0        0        0   136470 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/ediscovery_utils.py
+-rw-rw-rw-   0        0        0   101465 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/entity_manager.py
+-rw-rw-rw-   0        0        0    36915 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/file_storage_optimization.py
+-rw-rw-rw-   0        0        0    45588 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/inventory_manager.py
+-rw-rw-rw-   0        0        0    34226 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/request_manager.py
+-rw-rw-rw-   0        0        0    20756 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/sensitive_data_governance.py
+-rw-rw-rw-   0        0        0    10277 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activitycontrol.py
+-rw-rw-rw-   0        0        0    35180 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/agent.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.090238 cvpysdk-11.32/cvpysdk/agents/
+-rw-rw-rw-   0        0        0      863 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/agents/__init__.py
+-rw-rw-rw-   0        0        0     7472 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/agents/exchange_database_agent.py
+-rw-rw-rw-   0        0        0    47512 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/alert.py
+-rw-rw-rw-   0        0        0    26553 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/array_management.py
+-rw-rw-rw-   0        0        0    10120 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/backup_network_pairs.py
+-rw-rw-rw-   0        0        0    92668 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/backupset.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.152765 cvpysdk-11.32/cvpysdk/backupsets/
+-rw-rw-rw-   0        0        0      863 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/backupsets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.168368 cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/
+-rw-rw-rw-   0        0        0      876 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/__init__.py
+-rw-rw-rw-   0        0        0     2501 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/kubernetes.py
+-rw-rw-rw-   0        0        0    10718 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/vmware.py
+-rw-rw-rw-   0        0        0    18407 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/aadbackupset.py
+-rw-rw-rw-   0        0        0     3275 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/adbackupset.py
+-rw-rw-rw-   0        0        0     2695 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/cabackupset.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.168368 cvpysdk-11.32/cvpysdk/backupsets/cloudapps/
+-rw-rw-rw-   0        0        0      874 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/cloudapps/__init__.py
+-rw-rw-rw-   0        0        0     9083 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/cloudapps/salesforce_backupset.py
+-rw-rw-rw-   0        0        0    11908 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/db2backupset.py
+-rw-rw-rw-   0        0        0    72677 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/fsbackupset.py
+-rw-rw-rw-   0        0        0     4615 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/hanabackupset.py
+-rw-rw-rw-   0        0        0     3639 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/nasbackupset.py
+-rw-rw-rw-   0        0        0    11438 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/postgresbackupset.py
+-rw-rw-rw-   0        0        0     3721 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/sharepointbackupset.py
+-rw-rw-rw-   0        0        0    12986 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/vsbackupset.py
+-rw-rw-rw-   0        0        0     6246 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/certificates.py
+-rw-rw-rw-   0        0        0   270983 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/client.py
+-rw-rw-rw-   0        0        0    76883 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/clientgroup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.183988 cvpysdk-11.32/cvpysdk/clients/
+-rw-rw-rw-   0        0        0      860 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/clients/__init__.py
+-rw-rw-rw-   0        0        0     6864 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/clients/onedrive_client.py
+-rw-rw-rw-   0        0        0     9029 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/clients/vmclient.py
+-rw-rw-rw-   0        0        0   146330 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/commcell.py
+-rw-rw-rw-   0        0        0    24026 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/commcell_migration.py
+-rw-rw-rw-   0        0        0    32624 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/constants.py
+-rw-rw-rw-   0        0        0    16567 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/content_analyzer.py
+-rw-rw-rw-   0        0        0    30092 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/credential_manager.py
+-rw-rw-rw-   0        0        0    17286 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/cvpysdk.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.230869 cvpysdk-11.32/cvpysdk/datacube/
+-rw-rw-rw-   0        0        0      879 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/__init__.py
+-rw-rw-rw-   0        0        0     3294 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/constants.py
+-rw-rw-rw-   0        0        0     6634 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/datacube.py
+-rw-rw-rw-   0        0        0    36258 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/datasource.py
+-rw-rw-rw-   0        0        0    18093 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/handler.py
+-rw-rw-rw-   0        0        0     1997 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/sedstype.py
+-rw-rw-rw-   0        0        0    54808 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/deduplication_engines.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.262118 cvpysdk-11.32/cvpysdk/deployment/
+-rw-rw-rw-   0        0        0      863 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/deployment/__init__.py
+-rw-rw-rw-   0        0        0    17053 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/deployment/cache_config.py
+-rw-rw-rw-   0        0        0     3650 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/deployment/deploymentconstants.py
+-rw-rw-rw-   0        0        0    19233 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/deployment/download.py
+-rw-rw-rw-   0        0        0    30374 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/deployment/install.py
+-rw-rw-rw-   0        0        0     6862 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/deployment/uninstall.py
+-rw-rw-rw-   0        0        0     6091 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/dev_test_group.py
+-rw-rw-rw-   0        0        0    42515 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/disasterrecovery.py
+-rw-rw-rw-   0        0        0    23493 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/domains.py
+-rw-rw-rw-   0        0        0    51805 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/download_center.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.308996 cvpysdk-11.32/cvpysdk/drorchestration/
+-rw-rw-rw-   0        0        0      882 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/__init__.py
+-rw-rw-rw-   0        0        0    48119 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/blr_pairs.py
+-rw-rw-rw-   0        0        0     3808 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/dr_orchestration_job_phase.py
+-rw-rw-rw-   0        0        0     7099 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/drjob.py
+-rw-rw-rw-   0        0        0    33528 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/drorchestrationoperations.py
+-rw-rw-rw-   0        0        0    20998 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/failovergroups.py
+-rw-rw-rw-   0        0        0    29317 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/replication_groups.py
+-rw-rw-rw-   0        0        0    12423 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/replication_pairs.py
+-rw-rw-rw-   0        0        0    13215 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/replicationmonitor.py
+-rw-rw-rw-   0        0        0     8905 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/eventviewer.py
+-rw-rw-rw-   0        0        0    25244 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/exception.py
+-rw-rw-rw-   0        0        0     9765 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/globalfilter.py
+-rw-rw-rw-   0        0        0    19921 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/hac_clusters.py
+-rw-rw-rw-   0        0        0    38514 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/identity_management.py
+-rw-rw-rw-   0        0        0    19706 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/index_pools.py
+-rw-rw-rw-   0        0        0    56990 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/index_server.py
+-rw-rw-rw-   0        0        0   131423 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/instance.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.425388 cvpysdk-11.32/cvpysdk/instances/
+-rw-rw-rw-   0        0        0      862 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/__init__.py
+-rw-rw-rw-   0        0        0     2399 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/aadinstance.py
+-rw-rw-rw-   0        0        0     2827 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/bigdataappsinstance.py
+-rw-rw-rw-   0        0        0     4702 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cainstance.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.466717 cvpysdk-11.32/cvpysdk/instances/cloudapps/
+-rw-rw-rw-   0        0        0      873 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/__init__.py
+-rw-rw-rw-   0        0        0    23441 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/amazon_instance.py
+-rw-rw-rw-   0        0        0     8534 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/cloud_database_instance.py
+-rw-rw-rw-   0        0        0    32465 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/cloud_storage_instance.py
+-rw-rw-rw-   0        0        0     6414 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/dynamics365_instance.py
+-rw-rw-rw-   0        0        0    17755 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/google_instance.py
+-rw-rw-rw-   0        0        0    33100 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/salesforce_instance.py
+-rw-rw-rw-   0        0        0     5195 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/spanner_instance.py
+-rw-rw-rw-   0        0        0    13394 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/teams_instance.py
+-rw-rw-rw-   0        0        0    24491 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/db2instance.py
+-rw-rw-rw-   0        0        0     4930 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/dbinstance.py
+-rw-rw-rw-   0        0        0    18464 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/instances/hanainstance.py
+-rw-rw-rw-   0        0        0    15761 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/informixinstance.py
+-rw-rw-rw-   0        0        0    16033 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lndbinstance.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.497966 cvpysdk-11.32/cvpysdk/instances/lotusnotes/
+-rw-rw-rw-   0        0        0      874 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lotusnotes/__init__.py
+-rw-rw-rw-   0        0        0    15182 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndbinstance.py
+-rw-rw-rw-   0        0        0     8851 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndminstance.py
+-rw-rw-rw-   0        0        0     9268 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndocinstance.py
+-rw-rw-rw-   0        0        0     7983 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lotusnotes/lninstance.py
+-rw-rw-rw-   0        0        0    24121 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/mysqlinstance.py
+-rw-rw-rw-   0        0        0    53422 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/oracleinstance.py
+-rw-rw-rw-   0        0        0    26338 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/postgresinstance.py
+-rw-rw-rw-   0        0        0    18937 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/saporacleinstance.py
+-rw-rw-rw-   0        0        0     9192 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/sharepointinstance.py
+-rw-rw-rw-   0        0        0     4584 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/splunkinstance.py
+-rw-rw-rw-   0        0        0    61965 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/sqlinstance.py
+-rw-rw-rw-   0        0        0    43205 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/sybaseinstance.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.669842 cvpysdk-11.32/cvpysdk/instances/virtualserver/
+-rw-rw-rw-   0        0        0      862 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/__init__.py
+-rw-rw-rw-   0        0        0     5325 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/alibaba_cloud.py
+-rw-rw-rw-   0        0        0     5419 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/amazon_web_services.py
+-rw-rw-rw-   0        0        0     4316 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/azure.py
+-rw-rw-rw-   0        0        0     4810 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/azure_resource_manager.py
+-rw-rw-rw-   0        0        0     4861 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/azure_stack.py
+-rw-rw-rw-   0        0        0     4883 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/fusioncompute.py
+-rw-rw-rw-   0        0        0     3647 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/google_cloud_platform.py
+-rw-rw-rw-   0        0        0     4645 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/hyperv.py
+-rw-rw-rw-   0        0        0     4430 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/kubernetes.py
+-rw-rw-rw-   0        0        0     1177 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/null.py
+-rw-rw-rw-   0        0        0     4943 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/nutanix_ahv.py
+-rw-rw-rw-   0        0        0     4554 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/openstack.py
+-rw-rw-rw-   0        0        0     5320 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/oracle_cloud.py
+-rw-rw-rw-   0        0        0     4125 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/oracle_cloud_infrastructure.py
+-rw-rw-rw-   0        0        0     4225 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/oraclevm.py
+-rw-rw-rw-   0        0        0     4333 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/red_hat_virtualization.py
+-rw-rw-rw-   0        0        0     4488 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/vcloud_director.py
+-rw-rw-rw-   0        0        0     4401 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/vmware.py
+-rw-rw-rw-   0        0        0     4371 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/xen.py
+-rw-rw-rw-   0        0        0     2007 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/vminstance.py
+-rw-rw-rw-   0        0        0    13055 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/vsinstance.py
+-rw-rw-rw-   0        0        0     7827 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/internetoptions.py
+-rw-rw-rw-   0        0        0   119599 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/job.py
+-rw-rw-rw-   0        0        0    33588 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/key_management_server.py
+-rw-rw-rw-   0        0        0    13533 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/license.py
+-rw-rw-rw-   0        0        0    20426 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/metallic.py
+-rw-rw-rw-   0        0        0    27461 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/metricsreport.py
+-rw-rw-rw-   0        0        0    28226 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/monitoring.py
+-rw-rw-rw-   0        0        0    23387 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/name_change.py
+-rw-rw-rw-   0        0        0    34060 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/network.py
+-rw-rw-rw-   0        0        0    13795 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/network_throttle.py
+-rw-rw-rw-   0        0        0    36142 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/network_topology.py
+-rw-rw-rw-   0        0        0    48129 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/operation_window.py
+-rw-rw-rw-   0        0        0   138787 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/organization.py
+-rw-rw-rw-   0        0        0   106777 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/plan.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.701106 cvpysdk-11.32/cvpysdk/policies/
+-rw-rw-rw-   0        0        0      879 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/policies/__init__.py
+-rw-rw-rw-   0        0        0    74032 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/policies/configuration_policies.py
+-rw-rw-rw-   0        0        0     8072 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/policies/schedule_options.py
+-rw-rw-rw-   0        0        0    44091 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/policies/schedule_policies.py
+-rw-rw-rw-   0        0        0   184554 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/policies/storage_policies.py
+-rw-rw-rw-   0        0        0     3033 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/policy.py
+-rw-rw-rw-   0        0        0    26335 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/recovery_targets.py
+-rw-rw-rw-   0        0        0    11526 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/regions.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.716709 cvpysdk-11.32/cvpysdk/reports/
+-rw-rw-rw-   0        0        0      860 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/reports/__init__.py
+-rw-rw-rw-   0        0        0    19808 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/reports/report.py
+-rw-rw-rw-   0        0        0   108687 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/schedules.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.747964 cvpysdk-11.32/cvpysdk/security/
+-rw-rw-rw-   0        0        0      869 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/security/__init__.py
+-rw-rw-rw-   0        0        0    29798 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/security/role.py
+-rw-rw-rw-   0        0        0    16846 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/security/security_association.py
+-rw-rw-rw-   0        0        0     8966 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/security/two_factor_authentication.py
+-rw-rw-rw-   0        0        0    42885 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/security/user.py
+-rw-rw-rw-   0        0        0    38467 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/security/usergroup.py
+-rw-rw-rw-   0        0        0    30539 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/services.py
+-rw-rw-rw-   0        0        0   104242 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/storage.py
+-rw-rw-rw-   0        0        0    37723 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/storage_pool.py
+-rw-rw-rw-   0        0        0   126396 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclient.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.910173 cvpysdk-11.32/cvpysdk/subclients/
+-rw-rw-rw-   0        0        0      863 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/__init__.py
+-rw-rw-rw-   0        0        0     1952 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/aadsubclient.py
+-rw-rw-rw-   0        0        0     4182 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/adsubclient.py
+-rw-rw-rw-   0        0        0     4110 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/bigdataappssubclient.py
+-rw-rw-rw-   0        0        0    11760 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/casesubclient.py
+-rw-rw-rw-   0        0        0     3650 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/casubclient.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.970136 cvpysdk-11.32/cvpysdk/subclients/cloudapps/
+-rw-rw-rw-   0        0        0      874 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/__init__.py
+-rw-rw-rw-   0        0        0     7660 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/cloud_database_subclient.py
+-rw-rw-rw-   0        0        0    15228 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/cloud_storage_subclient.py
+-rw-rw-rw-   0        0        0    42053 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/dynamics365_subclient.py
+-rw-rw-rw-   0        0        0    29846 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/google_subclient.py
+-rw-rw-rw-   0        0        0    51907 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/salesforce_subclient.py
+-rw-rw-rw-   0        0        0     3329 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/spanner_subclient.py
+-rw-rw-rw-   0        0        0     3704 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/teams_constants.py
+-rw-rw-rw-   0        0        0    47765 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/teams_subclient.py
+-rw-rw-rw-   0        0        0    13162 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/db2subclient.py
+-rw-rw-rw-   0        0        0     3424 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/dbsubclient.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.001402 cvpysdk-11.32/cvpysdk/subclients/exchange/
+-rw-rw-rw-   0        0        0      872 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchange/__init__.py
+-rw-rw-rw-   0        0        0    13470 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchange/contentstoremailbox_subclient.py
+-rw-rw-rw-   0        0        0    16906 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchange/exchange_database_subclient.py
+-rw-rw-rw-   0        0        0    17764 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchange/journalmailbox_subclient.py
+-rw-rw-rw-   0        0        0    73265 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchange/usermailbox_subclient.py
+-rw-rw-rw-   0        0        0    32624 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchsubclient.py
+-rw-rw-rw-   0        0        0    99425 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/fssubclient.py
+-rw-rw-rw-   0        0        0     6083 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/hanasubclient.py
+-rw-rw-rw-   0        0        0    15274 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/index_server_subclient.py
+-rw-rw-rw-   0        0        0     4834 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/informixsubclient.py
+-rw-rw-rw-   0        0        0    16884 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lndbsubclient.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.032812 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/
+-rw-rw-rw-   0        0        0      875 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/__init__.py
+-rw-rw-rw-   0        0        0    13018 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndbsubclient.py
+-rw-rw-rw-   0        0        0     7184 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndmsubclient.py
+-rw-rw-rw-   0        0        0     7947 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndocsubclient.py
+-rw-rw-rw-   0        0        0     9183 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lnsubclient.py
+-rw-rw-rw-   0        0        0    19522 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/mysqlsubclient.py
+-rw-rw-rw-   0        0        0    15585 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/nassubclient.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/o365apps_subclient.py
+-rw-rw-rw-   0        0        0    20278 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/oraclesubclient.py
+-rw-rw-rw-   0        0        0    15895 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/postgressubclient.py
+-rw-rw-rw-   0        0        0     5244 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/saporaclesubclient.py
+-rw-rw-rw-   0        0        0    56653 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/sharepointsubclient.py
+-rw-rw-rw-   0        0        0     4493 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/splunksubclient.py
+-rw-rw-rw-   0        0        0    15757 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/sqlsubclient.py
+-rw-rw-rw-   0        0        0    21028 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/sybasesubclient.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.157634 cvpysdk-11.32/cvpysdk/subclients/virtualserver/
+-rw-rw-rw-   0        0        0      877 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/__init__.py
+-rw-rw-rw-   0        0        0     6624 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/alibaba_cloud.py
+-rw-rw-rw-   0        0        0    24113 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/amazon_web_services.py
+-rw-rw-rw-   0        0        0     7647 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure.py
+-rw-rw-rw-   0        0        0    28032 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure_resource_manager.py
+-rw-rw-rw-   0        0        0     7341 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure_stack.py
+-rw-rw-rw-   0        0        0    10508 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/fusioncompute.py
+-rw-rw-rw-   0        0        0     9892 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/google_cloud_platform.py
+-rw-rw-rw-   0        0        0    29479 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/hyperv.py
+-rw-rw-rw-   0        0        0    72691 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/kubernetes.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.204508 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/
+-rw-rw-rw-   0        0        0      819 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/__init__.py
+-rw-rw-rw-   0        0        0     8233 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/amazon_live_sync.py
+-rw-rw-rw-   0        0        0     8315 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/azure_live_sync.py
+-rw-rw-rw-   0        0        0     6974 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/hyperv_live_sync.py
+-rw-rw-rw-   0        0        0     6628 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/vmware_live_sync.py
+-rw-rw-rw-   0        0        0    30597 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/vsa_live_sync.py
+-rw-rw-rw-   0        0        0     1231 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/null.py
+-rw-rw-rw-   0        0        0    14517 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/nutanix_ahv.py
+-rw-rw-rw-   0        0        0    22011 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/openstack.py
+-rw-rw-rw-   0        0        0     5112 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/oracle_cloud.py
+-rw-rw-rw-   0        0        0    13363 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/oracle_cloud_infrastructure.py
+-rw-rw-rw-   0        0        0    11967 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/oraclevm.py
+-rw-rw-rw-   0        0        0     1812 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/red_hat_openshift.py
+-rw-rw-rw-   0        0        0    11336 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/red_hat_virtualization.py
+-rw-rw-rw-   0        0        0     2606 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/vcloud_director.py
+-rw-rw-rw-   0        0        0    43570 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/vmware.py
+-rw-rw-rw-   0        0        0     9081 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/xen.py
+-rw-rw-rw-   0        0        0    12599 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/vminstancesubclient.py
+-rw-rw-rw-   0        0        0   129743 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/vssubclient.py
+-rw-rw-rw-   0        0        0     1933 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/system.py
+-rw-rw-rw-   0        0        0    72522 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/virtualmachinepolicies.py
+-rw-rw-rw-   0        0        0    57808 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/workflow.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.027746 cvpysdk-11.32/cvpysdk.egg-info/
+-rw-rw-rw-   0        0        0     7649 2023-06-15 08:11:25.000000 cvpysdk-11.32/cvpysdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9443 2023-06-15 08:11:25.000000 cvpysdk-11.32/cvpysdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:11:25.000000 cvpysdk-11.32/cvpysdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 06:48:49.000000 cvpysdk-11.32/cvpysdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-15 08:11:25.000000 cvpysdk-11.32/cvpysdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 08:11:25.000000 cvpysdk-11.32/cvpysdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 08:11:27.220131 cvpysdk-11.32/setup.cfg
+-rw-rw-rw-   0        0        0     2301 2023-06-15 06:13:13.000000 cvpysdk-11.32/setup.py
```

### Comparing `cvpysdk-11.30.1/LICENSE.txt` & `cvpysdk-11.32/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/PKG-INFO` & `cvpysdk-11.32/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvpysdk
-Version: 11.30.1
+Version: 11.32
 Summary: Commvault SDK for Python
 Home-page: https://github.com/Commvault/cvpysdk
 Author: Commvault Systems Inc.
 Author-email: Dev-PythonSDK@commvault.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Commvault/cvpysdk/issues
 Project-URL: Documentation, https://commvault.github.io/cvpysdk/
@@ -35,15 +35,15 @@
 ------------------
 
 CVPySDK can be installed directly from PyPI using pip:
 
     >>> pip install cvpysdk
 
 
-CVPySDK is available on GitHub `here <https://github.com/Commvault/cvpysdk>`_
+CVPySDK is available on GitHub `here <https://github.com/Commvault/cvpysdk>`__
 
 It can also be installed from source.
 
 After downloading, from within the ``cvpysdk`` directory, execute:
 
     >>> python setup.py install
 
@@ -205,14 +205,19 @@
 
 - All python code should be **PEP8** compliant.
 - All changes should be consistent with the design of the SDK.
 - The code should be formatted using **autopep8** with line-length set to **99** instead of default **79**.
 - All changes and any new methods/classes should be properly documented.
 - The doc strings should be of the same format as existing docs.
 
+Questions/Comments/Suggestions
+------------------------------
+If you have any questions or comments, please contact us `here <https://ma.commvault.com/>`__.
+Also Check out our community for `Automation <https://community.commvault.com/developer-tools-integration-and-automation-workflow-rest-powershell-etc-50>`_ incase of queries.
+
 Code of Conduct
 ***************
 
 Everyone interacting in the **CVPySDK** project's codebases, issue trackers,
 chat rooms, and mailing lists is expected to follow the
 `PyPA Code of Conduct`_.
```

### Comparing `cvpysdk-11.30.1/README.rst` & `cvpysdk-11.32/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ------------------
 
 CVPySDK can be installed directly from PyPI using pip:
 
     >>> pip install cvpysdk
 
 
-CVPySDK is available on GitHub `here <https://github.com/Commvault/cvpysdk>`_
+CVPySDK is available on GitHub `here <https://github.com/Commvault/cvpysdk>`__
 
 It can also be installed from source.
 
 After downloading, from within the ``cvpysdk`` directory, execute:
 
     >>> python setup.py install
 
@@ -190,14 +190,19 @@
 
 - All python code should be **PEP8** compliant.
 - All changes should be consistent with the design of the SDK.
 - The code should be formatted using **autopep8** with line-length set to **99** instead of default **79**.
 - All changes and any new methods/classes should be properly documented.
 - The doc strings should be of the same format as existing docs.
 
+Questions/Comments/Suggestions
+------------------------------
+If you have any questions or comments, please contact us `here <https://ma.commvault.com/>`__.
+Also Check out our community for `Automation <https://community.commvault.com/developer-tools-integration-and-automation-workflow-rest-powershell-etc-50>`_ incase of queries.
+
 Code of Conduct
 ***************
 
 Everyone interacting in the **CVPySDK** project's codebases, issue trackers,
 chat rooms, and mailing lists is expected to follow the
 `PyPA Code of Conduct`_.
```

### Comparing `cvpysdk-11.30.1/cvpysdk/__init__.py` & `cvpysdk-11.32/cvpysdk/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     -   **xmltodict**
 
 And Commvault Software v11 SP7 or later release with WebConsole installed
 
 """
 
 __author__ = 'Commvault Systems Inc.'
-__version__ = '11.30.1'
+__version__ = '11.32'
```

### Comparing `cvpysdk-11.30.1/cvpysdk/activate.py` & `cvpysdk-11.32/cvpysdk/activate.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/activateapps/__init__.py` & `cvpysdk-11.32/cvpysdk/activateapps/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/activateapps/constants.py` & `cvpysdk-11.32/cvpysdk/activateapps/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -550,83 +550,51 @@
     CRAWL_JOB_FAILED_STATE = [5, 6, 7, 8, 9, 10, 11, 12]
 
     CRAWL_JOB_COMPLETE_STATE = 4
 
     CRAWL_JOB_COMPLETE_ERROR_STATE = 13
 
     INVENTORY_ADD_REQUEST_JSON = {
-        "inventoryName": "",
-        "assets": [],
-        "analyticsEngineCloud": {
-            "cloudId": 0,
-            "cloudDisplayName": ""
-        }
-    }
-
-    ASSET_ADD_REQUEST_JSON = {
         "name": "",
-        "type": 0
-    }
-
-    ASSET_PROPERTY_JSON = {
-        "propertyValues": {
-            "nameValues": [
-
-            ]
+        "identityServers": [],
+        "indexServer": {
+            "cloudId": 0,
+            "displayName": ""
         }
     }
-    ASSET_PROPERTY_NAME_VALUE_PAIR_JSON = {
-        "name": "",
-        "value": ""
-    }
 
     FIELD_PROPERTY_NAME = 'name'
-    FIELD_PROPERTY_DNSHOST = 'dNSHostName'
+    FIELD_PROPERTY_DNSHOST = 'hostName'
     FIELD_PROPERTY_OS = 'operatingSystem'
-    FIELD_PROPERTY_IP = 'ipAddresses'
+    FIELD_PROPERTY_IP = 'ipAddress'
     FIELD_PROPERTY_COUNTRYCODE = 'countryCode'
-    FIELD_PROPERTY_CO = 'co'
-    FIELD_PROPERTY_DOMAIN = 'domainName'
 
     KWARGS_NAME = 'name'
     KWARGS_IP = 'ip'
     KWARGS_OS = 'os'
-    KWARGS_DOMAIN = 'domain'
     KWARGS_FQDN = 'fqdn'
-    KWARGS_COUNTRY_NAME = 'country_name'
     KWARGS_COUNTRY_CODE = 'country_code'
 
     FIELD_PROPS_MAPPING = {
         FIELD_PROPERTY_NAME: KWARGS_NAME,
         FIELD_PROPERTY_IP: KWARGS_IP,
         FIELD_PROPERTY_OS: KWARGS_OS,
-        FIELD_PROPERTY_DOMAIN: KWARGS_DOMAIN,
         FIELD_PROPERTY_DNSHOST: KWARGS_FQDN,
-        FIELD_PROPERTY_CO: KWARGS_COUNTRY_NAME,
         FIELD_PROPERTY_COUNTRYCODE: KWARGS_COUNTRY_CODE
     }
 
     ASSET_FILE_SERVER_PROPERTY = [
         FIELD_PROPERTY_NAME,
         FIELD_PROPERTY_DNSHOST,
         FIELD_PROPERTY_OS,
         FIELD_PROPERTY_IP,
-        FIELD_PROPERTY_COUNTRYCODE,
-        FIELD_PROPERTY_CO,
-        FIELD_PROPERTY_DOMAIN]
-
-    ASSET_ADD_TO_INVENTORY_JSON = {
-        "inventoryId": 0,
-        "assets": []
-    }
+        FIELD_PROPERTY_COUNTRYCODE
+    ]
 
-    ASSET_DELETE_FROM_INVENTORY_JSON = {
-        "inventoryId": 0,
-        "assets": []
-    }
+    IDENTITY_SERVER_ASSET_ADD_TO_INVENTORY_JSON = {"identityServers": [], "startDataCollection": True}
 
     VIEW_CATEGORY_PERMISSION = {
         "permissionId": 31,
         "permissionName": "View",
         "_type_": 122
     }
     EDIT_CATEGORY_PERMISSION = {
@@ -666,15 +634,15 @@
                 }
             ]
         }
     }
 
     class AssetType(Enum):
         """Asset type for inventory"""
-        NAME_SERVER = 61
+        IDENTITY_SERVER = 61
         FILE_SERVER = 132
 
 
 class PlanConstants:
     """Class to maintain constants related to DC plan activate operations"""
 
     INDEXING_ONLY_METADATA = 1
```

### Comparing `cvpysdk-11.30.1/cvpysdk/activateapps/ediscovery_utils.py` & `cvpysdk-11.32/cvpysdk/activateapps/ediscovery_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,30 +539,19 @@
         self._API_EXPORT = self._services['EDISCOVERY_EXPORT']
         self._API_EXPORT_STATUS = self._services['EDISCOVERY_EXPORT_STATUS']
         self._CREATE_POLICY = self._services['CREATE_UPDATE_SCHEDULE_POLICY']
         self._API_GET_EDISCOVERY_CLIENT_DETAILS_V1 = copy.deepcopy(self._services['EDISCOVERY_CLIENT_DETAILS'])
         self._API_DOC_TASK = self._services['EDISCOVERY_REQUEST_DOCUMENT_MARKER']
         self._API_CONFIGURE_TASK = self._services['EDISCOVERY_CONFIGURE_TASK']
         self._API_TASK_WORKFLOW = self._services['EDICOVERY_TASK_WORKFLOW']
-        from .inventory_manager import Inventory, Asset
         from .file_storage_optimization import FsoServer, FsoServerGroup
         from .sensitive_data_governance import Project
         from .request_manager import Request
 
-        if isinstance(class_object, Inventory):
-            self._type = 0  # Inventory
-            self._operation = 0
-            self._client_id = class_object.inventory_id
-            self._data_source_id = 0
-        elif isinstance(class_object, Asset):
-            self._type = 0  # Inventory
-            self._operation = 0
-            self._client_id = class_object.inventory_id
-            self._data_source_id = class_object.asset_id
-        elif isinstance(class_object, FsoServer):
+        if isinstance(class_object, FsoServer):
             self._client_id = class_object.server_id
             self._include_doc_count = 1
             self._limit = self._offset = 0
             self._sort_by = 2
             self._sort_dir = 0
             self._ds_type_names = f"{EdiscoveryConstants.DS_FILE},{EdiscoveryConstants.DS_CLOUD_STORAGE}"
             self._data_source_id = 0  # invoke on all data sources
```

### Comparing `cvpysdk-11.30.1/cvpysdk/activateapps/entity_manager.py` & `cvpysdk-11.32/cvpysdk/activateapps/entity_manager.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/activateapps/file_storage_optimization.py` & `cvpysdk-11.32/cvpysdk/activateapps/file_storage_optimization.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/activateapps/inventory_manager.py` & `cvpysdk-11.32/cvpysdk/activateapps/inventory_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
             _get_inventory_properties()         --  Gets all the properties of this inventory
 
              _get_schedule_object()             --  returns the schedule class object associated to this inventory
 
             _get_data_source_handler_object()   --  returns the datasource and default handler object for this inventory
 
+            _get_permission()                   --  returns the security associations for this inventory
+
             refresh()                           --  refresh the properties of the inventory
 
             get_assets()                        --  returns the Assets class object for this inventory
 
             share()                             --  shares inventory with other user or user group
 
             start_collection()                  --  starts collection job on this inventory
@@ -117,21 +119,21 @@
 
 Asset:
 
         __init__()                          --  initialise object of the Asset class
 
         _get_properties()                   --  returns the properties of the asset
 
-        refresh()                           --  refresh the asset associated with inventory
+        _response_not_success()             --  parses through the exception response, and raises SDKException
 
-        start_collection()                  --  starts collection job on this asset
+        refresh()                           --  refresh the asset associated with inventory
 
         get_job_history()                   --  returns the job history details of this asset
 
-        get_job_status()                    --  returns the job status details of this asset
+        get_job_status()                    --  returns the latest job status details of this asset
 
         get_asset_prop()                    --  returns the asset property value for the given property name
 
 
 Asset Attributes:
 -----------------
 
@@ -149,16 +151,14 @@
 
         **inventory_id**        --      returns the inventory id of this asset
 
 
 """
 import copy
 
-from ..activateapps.ediscovery_utils import EdiscoveryClientOperations
-
 from ..activateapps.constants import InventoryConstants
 from ..schedules import Schedules
 from ..exception import SDKException
 
 
 class Inventories():
     """Class for representing all inventories in the commcell."""
@@ -214,18 +214,18 @@
 
         """
         output = {}
         flag, response = self._cvpysdk_object.make_request(
             'GET', self._API_INVENTORIES
         )
         if flag:
-            if response.json() and 'inventoryList' in response.json():
-                inventories = response.json()['inventoryList']
+            if response.json() and 'inventories' in response.json():
+                inventories = response.json()['inventories']
                 for inventory in inventories:
-                    output[inventory['inventoryName'].lower()] = inventory
+                    output[inventory['displayName'].lower()] = inventory
                 return output
             raise SDKException('Inventory', '103')
         self._response_not_success(response)
 
     def add(self, inventory_name, index_server, name_server=None):
         """Adds inventory to the commcell with given inputs
 
@@ -252,38 +252,34 @@
                             if Index Server doesn't exists in commcell
 
         """
         if not isinstance(inventory_name, str) or not isinstance(index_server, str):
             raise SDKException('Inventory', '101')
         req_json = copy.deepcopy(InventoryConstants.INVENTORY_ADD_REQUEST_JSON)
         if name_server:
-            asset_json = copy.deepcopy(InventoryConstants.ASSET_ADD_REQUEST_JSON)
-            for server in name_server:
-                asset_json['name'] = server
-                req_json['assets'].append(asset_json)
-        req_json['inventoryName'] = inventory_name
+            req_json['identityServers'] = name_server
+        req_json['name'] = inventory_name
         if not self._commcell_object.index_servers.has(index_server):
             raise SDKException('Inventory', '102', "Given index server name not exists on this commcell")
         index_server_obj = self._commcell_object.index_servers.get(index_server)
-        req_json['analyticsEngineCloud']['cloudId'] = index_server_obj.cloud_id
-        req_json['analyticsEngineCloud']['cloudDisplayName'] = index_server_obj.cloud_name
+        req_json['indexServer']['cloudId'] = index_server_obj.cloud_id
+        req_json['indexServer']['displayName'] = index_server_obj.cloud_name
         flag, response = self._cvpysdk_object.make_request(
             'POST', self._API_INVENTORIES, req_json
         )
         if flag:
-            if response.json() and 'errorResp' in response.json():
-                err_resp = response.json()['errorResp']
-                if 'errorCode' in err_resp and err_resp['errorCode'] != 0:
+            if response.json():
+                if 'errorCode' in response.json() and response.json()['errorCode'] != 0:
                     raise SDKException(
                         'Inventory',
                         '102',
-                        f"Failed to create inventory with error [{err_resp['errorMessage']}]")
-                elif 'inventoryList' in response.json():
-                    inventory = response.json()['inventoryList'][0]
-                    inventory_id = inventory['inventoryId']
+                        f"Failed to create inventory with error [{response.json()['errorMessage']}]")
+                elif 'name' in response.json():
+                    inventory = response.json()['name']
+                    inventory_id = response.json()['id']
                     self.refresh()
                     return Inventory(self._commcell_object, inventory_name, inventory_id)
                 raise SDKException('Inventory', '102', f"Failed to create inventory with response - {response.json()}")
             raise SDKException('Inventory', '105')
         self._response_not_success(response)
 
     def delete(self, inventory_name):
@@ -308,24 +304,23 @@
 
         """
         if not isinstance(inventory_name, str):
             raise SDKException('Inventory', '101')
         if not self.has_inventory(inventory_name):
             raise SDKException('Inventory', '106')
         flag, response = self._cvpysdk_object.make_request(
-            'DELETE', self._API_DELETE_INVENTORY % self._inventories[inventory_name.lower()]['inventoryId']
+            'DELETE', self._API_DELETE_INVENTORY % self._inventories[inventory_name.lower()]['id']
         )
         if flag:
-            if response.json() and 'errorResp' in response.json():
-                err_resp = response.json()['errorResp']
-                if 'errorCode' in err_resp and err_resp['errorCode'] != 0:
+            if response.json():
+                if 'errorCode' in response.json() and response.json()['errorCode'] != 0:
                     raise SDKException(
                         'Inventory',
                         '102',
-                        f"Failed to Delete inventory with error [{err_resp['errorMessage']}]")
+                        f"Failed to Delete inventory with error [{response.json()['errorMessage']}]")
                 self.refresh()
             else:
                 raise SDKException('Inventory', '107')
         else:
             self._response_not_success(response)
 
     def refresh(self):
@@ -384,15 +379,15 @@
 
 
         """
         if not isinstance(inventory_name, str):
             raise SDKException('Inventory', '101')
 
         if self.has_inventory(inventory_name):
-            inventory_id = self._inventories[inventory_name.lower()]['inventoryId']
+            inventory_id = self._inventories[inventory_name.lower()]['id']
             return Inventory(self._commcell_object, inventory_name, inventory_id)
         raise SDKException('Inventory', '106')
 
 
 class Inventory():
     """Class for performing operations on a single inventory"""
 
@@ -420,36 +415,57 @@
         self._index_server_name = None
         self._index_server_cloud_id = None
         self._security_associations = None
         self._schedule = None
         self._data_source = None
         self._handler = None
         self._API_GET_INVENTORY_DETAILS = self._services['EDISCOVERY_INVENTORY']
-        self._API_SECURITY = self._services['SECURITY_ASSOCIATION']
         self._API_SECURITY_ENTITY = self._services['ENTITY_SECURITY_ASSOCIATION']
         self._API_GET_DEFAULT_HANDLER = self._services['EDISCOVERY_GET_DEFAULT_HANDLER']
+        self._API_PERMISSION = self._services['V4_ACTIVATE_DS_PERMISSION']
+        self._API_CRAWL = self._services['V4_INVENTORY_CRAWL']
 
         if not inventory_id:
             self._inventory_id = self._commcell_object.activate.inventory_manager().get(inventory_name).inventory_id
         else:
             self._inventory_id = inventory_id
         self.refresh()
-        self._ediscovery_client_obj = EdiscoveryClientOperations(class_object=self, commcell_object=commcell_object)
 
     def _response_not_success(self, response):
         """Helper function to raise an exception when reponse status is not 200 (OK).
 
             Args:
                 response    (object)    --  response class object,
 
                 received upon running an API request, using the `requests` python package
 
         """
         raise SDKException('Response', '101', self._update_response_(response.text))
 
+    def _get_permission(self):
+        """returns security association blob for this inventory
+
+                Args:
+
+                    None
+
+                Returns:
+
+                    dict    --  Security association blob
+
+        """
+        flag, response = self._cvpysdk_obj.make_request(
+            'GET', self._API_PERMISSION % self._inventory_id
+        )
+        if flag:
+            if response.json() and 'securityAssociations' in response.json():
+                return response.json()['securityAssociations']
+            raise SDKException('Inventory', '102', "Inventory permission fetch failed")
+        self._response_not_success(response)
+
     def _get_inventory_properties(self):
         """ Get inventory properties from the commcell
                 Args:
 
                     None
 
                 Returns:
@@ -457,29 +473,29 @@
                     dict        --  Properties of inventory
 
         """
         flag, response = self._cvpysdk_obj.make_request(
             'GET', self._API_GET_INVENTORY_DETAILS % self._inventory_id
         )
         if flag:
-            if response.json() and 'inventoryList' in response.json():
-                inventory_props = response.json()['inventoryList'][0]
-                self._index_server_name = inventory_props['analyticsEngineCloud']['cloudDisplayName']
-                self._index_server_cloud_id = inventory_props['analyticsEngineCloud']['cloudId']
-                self._inventory_name = inventory_props['inventoryName']
-                self._security_associations = inventory_props['securityAssociation']['associations']
+            if response.json():
+                inventory_props = response.json()
+                self._index_server_name = inventory_props['indexServer']['displayName']
+                self._index_server_cloud_id = inventory_props['indexServer']['cloudId']
+                self._inventory_name = inventory_props['displayName']
                 return inventory_props
             raise SDKException('Inventory', '104')
         self._response_not_success(response)
 
     def refresh(self):
         """Refresh the inventory details for associated object"""
         self._inventory_props = self._get_inventory_properties()
         self._schedule = self._get_schedule_object()
         self._data_source, self._handler = self._get_data_source_handler_object()
+        self._security_associations = self._get_permission()
 
     def get_assets(self):
         """Returns the Assets class instance for this inventory
 
                 Args:
 
                     None
@@ -505,15 +521,29 @@
                 Raises:
 
                     SDKException:
 
                             if failed to start collection job
 
         """
-        return self._ediscovery_client_obj.start_job()
+        flag, response = self._cvpysdk_obj.make_request(
+            'PUT', self._API_CRAWL % self._inventory_id
+        )
+        if flag:
+            if response.json():
+                if 'errorCode' in response.json() and response.json()['errorCode'] != 0:
+                    raise SDKException(
+                        'Inventory',
+                        '102',
+                        f"Failed to start crawl on inventory with error [{response.json()['errorMessage']}]")
+                return
+            else:
+                raise SDKException('Inventory', '102', "Unknown response while starting collection job on inventory")
+        else:
+            self._response_not_success(response)
 
     def share(self, user_or_group_name, allow_edit_permission=False, is_user=True, ops_type=1):
         """Shares inventory with given user or user group in commcell
 
                 Args:
 
                     user_or_group_name      (str)       --  Name of user or group
@@ -594,22 +624,21 @@
                 InventoryConstants.EDIT_CATEGORY_PERMISSION)
 
             # Associate existing associations to the request
         if ops_type == 1 and len(self.security_associations) > 1:
             request_json['securityAssociations']['associations'].extend(association_response)
 
         flag, response = self._cvpysdk_obj.make_request(
-            'POST', self._API_SECURITY, request_json
+            'PUT', self._API_PERMISSION % self._inventory_id, request_json
         )
         if flag:
-            if response.json() and 'response' in response.json():
-                response_json = response.json()['response'][0]
-                error_code = response_json['errorCode']
+            if response.json():
+                error_code = response.json()['errorCode']
                 if error_code != 0:
-                    error_message = response_json['errorString']
+                    error_message = response.json()['errorString']
                     raise SDKException(
                         'Inventory',
                         '102', error_message)
                 # update association list by refreshing inventory
                 self.refresh()
             else:
                 raise SDKException('Inventory', '111')
@@ -762,37 +791,42 @@
         self._inventory_id = None
         self._inventory_name = inventory_name
         if not inventory_id:
             self._inventory_id = self._commcell_object.activate.inventory_manager().get(inventory_name).inventory_id
         else:
             self._inventory_id = inventory_id
         self._assets = None
-        self._API_INVENTORIES = self._services['EDISCOVERY_INVENTORIES']
         self._API_ASSETS = self._services['EDISCOVERY_ASSETS']
+        self._API_ASSET = self._services['EDISCOVERY_ASSET']
         self.refresh()
 
     def _get_assets_properties(self):
         """gets the assets properties from inventory
 
                     Args:
                         None
 
                     Returns:
 
                         dict    --  containing asset properties
 
         """
-        inv_mgr = self._commcell_object.activate.inventory_manager()
-        inv_obj = inv_mgr.get(self._inventory_name)
-        inv_obj.refresh()
-        assets = {}
-        for asset in inv_obj.properties['assets']:
-            name = asset['name'].lower()
-            assets[name] = asset
-        return assets
+        flag, response = self._cvpysdk_obj.make_request(
+            'GET', self._API_ASSETS % self._inventory_id)
+        if flag:
+            if response.json() and 'assets' in response.json():
+                assets = {}
+                for asset in response.json()['assets']:
+                    name = asset['name'].lower()
+                    assets[name] = asset
+                return assets
+            else:
+                raise SDKException('Inventory', '102', "Unknown response while fetching assets on inventory")
+        else:
+            self._response_not_success(response)
 
     def refresh(self):
         """Refresh the assets details associated with this inventory"""
         self._assets = self._get_assets_properties()
 
     def _response_not_success(self, response):
         """Helper function to raise an exception when reponse status is not 200 (OK).
@@ -839,37 +873,34 @@
         """
         if not isinstance(asset_name, str):
             raise SDKException('Inventory', '101')
         if not self.has_asset(asset_name):
             raise SDKException('Inventory', '109')
         return Asset(self._commcell_object, self._inventory_name, asset_name, self._inventory_id)
 
-    def add(self, asset_name, asset_type=InventoryConstants.AssetType.NAME_SERVER, **kwargs):
+    def add(self, asset_name, asset_type=InventoryConstants.AssetType.IDENTITY_SERVER, **kwargs):
         """Adds asset to the inventory
 
                 Args:
 
                     asset_name          (str)       --  Name of the asset
 
                     asset_type          (Enum)      --  type of asset (Refer to InventoryConstants.AssetType class)
 
                     kwargs for FILE SERVER type Asset:
 
                             fqdn                --  File server FQDN
 
                             os                  --  File Server OS type
+                                                        (Default:Windows)
 
                             ip                  --  File server IP
 
                             country_code        --  Country code (ISO 3166 2-letter code)
 
-                            country_name        --  Country name
-
-                            domain              --  File Server Domain name(optional)
-
                 Returns:
 
                     object  --  Instance of Asset class
 
                 Raises:
 
                     SDKException:
@@ -877,48 +908,39 @@
                             if input is not valid
 
                             if failed to add asset to inventory
 
         """
         if not isinstance(asset_name, str) or not isinstance(asset_type, InventoryConstants.AssetType):
             raise SDKException('Inventory', '101')
-        request_json = copy.deepcopy(InventoryConstants.ASSET_ADD_TO_INVENTORY_JSON)
-        request_json['inventoryId'] = int(self._inventory_id)
-        asset_json = copy.deepcopy(InventoryConstants.ASSET_ADD_REQUEST_JSON)
-        asset_json['name'] = asset_name
-        asset_json['type'] = asset_type.value
-        property_json = copy.deepcopy(InventoryConstants.ASSET_PROPERTY_JSON)
+        request_json = {}
         if asset_type.value == InventoryConstants.AssetType.FILE_SERVER.value:
             for prop in InventoryConstants.ASSET_FILE_SERVER_PROPERTY:
                 prop_name = InventoryConstants.FIELD_PROPS_MAPPING[prop]
                 default_value = ""
                 if prop_name not in kwargs:
-                    # if domain is not passed, then form domain from fqdn
-                    if prop == InventoryConstants.FIELD_PROPERTY_DOMAIN:
-                        default_value = kwargs.get(InventoryConstants.KWARGS_FQDN)
-                        default_value = default_value.split(".", 1)[1]
                     # always use asset name as file server name
                     if prop == InventoryConstants.FIELD_PROPERTY_NAME:
                         default_value = asset_name
-                prop_json = copy.deepcopy(InventoryConstants.ASSET_PROPERTY_NAME_VALUE_PAIR_JSON)
-                prop_json['name'] = prop
-                prop_json['value'] = kwargs.get(prop_name, default_value)
-                property_json['propertyValues']['nameValues'].append(prop_json)
-            asset_json.update(property_json)
-        request_json['assets'].append(asset_json)
+                    if prop == InventoryConstants.FIELD_PROPERTY_OS:
+                        default_value = "Windows"
+                request_json[prop] = kwargs.get(prop_name, default_value)
+        else:
+            request_json = copy.deepcopy(InventoryConstants.IDENTITY_SERVER_ASSET_ADD_TO_INVENTORY_JSON)
+            request_json['identityServers'] = [asset_name]
+
         flag, response = self._cvpysdk_obj.make_request(
-            'PUT', self._API_INVENTORIES, request_json)
+            'PUT', self._API_ASSETS % self._inventory_id, request_json)
         if flag:
-            if response.json() and 'errorResp' in response.json():
-                err_resp = response.json()['errorResp']
-                if 'errorCode' in err_resp and err_resp['errorCode'] != 0:
+            if response.json():
+                if 'errorCode' in response.json() and response.json()['errorCode'] != 0:
                     raise SDKException(
                         'Inventory',
                         '102',
-                        f"Failed to add asset to inventory with error [{err_resp['errorMessage']}]")
+                        f"Failed to add asset to inventory with error [{response.json()['errorMessage']}]")
                 self.refresh()
                 return Asset(self._commcell_object, self._inventory_name, asset_name, self._inventory_id)
             raise SDKException('Inventory', '108')
         self._response_not_success(response)
 
     def delete(self, asset_name):
         """Delete the asset from the inventory
@@ -937,40 +959,28 @@
 
                             if input is not valid
 
                             if failed to delete the asset
 
                             if unable to find this asset in inventory
         """
+
         if not isinstance(asset_name, str):
             raise SDKException('Inventory', '101')
         if not self.has_asset(asset_name):
             raise SDKException('Inventory', '109')
-        request_json = copy.deepcopy(InventoryConstants.ASSET_DELETE_FROM_INVENTORY_JSON)
-        request_json['inventoryId'] = int(self._inventory_id)
-        if 'assetId' in self._assets[asset_name.lower()]:
-            request_json['assets'].append({'assetId': self._assets[asset_name.lower()]['assetId']})
-        else:
-            req = copy.deepcopy(InventoryConstants.ASSET_ADD_REQUEST_JSON)
-            asset_obj = self.get(asset_name)
-            asset_type = asset_obj.asset_type
-            # for file server asset, asset name will not be display name in backend delete request. so fetch fqdn
-            req['name'] = asset_obj.get_asset_prop(prop_name=InventoryConstants.FIELD_PROPERTY_DNSHOST)
-            req['type'] = asset_type
-            request_json['assets'].append(req)
         flag, response = self._cvpysdk_obj.make_request(
-            'PUT', self._API_ASSETS % self._inventory_id, request_json)
+            'DELETE', self._API_ASSET % (self._inventory_id, self._assets[asset_name.lower()]['id']))
         if flag:
             if response.json():
-                err_resp = response.json()['errorResp']
-                if 'errorCode' in err_resp and err_resp['errorCode'] != 0:
+                if 'errorCode' in response.json() and response.json()['errorCode'] != 0:
                     raise SDKException(
                         'Inventory',
                         '102',
-                        f"Failed to delete asset from inventory with error [{err_resp['errorMessage']}]")
+                        f"Failed to delete asset from inventory with error [{response.json()['errorMessage']}]")
                 self.refresh()
                 return
             raise SDKException('Inventory', '110')
         self._response_not_success(response)
 
     @property
     def assets(self):
@@ -1010,43 +1020,66 @@
         self._asset_name = asset_name
         self._asset_props = None
         self._asset_id = None
         self._crawl_start_time = None
         self._asset_type = None
         self._asset_status = None
         self._asset_name_values_props = None
+        self._API_ASSETS = self._services['EDISCOVERY_ASSETS']
+        self._API_ASSET = self._services['EDISCOVERY_ASSET']
+        self._API_ASSET_JOBS = self._services['EDISCOVERY_ASSET_JOBS']
         self.refresh()
-        self._ediscovery_client_obj = EdiscoveryClientOperations(class_object=self, commcell_object=commcell_object)
+
+    def _response_not_success(self, response):
+        """Helper function to raise an exception when reponse status is not 200 (OK).
+
+            Args:
+                response    (object)    --  response class object,
+
+                received upon running an API request, using the `requests` python package
+
+        """
+        raise SDKException('Response', '101', self._update_response_(response.text))
 
     def _get_properties(self):
         """Returns the properties of this asset
 
                 Args:
 
                     None
 
                 Returns:
 
                     dict        -- Containing properties of asset
 
         """
-        inv_mgr = self._commcell_object.activate.inventory_manager()
-        inv_obj = inv_mgr.get(self._inventory_name)
-        inv_obj.get_assets().refresh()
-        for asset in inv_obj.properties['assets']:
-            if asset['name'].lower() == self._asset_name.lower():
-                # for file server, we will not have asset id & crawl times
-                self._asset_id = asset.get('assetId', 0)
-                self._crawl_start_time = asset.get('crawlStartTime', 0)
-                self._asset_type = asset.get('type', 0)
-                self._asset_status = asset['status']
-                self._asset_name = asset['name']
-                self._asset_name_values_props = asset['propertyValues']['nameValues']
-                return asset
-        return {}
+
+        flag, response = self._cvpysdk_obj.make_request(
+            'GET', self._API_ASSETS % self._inventory_id)
+        if flag:
+            if response.json() and 'assets' in response.json():
+                for asset in response.json()['assets']:
+                    if asset['name'].lower() == self._asset_name.lower():
+                        self._asset_id = asset.get('id', "")
+                        self._crawl_start_time = asset.get('lastCollectionTime', 0)
+                        self._asset_type = asset.get('type', "")
+                        self._asset_status = asset.get('status', "NA")
+                        self._asset_name = asset['name']
+                        if self._asset_type == InventoryConstants.AssetType.FILE_SERVER.name:
+                            flag, response = self._cvpysdk_obj.make_request(
+                                'GET', self._API_ASSET % (self._inventory_id, self._asset_id))
+                            if flag:
+                                if response.json() and 'properties' in response.json():
+                                    self._asset_name_values_props = response.json()['properties']
+                        return asset
+                return {}
+            else:
+                raise SDKException('Inventory', '102', "Unknown response while fetching assets on inventory")
+        else:
+            self._response_not_success(response)
 
     def refresh(self):
         """Refresh the asset details associated with this"""
         self._asset_props = self._get_properties()
 
     def get_job_history(self):
         """Returns the job history details of this asset
@@ -1063,67 +1096,48 @@
                     SDKException:
 
                             if failed to get job history
 
                             if asset is not supported for this operation
 
         """
-        if self.asset_type != InventoryConstants.AssetType.NAME_SERVER.value:
+        if self.asset_type != InventoryConstants.AssetType.IDENTITY_SERVER.name:
             raise SDKException('Inventory', '102', "Not supported other than Name Server asset type")
-        return self._ediscovery_client_obj.get_job_history()
+        flag, response = self._cvpysdk_obj.make_request(
+            'GET', self._API_ASSET_JOBS % (self._inventory_id, self._asset_id))
+        if flag:
+            if response.json() and 'jobs' in response.json():
+                return response.json()['jobs']
+            raise SDKException('Inventory', '102', "Unknown response while fetching job history on inventory")
+        else:
+            self._response_not_success(response)
 
     def get_job_status(self):
-        """Returns the job status details of this asset
+        """Returns the latest job status details of this asset
 
                 Args:
                     None
 
                 Returns:
 
-                    dict    --  containing job status details
+                    str    --  last job status (Eg:- RUNNING / IDLE)
 
                 Raises:
 
                     SDKException:
 
                             if failed to get job status
 
                              if asset is not supported for this operation
 
         """
-        if self.asset_type != InventoryConstants.AssetType.NAME_SERVER.value:
-            raise SDKException('Inventory', '102', "Not supported other than Name Server asset type")
-        return self._ediscovery_client_obj.get_job_status()
-
-    def start_collection(self, wait_for_job=False, wait_time=60):
-        """Starts collection job on this asset
-
-                Args:
-
-                    wait_for_job        (bool)      --  specifies whether to wait for job to complete or not
-
-                    wait_time           (int)       --  time interval to wait for job completion in Mins
-                                                            Default : 60Mins
-
-                Return:
-
-                    None
-
-                Raises:
-
-                    SDKException:
-
-                            if failed to start collection job
-
-                            if asset is not supported for this operation
-
-        """
-        if self.asset_type != InventoryConstants.AssetType.NAME_SERVER.value:
+        if self.asset_type != InventoryConstants.AssetType.IDENTITY_SERVER.name:
             raise SDKException('Inventory', '102', "Not supported other than Name Server asset type")
-        return self._ediscovery_client_obj.start_job(wait_for_job=wait_for_job, wait_time=wait_time)
+        self.refresh()  # do refresh before getting current status
+        return self.asset_status
 
     def get_asset_prop(self, prop_name):
         """returns the property value for given property name for this asset
 
             Args:
 
                 prop_name       (str)       --  Name of the property
```

### Comparing `cvpysdk-11.30.1/cvpysdk/activateapps/request_manager.py` & `cvpysdk-11.32/cvpysdk/activateapps/request_manager.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/activateapps/sensitive_data_governance.py` & `cvpysdk-11.32/cvpysdk/activateapps/sensitive_data_governance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/activitycontrol.py` & `cvpysdk-11.32/cvpysdk/activitycontrol.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/agent.py` & `cvpysdk-11.32/cvpysdk/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,23 +197,24 @@
 
                     if response is not success
         """
         flag, response = self._cvpysdk_object.make_request('GET', self._AGENTS)
 
         if flag:
             if response.json() and 'agentProperties' in response.json():
-
                 agent_dict = {}
-
                 for dictionary in response.json()['agentProperties']:
                     temp_name = dictionary['idaEntity']['appName'].lower()
                     temp_id = str(dictionary['idaEntity']['applicationId']).lower()
                     agent_dict[temp_name] = temp_id
 
                 return agent_dict
+            elif self._client_object.vm_guid is not None and not self._client_object.properties.get('clientProps', {}).\
+                    get('isIndexingV2VSA', False):
+                return {}
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101', self._update_response_(response.text))
 
     @property
     def all_agents(self):
@@ -927,14 +928,28 @@
                     o_str = 'Failed to disable Backup\nError: "{0}"'.format(error_message)
                     raise SDKException('Agent', '102', o_str)
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101', self._update_response_(response.text))
 
+    def enable_ews_support_for_exchange_on_prem(self, ews_service_url : str):
+        """
+            Method to enable EWS backup support for an Exchange on-prem client.
+            Args:
+                ews_service_url (string) -- EWS Connection URL for your exchange server
+        """
+        if int(self.agent_id) != 137:
+            raise SDKException('Agent', '102', f'Invalid operation for {self.agent_name}')
+
+        _agent_properties = self.properties
+        _agent_properties["onePassProperties"]["onePassProp"]["ewsDetails"]["bUseEWS"] = True
+        _agent_properties["onePassProperties"]["onePassProp"]["ewsDetails"]["ewsConnectionUrl"] = ews_service_url
+        self.update_properties(_agent_properties)
+
     def refresh(self):
         """Refresh the properties of the Agent."""
         self._get_agent_properties()
 
         self._instances = None
         self._backupsets = None
         self._schedules = None
```

### Comparing `cvpysdk-11.30.1/cvpysdk/agents/__init__.py` & `cvpysdk-11.32/cvpysdk/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/agents/exchange_database_agent.py` & `cvpysdk-11.32/cvpysdk/agents/exchange_database_agent.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/alert.py` & `cvpysdk-11.32/cvpysdk/alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,18 @@
 
     **alert_criteria**          --  returns the criteria of an alert
 
     **notification_types**      --  returns the notification types of an alert
 
     **description**             --  returns the description of an alert
 
+    **users_list**              --  returns the list of users associated with the alert
+
+    **user_group_list**         --  returns the list of user groups associated with the alert
+
     **entities**                --  returns the list of entities associated with an alert
 
     **email_recipients**        --  returns the list of email recipients associated to the alert
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
@@ -330,28 +334,40 @@
                 "_type_": 17
             }
         }
 
         associations = []
 
         for entity, values in entities.items():
-            entity_obj = getattr(self._commcell_object, entity)
+            if entity == "entity_type_names":
+                for value in values:
+                    if value == "ALL_CLIENT_GROUPS_ENTITY":
+                        entity_type = 27
+                    else:
+                        entity_type = 2
+                    temp_dict = {
+                        "entityTypeName": value,
+                        "_type_": entity_type
+                    }
+                    associations.append(temp_dict)
+            else:
+                entity_obj = getattr(self._commcell_object, entity)
 
-            # this will allows us to loop through even for single item
-            values = values.split() if not isinstance(values, list) else values
+                # this will allows us to loop through even for single item
+                values = values.split() if not isinstance(values, list) else values
 
-            for value in values:
-                temp_dict = entity_dict[entity].copy()
-                for name, entity_attr in temp_dict.items():
-                    if name != "_type_":
-                        try: # to convert the string values to int types
-                            temp_dict[name] = int(getattr(entity_obj.get(value), entity_attr))
-                        except ValueError:
-                            temp_dict[name] = getattr(entity_obj.get(value), entity_attr)
-                associations.append(temp_dict)
+                for value in values:
+                    temp_dict = entity_dict[entity].copy()
+                    for name, entity_attr in temp_dict.items():
+                        if name != "_type_":
+                            try: # to convert the string values to int types
+                                temp_dict[name] = int(getattr(entity_obj.get(value), entity_attr))
+                            except ValueError:
+                                temp_dict[name] = getattr(entity_obj.get(value), entity_attr)
+                    associations.append(temp_dict)
 
         return associations
 
 
     def _get_alert_json(self, alert_json):
         """To form the json required to create an alert
 
@@ -854,17 +870,21 @@
                             pass
 
                 if 'regularNotifications' in self._alert_detail:
                     self._notification_types = self._alert_detail["regularNotifications"]
 
                 if 'userList' in self._alert_detail:
                     self._users_list = [user['name'] for user in self._alert_detail['userList']]
+                else:
+                    self._users_list = []
 
                 if 'userGroupList' in self._alert_detail:
                     self._user_group_list = [grp['name'] for grp in self._alert_detail['userGroupList']]
+                else:
+                    self._user_group_list = []
 
                 self._email_recipients = []
                 if 'nonGalaxyUserList' in self._alert_detail:
                     self._email_recipients = [email['name'] for email in self._alert_detail['nonGalaxyUserList']]
 
             else:
                 raise SDKException('Response', '102')
@@ -888,16 +908,21 @@
                     "alertrule": {
                         "alertName": self._alert_name
                     },
                     "criteria": {
                         "criteria": int(self._criteria[0]['criteria_id'])
                     },
                     "userList": {
+                        "userListOperationType": 1,
                         "userList": [{"userName": user} for user in self._users_list]
                     },
+                    "userGroupList": {
+                        "userGroupListOperationType": 1,
+                        "userGroupList": [{"userGroupName": user} for user in self._user_group_list]
+                    },
                     "nonGalaxyList": {
                         "nonGalaxyUserList": [{"nonGalaxyUser": email} for email in self._email_recipients]
                     },
                     "EntityList": {
                         "associations": self._entities_list
                     }
                 }
@@ -1036,14 +1061,36 @@
         return self._description
 
     @description.setter
     def description(self, description):
         """Modifies the Alert description"""
         self._description = description
         self._modify_alert_properties()
+    
+    @property
+    def users_list(self):
+        """Treats the users list as a read-only attribute."""
+        return self._users_list
+
+    @users_list.setter
+    def users_list(self, users_list):
+        """Modifies the users list"""
+        self._users_list = users_list
+        self._modify_alert_properties()
+    
+    @property
+    def user_group_list(self):
+        """Treats the user group list as a read-only attribute."""
+        return self._user_group_list
+
+    @user_group_list.setter
+    def user_group_list(self, user_group_list):
+        """Modifies the user group list"""
+        self._user_group_list = user_group_list
+        self._modify_alert_properties()
 
     def enable_notification_type(self, alert_notification_type):
         """Enable the notification type.
 
             Args:
                 alert_notification_type (str)  --  alert notification to enable
```

### Comparing `cvpysdk-11.30.1/cvpysdk/array_management.py` & `cvpysdk-11.32/cvpysdk/array_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     edit_array()                --  Method to Update Snap Configuration and Array Access Node MA
                                     for the given Array
 """
 
 from __future__ import unicode_literals
 from .job import Job
 from .exception import SDKException
+import base64
 
 
 class ArrayManagement(object):
     """Class for representing all the array management activities with the commcell."""
 
     def __init__(self, commcell_object):
         """ Initialize the ArrayManagement class instance for performing Snap related operations
@@ -348,14 +349,17 @@
                                 "id": 262144
                             }
                         }
                     ]
                 }
                 selectedMAs.append(node_dict)
 
+        if password is not None:
+            password = base64.encodebytes(password.encode()).decode()
+
         request_json = {
             "clientId": 0,
             "flags": 0,
             "assocType": assocType,
             "copyId": 0,
             "appId": 0,
             "selectedMAs":selectedMAs,
@@ -638,14 +642,15 @@
                     if "selectedMAs" in request_json:
                         for controller in range(len(request_json['selectedMAs'])):
                             if request_json['selectedMAs'][controller]['mediaAgent']['id'] == int(client_id):
                                 del request_json['selectedMAs'][controller]
                                 break
 
         request_json['configs'] = request_json.pop('configList')
+        del request_json['info']['region']
 
         flag, response = self._commcell_object._cvpysdk_object.make_request(
             'PUT', self.storage_arrays, request_json
         )
 
         if response.json() and 'errorCode' in response.json():
             error_code = response.json()['errorCode']
```

### Comparing `cvpysdk-11.30.1/cvpysdk/backup_network_pairs.py` & `cvpysdk-11.32/cvpysdk/backup_network_pairs.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupset.py` & `cvpysdk-11.32/cvpysdk/backupset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1445,15 +1445,17 @@
                 "mode": mode
             },
             "paths": [{"path": path} for path in paths],
             "options": {
                 "showDeletedFiles": options['show_deleted'],
                 "restoreIndex": options['restore_index'],
                 "vsDiskBrowse": options['vm_disk_browse'],
-                "vsFileBrowse": options.get('vs_file_browse', False)
+                "vsFileBrowse": options.get('vs_file_browse', False),
+                "includeMetadata": options.get('include_meta_data', False),
+                "hideUserHidden": options.get('hide_user_hidden', False)
             },
             "entity": {
                 "clientName": self._client_object.client_name,
                 "clientId": int(self._client_object.client_id),
                 "applicationId": int(self._agent_object.agent_id),
                 "instanceId": int(self._instance_object.instance_id),
                 "backupsetId": int(self.backupset_id),
@@ -2302,23 +2304,49 @@
     def refresh(self):
         """Refresh the properties of the Backupset."""
         self._get_backupset_properties()
 
         self.subclients = Subclients(self)
         self.schedules = Schedules(self)
 
-    def backed_up_files_count(self):
+    def backed_up_files_count(self, path="\\**\\*"):
         """Returns the count of the total number of files present in the backed up data
-         of all the subclients of the given backupset.
+         of all the subclients of the given backupset and given path.
+
+                Args:
+
+                    path        (str)       --  Folder path to find no of backed up files
+                                                    (Default: \\**\\*)
+
+                Returns:
+
+                    int --  No of backed up files count in given path
+
+                Raises:
+
+                    Exception:
+
+                        if browse response is not proper
          """
-        options_dic = {"operation": "find", "opType": 1, "path": "\**\*",
-               "_custom_queries": [{"type": "AGGREGATE", "queryId": "2",
-                                    "aggrParam": {"aggrType": "COUNT"}, "whereClause": [{
-                       "criteria": {
-                           "field": "Flags",
-                           "dataOperator": "IN",
-                           "values": ["file"]
-                       }
-                   }]}], "_raw_response": True}
+        options_dic = {"operation": "find", "opType": 1, "path": path,
+                       "_custom_queries": [{"type": "AGGREGATE", "queryId": "2",
+                                            "aggrParam": {"aggrType": "COUNT"}, "whereClause": [{
+                                                "criteria": {
+                                                    "field": "Flags",
+                                                    "dataOperator": "IN",
+                                                    "values": ["file"]
+                                                }
+                                            }]}], "_raw_response": True}
 
         browse_response = self._do_browse(options_dic)
-        return browse_response[1]['browseResponses'][0]['browseResult']['aggrResultSet'][0]['count']
+        if not len(browse_response) > 1:
+            raise SDKException('Backupset', '102', 'Browse response is not proper')
+        browse_response = browse_response[1]
+        if 'browseResponses' not in browse_response or len(browse_response['browseResponses']) == 0:
+            raise SDKException('Backupset', '102', 'Browse response is missing browseResponses')
+        browse_response = browse_response['browseResponses'][0]
+        if 'browseResult' not in browse_response:
+            raise SDKException('Backupset', '102', 'Browse response is missing browseResult')
+        browse_result = browse_response['browseResult']
+        if 'aggrResultSet' not in browse_result or len(browse_result['aggrResultSet']) == 0:
+            raise SDKException('Backupset', '102', 'Browse response is missing aggrResultSet')
+        return browse_result['aggrResultSet'][0].get('count', 0)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/__init__.py` & `cvpysdk-11.32/cvpysdk/backupsets/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/_virtual_server/__init__.py` & `cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/_virtual_server/kubernetes.py` & `cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/kubernetes.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/_virtual_server/vmware.py` & `cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/vmware.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/aadbackupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/aadbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/adbackupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/adbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/cabackupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/cabackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/cloudapps/__init__.py` & `cvpysdk-11.32/cvpysdk/backupsets/cloudapps/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/cloudapps/salesforce_backupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/cloudapps/salesforce_backupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/db2backupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/db2backupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/fsbackupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/fsbackupset.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,39 @@
                 "esxServerName": " ", "userPassword": {
 
                 }
             }
         }
         return bmr_restore_json
 
+    def _restore_bmr_firewallopts_json(self, hostname, direction, port):
+        """Get the JSON for firewall configuration options
+
+        Args:
+            hostname    (String)   -- The hostname of the machine.
+
+            direction   (Integer)  -- The direction of the connection.
+
+            port        (Integer)  -- The port at which the machine will communicate.
+
+        Returns :
+                    The firewall configuration options JSON required for Virtualize Me restores
+
+        """
+        bmr_firewall_restore_json = {
+            "direction": direction,
+            "connectionInfoList": [
+                {
+                    "hostname": hostname,
+                    "port": port
+                }
+            ]
+        }
+        return bmr_firewall_restore_json
+
     def _azure_advancedrestoreopts_json(self):
         """Get the JSON for Advanced restore options for azure
 
 
         Returns :
                     The Advanced restore options JSON required for Virtualize Me to Azure restores
 
@@ -611,15 +636,25 @@
 
         hwconfig, ipconfig, cs_username, cs_password = self._get_responsefile()
         response_json = self._restore_json(paths=[''])
 
         restore_json_system_state = self._restore_bmr_admin_json(ipconfig, hwconfig)
         restore_json_virtualserver = self._restore_bmr_virtualserveropts_json()
 
-        # get instance Id of the virtual client
+        #Checking for Firewall rules
+        if restore_options.get("FirewallClientGroup", "").strip():
+            fwconfigtocs = self._restore_bmr_firewallopts_json(restore_options.get("FirewallHostname"),
+                                                               restore_options.get("FirewallDirection"),
+                                                               restore_options.get("FirewallPort"))
+            restore_json_system_state['vmProvisioningOption']['virtualMachineOption'][0][
+                'oneTouchResponse']['clients'][0]['fwconfigtocs'] = fwconfigtocs
+            restore_json_system_state['vmProvisioningOption']['virtualMachineOption'][0]['oneTouchResponse']['csinfo'][
+                'fwClientGroupName'] = restore_options.get("FirewallClientGroup")
+
+        #Get instance Id of the virtual client
         virtual_client_object = self._commcell_object.clients.get(restore_options.get('VirtualizationClient'))
         virtual_agent_object = virtual_client_object.agents.get('Virtual Server')
         instances_list = virtual_agent_object.instances._instances
         instance_id = int(list(instances_list.values())[0])
         instance_name = list(instances_list.keys())[0]
 
         response_json['taskInfo']['subTasks'][0]['options'][
@@ -632,19 +667,17 @@
             'inPlace'] = False
         response_json['taskInfo']['subTasks'][0]['subTask']['subTaskType'] = 1
         response_json['taskInfo']['subTasks'][0]['subTask']['operationType'] = 4041
 
         vm_option = response_json['taskInfo']['subTasks'][0]['options']['adminOpts'][
             'vmProvisioningOption']['virtualMachineOption'][0]
 
-
         vm_option['vmInfo']['vmLocation']['instanceEntity']['clientName'] = restore_options.get('VirtualizationClient')
         vm_option['vmInfo']['vmLocation']['instanceEntity']['instanceId'] = instance_id
 
-
         if(response_json['taskInfo']['subTasks'][0]['options']['adminOpts'][
             'vmProvisioningOption']['virtualMachineOption'][0]['oneTouchResponse'][
             'hwconfig']['mem_size']) < 4096:
             vm_option['oneTouchResponse']['hwconfig']['mem_size'] = 4096
 
         if restore_options.get('CommServIP'):
             cs_ip = restore_options.get('CommServIP')
@@ -682,14 +715,17 @@
         if instance_name == 'vmware' or instance_name == 'hyper-v':
 
             vm_option['isoPath'] = restore_options.get('IsoPath')
 
             vm_option['vmInfo']['vmLocation']['pathName'] = restore_options.get('IsoPath', None)
 
             vm_option['oneTouchResponse']['clients'][0]['netconfig']['ipinfo']['interfaces'][0][
+                'protocols'][0]['useDhcp'] = True
+
+            vm_option['oneTouchResponse']['clients'][0]['netconfig']['ipinfo']['interfaces'][0][
                 'networkLabel'] = restore_options.get('NetworkLabel', None)
 
             if 'scsi_disks' in vm_option['oneTouchResponse']['hwconfig']:
                 vm_option['oneTouchResponse']['hwconfig']['scsi_disks'][0][
                     'dataStoreName'] = restore_options.get('Datastore', None)
 
             if 'ide_disks' in vm_option['oneTouchResponse']['hwconfig']:
```

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/hanabackupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/hanabackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/nasbackupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/nasbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/postgresbackupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/postgresbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/sharepointbackupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/sharepointbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/backupsets/vsbackupset.py` & `cvpysdk-11.32/cvpysdk/backupsets/vsbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/certificates.py` & `cvpysdk-11.32/cvpysdk/certificates.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/client.py` & `cvpysdk-11.32/cvpysdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,27 +53,30 @@
 
     _get_hidden_clients()                 --  gets all the hidden clients associated with the
     commcell
 
     _get_virtualization_clients()         --  gets all the virtualization clients associated with
     the commcell
 
+    _get_virtualization_access_nodes()    --  gets all the virtualization access nodes associated with
+    the commcell
+
     _get_client_dict()                    --  returns the client dict for client to be added to
     member server
 
     _member_servers()                     --  returns member clients to be associated with the
     Virtual Client
 
     _get_client_from_hostname()           --  returns the client name if associated with specified
     hostname if exists
 
     _get_hidden_client_from_hostname()    --  returns the client name if associated with specified
     hostname if exists
 
-     _get_client_from_displayname()        --  get the client name for given display name
+    _get_client_from_displayname()        --  get the client name for given display name
 
     has_client(client_name)               --  checks if a client exists with the given name or not
 
     has_hidden_client(client_name)        --  checks if a hidden client exists with the given name
 
     _process_add_response()               -- to process the add client request using API call
 
@@ -128,14 +131,17 @@
 
     **hidden_clients**          --  returns the dictionary consisting of only the hidden clients
     that are associated with the commcell and their information such as id and hostname
 
     **virtualization_clients**  --  returns the dictionary consisting of only the virtualization
     clients that are associated with the commcell and their information such as id and hostname
 
+    **virtualization_access_nodes** --  returns the dictionary consisting of only the virtualization
+    clients that are associated with the commcell and their information such as id and hostname
+
     **office365_clients**       --  Returns the dictionary consisting of all the office 365 clients that are
                                     associated with the commcell
 
     **dynamics365_clients**     --  Returns the dictionary consisting of all the Dynamics 365 clients
                                     that are associated with the commcell
 
     **salesforce_clients**      --  Returns the dictionary consisting of all the salesforce clients that are
@@ -343,14 +349,26 @@
     **cvd_port**                    -- returns cvd port of the client
 
     **vm_guid**                     -- returns guid of the vm client
 
     **company_name**                 -- returns company name for the client
 
     **is_privacy_enabled**          -- returns if client privacy is enabled
+
+    **latitude**                    -- Returns the latitude from geo location of the client
+
+    **longitude**                   -- Returns the longitude from geo location of the client
+
+    **is_vm**                       -- Returns True if its a VM client
+
+    **hyperv_id_of_vm**             -- Returns the Id of hyperV that the given VM is associated with
+
+    **associated_client_group**     -- Returns the list of clientgroups that the client is associated to
+
+    **company_id**                  -- Returns the company Id of the client
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 import os
 import re
@@ -401,24 +419,26 @@
         # them
         self._CLIENTS = self._ADD_CLIENT = self._services['GET_ALL_CLIENTS']
         self._OFFICE_365_CLIENTS = self._services['GET_OFFICE_365_ENTITIES']
         self._DYNAMICS365_CLIENTS = self._services['GET_DYNAMICS_365_CLIENTS']
         self._SALESFORCE_CLIENTS = self._services['GET_SALESFORCE_CLIENTS']
         self._ALL_CLIENTS = self._services['GET_ALL_CLIENTS_PLUS_HIDDEN']
         self._VIRTUALIZATION_CLIENTS = self._services['GET_VIRTUAL_CLIENTS']
+        self._GET_VIRTUALIZATION_ACCESS_NODES = self._services['GET_VIRTUALIZATION_ACCESS_NODES']
         self._FS_CLIENTS = self._services['GET_FILE_SERVER_CLIENTS']
         self._ADD_EXCHANGE_CLIENT = self._ADD_SHAREPOINT_CLIENT = self._ADD_SALESFORCE_CLIENT = \
             self._services['CREATE_PSEUDO_CLIENT']
         self._ADD_SPLUNK_CLIENT = self._services['CREATE_PSEUDO_CLIENT']
         self._ADD_NUTANIX_CLIENT = self._services['CREATE_NUTANIX_CLIENT']
         self._ADD_NAS_CLIENT = self._services['CREATE_NAS_CLIENT']
         self._ADD_ONEDRIVE_CLIENT = self._services['CREATE_PSEUDO_CLIENT']
         self._clients = None
         self._hidden_clients = None
         self._virtualization_clients = None
+        self._virtualization_access_nodes = None
         self._office_365_clients = None
         self._dynamics365_clients = None
         self._salesforce_clients = None
         self._file_server_clients = None
         self.refresh()
 
     def __str__(self):
@@ -663,16 +683,15 @@
                 return {
                     self.all_clients[sf_subclient['clientName'].lower()]['displayName']: {
                         'id': sf_subclient['clientId'],
                         'clientName': sf_subclient['clientName']
                     }
                     for sf_subclient in map(lambda org: org['sfSubclient'], response.json()['orgs'])
                 }
-            else:
-                raise SDKException('Response', '102')
+            return {}
         else:
             raise SDKException('Response', '101', self._update_response_(response.text))
 
     @property
     def salesforce_clients(self):
         """Returns the dict of all salesforce clients in the commcell"""
         if self._salesforce_clients is None:
@@ -787,14 +806,57 @@
 
                 return virtualization_clients
 
             return {}
         else:
             raise SDKException('Response', '101', self._update_response_(response.text))
 
+    def _get_virtualization_access_nodes(self):
+        """REST API call to get all virtualization access nodes in the commcell
+            Returns:
+                dict - consists of all access nodes in the commcell
+                {
+                     "display_name1": {
+                            "id": client1_id,
+                            "name": client1_name,
+                            "hostname": client1_hostname
+                    },
+                     "display_name2": {
+                            "id": client2_id,
+                            "name": client2_name,
+                            "hostname": client2_hostname
+                     },
+                }
+
+            Raises:
+                SDKException:
+                    if response is empty
+
+                    if response is not success
+        """
+        flag, response = self._cvpysdk_object.make_request('GET', self._GET_VIRTUALIZATION_ACCESS_NODES)
+
+        virtualization_access_nodes = {}
+        if flag and response:
+            if response.json() and 'clients' in response.json():
+                for virtualization_access_node in response.json()['clients']:
+                    client_id = virtualization_access_node.get('clientId')
+                    client_name = virtualization_access_node.get('clientName').lower()
+                    display_name = virtualization_access_node.get('displayName').lower()
+                    host_name = virtualization_access_node.get('hostName').lower()
+                    if client_name:
+                        virtualization_access_nodes[display_name] = {
+                            'id': client_id,
+                            'name': client_name,
+                            'hostName': host_name
+                        }
+            return virtualization_access_nodes
+        else:
+            raise SDKException('Response', '101', self._update_response_(response.text))
+
     def _get_fileserver_clients(self):
         """REST API call to get all file server clients in the commcell
 
             Returns:
                 dict    -   consists of all file server clients in the commcell
 
                     {
@@ -927,38 +989,37 @@
         # verify there is no client in the Commcell with the same name as the given hostname
         # for multi-instance clients
         if self.hidden_clients and hostname not in self.hidden_clients:
             for hidden_client in self.hidden_clients:
                 if hostname.lower() == self.hidden_clients[hidden_client]['hostname']:
                     return hidden_client
 
-    def _get_client_from_displayname(self, displayname):
-        """get the client name for given displayname
-            name
-
+    def _get_client_from_displayname(self, display_name):
+        """get the client name for given display name
             Args:
-                displayname    (str)   --  displayname of the  client on this commcell
+                displayname    (str)   --  display name of the  client on this commcell
 
             Returns:
-                str     -   name of the client associated with this displayname
-            
-                None    -   if no client has the displayname as the given input
+                str     -   name of the client associated with this display name
+
+                None    -   None when no clients exists with this name
             Raises:
                 Exception:
                     if multiple clients has same display name
         """
-        displayname_occurence = 0
-        for client  in self._get_clients():
-            if self._get_clients()[client]['displayName'] == displayname:
-                displayname_occurence += 1
+        display_name_occurence = 0
+        client_name = None
+        for client in self.all_clients:
+            if self.all_clients[client]['displayName'] == display_name:
+                display_name_occurence += 1
                 client_name = client
-        if displayname_occurence > 1:
-            raise Exception('multiple clients have same display name')
-        else:
-            return client_name
+            if display_name_occurence > 1:
+                raise SDKException('Client', '102', 'Multiple clients have the same display name')
+        return client_name
+
 
     @property
     def all_clients(self):
         """Returns the dictionary consisting of all the clients and their info.
 
             dict - consists of all clients in the commcell
                     {
@@ -986,38 +1047,38 @@
 
                 client_type(str)     --  OS/Type of client to be created
                     default : "windows"
 
                     Available Values for client_type : "windows"
                                                        "unix"
                                                        "unix cluster"
+                                                       "sap hana"
 
             Returns:
                 client object for the created client.
 
             Raises:
                 SDKException:
                     if client name type is incorrect
 
                     if response is empty
 
                     if failed to get client id from response
 
         """
+        client_type_dict = {
+            "windows": "WINDOWS",
+            "unix": "UNIX",
+            "unix cluster": 11,
+            "sap hana": 16
+        }
         if not isinstance(client_name, str):
             raise SDKException('Client', '101')
 
-        if "windows" in client_type.lower():
-            os_id = 0
-
-        if "unix" in client_type.lower():
-            os_id = 1
-
-        if "unix cluster" in client_type.lower():
-            os_id = 11
+        os_id = client_type_dict[client_type.lower()]
 
         request_json = {
             'App_CreatePseudoClientRequest':
                 {
                     "registerClient": "false",
                     "clientInfo": {
                         "clientType": os_id,
@@ -1144,14 +1205,34 @@
                          },
                     }
 
         """
         return self._virtualization_clients
 
     @property
+    def virtualization_access_nodes(self):
+        """Returns the dictionary consisting of the virtualization access nodes
+
+                dict - consists of all access nodes in the commcell
+                {
+                     "display_name1": {
+                            "id": client1_id,
+                            "name": client1_name,
+                            "hostname": client1_hostname
+                    },
+                     "display_name2": {
+                            "id": client2_id,
+                            "name": client2_name,
+                            "hostname": client2_hostname
+                     },
+                }
+        """
+        return self._virtualization_access_nodes
+
+    @property
     def file_server_clients(self):
         """Returns the dictionary consisting of the file server clients and their info.
 
             dict - consists of all file server clients in the commcell
                     {
                         "client1_name": {
 
@@ -1709,14 +1790,21 @@
 
                 azure_app_id            (str)       --  azure app id for sharepoint online
 
                 azure_app_key_id        (str)       --  app key for sharepoint online
 
                 azure_directory_id    (str)   --  azure directory id for sharepoint online
 
+                cloud_region            (int)   --  stores the cloud region for the SharePoint client
+                                                    - Default (Global Service) [1]
+                                                    - Germany [2]
+                                                    - China [3]
+                                                    - U.S. Government GCC [4]
+                                                    - U.S. Government GCC High [5]
+
 
             Returns:
                 object  -   instance of the Client class for this new client
 
             Raises:
                 SDKException:
                     if client with given name already exists
@@ -1806,19 +1894,23 @@
             },
             "entity": {
                 "clientName": client_name
             }
 
         }
         tenant_url = kwargs.get('tenant_url')
+        if 'cloud_region' in kwargs.keys():
+            cloud_region = kwargs.get('cloud_region')
+        else:
+            cloud_region = 1
         global_administrator = kwargs.get('global_administrator')
         request_json["clientInfo"]["sharepointPseudoClientProperties"]["sharepointBackupSet"][
             "spOffice365BackupSetProp"] = {
             "tenantUrlItem": tenant_url,
-            "cloudRegion": 1,
+            "cloudRegion": cloud_region,
             "isModernAuthEnabled": kwargs.get('is_modern_auth_enabled', False),
             "infraStructurePoolEnabled": False,
              "office365Credentials": {
                     "userName": ""
                 }
         }
         if global_administrator:
@@ -3314,45 +3406,45 @@
                     raise SDKException('Response', '102')
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101', self._update_response_(response.text))
 
     def get(self, name):
-        """Returns a client object if client name or host name or ID matches the client attribute
+        """Returns a client object if client name or host name or ID or display name matches the client attribute
             We check if specified name matches any of the existing client names else
             compare specified name with host names of existing clients else if name matches with the ID
 
             Args:
-                name (str/int)  --  name / hostname / ID of the client
+                name (str/int)  --  name / hostname / ID of the client / display name
 
             Returns:
                 object - instance of the Client class for the given client name
 
             Raises:
                 SDKException:
                     if type of the client name argument is not string or Int
 
                     if no client exists with the given name
         """
         if isinstance(name, str):
             name = name.lower()
             client_name = None
             client_id = None
-
+            client_from_hostname = None
             if self.has_client(name):
                 client_from_hostname = self._get_client_from_hostname(name)
                 if self.has_hidden_client(name) and not client_from_hostname and name not in self.all_clients:
                     client_from_hostname = self._get_hidden_client_from_hostname(name)
-            elif not self.has_client(name):
-                client_from_hostname = self._get_client_from_displayname(name)
             else:
-                raise SDKException(
-                    'Client', '102', 'No client exists with given name/hostname: {0}'.format(name)
-                )
+                name = self._get_client_from_displayname(name)
+                if name is None:
+                    raise SDKException(
+                        'Client', '102', 'No client exists with given name/hostname: {0}'.format(name)
+                    )
 
             client_name = name if client_from_hostname is None else client_from_hostname
 
             if client_name in self.all_clients:
                 client_id = self.all_clients[client_name]['id']
             elif client_name in self.hidden_clients:
                 client_id = self.hidden_clients[client_name]['id']
@@ -3450,14 +3542,15 @@
                 )
 
     def refresh(self):
         """Refresh the clients associated with the Commcell."""
         self._clients = self._get_clients()
         self._hidden_clients = self._get_hidden_clients()
         self._virtualization_clients = self._get_virtualization_clients()
+        self._virtualization_access_nodes = self._get_virtualization_access_nodes()
         self._office_365_clients = None
         self._file_server_clients = None
         self._salesforce_clients = None
 
 
 class Client(object):
     """Class for performing client operations for a specific client."""
@@ -3562,15 +3655,20 @@
         self._job_start_time = None
         self._timezone = None
         self._is_privacy_enabled = None
 
         self._readiness = None
         self._vm_guid = None
         self._company_name = None
-
+        self._is_vm = None
+        self._vm_hyperv_id = None
+        self._client_latitude = None
+        self._client_longitude = None
+        self._associated_client_groups = None
+        self._company_id = None
         self.refresh()
 
     def __repr__(self):
         """String representation of the instance of this class."""
         representation_string = 'Client class instance for Client: "{0}"'
         return representation_string.format(self.client_name)
 
@@ -3668,14 +3766,34 @@
 
                 if 'jobStartTime' in client_props:
                     self._job_start_time = client_props['jobStartTime']
 
                 if 'BlockLevelCacheDir' in client_props:
                     self._block_level_cache_dir = client_props['BlockLevelCacheDir']
 
+                if 'clientRegionInfo' in client_props:
+                    self._client_latitude = client_props.get('clientRegionInfo', {}).get('geoLocation', {}). \
+                        get('latitude')
+                    self._client_longitude = client_props.get('clientRegionInfo', {}).get('geoLocation', {}). \
+                        get('longitude')
+
+                if 'vmStatusInfo' in self._properties:
+                    self._is_vm = True
+                    self._vm_hyperv_id = self._properties.get('vmStatusInfo', {}).get('pseudoClient', {}).get(
+                        'clientId')
+                else:
+                    self._is_vm = False
+
+                if 'clientGroups' in self._properties:
+                    self._associated_client_groups = self._properties.get('clientGroups', {})
+
+                if 'company' in client_props:
+                    self._company_id = client_props.get('company', {}).get('shortName', {}).get('id')
+
+
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101', self._update_response_(response.text))
 
     def _request_json(self, option, enable=True, enable_time=None, job_start_time=None, **kwargs):
         """Returns the JSON request to pass to the API as per the options selected by the user.
@@ -4138,14 +4256,44 @@
 
     @property
     def properties(self):
         """Returns the client properties"""
         return copy.deepcopy(self._properties)
 
     @property
+    def latitude(self):
+        """Returns the client latitude from clientRegionInfo GeoLocation"""
+        return self._client_latitude
+
+    @property
+    def longitude(self):
+        """Returns the client Longitude from clientRegionInfo GeoLocation"""
+        return self._client_longitude
+
+    @property
+    def is_vm(self):
+        """Returns True if the given client is a VM else False"""
+        return self._is_vm
+
+    @property
+    def hyperv_id_of_vm(self):
+        """Returns the Hypervisor ID associated to a VM client"""
+        return self._vm_hyperv_id
+
+    @property
+    def associated_client_groups(self):
+        """Returns the list of client groups to which the given client is assocaited with"""
+        return self._associated_client_groups
+
+    @property
+    def company_id(self):
+        """Returns the client's Company ID"""
+        return self._company_id
+
+    @property
     def name(self):
         """Returns the Client name"""
         return self._properties['client']['clientEntity']['clientName']
 
     @property
     def display_name(self):
         """Returns the Client display name"""
@@ -5370,15 +5518,15 @@
 
     def change_o365_client_job_results_directory(
             self, new_directory_path, username=None, password=None):
         """
                 Change the Job Result Directory of a O365 Client
 
                 Arguments:
-                    new_directory   (str)   -- The new JR directory
+                    new_directory_path   (str)   -- The new JR directory
                         Example:
                             C:\ JR
                             or
                             <UNC-PATH>
 
 
                     username    (str)   --
@@ -5651,15 +5799,17 @@
             raise SDKException('Response', '101', self._update_response_(response.text))
 
     def set_dedup_property(self,
                            prop_name,
                            prop_value,
                            client_side_cache=None,
                            max_cache_db=None,
-                           high_latency_optimization=None):
+                           high_latency_optimization=None,
+                           variable_content_alignment=None
+                           ):
         """
             Set DDB propeties
 
           :param prop_name:    property name
         :param prop_value:   property value
         :return:
 
@@ -5678,14 +5828,20 @@
                                     2048
                                     4096
                                     8192
                                     16384
                                     32768
                                     65536
                                     131072
+                    variable_content_alignment: to increase the effectiveness of deduplication on the client computer.
+                                                Variable content alignment reduces the amount of data stored during a
+                                                backup operation.
+                               Values - None(Default) - DoNotModify the property value
+                                        True/False - Enable/Disable optimization respectively
+
                     high_latency_optimization: To set Optimization for High latency Networks
                                 Values - None(Default) - DoNotModify the property value
                                          True/False - Enable/Disable optimization respectively
         """
         if not (isinstance(prop_name, str) and isinstance(prop_value, str)):
             raise SDKException('Client', '101')
 
@@ -5697,14 +5853,19 @@
                         'enableClientSideDiskCache': client_side_cache,
                         'maxCacheDb': max_cache_db
                     }
                 }
                 if high_latency_optimization is not None:
                     dedupe_props['deDuplicationProperties'][
                         'enableHighLatencyOptimization'] = high_latency_optimization
+
+                if variable_content_alignment is not None:
+                    dedupe_props['deDuplicationProperties'][
+                        'enableVariableContentAlignment'] = variable_content_alignment
+
             else:
                 dedupe_props = {
                     'deDuplicationProperties': {
                         'clientSideDeduplication': prop_value,
                         'enableClientSideDiskCache': client_side_cache
                     }
                 }
```

### Comparing `cvpysdk-11.30.1/cvpysdk/clientgroup.py` & `cvpysdk-11.32/cvpysdk/clientgroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,14 +371,16 @@
             'equal to': 100,
             'not equal': 101,
             'any in selection': 108,
             'not in selection': 109,
             'is true': 1,
             'is false': 2,
             'contains': 10,
+            'starts with': 14,
+            'ends with': 15,
             }
         prop_id_dict = {
             'Name': 1,
             'Client': 2,
             'Agents Installed': 3,
             'Associated Client Group': 4,
             'Timezone': 5,
@@ -442,15 +444,15 @@
             'Timezone List': 72,
             'MediaAgent has Lucene Index Role List': 73,
             'Associated Storage Policy List': 74,
             'Timezone Region List': 75,
             'Clients With Encryption': 80,
             'Client CIDR Address Range': 81,
             'HAC Cluster': 85,
-            'Client Display Name': 116
+            'Client Display Name': 116,
             }
         ptype_dict = {
             'Name': 2,
             'Client': 4,
             'Agents Installed': 6,
             'Associated Client Group': 4,
             'Timezone': 4,
@@ -514,14 +516,15 @@
             'Timezone List': 7,
             'MediaAgent has Lucene Index Role List': 7,
             'Associated Storage Policy List': 7,
             'Timezone Region List': 7,
             'Clients With Encryption': 1,
             'Client CIDR Address Range': 10,
             'HAC Cluster': 1,
+            'Client Display Name': 2,
             }
 
         rule_mk = {
             "rule": {
                 "filterID": filter_dict[filter_condition],
                 "secValue": filter_value,
                 "propID": prop_id_dict[filter_rule],
@@ -900,14 +903,15 @@
 
         self._properties = None
         self._description = None
         self._is_backup_enabled = None
         self._is_restore_enabled = None
         self._is_data_aging_enabled = None
         self._is_smart_client_group = None
+        self._company_name = None
 
         self.refresh()
 
     def __repr__(self):
         """String representation of the instance of this class.
 
             Returns:
@@ -987,14 +991,16 @@
                     if control_options['activityType'] == 1:
                         self._is_backup_enabled = control_options['enableActivityType']
                     elif control_options['activityType'] == 2:
                         self._is_restore_enabled = control_options['enableActivityType']
                     elif control_options['activityType'] == 16:
                         self._is_data_aging_enabled = control_options['enableActivityType']
 
+        self._company_name = clientgroup_props.get('securityAssociations', {}).get('tagWithCompany', {}).get('providerDomainName')
+
     def _request_json_(self, option, enable=True, enable_time=None, **kwargs):
         """Returns the JSON request to pass to the API as per the options selected by the user.
 
             Args:
                 option (str)  --  string option for which to run the API for
                     e.g.; Backup / Restore / Data Aging
 
@@ -1279,14 +1285,19 @@
 
     @property
     def is_smart_client_group(self):
         """Returns boolean indicating whether client group is smart client group"""
         return self._is_smart_client_group
     
     @property
+    def company_name(self):
+        """Returns company name to which client group belongs to"""
+        return self._company_name
+    
+    @property
     def network(self):
         """Returns the object of Network class."""
         if self._networkprop is None:
             self._networkprop = Network(self)
 
         return self._networkprop
 
@@ -1969,7 +1980,49 @@
             raise SDKException('ClientGroup', '102', o_str)
 
     def refresh(self):
         """Refresh the properties of the ClientGroup."""
         self._initialize_clientgroup_properties()
         self._networkprop = Network(self)
         self._network_throttle = None
+
+    def change_company(self, target_company_name):
+        """
+        Changes Company for client group and its belonging clients
+
+        Args:
+            target_company_name (str)  --  Company name to which clientgroup and its clients to be migrated
+
+        Raises:
+            SDKException:
+                if response is empty
+
+                if response is not success
+        """
+        if target_company_name.lower() == 'commcell':
+            company_id = 0
+        else:
+            company_id = int(self._commcell_object.organizations.get(target_company_name).organization_id)
+    
+        request_json = {
+            "entities": [
+                {
+                    "name": self._clientgroup_name,
+                    "clientGroupId": int(self._clientgroup_id),
+                    "_type_": 28
+                }
+            ]
+        }
+        
+        req_url = self._services['ORGANIZATION_ASSOCIATION'] % company_id
+        flag, response = self._cvpysdk_object.make_request('PUT', req_url, request_json)
+
+        if flag:
+            if response.json():
+                if 'errorCode' in response.json() and response.json()['errorCode'] != 0:
+                    raise SDKException('Organization', '110', 'Error: {0}'.format(response.json()['errorMessage']))
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+        self.refresh()
```

### Comparing `cvpysdk-11.30.1/cvpysdk/clients/__init__.py` & `cvpysdk-11.32/cvpysdk/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/clients/onedrive_client.py` & `cvpysdk-11.32/cvpysdk/clients/onedrive_client.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/clients/vmclient.py` & `cvpysdk-11.32/cvpysdk/clients/vmclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/commcell.py` & `cvpysdk-11.32/cvpysdk/commcell.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 
     add_additional_setting()    --  adds registry key to the commserve property
 
     delete_additional_setting() --  deletes registry key from the commserve property
 
     download_software()         --  triggers the Download Software job with the given options
 
+    copy_software()             --  triggers the Copy Software job with the given options
+
     sync_remote_cache()         --  syncs remote cache
 
     get_remote_cache()     		--  returns the instance of the RemoteCache class
 
     push_servicepack_and_hotfixes() --  triggers installation of service pack and hotfixes
 
     install_software()              --  triggers the install Software job with the given options
@@ -107,20 +109,26 @@
 
     get_security_associations()         -- Get the security associations associated with the commcell
 
     get_password_encryption_config()    -- Get the Password encryption configuration for the commcell
 
     get_email_settings()                -- Get the SMTP settings for the commcell
 
+    set_email_settings()                -- Set the SMTP settings for the commcell
+
     get_commcell_properties()           -- Get the general, privacy and other properties of commcell
 
     get_commcell_organization_properties()     -- Get the organization properties of commcell
 
     add_service_commcell_associations()    -- adds an association for an entity on a service commcell
 
+    get_service_commcell_associations()     --  gets the association details for entity on commcell
+
+    remove_service_commcell_association()   --  removes association for an entity on all service commcells
+
     enable_tfa()                           --   Enables two factor authentication on this commcell
 
     disable_tfa()                          --  Disables two factor authentication on this commcell
 
     _get_commserv_metadata()               -- Returns back the commserv metadata on this commcell
 
     _get_commserv_oem_id()               -- Returns back the commserv OEM ID on this commcell
@@ -131,14 +139,25 @@
 
     switch_to_company()         --  Login to company as an operator, just like using switcher on Command Center
 
     reset_company()             --  Switch back to Commcell
     
     allow_users_to_enable_passkey()     --      Enable or Disable passkey authorization for company administrators and client owners
 
+    get_sla_configuration()         --  gets the sla configuration details at commcell level
+
+    get_workload_region()           --  gets the current workload region
+
+    get_user_suggestions()          --  gets details of entities matching given term
+
+    enable_limit_user_logon_attempts()  --  Enables limit user logon attempts feature.
+
+    disable_limit_user_logon_attempts()   -- Disables limit user logon attempts feature.
+
+
 Commcell instance Attributes
 ============================
 
     **commserv_guid**           --  returns the `CommServ` GUID, class instance is initalized for
 
     **commserv_hostname**       --  returns the hostname of the `CommServ`, class instance is
     initalized for
@@ -375,14 +394,15 @@
 from .job import JobManagement
 from .index_server import IndexServers
 from .hac_clusters import HACClusters
 from .index_pools import IndexPools
 from .deduplication_engines import DeduplicationEngines
 from .metallic import Metallic
 from .key_management_server import KeyManagementServers
+from .regions import Regions
 
 USER_LOGGED_OUT_MESSAGE = 'User Logged Out. Please initialize the Commcell object again.'
 USER_DOES_NOT_HAVE_PERMISSION = "User does not have permission on commcell properties"
 """str:     Message to be returned to the user, when trying the get the value of an attribute
 of the Commcell class, after the user was logged out.
 
 """
@@ -616,14 +636,15 @@
         self._deduplication_engines = None
         self._redirect_cc_idp = None
         self._tfa = None
         self._metallic = None
         self._kms = None
         self._privacy = None
         self._commcell_properties = None
+        self._regions = None
         self.refresh()
 
         del self._password
 
     def __repr__(self):
         """String representation of the instance of this class.
 
@@ -889,37 +910,60 @@
                 except ValueError:
                     return {'output': response.text}
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101', self._update_response_(response.text))
 
-    def get_gxglobalparam_value(self):
+    def get_gxglobalparam_value(self, parameters):
         """Makes a rest api call to get values from GXGlobalParam
 
+            Args:
+                parameters      (str/list)  --  The single parameter name or list of parameter names to get value for
+
             Returns:
-                dict    -   json response received from the server
+                str     --      If parameters argument is a string. None if the parameter is not found in response
+
+                list    --      If parameters argument is a list.
 
             Raises:
                 SDKException:
                     if response is empty
 
                     if response is not success
 
         """
+
+        parameters_orig = parameters
+        if isinstance(parameters, str):
+            parameters = [parameters]
+
+        if not isinstance(parameters, list):
+            raise SDKException('Commcell', '107')
+
         flag, response = self._cvpysdk_object.make_request(
-            'GET', self._services['GET_GLOBAL_PARAM']
+            'POST', self._services['GET_GLOBAL_PARAM'], {
+                'globalParamsRequestList': parameters
+            }
         )
 
         if flag:
-            if response.ok:
-                try:
-                    return response.json()
-                except ValueError:
-                    return {'output': response}
+            if response.json():
+                param_results = response.json().get('globalParamsResultList')
+
+                # If requested parameter is a string, then return the single value directly instead of the list response
+                if isinstance(parameters_orig, str):
+                    for param_result in param_results:
+                        if param_result.get('name').lower() == parameters_orig.lower():
+                            return param_result.get('value')
+
+                    # Return None if the requested parameter is not found in the response
+                    return None
+
+                return param_results
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101', self._update_response_(response.text))
 
     def _set_gxglobalparam_value(self, request_json):
         """ Updates GXGlobalParam table (Commcell level configuration parameters)
@@ -947,29 +991,29 @@
             Raises:
                 SDKException:
                     if response is empty
 
                     if response is not success
 
         """
-        if  isinstance(request_json, list):
+        if isinstance(request_json, list):
             global_params_list = request_json
             payload = {
                 "App_SetGlobalParamsReq": {
                     "globalParams": global_params_list
                 }
             }
             return self.qoperation_execute(payload)
 
         if not isinstance(request_json, dict):
             message = f"Received: {type(request_json)}. Expected: dict, list"
             raise SDKException('Commcell', 107, message)
 
         flag, response = self._cvpysdk_object.make_request(
-            'POST', self._services['GLOBAL_PARAM'], request_json
+            'POST', self._services['SET_GLOBAL_PARAM'], request_json
         )
 
         if flag:
             if response.json():
                 return response.json()
             else:
                 raise SDKException('Response', '102')
@@ -1475,16 +1519,15 @@
         except AttributeError:
             return USER_LOGGED_OUT_MESSAGE
 
     @property
     def commserv_client(self):
         """Returns the instance of the Client class for the CommServ client."""
         if self._commserv_client is None:
-            self._commserv_client = self.clients.get(self._commserv_name)
-
+            self._commserv_client = self.clients.get(self._id)
         return self._commserv_client
 
     @property
     def commcell_migration(self):
         """Returns the instance of the CommcellMigration class"""
         try:
             if self._commcell_migration is None:
@@ -1659,14 +1702,25 @@
             if self._kms is None:
                 self._kms = KeyManagementServers(self)
 
             return self._kms
         except AttributeError:
             return USER_LOGGED_OUT_MESSAGE
 
+    @property
+    def regions(self):
+        """Returns the instance of the Regions class."""
+        try:
+            if self._regions is None:
+                self._regions = Regions(self)
+
+            return self._regions
+        except AttributeError:
+            return USER_LOGGED_OUT_MESSAGE
+
     def logout(self):
         """Logs out the user associated with the current instance."""
         if self._headers['Authtoken'] is None:
             return 'User already logged out.'
 
         output = self._cvpysdk_object._logout()
         self._remove_attribs_()
@@ -2081,15 +2135,15 @@
         return download.sync_remote_cache(
             client_list=client_list)
 
     def download_software(self,
                           options=None,
                           os_list=None,
                           service_pack=None,
-                          cu_number=0,
+                          cu_number=1,
                           sync_cache=True,
                           sync_cache_list=None,
                           schedule_pattern=None):
         """Downloads the os packages on the commcell
 
             Args:
 
@@ -2166,23 +2220,82 @@
             service_pack=service_pack,
             cu_number=cu_number,
             sync_cache=sync_cache,
             sync_cache_list=sync_cache_list,
             schedule_pattern=schedule_pattern
         )
 
+    def copy_software(self,
+                      media_loc,
+                      username=None,
+                      password=None,
+                      sync_cache=True,
+                      schedule_pattern=None):
+        """copies media from the specified location on the commcell
+
+                    Args:
+
+                        media_loc      (str)           --  Media Location to be used for copy software
+
+                        username       (str)           --  username to authenticate to external location
+
+                        password       (str)           --  password to authenticate to external location
+
+                        sync_cache (bool)              --  True if download and sync
+                                                           False only download
+
+                        schedule_pattern(dict)         --  pattern for schedule task
+
+
+                    Returns:
+                        object - instance of the Job class for this copy software job
+
+                    Raises:
+                        SDKException:
+                            if Download job failed
+
+                            if response is empty
+
+                            if response is not success
+
+                            if another download job is running
+                    Usage:
+
+                        -   if media_location directory is local to the machine - username and password is not needed
+
+                            >>> commcell_obj.copy_software(media_loc = "C:\\Downloads\\Media")
+
+                        -   if Media_location directory is remote- username and passsword(base 64 encoded) are needed
+                            to authenticate the cache
+
+                            >>> commcell_obj.copy_software(
+                            media_loc = "\\subdomain.company.com\Media",
+                            username = "domainone\\userone",
+                            password = "base64encoded password"
+                            )
+                """
+        download = Download(self)
+        return download.copy_software(
+            media_loc=media_loc,
+            username=username,
+            password=password,
+            sync_cache=sync_cache,
+            schedule_pattern=schedule_pattern
+        )
+
     def push_servicepack_and_hotfix(
             self,
             client_computers=None,
             client_computer_groups=None,
             all_client_computers=False,
             all_client_computer_groups=False,
             reboot_client=False,
             run_db_maintenance=True,
-            maintenance_release_only=False):
+            maintenance_release_only=False,
+            **kwargs):
         """triggers installation of service pack and hotfixes
 
         Args:
             client_computers    (list)      -- Client machines to install service pack on
 
             client_computer_groups (list)   -- Client groups to install service pack on
 
@@ -2204,40 +2317,50 @@
             run_db_maintenance (bool)      -- boolean to specify whether to run db
             maintenance not
 
                 default: True
 
             maintenance_release_only (bool) -- for clients of feature releases lesser than CS, this option
             maintenance release of that client FR, if present in cache
+            **kwargs: (dict) -- Key value pairs for supporting conditional initializations
+                Supported -
+                schedule_pattern (dict)           -- Request JSON for scheduling the operation
 
         Returns:
-            object - instance of the Job class for this download job
+            object - instance of the Job/Task class for this download
 
         Raises:
                 SDKException:
+                    if schedule is not of type dictionary
+
                     if Download job failed
 
                     if response is empty
 
                     if response is not success
 
                     if another download job is already running
 
         **NOTE:** push_serivcepack_and_hotfixes cannot be used for revision upgrades
 
         """
+        schedule_pattern = kwargs.get("schedule_pattern", None)
+        if schedule_pattern:
+            if not isinstance(schedule_pattern, dict):
+                raise SDKException("Commcell", "101")
         install = Install(self)
         return install.push_servicepack_and_hotfix(
             client_computers=client_computers,
             client_computer_groups=client_computer_groups,
             all_client_computers=all_client_computers,
             all_client_computer_groups=all_client_computer_groups,
             reboot_client=reboot_client,
             run_db_maintenance=run_db_maintenance,
-            maintenance_release_only=maintenance_release_only
+            maintenance_release_only=maintenance_release_only,
+            schedule_pattern=schedule_pattern
         )
 
     def install_software(
             self,
             client_computers=None,
             windows_features=None,
             unix_features=None,
@@ -2591,14 +2714,85 @@
                 return response
             else:
                 raise SDKException('Response', '102')
         else:
             response_string = self._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
 
+    def set_email_settings(self, smtp_server, sender_name, sender_email, **kwargs):
+        """Set Email Server (SMTP) setup for commcell
+
+            Args:
+                smtp_server(str)    --  hostname of the SMTP server
+                sender_name(str)    --  Name of the sender
+                sender_email(str)   --  Email address of the sender to be used
+                ** kwargs(dict)     --  Key value pairs for supported arguments
+                Supported argument values:
+
+                    enable_ssl(boolean) --  option to represent whether ssl is supported for the EMail Server
+                                            Default value: False
+                    smtp_port(int)      --  Port number to be used by Email Server
+                                            Default value: 25
+                    username(str)       --  Username to be used
+                    password(str)       --  Password to be used
+
+            Returns:
+                None
+
+            Raises:
+                SDKException:
+                    if invalid argument type is passed
+                    if failed to update Email server
+                    if response is empty
+                    if response is not success
+
+        """
+
+        if not (isinstance(smtp_server, str) and isinstance(sender_email, str)
+                and isinstance(sender_name, str)):
+            raise SDKException("Commcell", "101")
+
+        enable_ssl = kwargs.get("enable_ssl", False)
+        smtp_port = kwargs.get("smtp_port", 25)
+        username = kwargs.get("username", "")
+        password = kwargs.get("password", "")
+
+        if not (isinstance(enable_ssl, bool) and isinstance(smtp_port, int)
+                and isinstance(username, str) and isinstance(password, str)):
+            raise SDKException("Commcell", "101")
+
+        request_json = {"smtpInfo":
+                            {"enableSSL": enable_ssl,
+                             "smtpServer": smtp_server,
+                             "smtpPort": smtp_port,
+                             "useAuthentication": False,
+                             "maxMailServerSize": 0,
+                             "userInfo": {
+                                 "password": username,
+                                 "userName": password
+                             },
+                             "senderInfo": {
+                                 "senderName": sender_name,
+                                 "senderAddress": sender_email
+                             }
+                             }
+                        }
+        url = self._services['EMAIL_SERVER']
+        flag, response = self._cvpysdk_object.make_request(
+            'POST', url, request_json
+        )
+        if flag:
+            if response.json():
+                error_code = response.json().get('errorCode', 0)
+                if error_code != 0:
+                    raise SDKException('Response', '101', self._update_response_(response.text))
+                return
+            raise SDKException('Response', '102')
+        raise SDKException('Response', '101', self._update_response_(response.text))
+
     def get_password_encryption_config(self):
         """ Get the password encryption config for commcell
         returns: (dict)
             "keyFilePath": String,
             "keyProviderName": String,
             "isKeyMovedToFile": Boolean
         """
@@ -3275,35 +3469,144 @@
             request_json['userOrGroup']['userGroupId'] = int(entity_name.user_group_id)
             request_json['userOrGroup']['userGroupName'] = entity_name.user_group_name
             request_json['userOrGroup']['_type_'] = 15
 
         if isinstance(entity_name, Organization):
             request_json['providerType'] = 5
             request_json['userOrGroup']['providerId'] = int(entity_name.organization_id)
-            request_json['userOrGroup']['providerDomainName'] = entity_name.organization_name
+            request_json['userOrGroup']['providerDomainName'] = entity_name.domain_name
             request_json['userOrGroup']['_type_'] = 61
+            org_det = self.get_user_suggestions(entity_name.domain_name)
+            if len(org_det)>0:
+                request_json['userOrGroup']['GUID'] = org_det[0].get('umGuid', '')
+                request_json['userOrGroup']['entityInfo'] = org_det[0].get('company',{}).get('entityInfo', '')
+
 
         if isinstance(entity_name, Domain):
             request_json['providerType'] = 2
             request_json['userOrGroup']['providerId'] = int(entity_name.domain_id)
             request_json['userOrGroup']['providerDomainName'] = entity_name.domain_name
             request_json['userOrGroup']['_type_'] = 61
 
         res_json = self._service_commcells_association()
         res_json['associations'].append(request_json)
         flag, response = self._cvpysdk_object.make_request(
             'POST', self._services['SERVICE_COMMCELL_ASSOC'], res_json
         )
-
         if flag:
             if response.json():
-                error_code = response.json().get('response', [{}])[0].get('errorCode', -1)
+                response_json = response.json().get('response', response.json())
+                error_code = response_json.get('errorCode', 1)
+                if error_code != 0:
+                    error_string = response_json.get('errorString', error_string)
+                    raise SDKException(
+                        'CommcellRegistration',
+                        '102',
+                        'Service Commcell Association Failed\n Error: "{0}"'.format(
+                            error_string
+                        )
+                    )
+                self.refresh()
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+    def get_service_commcell_associations(self, entity_name):
+        """Gets an entity's association details for every commcell it is associated to
+
+        Args:
+            entity_name  (object)     -- entity_name can be object of User,UserGroup,Domain and Organization Class
+
+        Returns:
+            list - list of dicts, each dict containing details of the entity's association with a service commcell
+
+            Example:
+                [
+                    {
+                        "userOrGroup": {
+                            "userId": ,
+                            "GUID": ,
+                            "userName": ,
+                            "_type_": ,
+                        },
+                        "entity": {
+                            "entityType": ,
+                            "entityName": ,
+                            "entityId": ,
+                            "_type_": ,
+                            "flags": ,
+                        },
+                        "properties": ,
+                    },
+                    {
+                        "userOrGroup": {...},
+                        "entity": {...},
+                        "properties": {...},
+                    },
+                    {
+                        "userOrGroup": {...},
+                        "entity": {...},
+                        "properties": {...},
+                    }
+                ]
+
+        """
+        res_json = self._service_commcells_association()
+        entity_associations = []
+        for association in res_json['associations']:
+            if isinstance(entity_name, User) and \
+                association['userOrGroup'].get('userName', '').lower() == entity_name.user_name.lower() and \
+                association['userOrGroup'].get('_type_') == 13:
+                entity_associations.append(association)
+            elif isinstance(entity_name, UserGroup) and \
+                association['userOrGroup'].get('userGroupName', '').lower() == entity_name.user_group_name.lower() and \
+                association['userOrGroup'].get('_type_') == 15:
+                entity_associations.append(association)
+            elif isinstance(entity_name, Organization) and \
+                association.get('providerType') in [5, 15] and \
+                association['userOrGroup'].get('providerDomainName', '').lower() == entity_name.domain_name.lower():
+                entity_associations.append(association)
+            elif isinstance(entity_name, Domain) and \
+                association.get('providerType') == 2 and \
+                association['userOrGroup'].get('providerDomainName', '').lower() == entity_name.domain_name.lower():
+                entity_associations.append(association)
+        return entity_associations
 
+    def remove_service_commcell_associations(self, entity_name):
+        """removes an entity's associations to every commcell
+
+        Args:
+
+            entity_name  (object)     -- entity_name can be object of User,UserGroup,Domain and Organization Class
+
+        Raises:
+            SDKException:
+                if response is empty
+
+                if remove association fails
+
+                if response is not success
+        """
+
+        res_json = self._service_commcells_association()
+
+        for association in self.get_service_commcell_associations(entity_name):
+            res_json['associations'].remove(association)
+
+        flag, response = self._cvpysdk_object.make_request(
+            'POST', self._services['SERVICE_COMMCELL_ASSOC'], res_json
+        )
+        if flag:
+            if response.json():
+                response_json = response.json().get('response', response.json())
+                error_code = response_json.get('errorCode', 1)
                 if error_code != 0:
-                    error_string = response.json().get('response', [{}])[0].get('errorString')
+                    error_string = response_json.get('errorString', error_string)
                     raise SDKException(
                         'CommcellRegistration',
                         '102',
                         'Service Commcell Association Failed\n Error: "{0}"'.format(
                             error_string
                         )
                     )
@@ -3490,7 +3793,182 @@
                 if errorCode != 0:
                     raise SDKException('Response', '101', 'Failed to enable passkey')
             else:
                 raise SDKException('Response', '102')
         else:
             response_string = self._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
+
+    def get_sla_configuration(self):
+        """Makes a rest api call to get SLA configuration at commcell level
+
+            Returns:
+                dict   -   sla details
+                example:
+                    {
+                        'slaDays': 7, 
+                        'excludedReason': '', 
+                        'useSystemDefaultSLA': False, 
+                        'excludeFromSLA': False, 
+                        'delayInterval': 0, 
+                        'inheritedSLA': {
+                            'slaDays': 0, 
+                            'entityType': 0, 
+                            'excludeFromSLA': False
+                        }
+                    }
+
+            Raises:
+                SDKException:
+                    if response is empty
+
+                    if response is not success
+
+        """
+        request_json = {"entities": [{"entity": {"commCellId": self.commcell_id, "_type_": 1}}]}
+        flag, response = self._cvpysdk_object.make_request(
+            'POST', self._services['GET_SLA'], payload=request_json
+        )
+
+        if flag:
+            if response.ok and response.json():
+                return response.json().get('entities', [{}])[0]
+            else:
+                raise SDKException('Response', '102')
+        else:
+            raise SDKException('Response', '101', self._update_response_(response.text))
+
+    def get_workload_region(self):
+        """Makes a rest api call to get commserve workload region
+
+            Returns:
+                dict    -   with region id,name
+                example:
+                    {
+                        'regionId': 2, 
+                        'displayName': 'Asia', 
+                        'regionName': 'Asia'
+                    }
+
+            Raises:
+                SDKException:
+                    if response is empty
+
+                    if response is not success
+
+        """
+        flag, response = self._cvpysdk_object.make_request('GET', self._services['WORKLOAD_REGION'] % self.commcell_id)
+
+        if flag:
+            if response.ok and response.json():
+                return response.json()
+            else:
+                raise SDKException('Response', '102')
+        else:
+            raise SDKException('Response', '101', self._update_response_(response.text))
+
+    def get_user_suggestions(self, term: str)->list:
+        """Makes a multicommcell api call to get user suggestions for entities
+            Args:
+                term (str) - the entity name to get matched suggestions of
+
+            Returns:
+                list    -   list of dicts with details of entity whose name matches for given term
+                example:
+                    [
+                        {
+                            "displayName": "",
+                            "groupId": 0,
+                            "umEntityType": 0,
+                            "umGuid": "",
+                            ...
+                            "groupGuid": "...",
+                            "company": {...},
+                        },
+                        {...},
+                        {...},
+                    ]
+
+            Raises:
+                SDKException:
+                    if response is empty
+
+                    if response is not success
+
+        """
+
+        headers = self._headers.copy()
+        headers['CVContext'] = 'comet'
+        flag, response = self._cvpysdk_object.make_request(
+            'GET', self._services['GET_USER_SUGGESTIONS']%term, headers=headers
+        )
+
+        if flag:
+            if response.json():
+                return response.json().get('users')
+            else:
+                raise SDKException('Response', '102')
+
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+    def enable_limit_user_logon_attempts(self, failed_login_attempt_limit=5, failed_login_attempts_within=3600,
+                                         account_lock_duration=86400, lock_duration_increment_by=3600):
+        """
+         Enable Limit user logon attempts feature
+         Args:
+             failed_login_attempt_limit             (int)   --  number of logon attempts a user is allowed
+                default : 5
+             failed_login_attempts_within           (int)   --  logon attempts a user is allowed within specified
+                default : 3600 secs                                        numbers of secs
+             account_lock_duration                  (int)   --  number of secs a locked account remains locked
+                default :  86400 secs
+             lock_duration_increment_by             (int)   --  increment the lock duration by specified secs
+                                                                after each consecutive user account lock
+                default : 3600 secs
+         Raises:
+            SDKException:
+                if response is empty
+                if response is not success
+                if failed to enable limit user logon feature
+        """
+        req_json = {
+            'failedLoginAttemptLimit': failed_login_attempt_limit,
+            'failedLoginAttemptsWithin': failed_login_attempts_within,
+            'accountLockDuration': account_lock_duration,
+            'accountLockDurationIncrements': lock_duration_increment_by
+        }
+        flag, response = self._cvpysdk_object.make_request(
+            'PUT', self._services['ACCOUNT_lOCK_SETTINGS'], req_json
+        )
+        if flag:
+            if response and response.json():
+                error_code = response.json().get('errorCode', -1)
+                if error_code != 0:
+                    error_string = response.json().get('errorMessage', '')
+                    raise SDKException(
+                        'Security',
+                        '102',
+                        'Failed to set account lock settings: "{0}"'.format(
+                            error_string
+                        )
+                    )
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+    def disable_limit_user_logon_attempts(self):
+        """
+        Disable limit user logon attempts feature.
+        Raises:
+            SDKException:
+                if response is empty
+                if response is not success
+                if failed to disable limit user logon feature
+        """
+        self.enable_limit_user_logon_attempts(failed_login_attempt_limit=-1,
+                                              failed_login_attempts_within=-1,
+                                              account_lock_duration=-1,
+                                              lock_duration_increment_by=-1)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/commcell_migration.py` & `cvpysdk-11.32/cvpysdk/commcell_migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,18 +176,36 @@
             raise SDKException('CommCellMigration', '104')
 
         if other_sql_instance:
             if sql_instance_name == "" or sql_user_name == "" or sql_password == "":
                 raise SDKException('CommCellMigration', '103')
             sql_password = b64encode(sql_password.encode()).decode()
 
+        common_options = {
+            "otherSqlInstance": other_sql_instance,
+            "pathType": self._path_type,
+            "dumpFolder": export_location,
+            "splitCSDB": 1,
+            "sqlLinkedServer": {
+                "sqlServerName": sql_instance_name,
+                "sqlUserAccount": {
+                    "userName": sql_user_name,
+                    "password": sql_password
+                }
+            }
+        }
+
         if self._path_type == 1:
             if network_user_name == "" or network_user_password == "":
                 raise SDKException('CommCellMigration', '103')
             network_user_password = b64encode(network_user_password.encode()).decode()
+            common_options["userAccount"] = {
+                "password": network_user_password,
+                "userName": network_user_name
+            }
 
         export_json = {
             "taskInfo": {
                 "task": {
                     "taskType": 1,
                     "isEditing": False,
                     "initiatedFrom": 2,
@@ -203,40 +221,24 @@
                         "subTask": {
                             "subTaskType": 1,
                             "operationType": 4029
                         },
                         "options": {
                             "adminOpts": {
                                 "ccmOption": {
-                                    "commonOptions": {
-                                        "otherSqlInstance": other_sql_instance,
-                                        "pathType": self._path_type,
-                                        "dumpFolder": export_location,
-                                        "splitCSDB": 1,
-                                        "userAccount": {
-                                            "password": network_user_password,
-                                            "userName": network_user_name
-                                        },
-                                        "sqlLinkedServer": {
-                                            "sqlServerName": sql_instance_name,
-                                            "sqlUserAccount": {
-                                                "userName": sql_user_name,
-                                                "password": sql_password
-                                            }
-                                        }
-                                    },
+                                    "commonOptions": common_options,
                                     "captureOptions": {
                                         "captureMediaAgents": capture_ma,
                                         "lastHours": 60,
                                         "remoteDumpDir": "",
                                         "remoteCSName": "",
                                         "captureSchedules": capture_schedules,
                                         "captureActivityControl": capture_activity_control,
                                         "captureOperationWindow": capture_opw,
-                                        "captureHolidays":capture_holidays,
+                                        "captureHolidays": capture_holidays,
                                         "pruneExportedDump": False,
                                         "autopickCluster": auto_pick_cluster,
                                         "copyDumpToRemoteCS": False,
                                         "useJobResultsDirForExport": False,
                                         "captureFromDB": {
                                             "csName": cs_name,
                                             "csDbName": database
@@ -271,15 +273,15 @@
                     sub_dict.append({'commCellName': self._commcell_name, "_type_": 36})
 
                 elif entity == "alerts":
                     sub_dict.append({'commCellName': self._commcell_name, "_type_": 42})
 
         if client_list:
             if other_sql_instance:
-                if  not sql_instance_name \
+                if not sql_instance_name \
                         or not sql_user_name \
                         or not sql_password \
                         or not client_ids:
                     raise SDKException('CommCellMigration', '106')
 
                 for index, client in enumerate(client_list):
                     temp_dic = {'clientName': client, "clientId": client_ids[index]}
@@ -314,14 +316,15 @@
                     {
                         "pathType": "Network",
                         "userName" : "username",
                         "password": "password",
                         "forceOverwrite": False,
                         "failIfEntityAlreadyExists": False,
                         "deleteEntitiesNotPresent": False,
+                        "deleteEntitiesIfOnlyfromSource": False,
                         "forceOverwriteHolidays": False,
                         "mergeHolidays": True,
                         "forceOverwriteOperationWindow": False,
                         "mergeOperationWindow": False,
                         "forceOverwriteSchedule": False,
                         "mergeSchedules": True
                     }
@@ -339,28 +342,41 @@
         """
         path_type = options_dictionary.get("pathType", "Local")
         network_user_name = options_dictionary.get("userName", "")
         network_user_password = options_dictionary.get("password", "")
         force_overwrite = options_dictionary.get('forceOverwrite', False)
         fail_if_entry_already_exists = options_dictionary.get('failIfEntityAlreadyExists', False)
         delete_entities_not_present = options_dictionary.get('deleteEntitiesNotPresent', False)
+        delete_only_source = options_dictionary.get('deleteEntitiesIfOnlyfromSource', False)
         fo_holidays = options_dictionary.get("forceOverwriteHolidays", False)
         merge_holidays = options_dictionary.get("mergeHolidays", True)
         fo_operation_window = options_dictionary.get("forceOverwriteOperationWindow", False)
         merge_operation_window = options_dictionary.get("mergeOperationWindow", False)
         fo_schedules = options_dictionary.get("forceOverwriteSchedule", False)
         merge_schedules = options_dictionary.get("mergeSchedules", True)
 
         if not (isinstance(path_type, str) and isinstance(import_location, str)):
             raise SDKException('CommCellMigration', '101')
 
+        common_options = {
+            "bRoboJob": False,
+            "databaseConfiguredRemote": False,
+            "pathType": self._path_type,
+            "dumpFolder": import_location,
+            "splitCSDB": 0
+        }
+
         if path_type.lower() == 'local':
             self._path_type = 0
         elif path_type.lower() == 'network':
             self._path_type = 1
+            common_options["userAccount"] = {
+                "password": network_user_password,
+                "userName": network_user_name
+            }
         else:
             raise SDKException('CommCellMigration', '104')
 
         if self._path_type == 1:
             if network_user_name == "" or network_user_password == "":
                 raise SDKException('CommCellMigration', '103')
 
@@ -396,37 +412,28 @@
                                         "specifyStagingPath": False,
                                         "forceOverwriteOperationWindow": fo_operation_window,
                                         "fallbackSpareGroup": "",
                                         "mergeOperationWindow": merge_operation_window,
                                         "pruneImportedDump": False,
                                         "alwaysUseFallbackDataPath": True,
                                         "deleteEntitiesNotPresent": delete_entities_not_present,
+                                        "deleteEntitiesIfOnlyfromSource": delete_only_source,
                                         "forceOverwrite": force_overwrite,
                                         "mergeHolidays": merge_holidays,
                                         "forceOverwriteSchedule": fo_schedules,
                                         "fallbackDrivePool": "",
                                         "mergeActivityControl": True,
                                         "fallbackMediaAgent": "",
                                         "mergeSchedules": merge_schedules,
                                         "failIfEntityAlreadyExists": fail_if_entry_already_exists,
                                         "fallbackLibrary": "",
                                         "skipConflictMedia": False,
                                         "stagingPath": ""
                                     },
-                                    "commonOptions": {
-                                        "bRoboJob": False,
-                                        "databaseConfiguredRemote": False,
-                                        "pathType": self._path_type,
-                                        "dumpFolder": import_location,
-                                        "splitCSDB": 0,
-                                        "userAccount": {
-                                            "password": network_user_password,
-                                            "userName": network_user_name
-                                        }
-                                    }
+                                    "commonOptions": common_options
                                 }
                             }
                         }
                     }
                 ]
             }
         }
```

### Comparing `cvpysdk-11.30.1/cvpysdk/content_analyzer.py` & `cvpysdk-11.32/cvpysdk/content_analyzer.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/credential_manager.py` & `cvpysdk-11.32/cvpysdk/credential_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,14 +41,19 @@
 
     owner_json()                --  returns json blob for setting user or usergroup as creator
 
     refresh()                   --  refreshes the list of credentials on this commcell
 
     delete()                    --  deletes the credential record on this commcell
 
+    get_security_associations() --  Returns the security association dictionary for a given user or user group
+
+    add_azure_cloud_creds()     --  Creates azure access key based credential on this commcell
+
+
 Credential:
     __init__()                  --  initiaizes the credential class object
 
     __repr__()                  --  returns the string for the instance of the
                                     credential class
 
     _get_credential_id()        --  Gets the Credential id associated with this Credential
@@ -76,14 +81,15 @@
 
 
 """
 
 from base64 import b64encode
 from .security.usergroup import UserGroups
 from .exception import SDKException
+from .constants import Credential_Type
 
 
 class Credentials(object):
     """Class for maintaining all the configured credential on this commcell"""
 
     def __init__(self, commcell_object):
         """Initializes the credentials class object for this commcell
@@ -95,15 +101,15 @@
                 object - instance of the Clients class
         """
         self._commcell_object = commcell_object
         self._services = commcell_object._services
         self._credentials = self._get_credentials()
         self.record_type = {
             'windows': 1,
-            'Linux': 2
+            'linux': 2
         }
 
     def __str__(self):
         """Representation string consisting of all Credentials of the commcell.
 
             Returns:
                 str - string of all the Credentials configured on the commcell
@@ -174,15 +180,14 @@
 
     def get(self, credential_name):
         """Returns the Credential object for the specified Credential name
 
             Args:
                 credential_name  (str)    --  name of the Credential for which the object has to
                                               be created
-
             Raises:
                 SDKException:
                     if Credential doesn't exist with specified name
         """
         if not self.has_credential(credential_name):
             raise SDKException(
                 'Credential', '102', "Credential {0} doesn't exists on this commcell.".format(
@@ -345,14 +350,153 @@
             else:
                 raise SDKException('Response', '102')
         else:
             response_string = self._commcell_object._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
         self.refresh()
 
+    def get_security_associations(self, owner, is_user=False):
+        """
+        Returns the security association dictionary for a given user or user group
+        Args:
+            owner(str)          -   Owner of the user or user group
+            is_user(bool)       -   True if the owner is a user
+                                    False if the owner is a user group
+
+        Returns:
+            dict containing the security association
+        """
+        if is_user is True:
+            userOrGroupInfo = {
+                "entityTypeName": "USER_ENTITY",
+                "userGroupName": owner,
+                "userGroupId": int(self._commcell_object.users.get(owner).user_id)
+            }
+        else:
+            userOrGroupInfo = {
+                "entityTypeName": "USERGROUP_ENTITY",
+                "userGroupName": owner,
+                "userGroupId": int(self._commcell_object.user_groups.get(owner).user_group_id)
+            }
+        security_association = {
+            "associationsOperationType": 1,
+            "associations": [
+                {
+                    "userOrGroup": [
+                        userOrGroupInfo
+                    ],
+                    "properties": {
+                        "isCreatorAssociation": False,
+                        "permissions": [
+                            {
+                                "permissionId": 218,
+                                "_type_": 122,
+                                "permissionName": "User Credential"
+                            }
+                        ]
+                    }
+                }
+            ]
+        }
+        return security_association
+
+    def add_azure_cloud_creds(self, credential_name, account_name, access_key_id, **kwargs):
+        """Creates azure access key based credential on this commcell
+
+            Args:
+
+                credential_name (str)   --  name to be given to credential account
+
+                account_name  (str)     --  name of the azure storage account
+
+                access_key_id   (str)   --  access key for azure storage
+
+                ** kwargs(dict)         --  Key value pairs for supported arguments
+
+                Supported argument values:
+                    owner(str)                  -   owner of the credentials
+                    is_user(bool)               -   Represents whether owner passed is a user or user group
+                                                    is_user=1 for user, is_user=0 for usergroup
+                    description(str)            -   description of the credentials
+
+            Raises:
+                SDKException:
+                    if arguments type is incorrect
+
+                    if credential account is already present on the commcell
+
+                    if string format are not proper
+
+                    if response is not successful
+
+        """
+        owner = kwargs.get("owner", "")
+        is_user = kwargs.get("is_user", True)
+        description = kwargs.get("description", "")
+
+        if not (isinstance(access_key_id, str) and isinstance(owner, str)
+                and isinstance(is_user, bool) and isinstance(account_name, str)
+                and isinstance(description, str) and isinstance(credential_name, str)):
+            raise SDKException("Credential", "101")
+
+        if self.has_credential(credential_name):
+            raise SDKException(
+                'Credential', '102', "Credential {0} already exists on this commcell.".format(
+                    credential_name)
+            )
+
+        creator = self.owner_json(owner=owner, isuser_flag=is_user)
+        password = b64encode(access_key_id.encode()).decode()
+        additional_information = {
+            "azureCredInfo": {
+                "authType": "AZURE_OAUTH_SHARED_SECRET",
+                "endpoints": {
+                    "activeDirectoryEndpoint": "https://login.microsoftonline.com/",
+                    "storageEndpoint": "blob.core.windows.net",
+                    "resourceManagerEndpoint": "https://management.azure.com/"
+                }
+            }
+        }
+        create_credential_account = {
+            "credentialRecordInfo": [
+                {
+                    "credentialRecord": {
+                        "credentialName": credential_name
+                    },
+                    "securityAssociations": self.get_security_associations(owner, is_user),
+                    "createAs": creator["createAs"],
+                    "record": {
+                        "userName": account_name,
+                        "password": password
+                    },
+                    "recordType": "MICROSOFT_AZURE",
+                    "additionalInformation": additional_information,
+                    "description": description
+                }
+            ]
+        }
+
+        request = self._services['CREDENTIAL']
+        flag, response = self._commcell_object._cvpysdk_object.make_request(
+            'POST', request, create_credential_account
+        )
+        if flag:
+            if response.json():
+                response_json = response.json()['error']
+                error_code = response_json['errorCode']
+                error_message = response_json['errorMessage']
+                if not error_code == 0:
+                    raise SDKException('Response', '101', error_message)
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._commcell_object._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+        self.refresh()
+
 
 class Credential(object):
     """"Class for representing a particular Credential record on this commcell"""
 
     def __init__(self, commcell_object, credential_name, credential_id=None):
         """Initialize the Credential class object for specified Credential
 
@@ -530,34 +674,36 @@
             self._credential_name)
         flag, response = self._commcell_object._cvpysdk_object.make_request(
             'GET', property_request
         )
 
         if flag:
             if response.json() and 'credentialRecordInfo' in response.json():
+                json_resp = response.json()
                 self._credential_properties = response.json()['credentialRecordInfo'][0]
 
                 self._credential_id = self._credential_properties['credentialRecord'].get(
                     'credentialId')
                 self._credential_name = self._credential_properties['credentialRecord'].get(
                     'credentialName')
                 self._credential_user_name = self._credential_properties['record']['userName']
                 self._record_type = self._credential_properties['recordType']
                 self._credential_owner_json = self._credential_properties.get('createAs', {})
-                if "userGroup" in self._credential_owner_json:
-                    cred_id = self._credential_owner_json.get('userGroup', {}).get('userGroupId')
-                    urs = UserGroups(self._commcell_object)
-                    all_groups = urs.all_user_groups
-                    for group_name, group_id in all_groups.items():
-                        if group_id == str(cred_id):
-                            self._credential_owner = group_name
-                else:
-                    self._credential_owner = self._credential_owner_json.get('user', {}).get(
-                        'user').get('userName')
-                    self._credential_owner_json = self._credential_owner_json.get('user')
+                if self._record_type != Credential_Type.MICROSOFT_AZURE.value: # Azure Storage Credentials
+                    if "userGroup" in self._credential_owner_json:
+                        cred_id = self._credential_owner_json.get('userGroup', {}).get('userGroupId')
+                        urs = UserGroups(self._commcell_object)
+                        all_groups = urs.all_user_groups
+                        for group_name, group_id in all_groups.items():
+                            if group_id == str(cred_id):
+                                self._credential_owner = group_name
+                    else:
+                        self._credential_owner = self._credential_owner_json.get('user', {}).get(
+                            'user').get('userName')
+                        self._credential_owner_json = self._credential_owner_json.get('user')
             else:
                 raise SDKException('Response', '102')
 
         else:
             response_string = self._commcell_object._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/cvpysdk.py` & `cvpysdk-11.32/cvpysdk/cvpysdk.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/datacube/__init__.py` & `cvpysdk-11.32/cvpysdk/datacube/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/datacube/constants.py` & `cvpysdk-11.32/cvpysdk/datacube/constants.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/datacube/datacube.py` & `cvpysdk-11.32/cvpysdk/datacube/datacube.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/datacube/datasource.py` & `cvpysdk-11.32/cvpysdk/datacube/datasource.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/datacube/handler.py` & `cvpysdk-11.32/cvpysdk/datacube/handler.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/datacube/sedstype.py` & `cvpysdk-11.32/cvpysdk/datacube/sedstype.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/deduplication_engines.py` & `cvpysdk-11.32/cvpysdk/deduplication_engines.py`

 * *Files 1% similar despite different names*

```diff
@@ -888,28 +888,29 @@
                     o_str = 'DDB recon job failed\nError: "{0}"'.format(error_message)
                     raise SDKException('Storage', '102', o_str)
                 raise SDKException('Storage', '112')
             raise SDKException('Response', '102')
         response_string = self._commcell_object._update_response_(response.text)
         raise SDKException('Response', '101', response_string)
 
-    def run_space_reclaimation(self, level=3, clean_orphan_data=False, use_scalable_resource=True):
+    def run_space_reclaimation(self, level=3, clean_orphan_data=False, use_scalable_resource=True, num_streams="max"):
         """
         runs DDB Space reclaimation job with provided level
 
         Args:
             level (int) - criteria for space reclaimation level (1, 2, 3, 4)
                         Default: 3
 
             clean_orphan_data (bool) - run space reclaimation with OCL or not (True/False)
                         Default: False
 
             use_scalable_resource (bool)    - Use Scalable Resource Allocation while running DDB Space Reclamation Job
                         Default: True
 
+            num_streams (str)   -- Number of streams with which job will run.
         Returns:
              object - instance of Job class for DDB Verification job
 
         Raises:
              SDKException:
                 if invalid level is provided
 
@@ -921,14 +922,20 @@
         """
         if not (isinstance(level, int)) and level not in range(1, 4):
             raise SDKException('Storage', '101')
 
         if not isinstance(use_scalable_resource, bool):
             raise SDKException('Storage', '101')
 
+        use_max_streams = "true"
+        max_num_of_streams = 0
+        if str(num_streams) != "max":
+            max_num_of_streams = int(num_streams)
+            use_max_streams = "false"
+
         level_map = {
             1: 80,
             2: 60,
             3: 40,
             4: 20
         }
         clean_orphan_data = str(clean_orphan_data).lower()
@@ -953,30 +960,31 @@
                             "subTaskType": "ADMIN",
                             "operationType": "ARCHIVE_CHECK"
                         },
                         "options": {
                             "backupOpts": {
                                 "mediaOpt": {
                                     "auxcopyJobOption": {
-                                        "useMaximumStreams": "true",
-                                        "maxNumberOfStreams": 0,
+                                        "useMaximumStreams": use_max_streams,
+                                        "maxNumberOfStreams": max_num_of_streams,
                                         "allCopies": "true",
                                         "mediaAgent": {
                                             "mediaAgentName": ""
                                         },
                                         "useScallableResourceManagement": f"{use_scalable_resource}"
                                     }
                                 }
                             },
                             "adminOpts": {
                                 "archiveCheckOption": {
                                     "ddbVerificationLevel": "DDB_DEFRAGMENTATION",
                                     "backupLevel": "FULL",
                                     "defragmentationPercentage": level_map.get(level),
-                                    "ocl": clean_orphan_data
+                                    "ocl": clean_orphan_data,
+                                    "runDefrag": "true"
                                 }
                             }
                         },
                         "subTaskOperation": "OVERWRITE"
                     }
                 }
             }
```

### Comparing `cvpysdk-11.30.1/cvpysdk/deployment/__init__.py` & `cvpysdk-11.32/cvpysdk/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/deployment/cache_config.py` & `cvpysdk-11.32/cvpysdk/deployment/cache_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,24 @@
 
         Raises:
             SDKException:
             - Failed to execute the api
 
             - Response is incorrect/empty
         """
-        response = self.commcell_object.get_gxglobalparam_value()
+        try:
+            response = self.commcell_object.get_gxglobalparam_value()
+        except Exception:
+            try:
+                response = self.commcell_object.get_gxglobalparam_value('Patch Directory')
+            except Exception:
+                raise SDKException('Response', '101', 'Failed to execute api for get_cs_cache_path')
+            if response == '':
+                raise SDKException('Response', '102')
+            return response
         if response['error']['errorCode'] != 0:
             error_message = "Failed with error: [{0}]".format(
                 response['error']['errorMessage']
             )
             raise SDKException(
                 'Response',
                 '101',
@@ -393,15 +402,16 @@
                         "id": self.client_object.client_id,
                         "name": self.client_object.client_name
                     }
                 },
                 "uaList": {
                     "addedList": {
                         "id": entity_id,
-                        "name": entity_name
+                        "name": entity_name,
+                        "type": entity_type
                     }
                 }
             }
         }
 
         flag, response = self._cvpysdk_object.make_request(
             'POST', self._services['EXECUTE_QCOMMAND'], request_json
```

### Comparing `cvpysdk-11.30.1/cvpysdk/deployment/deploymentconstants.py` & `cvpysdk-11.32/cvpysdk/deployment/deploymentconstants.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     list of Unix features supported
     """
     COMMSERVE = 1020
     CASSANDRA = 1211
     CLOUD_APPS = 1140
     DOMINO_DATABASE = 1051
     FILE_SYSTEM = 1101
+    FILE_SYSTEM_CORE = 1002
     FILE_SYSTEM_FOR_IBMI = 1137
     FILE_SYSTEM_FOR_OPEN_VMS = 1138
     MEDIA_AGENT = 1301
     ORACLE = 1204
     POSTGRESQL = 1209
     SAPHANA = 1210
     SQLSERVER = 1212
@@ -86,31 +87,34 @@
     """
     COMMSERVE = 20
     ACTIVE_DIRECTORY = 703
     CLOUD_APPS = 730
     DOMINO_DATABASE = 201
     EXCHANGE = 151
     FILE_SYSTEM = 702
+    FILE_SYSTEM_CORE = 1
     MEDIA_AGENT = 51
     SHAREPOINT = 101
     ORACLE = 352
     POSTGRESQL = 362
     SQLSERVER = 353
     VIRTUAL_SERVER = 713
     VSS_PROVIDER = 453
+    VSS_HARDWARE_PROVIDER = 455
     WEB_CONSOLE = 726
     TEST_AUTOMATION = 719
     PYTHON_SDK = 754
     COMMSERVE_LITE = 25
     CONTENT_ANALYZER = 729
     INDEX_STORE = 55
     INDEX_GATEWAY = 263
     CONTENT_EXTRACTOR = 259
     DB2_AGENT = 351
     INFORMIX = 360
+    SYBASE = 1202
 
 
 class OSNameIDMapping(Enum):
     """
     Class for os name to id mapping
     """
     WINDOWS_32 = 1
```

### Comparing `cvpysdk-11.30.1/cvpysdk/deployment/download.py` & `cvpysdk-11.32/cvpysdk/deployment/download.py`

 * *Files 18% similar despite different names*

```diff
@@ -77,14 +77,16 @@
                 cu_number (int)                --  maintenance release number
 
                 sync_cache (bool)              --  True if download and sync
                                                    False only download
                 
                 sync_cache_list (list)         --  list of names of remote caches to sync
                                                    use None to sync all caches
+
+                schedule_pattern (dict)        --  pattern for schedule task
                                                    
 
             Returns:
                 object - instance of the Job class for this download job
 
             Raises:
                 SDKException:
@@ -240,14 +242,134 @@
                                     }
                                 }
                             }
                         }
                     }
                 ]
             }
+        }
+
+        if schedule_pattern:
+            request_json = SchedulePattern().create_schedule(request_json, schedule_pattern)
+
+        flag, response = self._cvpysdkcommcell_object.make_request(
+            'POST', self._services['CREATE_TASK'], request_json
+        )
+
+        if flag:
+            if response.json():
+                if "jobIds" in response.json():
+                    return Job(self.commcell_object, response.json()['jobIds'][0])
+
+                elif "taskId" in response.json():
+                    return Schedules(self.commcell_object).get(task_id=response.json()['taskId'])
+
+                else:
+                    raise SDKException('Download', '101')
+
+            else:
+                raise SDKException('Response', '102')
+        else:
+            raise SDKException('Response', '101')
+
+    def copy_software(self, media_loc, username=None, password=None, sync_cache=True, schedule_pattern=None):
+        """copies media from the specified location on the commcell
+
+                    Args:
+
+                        media_loc      (str)           --  Media Location to be used for copy software
+
+                        username       (str)           --  username to authenticate to external location
+
+                        password       (str)           --  password to authenticate to external location
+
+                        sync_cache (bool)              --  True if download and sync
+                                                           False only download
+
+                        schedule_pattern(dict)         --  pattern for schedule task
+
+
+                    Returns:
+                        object - instance of the Job class for this copy software job
+
+                    Raises:
+                        SDKException:
+                            if Download job failed
+
+                            if response is empty
+
+                            if response is not success
+
+                            if another download job is running
+                    Usage:
+
+                        -   if media_location directory is local to the machine - username and password is not needed
+
+                            >>> commcell_obj.copy_software(media_loc = "C:\\Downloads\\Media")
+
+                        -   if Media_location directory is remote- username and passsword(base 64 encoded) are needed
+                            to authenticate the cache
+
+                            >>> commcell_obj.copy_software(
+                            media_loc = "\\subdomain.company.com\Media",
+                            username = "domainone\\userone",
+                            password = "base64encoded password"
+                            )
+                """
+        client_auth = {}
+        if username:
+            if password is None:
+                raise Exception(f"Password missing for remote location {media_loc}")
+            client_auth = {
+                "userName": username,
+                "password": password
+            }
+        request_json = {
+            "taskInfo": {
+                "task": {
+                    "taskType": 1,
+                    "initiatedFrom": 2,
+                    "policyType": 0,
+                    "alert": {
+                        "alertName": ""
+                    },
+                    "taskFlags": {
+                        "isEdgeDrive": False,
+                        "disabled": False
+                    }
+                },
+                "subTasks": [
+                    {
+                        "subTaskOperation": 1,
+                        "subTask": {
+                            "subTaskType": 1,
+                            "operationType": 4019
+                        },
+                        "options": {
+                            "adminOpts": {
+                                "updateOption": {
+                                    "syncUpdateCaches": sync_cache,
+                                    "copyUpdates": True,
+                                    "copySoftwareAndUpdates": True,
+                                    "clientAndClientGroups": [
+                                        {
+                                            "_type_": 2
+                                        }
+                                    ],
+                                    "downloadUpdatesJobOptions": {
+                                        "downloadSoftware": True,
+                                        "updateCachePath": media_loc,
+                                        "clientAuth": client_auth
+                                    }
+                                }
+                            }
+                        }
+                    }
+                ]
+            }
         }
 
         if schedule_pattern:
             request_json = SchedulePattern().create_schedule(request_json, schedule_pattern)
 
         flag, response = self._cvpysdkcommcell_object.make_request(
             'POST', self._services['CREATE_TASK'], request_json
```

### Comparing `cvpysdk-11.30.1/cvpysdk/deployment/install.py` & `cvpysdk-11.32/cvpysdk/deployment/install.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     install_software                 --  Installs the features selected on the machines selected
 
 """
 
 from ..job import Job
 from ..exception import SDKException
 from ..deployment.deploymentconstants import UnixDownloadFeatures, WindowsDownloadFeatures
+from ..schedules import SchedulePattern, Schedules
 
 
 class Install(object):
     """"class for installing software packages"""
 
     def __init__(self, commcell_object):
         """Initialize object of the Install class.
@@ -195,15 +196,16 @@
             self,
             client_computers=None,
             client_computer_groups=None,
             all_client_computers=False,
             all_client_computer_groups=False,
             reboot_client=False,
             run_db_maintenance=True,
-            maintenance_release_only=False):
+            maintenance_release_only=False,
+            **kwargs):
         """Installs the software packages on the clients
 
         Args:
             client_computers (list)               -- Client machines to install service pack on
 
             client_computer_groups (list)         -- Client groups to install service pack on
 
@@ -226,33 +228,42 @@
             maintenance not
 
                 default: True
 
             maintenance_release_only (bool)       -- for clients of feature releases lesser than CS, this option
             maintenance release of that client FR, if present in cache
 
+            **kwargs: (dict) -- Key value pairs for supporting conditional initializations
+                Supported -
+                schedule_pattern (dict)           -- Request JSON for scheduling the operation
+
         Returns:
-            object - instance of the Job class for this download job
+            object - instance of the Job/Task class for this download
 
         Raises:
                 SDKException:
+                    if schedule is not of type dictionary
+
                     if Download job failed
 
                     if response is empty
 
                     if response is not success
 
                     if another download job is already running
 
         **NOTE:** push_serivcepack_and_hotfixes cannot be used for revision upgrades
 
         """
         selected_clients = []
         selected_client_groups = []
-
+        schedule_pattern = kwargs.get('schedule_pattern', None)
+        if schedule_pattern:
+            if not isinstance(schedule_pattern, dict):
+                raise SDKException("Install", "101")
         if not any([all_client_computers,
                     all_client_computer_groups,
                     client_computers,
                     client_computer_groups]):
             raise SDKException('Install', '101')
 
         commcell_client_computers = self.commcell_object.clients.all_clients
@@ -319,23 +330,30 @@
                                 }
                             },
                         }
                     }
                 ]
             }
         }
+
+        if schedule_pattern:
+            request_json = SchedulePattern().create_schedule(request_json, schedule_pattern)
+
         flag, response = self._cvpysdk_object.make_request(
             'POST', self._services['CREATE_TASK'], request_json
         )
 
         if flag:
             if response.json():
                 if "jobIds" in response.json():
                     return Job(self.commcell_object, response.json()['jobIds'][0])
 
+                elif schedule_pattern and "taskId" in response.json():
+                    return Schedules(self.commcell_object).get(task_id=response.json()['taskId'])
+
                 else:
                     raise SDKException('Install', '107')
 
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101')
@@ -405,17 +423,60 @@
 
             db2_logs_location (dict) - dictionary of db2 logs location
             Ex: db2_logs_location = {
                                     "db2ArchivePath": "/opt/Archive/",
                                     "db2RetrievePath": "/opt/Retrieve/",
                                     "db2AuditErrorPath": "/opt/Audit/"
                             }
-            
             index_cache_location (str) - Set index cache location for MA package
             Ex: index_cache_location = "/opt/IndexCache/"
+            firewall_inputs (dict) - dictionary for firewall configuration
+            Ex: firewall_inputs = {
+                                  "enableFirewallConfig": True,
+                                  "firewallConnectionType": 1,
+                                  "httpProxyConfigurationType": 0,
+                                  "proxyClientName": "Proxy_client_name",
+                                  "proxyHostName": "Proxy_host_name",
+                                  "portNumber": "port_number",
+                                  "encryptedTunnel": "encrypted_tunnel"
+                            }
+
+            firewall_inputs can take the following values
+
+            Ex 1: Client can open connection to CS
+             firewall_inputs = {
+                                  "enableFirewallConfig": True,
+                                  "firewallConnectionType": 0,
+                                  "proxyClientName": "",
+                                  "proxyHostName": "",
+                                  "portNumber": "port_number",
+                                  "httpProxyConfigurationType": 0,
+                                  "encryptedTunnel": True/False
+                            }
+            Ex 2: CS can open connection to Client
+                 firewall_inputs = {
+                                  "enableFirewallConfig": True,
+                                  "firewallConnectionType": 1,
+                                  "proxyClientName": "",
+                                  "proxyHostName": "",
+                                  "portNumber": "port_number",
+                                  "httpProxyConfigurationType": 0,
+                                  "encryptedTunnel": True/False
+                            }
+
+            Ex 3: Client can communicate to CS using Proxy
+                 firewall_inputs = {
+                                  "enableFirewallConfig": True,
+                                  "firewallConnectionType": 2,
+                                  "httpProxyConfigurationType": 0,
+                                  "proxyClientName": "Proxy_client_name",
+                                  "proxyHostName": "Proxy_host_name",
+                                  "portNumber": "port_number",
+                                  "encryptedTunnel": True/False
+                            }
 
         Returns:
                 object - instance of the Job class for this install_software job
 
         Raises:
             SDKException:
                 if install job failed
@@ -477,14 +538,15 @@
             commcell_name = self.commcell_object.commserv_name
 
             client_details = []
             for client_name in client_computers:
                 client_details.append(
                     {
                         "clientEntity": {
+                            "clientId": 0,
                             "clientName": client_name,
                             "commCellName": commcell_name
                         }
                     })
 
         else:
             raise SDKException('Install', '106')
@@ -495,14 +557,15 @@
                 raise SDKException('Install', '103')
             selected_client_groups = [{'clientGroupName': client_group}
                                       for client_group in client_group_name]
 
         install_flags = kwargs.get('install_flags')
         db2_logs = kwargs.get('db2_logs_location', {})
         index_cache_location = kwargs.get('index_cache_location', None)
+        firewall_inputs = kwargs.get('firewall_inputs', {})
 
         request_json = {
             "taskInfo": {
                 "associations": [
                     {
                         "commCellId": 2
                     }
@@ -526,18 +589,18 @@
                                     "reuseADCredentials": False,
                                     "installOSType": os_type,
                                     "discoveryType": 0,
                                     "installerOption": {
                                         "requestType": 0,
                                         "Operationtype": 0,
                                         "CommServeHostName":
-                                            self.commcell_object.commserv_hostname,
+                                            self.commcell_object.commserv_name,
                                         "RemoteClient": False,
                                         "installFlags": {
-                                            "allowMultipleInstances": True,
+                                            "allowMultipleInstances": kwargs.get('allowMultipleInstances', False),
                                             "restoreOnlyAgents": False,
                                             "killBrowserProcesses": True,
                                             "install32Base": install_flags.get('install32Base',
                                                                                False) if install_flags else False,
                                             "disableOSFirewall": False,
                                             "stopOracleServices": False,
                                             "skipClientsOfCS": False,
@@ -555,14 +618,15 @@
                                         },
                                         "User": {
                                             "userName": "admin",
                                             "userId": 1
                                         },
                                         "clientComposition": [
                                             {
+                                                "activateClient": True,
                                                 "overrideSoftwareCache": True if sw_cache_client else False,
                                                 "softwareCacheOrSrmProxyClient": {
                                                     "clientName": sw_cache_client if sw_cache_client else ""
                                                 },
                                                 "packageDeliveryOption": 0,
                                                 "components": {
                                                     "commonInfo": {
@@ -615,14 +679,19 @@
                 "indexCacheDirectory": {
                     "path": index_cache_location
                 }
             }
             request_json["taskInfo"]["subTasks"][0]["options"]["adminOpts"]["clientInstallOption"]["installerOption"][
                 "clientComposition"][0]["components"]["mediaAgent"] = index_cache_dict
 
+        if firewall_inputs:
+            request_json["taskInfo"]["subTasks"][0]["options"]["adminOpts"]["clientInstallOption"]["installerOption"][
+                "installFlags"]["firewallInstall"] = firewall_inputs
+
+
         flag, response = self._cvpysdk_object.make_request(
             'POST', self._services['CREATE_TASK'], request_json
         )
 
         if flag:
             if response.json():
                 if "jobIds" in response.json():
```

### Comparing `cvpysdk-11.30.1/cvpysdk/deployment/uninstall.py` & `cvpysdk-11.32/cvpysdk/deployment/uninstall.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/dev_test_group.py` & `cvpysdk-11.32/cvpysdk/dev_test_group.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/disasterrecovery.py` & `cvpysdk-11.32/cvpysdk/disasterrecovery.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/domains.py` & `cvpysdk-11.32/cvpysdk/domains.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
     __repr__()                  --  returns the string representation of an instance of this class
 
     _get_domain_id()            --  Gets the domain id associated with this domain
 
     _get_domain_properties      --  get the properties of the domain
 
+    set_sso                     --  Enables/Disables single sign on a domain
+
 
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 from base64 import b64encode
@@ -420,60 +422,60 @@
                     "domainName": netbios_name
                 }
             }
         }
 
         if kwargs:
             custom_provider = {
-                    "providerTypeId": 0,
-                    "attributes": [
-                        {
-                            "attrId": 6,
-                            "attributeName": "User group filter",
-                            "staticAttributeString": "(objectClass=group)",
-                            "customAttributeString": kwargs.get('group_filter', ''),
-                            "attrTypeFlags": 1
-                        },
-                        {
-                            "attrId": 7,
-                            "attributeName": "User filter",
-                            "staticAttributeString": "(&(objectCategory=User)(sAMAccountName=*))",
-                            "customAttributeString": kwargs.get('user_filter', ''),
-                            "attrTypeFlags": 1
-                        },
-                        {
-                          "attrId": 9,
-                          "attributeName": "Unique identifier",
-                          "staticAttributeString": "sAMAccountName",
-                          "customAttributeString": kwargs.get('unique_identifier', ''),
-                          "attrTypeFlags": 1
-                        },
-                        {
-                          "attrId": 10,
-                          "attributeName": "base DN",
-                          "staticAttributeString": "baseDN",
-                          "customAttributeString": kwargs.get('base_dn', ''),
-                          "attrTypeFlags": 1
-                        },
-                        {
-                            "attrTypeFlags": 6,
-                            "customAttributeString": kwargs.get('email_attribute', 'mail'),
-                            "attrId": 3,
-                            "attributeName": "Email",
-                            "staticAttributeString": "mail"
-                        },
-                        {
-                            "attrTypeFlags": 6,
-                            "customAttributeString": kwargs.get('guid_attribute', 'objectGUID'),
-                            "attrId": 4,
-                            "attributeName": "GUID",
-                            "staticAttributeString": "objectGUID"
-                        }
-                    ]
-                }
+                "providerTypeId": 0,
+                "attributes": [
+                    {
+                        "attrId": 6,
+                        "attributeName": "User group filter",
+                        "staticAttributeString": "(objectClass=group)",
+                        "customAttributeString": kwargs.get('group_filter', ''),
+                        "attrTypeFlags": 1
+                    },
+                    {
+                        "attrId": 7,
+                        "attributeName": "User filter",
+                        "staticAttributeString": "(&(objectCategory=User)(sAMAccountName=*))",
+                        "customAttributeString": kwargs.get('user_filter', ''),
+                        "attrTypeFlags": 1
+                    },
+                    {
+                        "attrId": 9,
+                        "attributeName": "Unique identifier",
+                        "staticAttributeString": "sAMAccountName",
+                        "customAttributeString": kwargs.get('unique_identifier', ''),
+                        "attrTypeFlags": 1
+                    },
+                    {
+                        "attrId": 10,
+                        "attributeName": "base DN",
+                        "staticAttributeString": "baseDN",
+                        "customAttributeString": kwargs.get('base_dn', ''),
+                        "attrTypeFlags": 1
+                    },
+                    {
+                        "attrTypeFlags": 6,
+                        "customAttributeString": kwargs.get('email_attribute', 'mail'),
+                        "attrId": 3,
+                        "attributeName": "Email",
+                        "staticAttributeString": "mail"
+                    },
+                    {
+                        "attrTypeFlags": 6,
+                        "customAttributeString": kwargs.get('guid_attribute', 'objectGUID'),
+                        "attrId": 4,
+                        "attributeName": "GUID",
+                        "staticAttributeString": "objectGUID"
+                    }
+                ]
+            }
             domain_create_request["provider"]["customProvider"] = custom_provider
 
         if kwargs.get('additional_settings'):
             domain_create_request["provider"]['additionalSettings'] = kwargs.get('additional_settings')
 
         flag, response = self._cvpysdk_object.make_request(
             'POST', self._DOMAIN_CONTROLER, domain_create_request
@@ -567,14 +569,58 @@
             response_string = self._commcell_object._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
 
     def refresh(self):
         """Refresh the properties of the domain."""
         self._get_domain_properties()
 
+    def set_sso(self, flag=True, **kwargs):
+        """Enables/Disables single sign on the domain
+            Args:
+                flag(bool)      --  True    - enables SSO
+                                    False   - disables SSO
+                ** kwargs(dict) --  Key value pairs for supported arguments
+                Supported argument values:
+                username(str)       --  Username to be used
+                password(str)       --  Password to be used
+
+            Returns:
+                None
+
+            Raises:
+                SDKException:
+                    if arguments passed are of incorrect types
+                    if failed to enable SSO
+                    if response is empty
+                    if response is not success
+        """
+
+        if not isinstance(flag, bool):
+            raise SDKException('Domain', '101')
+        request_json = {"enableSSO": flag}
+        username = kwargs.get("username", None)
+        password = kwargs.get("password", None)
+        if username and password:
+            if not (isinstance(username, str) and isinstance(password, str)):
+                raise SDKException('Domain', '101')
+            request_json["username"] = username
+            request_json["password"] = b64encode(password.encode()).decode()
+        url = self._commcell_object._services['DOMAIN_SSO'] % self.domain_id
+        flag, response = self._commcell_object._cvpysdk_object.make_request(
+            'PUT', url, request_json
+        )
+        if flag:
+            if response.json():
+                error_code = response.json().get('errorCode', 0)
+                if error_code != 0:
+                    raise SDKException('Response', '101', self._commcell_object._update_response_(response.text))
+                return
+            raise SDKException('Response', '102')
+        raise SDKException('Response', '101', self._commcell_object._update_response_(response.text))
+
     @property
     def domain_name(self):
         """Returns the User display name"""
         return self._properties['shortName']['domainName']
 
     @property
     def domain_id(self):
```

### Comparing `cvpysdk-11.30.1/cvpysdk/download_center.py` & `cvpysdk-11.32/cvpysdk/download_center.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/drorchestration/__init__.py` & `cvpysdk-11.32/cvpysdk/drorchestration/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/drorchestration/blr_pairs.py` & `cvpysdk-11.32/cvpysdk/drorchestration/blr_pairs.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/drorchestration/dr_orchestration_job_phase.py` & `cvpysdk-11.32/cvpysdk/drorchestration/dr_orchestration_job_phase.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/drorchestration/drjob.py` & `cvpysdk-11.32/cvpysdk/drorchestration/drjob.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,23 @@
 from cvpysdk.exception import SDKException
 from cvpysdk.job import Job
 from cvpysdk.drorchestration.dr_orchestration_job_phase import DRJobPhases, DRJobPhaseToText
 
 
 class DRJob(Job):
     """Class for performing DR orchestration operations on ReplicationMonitor."""
+
     def __init__(self, commcell_object, job_id):
         """Initialise the DR job"""
         self._replication_job_stats = None
 
-        self._REPLICATION_STATS = commcell_object._services['DR_JOB_STATS'] % job_id
+        service_url = (commcell_object._services['DRORCHESTRATION_JOB_STATS']
+                       if commcell_object.commserv_version > 30
+                       else commcell_object._services['DR_JOB_STATS'])
+        self._REPLICATION_STATS = service_url % job_id
 
         Job.__init__(self, commcell_object, job_id)
 
     def __repr__(self):
         representation_string = 'DRJob class instance for job id: "{0}"'
         return representation_string.format(self.job_id)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/drorchestration/drorchestrationoperations.py` & `cvpysdk-11.32/cvpysdk/drorchestration/drorchestrationoperations.py`

 * *Files 0% similar despite different names*

```diff
@@ -850,16 +850,17 @@
                     If DR orchestration phase failed at any stage
         """
 
         if not isinstance(jobId, str) and not isinstance(
                 replicationId, str):
             raise SDKException('DROrchestrationOperations', '101')
 
-        _DR_JOB_STATS = self._commcell_object._services['DR_GROUP_JOB_STATS'] % (
-            jobId, self.dr_group_id, replicationId)
+        _DR_JOB_STATS = (self._services['FAILOVER_GROUP_JOB_STATS']
+                         if self._commcell_object.commserv_version > 30
+                         else self._services['DR_GROUP_JOB_STATS']) % (jobId, self.dr_group_id, replicationId)
 
         # passing the built json to get DR orchestration job phases
         (flag, response) = self._commcell_object._cvpysdk_object.make_request(
             method='GET', url=_DR_JOB_STATS)
 
         if flag:
             if response.json():
```

### Comparing `cvpysdk-11.30.1/cvpysdk/drorchestration/failovergroups.py` & `cvpysdk-11.32/cvpysdk/drorchestration/failovergroups.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 FailoverGroups:     Class for getting information of all failover groups in the commcell
 
 FailoverGroup:      Class for a failover group that gives us all the live sync pairs associated to in,
                     with addition to the clients/hypervisors associated
 
 
 FailoverGroups:
+    FailoverGroupSourceTypes                    --  Enum to represent all type of sources for failover groups
     FailoverGroupTypes                          --  Enum to represent all types of failover groups
     DRReplicationTypes                          --  Enum to represent all live sync types
     __init__(commcell_object)                   --  Initialize the object of failovergroups class for commcell
 
     __str__()                                   --  Returns the list of all failover groups
 
     __repr__()                                  --  Returns the string for the instance of the FailoverGroups class
@@ -61,19 +62,29 @@
 
     ##### internal methods #####
     _get_failover_group_dict()                  --  Gets the failover group information from FailoverGroups class
 
     _get_failover_group_properties()            --  Get the failover group properties
 
     ##### properties #####
+    failover_group_id                           --  The ID of the failover group
+
     failover_group_name                         --  The name of the failover group
 
+    replication_type                            --  The DRReplicationTypes key for replication of failover group
+
+    group_type                                  --  The FailoverGroupTypes for operation of failover group
+
+    source_type                                 --  The FailoverGroupSourceTypes of source of failover group
+
     is_client_group                             --  Whether the VM pairs are part of a client group or not
 
-    vm_pair_ids                                 --  The ID of the live sync pairs
+    replication_pairs                           --  The ReplicationPairs class for failover group
+
+    vm_pair_ids                                 --  The ID of the replication pairs
 
     vm_pairs                                    --  Returns the live sync pair objects for each VM pair of the group
                                                         as a mapping of source VM name and VM pair object
 
     replication_groups                          --  The names of all replication groups associated
                                                     to the failover group
 
@@ -93,20 +104,25 @@
 
     user_for_approval                           --  Returns the name of the user set in failover group
                                                         for approval
 
 """
 from enum import Enum
 from ..exception import SDKException
-from .replication_pairs import ReplicationPair
+from .replication_pairs import ReplicationPairs
 
 
 class FailoverGroups:
     """Class for getting all the failover groups in commcell."""
 
+    class FailoverGroupSourceTypes(Enum):
+        BACKUP = 0
+        REPLICATION = 1
+        TEMPLATES = 2
+
     class FailoverGroupTypes(Enum):
         """ Enum to map Failover Group Types to integers"""
         LIVE_MOUNT = 1
         LIVE_SYNC = 2
         RESTORE = 4
         LIVE_RECOVERY = 8
         FAILOVER = 16
@@ -212,38 +228,52 @@
     def _get_failover_groups(self):
         """REST API call for all the failover groups in the commcell.
             Args:
 
             Returns:
                 dict - consists of all failover groups
                     {
-                         "failover_group_name1": {id: '1', 'type': VSA_PERIODIC, 'operation_type': FAILOVER},
-                         "failover_group_name2": {id: '2', 'type': VSA_CONTINUOUS, 'operation_type': FAILOVER}
+                        "failover_group_name1": {
+                            'id': '1',
+                            'type': LIVE_SYNC,
+                            'operation_type': FAILOVER,
+                            'source_type': REPLICATION
+                        },
+                        "failover_group_name2": {
+                            'id': '2',
+                            'type': SNAP_ARRAY,
+                            'operation_type': TEST_FAILOVER
+                            'source_type': REPLICATION
+                        }
                     }
 
             Raises:
                 SDKException:
                     if response is empty
                     if response is not success
         """
         failover_groups = {}
 
         flag, response = self._commcell_object._cvpysdk_object.make_request(
-            'GET', self._services['DR_GROUPS'])
+            'GET', (self._services['FAILOVER_GROUPS']
+                    if self._commcell_object.commserv_version > 30
+                    else self._services['DR_GROUPS']))
         if flag:
             if 'vApp' in response.json():
                 for failover_group in response.json().get('vApp', []):
                     failover_group_id = str(failover_group.get('vAppEntity', {}).get('vAppId'))
                     failover_group_name = failover_group.get('vAppEntity', {}).get('vAppName', '').lower()
                     operation_type = self.FailoverGroupTypes(int(failover_group.get('operationType', 16)))
                     replication_type = self.DRReplicationTypes(int(failover_group.get('replicationType', 0)))
+                    source_type = self.FailoverGroupSourceTypes(int(failover_group.get('source', 1)))
                     failover_groups[failover_group_name] = {
                         'id': failover_group_id,
                         'operation_type': operation_type,
-                        'type': replication_type
+                        'type': replication_type,
+                        'source_type': source_type
                     }
                 return failover_groups
             raise SDKException('Response', '102')
 
         response_string = self._commcell_object._update_response_(response.text)
         raise SDKException('Response', '101', response_string)
 
@@ -277,15 +307,15 @@
 
         self._source_client = None
         self._destination_client = None
         self._destination_agent = None
         self._source_instance = None
         self._destination_instance = None
 
-        self._vm_pairs = {}
+        self._replication_pairs = None
 
         self.refresh()
 
     def __repr__(self):
         """String representation of the instance of the failover group"""
         return f'FailoverGroup class instance for {self._failover_group_name}'
 
@@ -320,60 +350,93 @@
                 SDKException:
                     if response is empty
 
                     if response is not success
         """
         flag, response = self._commcell_object._cvpysdk_object.make_request(
             'GET',
-            self._services['GET_DR_GROUP'] % str(self._failover_group_dict.get('id'))
+            (self._services['GET_FAILOVER_GROUP']
+             if self._commcell_object.commserv_version > 30
+             else self._services['GET_DR_GROUP']) % str(self.failover_group_id)
         )
         if flag:
             if 'vApp' in response.json():
                 return response.json().get('vApp', [{}])[0]
             raise SDKException('Response', '102')
         response_string = self._commcell_object._update_response_(response.text)
         raise SDKException('Response', '101', response_string)
 
     def refresh(self):
         """ Refresh the failover group properties """
         self._failover_group_properties = self._get_failover_group_properties()
-        self._vm_pairs = None
+        self.replication_pairs.refresh()
+
+    @property
+    def failover_group_id(self):
+        """Returns: (str) The ID of the failover group"""
+        return self._failover_group_dict.get('id')
 
     @property
     def failover_group_name(self):
         """Returns: (str) The name of the failover group"""
         return self._failover_group_name
 
     @property
+    def replication_type(self):
+        """Returns: (DRReplicationTypes) The type of replication"""
+        return self._failover_group_dict.get('type')
+
+    @property
+    def group_type(self):
+        """Returns: (FailoverGroupTypes) The type of failover group"""
+        return self._failover_group_dict.get('operation_type')
+
+    @property
+    def source_type(self):
+        """Returns: (FailoverGroupSourceTypes) The type of failover group's source"""
+        return self._failover_group_dict.get('source_type')
+
+    @property
     def is_client_group(self):
         """Returns: (bool) Whether this failover group has a client group or not"""
         return self._failover_group_properties.get('isClientGroup')
 
     @property
+    def replication_pairs(self):
+        """
+        Returns: (ReplicationPairs) Returns the ReplicationPairs object that belongs to this failover group
+        Note: Implemented only for live sync failover groups
+        """
+        if not self._replication_pairs:
+            if self.replication_type == FailoverGroups.DRReplicationTypes.LIVE_SYNC:
+                self._replication_pairs = ReplicationPairs(self._commcell_object,
+                                                           failover_group_id=self.failover_group_id)
+        return self._replication_pairs
+
+    @property
     def vm_pair_ids(self):
         """Returns: (List[str]) Returns the VM pair IDs that belong to this failover group"""
-        vm_sequence = (self._failover_group_properties.get('config', {}).get('vmGroups', [{}])[0]
-                       .get('vmSequence', []))
-        return [str(vm_info.get('replicationId')) for vm_info in vm_sequence if 'replicationId' in vm_info]
+        return list(self.replication_pairs.replication_pairs)
 
     @property
     def vm_pairs(self):
         """
         Returns: (dict) The list of all live sync VM pairs
             eg:
                 {
                     <source_vm1>: <Replication_pair_obj1>,
                     <source_vm2>: <Replication_pair_obj2>
                 }
         """
-        if not self._vm_pairs:
-            for replication_id in self.vm_pair_ids:
-                vm_pair = ReplicationPair(self._commcell_object, replication_id)
-                self._vm_pairs[vm_pair.source_vm] = vm_pair
-        return self._vm_pairs
+        replication_pair_objects = {}
+        for replication_pair_id, replication_pair_dict in self.replication_pairs.replication_pairs.items():
+            source_vm_name = replication_pair_dict.get('source_vm')
+            replication_pair_object = self.replication_pairs.get(replication_id=replication_pair_id)
+            replication_pair_objects[source_vm_name] = replication_pair_object
+        return replication_pair_objects
 
     @property
     def replication_groups(self):
         """Returns: (list) The list of all replication group names"""
         group_names = {vm_pair.replication_group_name for vm_pair in self.vm_pairs.values()}
         return list(group_names)
 
@@ -430,10 +493,10 @@
             false: if approval not set in failover group
         """
         return self._failover_group_properties.get('approvalRequired')
 
     @property
     def user_for_approval(self):
         """Returns: user name set in failover group"""
-        user_name = (self._failover_group_properties.get('usersForApproval',[{}])[0]
-                     .get('userEntity',{}).get('userName',''))
+        user_name = (self._failover_group_properties.get('usersForApproval', [{}])[0]
+                     .get('userEntity', {}).get('userName', ''))
         return user_name
```

### Comparing `cvpysdk-11.30.1/cvpysdk/drorchestration/replication_groups.py` & `cvpysdk-11.32/cvpysdk/drorchestration/replication_groups.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/drorchestration/replicationmonitor.py` & `cvpysdk-11.32/cvpysdk/drorchestration/replicationmonitor.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/eventviewer.py` & `cvpysdk-11.32/cvpysdk/eventviewer.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/exception.py` & `cvpysdk-11.32/cvpysdk/exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -413,23 +413,40 @@
         '110': 'Failed to update the properties of the Organization',
         '111': ('Plan is not associated with the organization. '
                 'Add plan to the Organization, and then set it as the default'),
         '112': 'Failed to activate organization',
         '113': 'Failed to deactivate organization',
         '114': 'Input is not provided in expected manner'
     },
+    'RemoteOrganization': {
+        '101': 'Failed to update organization operators remotely',
+        '102': 'Failed to activate organization remotely',
+        '103': 'Failed to deactivate organization remotely',
+        '104': 'Failed to update organization tags remotely',
+        '105': 'Data type of the input(s) is not valid',
+        '106': '',
+        '107': 'Email address is not valid',
+        '108': 'Organization already exists',
+        '109': 'Failed to add organization remotely',
+        '110': 'No organization exists with the given name in workloads or idp'
+    },
     'StoragePool': {
         '101': 'Data type of the input(s) is not valid',
         '102': '',
         '103': 'No storage pool exists with the given name',
     },
     'Monitoring': {
         '101': 'Data type of the input(s) is not valid',
         '102': ''
     },
+    'ReplicationPairs': {
+        '101': 'Failed to get replication pairs information',
+        '102': 'Invalid response received for replication pairs',
+        '103': 'Replication Pair not found'
+    },
     'BLRPairs': {
         '101': 'Data type of the input(s) is not valid',
         '102': 'BLR Pair not found',
         '103': 'RPStore not found'
     },
     'ReplicationGroup': {
         '101': 'Data type of the input(s) is not valid',
@@ -552,18 +569,21 @@
         '102': ''
     },
     'KeyManagementServer': {
         '101': 'Data type of the input(s) is not valid',
         '102': 'Key Management Server not found',
         '103': 'Key Management Server type is not valid',
         '104': 'Key Management Server type not found',
+        '105': 'Invalid key provider authentication type',
+        '106': 'Invalid KMS name'
     },
     'Region': {
         '101': 'Entity type not found.',
-        '102': ''
+        '102': '',
+        '103': ''
     }
 }
 
 
 class SDKException(Exception):
     """Exception class for raising exception specific to a module."""
```

### Comparing `cvpysdk-11.30.1/cvpysdk/globalfilter.py` & `cvpysdk-11.32/cvpysdk/globalfilter.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/hac_clusters.py` & `cvpysdk-11.32/cvpysdk/hac_clusters.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/identity_management.py` & `cvpysdk-11.32/cvpysdk/identity_management.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/index_pools.py` & `cvpysdk-11.32/cvpysdk/index_pools.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/index_server.py` & `cvpysdk-11.32/cvpysdk/index_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,28 +85,34 @@
 
     refresh()                           --  refresh all the properties of client
 
     update_roles_data()                 --  fetches the cloud roles data from commcell
 
     modify()                            --  to modify the index server node details
 
+    change_plan()                       --  changes the plan of a given index server
+
     update_role()                       --  to update the roles assigned to cloud
 
     hard_commit                         --  do hard commit on specified index server solr core
 
     get_all_cores                       --  gets all the cores in index server
 
     _create_solr_query()                --  Create solr search query based on inputs provided
 
     execute_solr_query()                --  Creates solr url based on input and executes it on solr on given core
 
     get_index_node()                    --  returns an Index server node object for given node name
 
     get_os_info()                       --  returns the OS type for the Index server
 
+    get_plan_info()                     --  Returns the plan information of the index server
+
+    __form_field_query()                --  returns the query with the key and value passed
+
 IndexServer Attributes
 ----------------------
 
     **properties**                      --  returns the properties of this index server
 
     **roles_data**                      --  returns all the available cloud roles data
 
@@ -139,14 +145,16 @@
 
     **is_cloud**                        --  returns boolean True if the Index server is cloud else returns False
 
     **node_count**                      --  returns the number of Index server nodes
 
     **os_info**                         --  returns the OS type for the Index server
 
+    **plan_name**                       --  Returns the plan name associated with index server
+
 
 IndexNode
 =========
 
     __init__()                          --  initializes the class with commcell object
                                             Index server cloud id and Node client name
 
@@ -645,14 +653,15 @@
         self._services = self._commcell_obj._services
         if cloud_id:
             self._cloud_id = cloud_id
         else:
             self._cloud_id = self._get_cloud_id()
         self._properties = None
         self._roles_obj = None
+        self.plan_info = None
         self.os_type = None
         self.refresh()
 
     def __repr__(self):
         """String representation of the instance of this class."""
         return 'IndexServer class instance for index server: "{0}"'.format(
             self._engine_name)
@@ -674,14 +683,16 @@
         """Refresh the index server properties"""
         self._commcell_obj.index_servers.refresh()
         self._get_properties()
         if self.os_type is None:
             self.os_type = self.get_os_info()
         if not self._roles_obj:
             self._roles_obj = _Roles(self._commcell_obj)
+        if self.plan_info is None:
+            self.plan_info = self.get_plan_info()
 
     def update_roles_data(self):
         """Synchronize the cloud roles data with the commcell"""
         self._roles_obj.update_roles_data()
 
     def modify(self, index_location, node_name, node_params):
         """Modifies the properties of an index server
@@ -724,14 +735,48 @@
             if response.json():
                 if 'cloudId' in response.json():
                     self.refresh()
                     return
             raise SDKException('Response', '102')
         raise SDKException('Response', '101')
 
+    def change_plan(self, plan_name):
+        """Modifies the plan used by an index server
+
+            Args:
+                plan_name      (str)       --  Name of the plan to be used for the index server
+            Raises:
+                SDKException:
+                    Response was not success.
+                    Response was empty.
+                    if plan with given name doesn't exist
+        """
+        if not self._commcell_obj.plans.has_plan(plan_name):
+            raise SDKException(
+                'Plan', '102', f"Plan with name [{plan_name}] doesn't exist")
+        request_json = {
+            "opType": IndexServerConstants.OPERATION_EDIT,
+            "type": 1,
+            "planInfo": {
+                "planId": int(self._commcell_obj.plans.get(plan_name).plan_id)
+            },
+            "cloudInfoEntity": {
+                "cloudId": self.cloud_id
+            }
+        }
+        flag, response = self._cvpysdk_object.make_request(
+            "POST", self._services['CLOUD_MODIFY'], request_json)
+        if flag:
+            if response.json():
+                if 'cloudId' in response.json():
+                    self.refresh()
+                    return
+            raise SDKException('Response', '102')
+        raise SDKException('Response', '101')
+
     def update_role(self, props=None):
         """Updates a role of an Index Server
 
             Args:
                 props               (list)  --  array of dictionaries
                 consisting details of the roles such as role name
                 and operation type.
@@ -914,19 +959,20 @@
                 field_query = f"{field_query}&exclude=false"
 
             ex_query = ""
             if not op_params:
                 op_params = {'wt': "json"}
             else:
                 op_params['wt'] = "json"
-            for key, value in op_params.items():
-                if value is None:
-                    ex_query += f'&{key}'
+            for key, values in op_params.items():
+                if isinstance(values, list):
+                    for value in values:
+                        ex_query += self.__form_field_query(key, value)
                 else:
-                    ex_query += f'&{key}={str(value)}'
+                    ex_query += self.__form_field_query(key, values)
             final_url = f'{search_query}{field_query}{ex_query}'
             return final_url
         except Exception as excp:
             raise SDKException('IndexServers', '104', f"Something went wrong while creating solr query - {excp}")
 
     def execute_solr_query(
             self,
@@ -1007,14 +1053,21 @@
 
         """
         node_name = node_name.lower()
         if node_name in self.client_name:
             return IndexNode(self._commcell_obj, self.engine_name, node_name)
         raise SDKException("IndexServers", '104', 'Index server node not found')
 
+    def get_plan_info(self):
+        """Returns the plan information of the index server"""
+        client = self._commcell_obj.clients.get(self.index_server_client_id)
+        instance_props = client.properties.get("pseudoClientInfo", {}).get("distributedClusterInstanceProperties", {})
+        plan_details = instance_props.get("clusterConfig",{}).get("cloudInfo", {}).get("planInfo", {})
+        return plan_details
+
     def get_os_info(self):
         """Returns the OS type for the Index server"""
 
         nodes_name = self.client_name
         nodes = [self._commcell_obj.clients.get(node) for node in nodes_name]
         nodes_os_info = [node.os_info for node in nodes]
         if IndexServerOSType.WINDOWS.value.lower() in nodes_os_info[0].lower():
@@ -1024,14 +1077,35 @@
             return IndexServerOSType.WINDOWS.value
         else:
             for node in nodes_os_info[1:]:
                 if IndexServerOSType.WINDOWS.value.lower() in node.lower():
                     return IndexServerOSType.MIXED.value
             return IndexServerOSType.UNIX.value
 
+    def __form_field_query(self, key, value):
+        """
+        Returns the query with the key and value passed
+        Args:
+                key(str)    -- key for forming the query
+                value(str)  -- value for forming the query
+            Returns:
+                query to be executed against solr
+        """
+        query = None
+        if value is None:
+            query = f'&{key}'
+        else:
+            query = f'&{key}={str(value)}'
+        return query
+
+    @property
+    def plan_name(self):
+        """Returns the plan name associated with index server"""
+        return self.plan_info.get("planName")
+
     @property
     def os_info(self):
         """Returns the OS type for the Index server"""
         return self.os_type
 
     @property
     def is_cloud(self):
```

### Comparing `cvpysdk-11.30.1/cvpysdk/instance.py` & `cvpysdk-11.32/cvpysdk/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     has_instance(instance_name)     --  checks if a instance exists with the given name or not
 
     get(instance_name)              --  returns the Instance class object
     of the input backup set name
 
     _process_add_response()         --  to process the add instance request using API call
 
+    add_sap_hana_instance()         --  method to add new sap hana instance
+
     add_informix_instance()         --  adds new Informix Instance to given Client
 
     delete()                        --  deletes the instance specified by the instance_name
     from the agent.
 
     add_sybase_instance()           --  To add sybase server instance
 
@@ -527,14 +529,76 @@
             else:
                 raise SDKException('Response', '102')
         else:
             response_string = self._commcell_object._update_response_(
                 response.text)
             raise SDKException('Response', '101', response_string)
 
+    def add_sap_hana_instance(self, **kwargs):
+        """Adds new sap hana instance to given client
+            Args:
+                sid             (str)   -- Database SID
+                hana_client_name(str)   --  Client where the hana server exists
+                db_user_name   (str)    -- postgres user name
+                db_password    (str)    -- DB password
+                storage_policy  (str)   --  Storage Policy name
+            Returns:
+                object - instance of the Instance class
+
+            Raises:
+                SDKException:
+                    if None value in sap hana options
+
+                    if sap hana instance with same name already exists
+
+                    if given storage policy does not exists in commcell
+        """
+
+        if self.has_instance(kwargs.get('sid', '')):
+            raise SDKException(
+                'Instance', '102', 'Instance "{0}" already exists.'.format(
+                    kwargs.get('sid', ''))
+            )
+        password = b64encode(kwargs.get("db_password", "").encode()).decode()
+        request_json = {
+            "instanceProperties": {
+                "instance": {
+                    "clientName": self._client_object.client_name,
+                    "instanceName": kwargs.get('sid', ''),
+                    "applicationId": 135,
+                },
+                "saphanaInstance": {
+                    "dbInstanceNumber": "00",
+                    "hdbsqlLocationDirectory": f"/usr/sap/{kwargs.get('sid', '')}/HDB00/exe",
+                    "SAPHANAUser": {
+                        "userName": f"{kwargs.get('sid', '').lower()}adm"
+                    },
+                    "dbUser": {
+                        "userName": kwargs.get("db_user_name", ""),
+                        "password": password
+                    },
+                    "saphanaStorageDevice": {
+                        "logBackupStoragePolicy": {
+                            "storagePolicyName": kwargs.get("storage_policy", "")
+                        },
+                        "commandLineStoragePolicy": {
+                            "storagePolicyName": kwargs.get("storage_policy", "")
+                        }
+                    },
+                    "DBInstances": [
+                        {
+                            "clientName": kwargs.get("hana_client_name", "")
+                        }
+                    ]
+
+                }
+            }
+        }
+        self._process_add_response(request_json)
+
     def delete(self, instance_name):
         """Deletes the instance specified by the instance_name from the agent.
 
             Args:
                 instance_name (str)  --  name of the instance to remove from the agent
 
             Raises:
@@ -645,29 +709,29 @@
                 '102',
                 'Storage Policy: "{0}" does not exist in the Commcell'.format(
                     sybase_options["storage_policy"])
             )
 
         # encodes the plain text password using base64 encoding
         sa_password = b64encode(sybase_options["sa_password"].encode()).decode()
-        localadmin_password = b64encode(sybase_options["localadmin_password"].encode()).decode()
 
         enable_auto_discovery = sybase_options["enable_auto_discovery"]
 
         request_json = {
             "instanceProperties": {
                 "instance": {
                     "clientName": self._client_object.client_name,
                     "appName": "Sybase",
                     "instanceName": sybase_options["instance_name"],
                     "_type_": 5,
                     "applicationId": 5
                 },
                 "sybaseInstance": {
                     "sybaseOCS": sybase_options["sybase_ocs"],
+                    "sybaseBlockSize": 65536,
                     "backupServer": sybase_options["backup_server"],
                     "sybaseHome": sybase_options["sybase_home"],
                     "sybaseASE": sybase_options["sybase_ase"],
                     "configFile": sybase_options["config_file"],
                     "enableAutoDiscovery": enable_auto_discovery,
                     "sharedMemoryDirectory": sybase_options["shared_memory_directory"],
                     "defaultDatabaseStoragePolicy": {
@@ -677,14 +741,17 @@
                     "localAdministrator": {
                         "password": localadmin_password,
                         "userName": sybase_options["localadmin_username"]
                     }
                 }
             }
         }
+        if "localadmin_password" in sybase_options.keys():
+            localadmin_password = b64encode(sybase_options["localadmin_password"].encode()).decode()
+            request_json['instanceProperties']['sybaseInstance']['localAdministrator']['password'] = localadmin_password
 
         flag, response = self._cvpysdk_object.make_request(
             'POST', self._services['ADD_INSTANCE'], request_json
         )
         if flag:
             if response.json() and 'response' in response.json():
                 error_code = response.json()['response']['errorCode']
@@ -699,14 +766,15 @@
                     )
                 else:
                     instance_name = response.json(
                     )['response']['entity']['instanceName']
                     instance_id = response.json(
                     )['response']['entity']['instanceId']
                     agent_name = self._agent_object.agent_name
+                    self.refresh()
                     return self.get(instance_name)
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101', self._update_response_(response.text))
 
     def add_db2_instance(self, db2_options):
@@ -2077,15 +2145,15 @@
             restore_option["to_time"] = to_time
 
         # set versions
         if "versions" in restore_option:
             versions = restore_option['versions']
             if not isinstance(versions, list):
                 raise SDKException('Instance', '101')
-            if 'win' in self._agent_object._client_object.os_info.lower():
+            if 'win' in self._agent_object._client_object.os_info.lower() or self._agent_object._agent_name == "virtual server":
                 version_string = "|\\|#15!vErSiOnS|#15!\\{0}"
             else:
                 version_string = "|/|#15!vErSiOnS|#15!/{0}"
 
             for version in versions:
                 version = version_string.format(version)
                 restore_option["paths"].append(version)
@@ -2754,14 +2822,17 @@
                 'clientName': value.get("iscsi_server")
             }
 
         # Add this option to enable restoring of troubleshooting folder
         if value.get("include_metadata", False):
             self._browse_restore_json["includeMetaData"] = True
 
+        if value.get('cvcBrowse'):
+            self._browse_restore_json["cvcBrowse"] = True
+
     def _restore_common_opts_json(self, value):
         """ Method to set commonOpts for restore
 
         Args:
              value  (dict)  -- restore options dictionary
 
         """
```

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/__init__.py` & `cvpysdk-11.32/cvpysdk/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/aadinstance.py` & `cvpysdk-11.32/cvpysdk/instances/aadinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/bigdataappsinstance.py` & `cvpysdk-11.32/cvpysdk/instances/bigdataappsinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/cainstance.py` & `cvpysdk-11.32/cvpysdk/instances/cainstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/cloudapps/__init__.py` & `cvpysdk-11.32/cvpysdk/instances/cloudapps/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/cloudapps/amazon_instance.py` & `cvpysdk-11.32/cvpysdk/instances/cloudapps/amazon_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/cloudapps/cloud_database_instance.py` & `cvpysdk-11.32/cvpysdk/instances/cloudapps/cloud_database_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/cloudapps/cloud_storage_instance.py` & `cvpysdk-11.32/cvpysdk/instances/cloudapps/cloud_storage_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/cloudapps/dynamics365_instance.py` & `cvpysdk-11.32/cvpysdk/instances/cloudapps/dynamics365_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/cloudapps/google_instance.py` & `cvpysdk-11.32/cvpysdk/instances/cloudapps/google_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/cloudapps/salesforce_instance.py` & `cvpysdk-11.32/cvpysdk/instances/cloudapps/salesforce_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/cloudapps/spanner_instance.py` & `cvpysdk-11.32/cvpysdk/instances/cloudapps/spanner_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/cloudapps/teams_instance.py` & `cvpysdk-11.32/cvpysdk/instances/cloudapps/teams_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/db2instance.py` & `cvpysdk-11.32/cvpysdk/instances/db2instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,16 +584,21 @@
         request_json["taskInfo"]["subTasks"][0]["options"]["restoreOptions"]["db2Option"][
             "storagePaths"] = [target_path]
 
         request_json["taskInfo"]["subTasks"][0]["options"]["restoreOptions"]["db2Option"][
             "databaseTableRstOptions"] = table_json
 
         request_json['taskInfo']["subTasks"][0]["options"]["restoreOptions"][
+            "browseOption"]["backupset"]["backupsetId"] = int(self.backupsets.get(aux_backupset_name).backupset_id)
+
+        request_json['taskInfo']["subTasks"][0]["options"]["restoreOptions"][
             "browseOption"]["backupset"]["backupsetName"] = aux_backupset_name
 
+        request_json["taskInfo"]["subTasks"][0]["options"]["restoreOptions"]["db2Option"][
+            "restoreArchiveLogs"] = False
+
         request_json['taskInfo']["subTasks"][0]["options"]["restoreOptions"][
             "fileOption"]["filterItem"] = tables_path
         request_json['taskInfo']["subTasks"][0]["options"]["restoreOptions"][
             "fileOption"]["sourceItem"] = tables_path
-
         return self._process_restore_response(request_json)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/dbinstance.py` & `cvpysdk-11.32/cvpysdk/instances/dbinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/hanainstance.py` & `cvpysdk-11.32/cvpysdk/instances/hanainstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/informixinstance.py` & `cvpysdk-11.32/cvpysdk/instances/informixinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/lndbinstance.py` & `cvpysdk-11.32/cvpysdk/instances/lndbinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/__init__.py` & `cvpysdk-11.32/cvpysdk/instances/lotusnotes/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/lndbinstance.py` & `cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndbinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/lndminstance.py` & `cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndminstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/lndocinstance.py` & `cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndocinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/lotusnotes/lninstance.py` & `cvpysdk-11.32/cvpysdk/instances/lotusnotes/lninstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/mysqlinstance.py` & `cvpysdk-11.32/cvpysdk/instances/mysqlinstance.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,17 @@
     **is_xtrabackup_enabled**           -- Returns the MySQL Server xtrabackup enabled flag
 
     **proxy_options**                   -- Returns the MySQL Server proxy options
 
     **mysql_enterprise_backup_binary_path** --  Returns the MySQL Enterprise backup binary path
     details
 
+    **no_lock_status**                  --  Returns the No Lock check box status for MySQL Instance
+
+    **ssl_enabled**                     --  Returns(boolean) True/False based on SSL status
 
 """
 
 from __future__ import unicode_literals
 from ..instance import Instance
 from ..exception import SDKException
 
@@ -305,14 +308,46 @@
         meb_bin_path_update = {
             "enableMEB": False if value == '' else True,
             "mebBinPath": value
         }
         properties['mySqlInstance']['mebSettings'] = meb_bin_path_update
         self.update_properties(properties)
 
+    @property
+    def no_lock_status(self):
+        """ Returns the status of No Lock Checkbox in MySQL Instance
+
+            Returns:
+            (bool)  --  True if No Lock checkbox is enabled
+                        False if No Lock checkbox is disabled
+
+        """
+        return self._properties.get('mySqlInstance', {}).get('EnableNoLocking', False)
+
+    @no_lock_status.setter
+    def no_lock_status(self, value):
+        """ Setter for No Lock property in MySQL Instance
+
+            Args:
+
+                value (bool)  -- True or False to enable or disable the No Lock
+                property in MySQL Instance
+
+        """
+        if not isinstance(value, bool):
+            raise SDKException('Instance', '101')
+        properties = self._properties
+        properties['mySqlInstance']['EnableNoLocking'] = value
+        self.update_properties(properties)
+
+    @property
+    def ssl_enabled(self):
+        """ Returns(boolean) True/False based on SSL status """
+        return self._properties.get('mySqlInstance', {}).get('sslEnabled', False)
+
     def _get_instance_properties(self):
         """Gets the properties of this instance.
 
             Raises:
                 SDKException:
                     if response is empty
```

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/oracleinstance.py` & `cvpysdk-11.32/cvpysdk/instances/oracleinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/postgresinstance.py` & `cvpysdk-11.32/cvpysdk/instances/postgresinstance.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,14 +75,22 @@
 
     **use_master_for_log_backup**        --  Returns True if master is used for log backup
 
     **use_master_for_data_backup**       --  Returns True if master is used for data backup
 
     **archive_delete**                   --  Returns True if archive delete is enabled for instance
 
+    **postgres_ssl_status**              --  Returns True/False based on if ssl is enabled or not
+
+    **postgres_ssl_ca_file**             --  Returns SSL CA file path
+
+    **postgres_ssl_key_file**            --  Returns SSL key file path
+
+    **postgres_ssl_cert_file**           --  Returns SSL cert file path
+
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 from base64 import b64encode
 from ..instance import Instance
@@ -102,25 +110,24 @@
             Returns:
                 object - instance of the Instances class
 
         """
         super(
             PostgreSQLInstance,
             self).__init__(
-                agent_object,
-                instance_name,
-                instance_id)
+            agent_object,
+            instance_name,
+            instance_id)
         self.backup_object = None
         self.backupset_object = None
         self.sub_client_object = None
         self.postgres_restore_json = None
         self._postgres_restore_options = None
         self._destination_restore_json = None
 
-
     @property
     def postgres_bin_directory(self):
         """Returns the bin directory of postgres server
 
             Return Type: str
 
         """
@@ -268,26 +275,30 @@
     def standby_instance_name(self):
         """Returns the standby instance name
 
             Return Type: str
 
         """
         if self.is_standby_enabled:
-            return self._properties.get('postGreSQLInstance', {}).get('standbyOptions', {}).get('standbyInstance', {}).get('instanceName', {})
+            return self._properties.get('postGreSQLInstance', {}).get('standbyOptions', {}).get('standbyInstance',
+                                                                                                {}).get('instanceName',
+                                                                                                        "")
         return None
 
     @property
     def standby_instance_id(self):
         """Returns the standby instance id
 
             Return Type: str
 
         """
         if self.is_standby_enabled:
-            return self._properties.get('postGreSQLInstance', {}).get('standbyOptions', {}).get('standbyInstance', {}).get('instanceId', {})
+            return self._properties.get('postGreSQLInstance', {}).get('standbyOptions', {}).get('standbyInstance',
+                                                                                                {}).get('instanceId',
+                                                                                                        "")
         return None
 
     @property
     def is_standby_enabled(self):
         """Returns True if standby enabled. False if not
 
             Return Type: bool
@@ -322,15 +333,16 @@
     @property
     def use_master_for_data_backup(self):
         """ Returns True if master is used for data backup
 
             Return Type: bool
 
         """
-        return self._properties.get('postGreSQLInstance', {}).get('standbyOptions', {}).get('useMasterForDataBkp', False)
+        return self._properties.get('postGreSQLInstance', {}).get('standbyOptions', {}).get('useMasterForDataBkp',
+                                                                                            False)
 
     @use_master_for_data_backup.setter
     def use_master_for_data_backup(self, value):
         """ Setter for user master for data backup standby property
 
             Args:
 
@@ -339,14 +351,34 @@
         """
         if not isinstance(value, bool):
             raise SDKException('Instance', '101')
         properties = self._properties
         properties['postGreSQLInstance']['standbyOptions']['useMasterForDataBkp'] = value
         self.update_properties(properties)
 
+    @property
+    def postgres_ssl_status(self):
+        """Returns True/False based on if ssl is enabled or not"""
+        return self._properties.get("postGreSQLInstance", {}).get("sslOpt", {}).get("sslEnabled", False)
+
+    @property
+    def postgres_ssl_ca_file(self):
+        """Returns: str - ssl ca file path"""
+        return self._properties.get("postGreSQLInstance", {}).get("sslOpt", {}).get("sslCa", "")
+
+    @property
+    def postgres_ssl_key_file(self):
+        """Returns: str - ssl key file path"""
+        return self._properties.get("postGreSQLInstance", {}).get("sslOpt", {}).get("sslKey", "")
+
+    @property
+    def postgres_ssl_cert_file(self):
+        """Returns:str - ssl cert file path"""
+        return self._properties.get("postGreSQLInstance", {}).get("sslOpt", {}).get("sslCert", "")
+
     def change_sa_password(self, value):
         """ Changes postgresql user password
 
             Args:
 
                 value (bool)  -- PostgreSQL password
```

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/saporacleinstance.py` & `cvpysdk-11.32/cvpysdk/instances/saporacleinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/sharepointinstance.py` & `cvpysdk-11.32/cvpysdk/instances/sharepointinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/splunkinstance.py` & `cvpysdk-11.32/cvpysdk/instances/splunkinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/sqlinstance.py` & `cvpysdk-11.32/cvpysdk/instances/sqlinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/sybaseinstance.py` & `cvpysdk-11.32/cvpysdk/instances/sybaseinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/__init__.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/alibaba_cloud.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/alibaba_cloud.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/amazon_web_services.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/amazon_web_services.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/azure.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/azure.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/azure_resource_manager.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/azure_resource_manager.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/azure_stack.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/azure_stack.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/fusioncompute.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/xen.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # --------------------------------------------------------------------------
 
 """File for operating on a Virtual Server Fusion Compute Instance.
 
-FusionComputeInstance is the only class defined in this file.
+XenInstance is the only class defined in this file.
 
-FusionComputeInstance: Derived class from VirtualServer  Base class, representing a
+XenInstance: Derived class from VirtualServer  Base class, representing a
                            Fusion Compute instance, and to perform operations on that instance
 
 HyperVInstance:
 
     __init__(agent_object,instance_name,instance_id)    -- initialize object of FusionCompute
                                                                 Instance object associated with the
                                                                         VirtualServer Instance
@@ -40,43 +40,43 @@
 
 
 """
 
 from ..vsinstance import VirtualServerInstance
 
 
-class FusionComputeInstance(VirtualServerInstance):
+class Xen(VirtualServerInstance):
     """Class for representing an Hyper-V of the Virtual Server agent."""
 
     def __init__(self, agent, instance_name, instance_id=None):
         """Initialize the Instance object for the given Virtual Server instance.
 
             Args:
                 class_object (agent_object,instance_name,instance_id)  --  instance of the
                                                                                 Agent class,
                                                                                 instance name,
                                                                                 instance id
 
         """
-        super(FusionComputeInstance, self).__init__(agent, instance_name, instance_id)
-        self._vendor_id = 14
+        super(Xen, self).__init__(agent, instance_name, instance_id)
+        self._vendor_id = 3
         self._server_name = None
 
     def _get_instance_properties(self):
         """
         Get the properties of this instance
 
         Raise:
             SDK Exception:
                 if response is not empty
                 if response is not success
         """
 
-        super(FusionComputeInstance, self)._get_instance_properties()
-        # waiting for praveen form
+        super(Xen, self)._get_instance_properties()
+        self._server_name = self._instance.get('clientName', '')
 
     def _get_instance_properties_json(self):
         """get the all instance related properties of this subclient.
 
           Returns:
                dict - all instance properties put inside a dict
 
@@ -93,9 +93,16 @@
                 }
             }
         }
         return instance_json
 
     @property
     def server_host_name(self):
-        """return the Fusion compute VRM  associated with the PseudoClient"""
+        """getter for the domain name in the vmware vendor json"""
+        # Till support for instace is provied, enter server name as list and return eg: return ['2.3.4.5']
+        return None
+
+
+    @property
+    def server_name(self):
+        """getter for the domain name in the vmware vendor json"""
         return self._server_name
```

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/google_cloud_platform.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/google_cloud_platform.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/hyperv.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/hyperv.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/kubernetes.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         super(KubernetesInstance, self)._get_instance_properties()
 
         if "vmwareVendor" in self._virtualserverinstance:
             self._vmwarvendor = self._virtualserverinstance['vmwareVendor']['virtualCenter']
 
             self._server_name.append(self._instance['clientName'])
 
-            self._server_host_name.append(self._vmwarvendor["domainName"])
+            self._server_host_name.append(self._vmwarvendor.get("domainName", ''))
 
     def _get_instance_properties_json(self):
         """get the all instance related properties of this subclient.
 
            Returns:
                 dict - all instance properties put inside a dict
```

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/null.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/null.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/nutanix_ahv.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/nutanix_ahv.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/openstack.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/openstack.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/oracle_cloud.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/oracle_cloud.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/oracle_cloud_infrastructure.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/oracle_cloud_infrastructure.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/oraclevm.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/oraclevm.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/red_hat_virtualization.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/red_hat_virtualization.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/vcloud_director.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/vcloud_director.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/vmware.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/vmware.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/virtualserver/xen.py` & `cvpysdk-11.32/cvpysdk/instances/virtualserver/fusioncompute.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # --------------------------------------------------------------------------
 
 """File for operating on a Virtual Server Fusion Compute Instance.
 
-XenInstance is the only class defined in this file.
+FusionComputeInstance is the only class defined in this file.
 
-XenInstance: Derived class from VirtualServer  Base class, representing a
+FusionComputeInstance: Derived class from VirtualServer  Base class, representing a
                            Fusion Compute instance, and to perform operations on that instance
 
 HyperVInstance:
 
     __init__(agent_object,instance_name,instance_id)    -- initialize object of FusionCompute
                                                                 Instance object associated with the
                                                                         VirtualServer Instance
@@ -40,43 +40,51 @@
 
 
 """
 
 from ..vsinstance import VirtualServerInstance
 
 
-class Xen(VirtualServerInstance):
-    """Class for representing an Hyper-V of the Virtual Server agent."""
+class FusionComputeInstance(VirtualServerInstance):
+    """Class for representing a Fusion Compute of the Virtual Server agent."""
 
     def __init__(self, agent, instance_name, instance_id=None):
         """Initialize the Instance object for the given Virtual Server instance.
 
             Args:
                 class_object (agent_object,instance_name,instance_id)  --  instance of the
                                                                                 Agent class,
                                                                                 instance name,
                                                                                 instance id
 
         """
-        super(Xen, self).__init__(agent, instance_name, instance_id)
-        self._vendor_id = 3
-        self._server_name = None
+
+        self._vendor_id = 14
+        self._server_name = []
+        self._vmwarvendor = None
+        self._server_host_name = []
+        super(FusionComputeInstance, self).__init__(agent, instance_name, instance_id)
 
     def _get_instance_properties(self):
         """
         Get the properties of this instance
 
         Raise:
             SDK Exception:
                 if response is not empty
                 if response is not success
         """
 
-        super(Xen, self)._get_instance_properties()
-        self._server_name = self._instance.get('clientName', '')
+        super(FusionComputeInstance, self)._get_instance_properties()
+        if "vmwareVendor" in self._virtualserverinstance:
+            self._vmwarvendor = self._virtualserverinstance['vmwareVendor']['virtualCenter']
+
+            self._server_name.append(self._instance['clientName'])
+
+            self._server_host_name.append(self._vmwarvendor["domainName"])
 
     def _get_instance_properties_json(self):
         """get the all instance related properties of this subclient.
 
           Returns:
                dict - all instance properties put inside a dict
 
@@ -85,24 +93,27 @@
             "instanceProperties": {
                 "isDeleted": False,
                 "instance": self._instance,
                 "instanceActivityControl": self._instanceActivityControl,
                 "virtualServerInstance": {
                     "vsInstanceType": self._virtualserverinstance['vsInstanceType'],
                     "associatedClients": self._virtualserverinstance['associatedClients'],
-                    "vmwareVendor": {}
+                    "vmwareVendor": self._virtualserverinstance['vmwareVendor']
                 }
             }
         }
         return instance_json
 
     @property
     def server_host_name(self):
-        """getter for the domain name in the vmware vendor json"""
-        # Till support for instace is provied, enter server name as list and return eg: return ['2.3.4.5']
-        return None
-
+        """return the Fusion compute VRM  associated with the PseudoClient"""
+        return self._server_host_name
 
     @property
     def server_name(self):
         """getter for the domain name in the vmware vendor json"""
         return self._server_name
+
+    @property
+    def _user_name(self):
+        """getter for the username from the vmware vendor json"""
+        return self._vmwarvendor.get("userName", "")
```

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/vminstance.py` & `cvpysdk-11.32/cvpysdk/instances/vminstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/instances/vsinstance.py` & `cvpysdk-11.32/cvpysdk/instances/vsinstance.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,17 @@
                     instance_proxies   (List)  --  returns the proxies list
         """
         instance_members = self.associated_clients
         instance_proxies = []
         for member in instance_members:
             if self._commcell_object.client_groups.has_clientgroup(member):
                 client_group = self._commcell_object.client_groups.get(member)
-                instance_proxies.extend(client_group.associated_clients)
+                clients_obj = self._commcell_object.clients
+                instance_proxies.extend(list(set(clients_obj.virtualization_access_nodes).intersection(
+                    set(clients.lower() for clients in client_group.associated_clients))))
             else:
                 instance_proxies.append(member)
 
         return list(dict.fromkeys(instance_proxies))
 
     @property
     def server_name(self):
```

### Comparing `cvpysdk-11.30.1/cvpysdk/internetoptions.py` & `cvpysdk-11.32/cvpysdk/internetoptions.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/job.py` & `cvpysdk-11.32/cvpysdk/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,14 +484,16 @@
                                     percent_complete = job_summary['percentComplete']
                                     backup_level = job_summary.get('backupLevelName')
 
                                     app_type = ''
                                     job_type = ''
                                     pending_reason = ''
                                     subclient_id = ''
+                                    client_id = ''
+                                    client_name = ''
                                     job_elapsed_time = 0
                                     job_start_time = 0
 
                                     if 'jobElapsedTime' in job_summary:
                                         job_elapsed_time = job_summary['jobElapsedTime']
 
                                     if 'jobStartTime' in job_summary:
@@ -506,22 +508,28 @@
                                     if 'pendingReason' in job_summary:
                                         pending_reason = job_summary['pendingReason']
 
                                     if 'subclient' in job_summary:
                                         job_subclient = job_summary['subclient']
                                         if 'subclientId' in job_subclient:
                                             subclient_id = job_subclient['subclientId']
+                                        if 'clientId' in job_subclient:
+                                            client_id = job_subclient['clientId']
+                                        if 'clientName' in job_subclient:
+                                            client_name = job_subclient['clientName']
 
                                     jobs_dict[job_id] = {
                                         'operation': operation,
                                         'status': status,
                                         'app_type': app_type,
                                         'job_type': job_type,
                                         'percent_complete': percent_complete,
                                         'pending_reason': pending_reason,
+                                        'client_id': client_id,
+                                        'client_name': client_name,
                                         'subclient_id': subclient_id,
                                         'backup_level': backup_level,
                                         'job_start_time': job_start_time,
                                         'job_elapsed_time': job_elapsed_time
 
                                     }
 
@@ -2036,15 +2044,15 @@
         while attempts < 5:  # Retrying to ignore the transient case when no jobs are found
             flag, response = self._cvpysdk_object.make_request('GET', self._JOB)
             attempts += 1
 
             if flag:
                 if response.json():
                     if response.json().get('totalRecordsWithoutPaging', 0) == 0:
-                        time.sleep(3)
+                        time.sleep(2**attempts)
                         continue
 
                     if 'jobs' in response.json():
                         for job in response.json()['jobs']:
                             return job['jobSummary']
                 else:
                     if attempts > 4:
```

### Comparing `cvpysdk-11.30.1/cvpysdk/license.py` & `cvpysdk-11.32/cvpysdk/license.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/metallic.py` & `cvpysdk-11.32/cvpysdk/metallic.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/metricsreport.py` & `cvpysdk-11.32/cvpysdk/metricsreport.py`

 * *Files 3% similar despite different names*

```diff
@@ -649,7 +649,42 @@
                       '-si CommservSurveyRandomizationEnabled -si y -si {0}'.format(minutes))
 
         flag, response = self._commcell_object._cvpysdk_object.make_request(
             'POST', qcommand, qoperation
         )
         if not flag:
             raise SDKException('Response', '101', response.text)
+
+
+class LocalMetrics:
+    """class for operation in localmetrics"""
+
+    def __init__(self, commcell_object, islocalmetrics= True):
+        self._commcell_object = commcell_object
+        self._islocalmetrics = islocalmetrics
+        self._LOCAL_METRICS = self._commcell_object._services['LOCAL_METRICS'] % self._islocalmetrics
+        self._get_metrics_config()
+
+    def _get_metrics_config(self):
+        flag, response = self._commcell_object._cvpysdk_object.make_request(
+            'GET', self._LOCAL_METRICS
+        )
+        if flag:
+            self._metrics_config = response.json()
+            config_value = self._metrics_config['config']
+            return config_value
+        else:
+            raise SDKException('Response', '101', response.text)
+
+    def refresh(self):
+        """updates metrics object with the latest configuration"""
+        self._get_metrics_config()
+
+    @property
+    def last_upload_time(self):
+        """ get last upload time"""
+        return self._metrics_config['config']['lastCollectionTime']
+
+    @property
+    def nextup_load_time(self):
+        """get the next upload time"""
+        return self._metrics_config['config']['nextUploadTime']
```

### Comparing `cvpysdk-11.30.1/cvpysdk/monitoring.py` & `cvpysdk-11.32/cvpysdk/monitoring.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/name_change.py` & `cvpysdk-11.32/cvpysdk/name_change.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/network.py` & `cvpysdk-11.32/cvpysdk/network.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/network_throttle.py` & `cvpysdk-11.32/cvpysdk/network_throttle.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/network_topology.py` & `cvpysdk-11.32/cvpysdk/network_topology.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/operation_window.py` & `cvpysdk-11.32/cvpysdk/operation_window.py`

 * *Files 14% similar despite different names*

```diff
@@ -105,14 +105,16 @@
         client_operation_window_details = OperationWindowDetails(client, ruleId, client_operation_window.entity_details)
         # You can use get(OperationWindow) method to modify a rule too.
         client_operation_window_details.modify_operation_window(name="Modified operation window example on clientLevel")
 """
 
 from __future__ import absolute_import
 import time
+import datetime
+import calendar
 from datetime import timedelta
 from .exception import SDKException
 from .clientgroup import ClientGroup
 from .client import Client
 from .agent import Agent
 from .instance import Instance
 from .backupset import Backupset
@@ -297,18 +299,40 @@
                         sunday/ monday/ tuesday/ wednesday/ thursday/ friday/ saturday
 
                     default- Weekdays
 
                 start_time  (int)     -- The start time for the "do not run" interval.
                     Valid values are UNIX-style timestamps (seconds since January 1, 1970).
                     default - 28800 (8 AM)
+                    Must specify one timestamp for start time for all the weekdays, otherwise
+                    make a list for each weekday mentioned in the day_of_week list.
+
+                start_time (list)    -- The list of start timestamps for each weekday mentioned
+                    in the day_of_week list.
 
                 end_time    (int)     -- The end time for the "do not run" interval.
                     Valid values are UNIX-style timestamps (seconds since January 1, 1970).
                     default - 86400 (6 PM)
+                    Must specify one timestamp for end time for all the weekdays, otherwise
+                    make a list for each weekday mentioned in the day_of_week list.
+
+                end_time   (list)    -- The list of end timestamps for each weekday mentioned
+                    in the day_of_week list.
+
+                Example:
+                    1. day_of_week : ["sunday", "thursday", "saturday"]
+                       start_time  : 28800
+                       end_time    : 86400
+                       The above inputs specify that for all the three days mentioned, start_time and end_time of
+                       operation window would be same
+                    2. day_of_week : ["monday","friday"]
+                       start_time  : [3600, 28800]
+                       end_time    : [18000, 86400]
+                       The above input specify that on monday operation window starts at 3600 and ends at 18000 whereas
+                       on friday, the operation window starts at 28800 and ends at 86400
 
                 do_not_submit_job   (bool) -- doNotSubmitJob of the operation rule
 
             Returns:
                 Returns the instance of created Operation window details
 
             Raises:
@@ -316,19 +340,18 @@
                     if the Operation window could not be created
 
                     if response is empty
 
                     if response is not success
 
         """
-
         if start_date is None:
-            start_date = int(time.time())
+            start_date = int(calendar.timegm(datetime.date.today().timetuple()))
         if end_date is None:
-            end_date = int(time.time()) + int(timedelta(days=365).total_seconds())
+            end_date = start_date
         if start_time is None:
             start_time = int(timedelta(hours=8).total_seconds())
         if end_time is None:
             end_time = int(timedelta(hours=18).total_seconds())
 
         operations_list = []
         if operations is None:
@@ -354,28 +377,51 @@
         if week_of_the_month:
             for week in week_of_the_month:
                 if week.lower() not in WEEK_OF_THE_MONTH_MAPPING:
                     response_string = "Invalid input %s for week_of_the_month" % week
                     raise SDKException('OperationWindow', '102', response_string)
                 week_of_the_month_list.append(WEEK_OF_THE_MONTH_MAPPING[week.lower()])
 
+        daytime_list = []
+        num_of_days = len(day_of_week_list)
+        if isinstance(start_time, int) and isinstance(end_time, int):
+            daytime_list.append(
+                {
+                    "startTime": start_time,
+                    "endTime": end_time,
+                    "weekOfTheMonth": week_of_the_month_list,
+                    "dayOfWeek": day_of_week_list
+                }
+            )
+        elif isinstance(start_time, list) and isinstance(end_time, list):
+            if not(num_of_days == len(start_time) == len(end_time)):
+                response_string = "did not specify start time and end time for all the given week days"
+                raise SDKException('OperationWindow', '102', response_string)
+            for week_day in range(num_of_days):
+                daytime_list.append(
+                    {
+                        "startTime": start_time[week_day],
+                        "endTime": end_time[week_day],
+                        "weekOfTheMonth": week_of_the_month_list,
+                        "dayOfWeek": [day_of_week_list[week_day]]
+                    }
+                )
+        else:
+            response_string = "Both start_time and end_time should be of same type."
+            raise SDKException('OperationWindow', '102', response_string)
+
         payload = {
             "operationWindow": {
                 "ruleEnabled": True,
                 "doNotSubmitJob": do_not_submit_job,
                 "startDate": start_date,
                 "endDate": end_date,
                 "name": name,
                 "operations": operations_list,
-                "dayTime": [{
-                    "startTime": start_time,
-                    "endTime": end_time,
-                    "weekOfTheMonth": week_of_the_month_list,
-                    "dayOfWeek": day_of_week_list
-                }]
+                "dayTime": daytime_list
             },
             "entity": {
                 "clientGroupId": int(self.clientgroup_id),
                 "clientId": int(self.client_id),
                 "applicationId": int(self.agent_id),
                 "instanceId": int(self.instance_id),
                 "backupsetId": int(self.backupset_id),
@@ -480,25 +526,25 @@
                 if int(error_code) == 0:
                     list_of_rules = response.json().get("operationWindow")
                     operation_reverse_mapping = {value: key for key, value in OPERATION_MAPPING.items()}
                     wotm_reverse_mapping = {value: key for key, value in WEEK_OF_THE_MONTH_MAPPING.items()}
                     if list_of_rules is not None:
                         for operation_rule in list_of_rules:
                             operations = operation_rule.get("operations")
-                            week_of_the_month = operation_rule.get("dayTime", [{}])[0].get("weekOfTheMonth")
-                            day_of_week = operation_rule.get("dayTime", [{}])[0].get("dayOfWeek")
                             if operations is not None:
                                 operation_rule["operations"] = [operation_reverse_mapping[operation] for operation in
                                                                 operations]
-                            if week_of_the_month is not None:
-                                operation_rule["dayTime"][0]["weekOfTheMonth"] = [wotm_reverse_mapping[week] for week in
-                                                                                  week_of_the_month]
-                            if day_of_week is not None:
-                                operation_rule["dayTime"][0]["dayOfWeek"] = [DAY_OF_WEEK_MAPPING[day] for day in
-                                                                             day_of_week]
+                            day_time_list = operation_rule.get("dayTime", [])
+                            for day_time in day_time_list:
+                                if day_time.get("weekOfTheMonth"): # if we have weekOfTheMonth, we replace it with name.
+                                    day_time['weekOfTheMonth'] = [wotm_reverse_mapping[week] for week in day_time.get("weekOfTheMonth")]
+
+                                if day_time.get("dayTime"): # if we have dayTime, we replace it with name.
+                                    day_time['dayTime'] = [DAY_OF_WEEK_MAPPING[day] for day in day_time['dayTime']]
+                            operation_rule['dayTime'] = day_time_list
                     return list_of_rules
                 raise SDKException('OperationWindow', '104')
             raise SDKException('Response', '102')
         response_string = self._update_response(response.text)
         raise SDKException('Response', '102', response_string)
 
     def get(self, rule_id=None, name=None):
@@ -633,20 +679,42 @@
                     day_of_week (list)    -- List of days of the week on which the operation rule applies to
                         Acceptable Values:
                             sunday/ monday/ tuesday/ wednesday/ thursday/ friday/ saturday
 
                         default- Weekdays
 
                     start_time  (int)     -- The start time for the "do not run" interval.
-                        Valid values are UNIX-style timestamps (seconds since January 1, 1970).
-                        default - 28800 (8 AM)
+                    Valid values are UNIX-style timestamps (seconds since January 1, 1970).
+                    default - 28800 (8 AM)
+                    Must specify one timestamp for start time for all the weekdays, otherwise
+                    make a list for each weekday mentioned in the day_of_week list.
 
-                    end_time    (int)     -- The end time for the "do not run" interval.
-                        Valid values are UNIX-style timestamps (seconds since January 1, 1970).
-                        default - 86400 (6 PM)
+                start_time (list)    -- The list of start timestamps for each weekday mentioned
+                    in the day_of_week list.
+
+                end_time    (int)     -- The end time for the "do not run" interval.
+                    Valid values are UNIX-style timestamps (seconds since January 1, 1970).
+                    default - 86400 (6 PM)
+                    Must specify one timestamp for end time for all the weekdays, otherwise
+                    make a list for each weekday mentioned in the day_of_week list.
+
+                end_time   (list)    -- The list of end timestamps for each weekday mentioned
+                    in the day_of_week list.
+
+                Example:
+                    1. day_of_week : ["sunday", "thursday", "saturday"]
+                       start_time  : 28800
+                       end_time    : 86400
+                       The above inputs specify that for all the three days mentioned, start_time and end_time of
+                       operation window would be same
+                    2. day_of_week : ["monday","friday"]
+                       start_time  : [3600, 28800]
+                       end_time    : [18000, 86400]
+                       The above input specify that on monday operation window starts at 3600 and ends at 18000 whereas
+                       on friday, the operation window starts at 28800 and ends at 86400
 
                     do_not_submit_job   (bool)  -- doNotSubmitJob of the operation rule
 
             Raises:
                 SDKException:
                     if the Operation window could not be Modified
 
@@ -673,30 +741,51 @@
             operations_list = [OPERATION_MAPPING[operation.upper()] for operation in operations]
 
         week_of_the_month_list = []
         if week_of_the_month:
             week_of_the_month_list = [WEEK_OF_THE_MONTH_MAPPING[week.lower()] for week in week_of_the_month]
 
         day_of_week_list = [DAY_OF_WEEK_MAPPING.index(day.lower()) for day in day_of_week]
-
+        daytime_list = []
+        num_of_days = len(day_of_week_list)
+        if isinstance(start_time, int) and isinstance(end_time, int):
+            daytime_list.append(
+                {
+                    "startTime": start_time,
+                    "endTime": end_time,
+                    "weekOfTheMonth": week_of_the_month_list,
+                    "dayOfWeek": day_of_week_list
+                }
+            )
+        elif isinstance(start_time, list) and isinstance(end_time, list):
+            if not (num_of_days == len(start_time) == len(end_time)):
+                response_string = "did not specify start time and end time for all the given week days"
+                raise SDKException('OperationWindow', '102', response_string)
+            for week_day in range(num_of_days):
+                daytime_list.append(
+                    {
+                        "startTime": start_time[week_day],
+                        "endTime": end_time[week_day],
+                        "weekOfTheMonth": week_of_the_month_list,
+                        "dayOfWeek": [day_of_week_list[week_day]]
+                    }
+                )
+        else:
+            response_string = "Both start_time and end_time should be of same type."
+            raise SDKException('OperationWindow', '102', response_string)
         payload = {
             "operationWindow": {
                 "ruleEnabled": True,
                 "doNotSubmitJob": do_not_submit_job,
                 "startDate": start_date,
                 "endDate": end_date,
                 "name": name,
                 "ruleId": int(self.rule_id),
                 "operations": operations_list,
-                "dayTime": [{
-                    "startTime": start_time,
-                    "endTime": end_time,
-                    "weekOfTheMonth": week_of_the_month_list,
-                    "dayOfWeek": day_of_week_list
-                }]
+                "dayTime": daytime_list
             },
             "entity": {
                 "clientGroupId": int(self._clientgroup_id),
                 "clientId": int(self._client_id),
                 "applicationId": int(self._agent_id),
                 "instanceId": int(self._instance_id),
                 "backupsetId": int(self._backupset_id),
@@ -736,21 +825,35 @@
                 self._do_not_submit_job = response_json.get('doNotSubmitJob')
                 self._name = response_json.get('name')
                 self._start_date = response_json.get('startDate')
                 self._end_date = response_json.get('endDate')
                 operations = response_json.get('operations')
                 operation_reverse_mapping = {value: key for key, value in OPERATION_MAPPING.items()}
                 self._operations = [operation_reverse_mapping[operation] for operation in operations]
-                week_of_the_month = response_json.get("dayTime", [{}])[0].get("weekOfTheMonth", [])
+                week_of_the_month = response_json.get("dayTime")[0].get('weekOfTheMonth', [])
+                if len(response_json.get("dayTime", [])) == 1:
+                    start_time = response_json.get("dayTime")[0]['startTime']
+                    end_time = response_json.get("dayTime")[0]['endTime']
+                    day_of_week = response_json.get("dayTime")[0]['dayOfWeek']
+                else:
+                    day_of_week = []
+                    start_time = []
+                    end_time = []
+                    for week_day in response_json.get("dayTime", []):
+                        if week_day.get("dayOfWeek"):
+                            day_of_week.append(week_day.get("dayOfWeek")[0])
+                        if week_day.get("startTime") is not None:
+                            start_time.append(week_day.get("startTime"))
+                        if week_day.get("endTime") is not None:
+                            end_time.append(week_day.get("endTime"))
                 wotm_reverse_mapping = {value: key for key, value in WEEK_OF_THE_MONTH_MAPPING.items()}
                 self._week_of_the_month = [wotm_reverse_mapping[week] for week in week_of_the_month]
-                day_of_week = response_json.get('dayTime', [{}])[0].get('dayOfWeek')
                 self._day_of_week = [DAY_OF_WEEK_MAPPING[day] for day in day_of_week]
-                self._start_time = response_json.get('dayTime', [{}])[0].get('startTime')
-                self._end_time = response_json.get('dayTime', [{}])[0].get('endTime')
+                self._start_time = start_time
+                self._end_time = end_time
             else:
                 raise SDKException('OperationWindow', '102',
                                    response_json.get("error", {}).get('errorMessage'))
         else:
             raise SDKException('Response', '102')
 
     @property
@@ -877,30 +980,34 @@
     @start_time.setter
     def start_time(self, start_time):
         """
         Modifies the start_time of the operation rule
         Args:
             start_time: (int)     -- The start time for the "do not run" interval.
                     Valid values are UNIX-style timestamps (seconds since January 1, 1970).
+                        (list)    -- The list of start timestamps for each weekday mentioned
+                    in the day_of_week list.
         Returns: None
         """
         self.modify_operation_window(start_time=start_time)
 
     @property
     def end_time(self):
         """Treats end_time as a read-only attribute."""
         return self._end_time
 
     @end_time.setter
     def end_time(self, end_time):
         """
         Modifies the end_time of the operation rule
         Args:
-            end_time: -- The end time for the "do not run" interval.
+            end_time: (int)     -- The end time for the "do not run" interval.
                     Valid values are UNIX-style timestamps (seconds since January 1, 1970).
+                      (list)    -- The list of end timestamps for each weekday mentioned
+                    in the day_of_week list.
         Returns: None
         """
         self.modify_operation_window(end_time=end_time)
 
     @property
     def rule_id(self):
         """Treats rule_id as read-only attribute"""
```

### Comparing `cvpysdk-11.30.1/cvpysdk/organization.py` & `cvpysdk-11.32/cvpysdk/organization.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,14 +36,24 @@
 
     #. Update the default plan of the organization
 
     #. Enabling Operator role for a user
 
     #. Disabling Operator role for a user
 
+This module now also supports remote operations added as part of Ring Routing project
+
+    #. Enable fanout to view all organizations from associated service commcells
+
+    #. Add new organization remotely to a service commcell
+
+    #. Delete an organization in service commcell remotely
+
+    #. Manage operators, tags of the organization remotely
+
 Organizations
 =============
 
     __init__(commcell_object)   --  initializes object of the Organizations class associated
     with the commcell
 
     __str__()                   --  returns all the organizations associated with the commcell
@@ -53,33 +63,41 @@
     __len__()                   --  returns the number of organizations configured on the Commcell
 
     __getitem__()               --  returns the name of the organization for the organization Id
     or the details for the given organization name
 
     _get_organizations()        --  returns all organizations added to the commcell
 
+    _get_headers()              --  returns headers required for remote operations
+
     has_organization()          --  checks whether the organization with given name exists or not
 
     add()                       --  adds a new organization to the commcell
 
+    add_remote_org()            --  adds a new organization to given service commcell
+
     get()                       --  returns Organization class object for the specified input name
 
-    delete()                    --  deletes an organization from the commcell
+    get_remote_org()            --  returns RemoteOrganization class object for given input
+
+    delete()                    --  deletes an organization from the commcell or service commcell
 
     dissociate_plans()          -- disassociates plans from the organization
 
-    refresh()                   --  refresh the list of organizations associated with the commcell
+    refresh()                   --  refresh the list of organizations in given commcell and/or service commcells
 
 Organizations Attributes
 ------------------------
 
     **all_organizations**   --  returns the dict consisting of organizations and their details
 
     **all_organizations_props** -- returns the dict consisting of organizations and their guid's
 
+    **fanout**              --  determines if remote operations will be performed, returns current fanout set
+
 
 Organization
 ============
 
     __init__()                  --  initializes instance of the Organization class for doing
     operations on the selected Organization
 
@@ -236,22 +254,73 @@
         **isAllowUserstoEnablePasskeyEnabled** -- Returns True - If users have rights to enable passkey
 
         **is_company_privacy_enabled**         -- Returns True if the privacy is enabled for organization
 
         **is_owner_data_privacy_enabled**      -- Returns True if the privacy is enabled for owner of client in
         organization
 
+        **company_theme**           --  Returns the company level theme if it exists
+
+RemoteOrganization
+============
+
+    __init__()                  --  initializes instance of the RemoteOrganization class for doing
+    remote operations on the selected Organization
+
+    __repr__()                  --  returns the string representation of an instance of this class
+
+    _get_organization_id()      --  gets the local ID of the RemoteOrganization
+
+    _get_properties()           --  get the properties of the organization by fanout
+
+    refresh()                   --  refresh the properties of the organization
+
+    activate()                  --  To activate the organization
+
+    deactivate()                --  To deactivate the organization
+    
+    get_entity_counts()         --  To get the counts of associated entities for company
+
+
+Organization Attributes
+-----------------------
+
+    Following attributes are available for an instance of the RemoteOrganization class:
+
+        **organization_id**         --  returns the local id of the organization
+
+        **organization_name**       --  returns the name of the organization
+
+        **homecell**                --  returns the commserve name of the service commcell of this org
+
+        **organization_name**       --  returns the name of the organization
+
+        **domain_name**             --  returns the primary domain associated with the organization (alias)
+
+         **reseller_enabled**       -- returns if reseller is enabled or not
+
+        **is_backup_disabled**       -- returns the backup activity status for the Organization
+
+        **is_restore_disabled**      -- returns the restore activity status for the Organization
+
+        **is_login_disabled**        -- returns the Login activity status for the Organization
+
+        **tags**                    -- Returns Tags associated with Organisation
+
+        **operators**               -- Returns Operators associated with this Organization
+
 """
 
 import re
+import json
 
 from datetime import datetime
 
 from .exception import SDKException
-
+from .constants import ENTITY_TYPE_MAP
 from .security.user import User
 from .security.usergroup import UserGroup
 from .security.two_factor_authentication import TwoFactorAuthentication
 
 from base64 import b64encode
 
 
@@ -272,14 +341,15 @@
 
         self._cvpysdk_object = commcell_object._cvpysdk_object
         self._services = commcell_object._services
         self._update_response_ = commcell_object._update_response_
 
         self._organizations_api = self._services['ORGANIZATIONS']
         self._organizations = None
+        self._fanout = False
 
         self.refresh()
 
     def __str__(self):
         """Representation string consisting of all organizations present in the Commcell.
 
             Returns:
@@ -347,27 +417,32 @@
             Raises:
                 SDKException:
                     if response is empty
 
                     if response is not success
 
         """
-        flag, response = self._cvpysdk_object.make_request('GET', self._organizations_api)
-
+        flag, response = self._cvpysdk_object.make_request('GET', self._organizations_api, headers=self._get_headers())
         if flag:
             organizations = {}
             self._adv_config = {}
             if response.json() and 'providers' in response.json():
                 for provider in response.json()['providers']:
+                    if self._fanout and "idpCompanyDetails" in provider:
+                        continue # to avoid dummy companies
                     name = provider['connectName'].lower()
                     organization_id = provider['shortName']['id']
                     organization_guid = provider['providerGUID']
+                    cloud_service_organizations = provider.get("organizationCloudServiceDetails", [{}])[0].\
+                        get("cloudService", {}).get('redirectUrl')
                     organizations[name] = organization_id
                     self._adv_config[name] = {
-                        'GUID': organization_guid
+                        'GUID': organization_guid,
+                        'redirect_url': cloud_service_organizations,
+                        'home_commcell':provider.get('commcell',{}).get('commCellName'),
                     }
 
             self._get_associated_entities_count()
 
             return organizations
         response_string = self._update_response_(response.text)
         raise SDKException('Response', '101', response_string)
@@ -388,33 +463,51 @@
                 SDKException:
                     if response is empty
 
                     if response is not success
 
         """
         flag, response = self._cvpysdk_object.make_request(
-            'GET', self._organizations_api+"?Fl=providers.associatedEntitiesCount,providers.shortName,providers.connectName")
+            'GET',
+            f"{self._organizations_api}?Fl=providers.associatedEntitiesCount,providers.shortName,providers.connectName",
+            headers = self._get_headers()
+        )
 
         if flag:
             if response.json() and 'providers' in response.json():
                 for provider in response.json().get('providers'):
                     name = provider.get('connectName').lower()
                     organization_entites_count = provider.get('associatedEntitiesCount')
                     if name:
-                        self._adv_config[name] = {
-                            'count': organization_entites_count
-                        }
+                        if name in self._adv_config.keys():
+                            self._adv_config[name].update({'count': organization_entites_count})
 
                 return
             else:
                 raise SDKException('Response', '102')
         else:
             response_string = self._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
 
+    def _get_headers(self, target:str=None):
+        """
+        Returns fanout headers if fanout is set
+
+        Args:
+            target (str) -- target service commserve name (if applicable)
+        """
+        if not self._fanout:
+            return None
+        headers = self._commcell_object._headers.copy()
+        headers['CVContext']='Comet'
+        if target:
+            headers['_cn'] = target
+            headers['Comet-Commcells'] = target
+        return headers
+
     @property
     def all_organizations(self):
         """Returns the dictionary consisting of all the organizations and their info.
 
             dict - consists of all the organizations configured on the commcell
 
                 {
@@ -424,33 +517,58 @@
                 }
 
         """
         return self._organizations
 
     @property
     def all_organizations_props(self):
-        """Returns the dictionary consisting of all the organizations guid info.
+        """Returns the dictionary consisting of all the organizations guid info and redirect URL if present.
 
-            dict - consists of all the organizations configured on the commcell
+            dict - consists of all the organizations configured on the commcell and/or service commcells
 
                 {
                     "organization1_name":
                      {
-                     GUID : "49DADF71-247E-4D59-8BD8-CF7BFDF7DB28"
+                     GUID : "49DADF71-247E-4D59-8BD8-CF7BFDF7DB28",
+                     redirect_url: "<Webconsole url>",
+                     home_commcell: "<commserve name>",
+                     count: 11
                      },
 
                     "organization2_name":
                     {
-                    GUID : "49DADF71-247E-4D59-8BD8-CF7BFDF7DB27"
+                    GUID : "49DADF71-247E-4D59-8BD8-CF7BFDF7DB27",
+                    redirect_url: None,
+                    home_commcell: "<commserve name>",
+                    count: 8
                     }
                 }
 
         """
         return self._adv_config
 
+    @property
+    def fanout(self)->bool:
+        """Returns status of fanout headers are enabled or not
+        Returns:
+            bool    -   True/False
+        """
+        return self._fanout
+
+    @fanout.setter
+    def fanout(self, value:bool=True):
+        """
+        Sets if fanout is required or not
+        
+        Args:
+            value (bool) -- False if fanout not required
+        """
+        self._fanout = value
+        self.refresh()
+
     def has_organization(self, name):
         """Checks if an organization exists in the Commcell with the input organization name.
 
             Args:
                 name    (str)   --  name of the organization
 
             Returns:
@@ -462,14 +580,177 @@
 
         """
         if not isinstance(name, str):
             raise SDKException('Organization', '101')
 
         return self._organizations and name.lower() in self._organizations
 
+    def add_remote_org(self,
+            name,
+            email,
+            contact_name,
+            company_alias,
+            **options):
+        """Adds a new organization with the given name to the Commcell.
+
+            Args:
+                name            (str)   --  name of the organization to create
+
+                email           (str)   --  email of the primary contact
+
+                contact_name    (str)   --  name of the primary contact
+
+                company_alias   (str)   --  alias of the company
+
+                email_domain    (list)  --  list of email domains supported for the organization
+
+                    if no value is given, domain of the user creating the organization will be used
+
+                    default: None
+
+                primary_domain  (str)   --  custom primary domain for organization
+
+                    default: None
+
+                default_plans   (list)  --  list of default plans to be associated with the
+                organization
+
+                    default: None
+
+                send_email      (bool) --  If set to true, a welcome email is sent to the
+                primary contact user.
+
+                    default: False
+
+                target          (str)   --  service commcell name where to add organization
+                    
+                    default: current commcell
+
+            Returns:
+                object  -   instance of the RemoteOrganization class
+
+            Raises:
+                SDKException:
+                    if organization with the given name already exists
+
+                    if inputs are not valid
+
+                    if failed to create the organization remotely
+
+                    if response is empty
+
+                    if response is not success
+
+        """
+        if not self._fanout:
+            raise Exception('Enable fanout property to perform remote operations')
+        if self.has_organization(name):
+            raise SDKException('RemoteOrganization', '108')
+
+        if not (isinstance(name, str) and
+                isinstance(email, str) and
+                isinstance(contact_name, str) and
+                isinstance(company_alias, str)):
+            raise SDKException('RemoteOrganization', '105')
+
+        if not re.match(r'[^@]+@[^@]+\.[^@]+', email):
+            raise SDKException('RemoteOrganization', '107')
+
+        email_domain=options.get('email_domain')
+        primary_domain=options.get('primary_domain')
+        default_plans=options.get('default_plans')
+        enable_auto_discover=options.get('enable_auto_discover',False)
+        send_email=options.get('send_email',False)
+        target=options.get('target')
+
+        if email_domain is None:
+            email_domain = [email.split('@')[1]]
+
+        if primary_domain is None:
+            primary_domain = ''
+
+        plans_list = []
+
+        if default_plans:
+            if not isinstance(default_plans, list):
+                raise SDKException('RemoteOrganization', '105')
+            else:
+                for plan in default_plans:
+                    if not self._commcell_object.plans.has_plan(plan):
+                        raise SDKException(
+                            'RemoteOrganization',
+                            '106',
+                            'Plan: "{0}" does not exist on Commcell'.format(plan)
+                        )
+                    else:
+                        temp_plan = self._commcell_object.plans.get(plan)
+                        temp = {
+                            'plan': {
+                                'planId': int(temp_plan.plan_id)
+                            }
+                        }
+                        plans_list.append(temp)
+
+                        del temp
+                        del temp_plan
+
+        request_json = {
+            'organizationInfo': {
+                'organization': {
+                    'connectName': name,
+                    'emailDomainNames': email_domain,
+                    'shortName': {
+                        'domainName': company_alias
+                    }
+                },
+                'organizationProperties': {
+                    'enableAutoDiscovery': enable_auto_discover,
+                    'primaryDomain': primary_domain,
+                    'primaryContacts': [
+                        {
+                            'fullName': contact_name,
+                            'email': email
+                        }
+                    ],
+                },
+                'planDetails': plans_list
+            }
+        }
+
+        send_email and request_json.update({'sendEmail': send_email})
+
+        if target is None:
+            target = self._commcell_object.commserv_name
+        __, response = self._cvpysdk_object.make_request(
+            'POST', self._organizations_api, request_json, headers=self._get_headers(target)
+        )
+
+        self.refresh()
+
+        if response.json():
+            if 'response' in response.json():
+                error_code = response.json()['response']['errorCode']
+
+                if error_code == 0:
+                    return self.get_remote_org(name)
+
+                raise SDKException(
+                    'RemoteOrganization', '109', 'Response: {0}'.format(response.json())
+                )
+
+            elif 'errorMessage' in response.json():
+                raise SDKException(
+                    'RemoteOrganization', '109', 'Error: "{0}"'.format(response.json()['errorMessage'])
+                )
+
+            else:
+                raise SDKException('RemoteOrganization', '109', 'Response: {0}'.format(response.json()))
+        else:
+            raise SDKException('Response', '102')
+
     def add(self,
             name,
             email,
             contact_name,
             company_alias,
             email_domain=None,
             primary_domain=None,
@@ -653,14 +934,46 @@
 
         name = name.lower()
 
         if self.has_organization(name):
             return Organization(self._commcell_object, name, self._organizations[name])
         raise SDKException('Organization', '103')
 
+    def get_remote_org(self, name):
+        """Returns an instance of the RemoteOrganization class for the given organization name.
+
+            Args:
+                name    (str)   --  name of the remote organization to get the instance of
+
+            Returns:
+                object  -   instance of the RemoteOrganization class for the given organization name
+
+            Raises:
+                SDKException:
+                    if type of the organization name argument is not string
+
+                    if no organization exists with the given name
+
+        """
+        if not self._fanout:
+            raise Exception('Enable fanout property to perform remote operations')
+        if not isinstance(name, str):
+            raise SDKException('RemoteOrganization', '105')
+
+        name = name.lower()
+
+        if self.has_organization(name):
+            return RemoteOrganization(
+                self._commcell_object,
+                name,
+                self._organizations[name],
+                self._adv_config[name]['home_commcell']
+            )
+        raise SDKException('RemoteOrganization', '110')
+
     def delete(self, name):
         """Deletes the organization with the given name from the Commcell.
 
             Args:
                 name            (str)   --  name of the organization to delete
 
             Returns:
@@ -676,20 +989,27 @@
 
                     if response is not success
 
         """
         if not self.has_organization(name):
             raise SDKException('Organization', '103')
 
-        self.get(name).deactivate()
+        if self._fanout:
+            org = self.get_remote_org(name)
+            target = org.homecell
+        else:
+            org = self.get(name)
+            target = None
+            
+        org.deactivate()
 
         organization_id = self._organizations[name.lower()]
 
         flag, response = self._cvpysdk_object.make_request(
-            'DELETE', self._services['ORGANIZATION'] % organization_id
+            'DELETE', self._services['ORGANIZATION'] % organization_id, headers=self._get_headers(target)
         )
 
         self.refresh()
 
         if flag:
             if response.json():
                 error_message = response.json()['errorMessage']
@@ -750,14 +1070,15 @@
         self._machine_count = None
         self._user_count = None
         self._default_plan = []
         self._contacts = {}
         self._plans = {}
         self._organization_info = None
         self._operator_role = None
+        self._operators = None
         self._plan_details = None
         self._server_count = None
         self._user_groups = None
         self._sender_email = None
         self._sender_name = None
         self._supported_solutions = None
         self._org_creation_time = None
@@ -990,24 +1311,26 @@
                 for plan in organization_properties.get('defaultPlans', []):
                     self._default_plan.append(plan['plan']['planName'])
 
                 for plan in self._organization_info.get('planDetails', []):
                     self._plans[plan['plan']['planName'].lower()] = plan['plan']['planId']
 
                 self._operator_role = organization_properties['operatorRole']['roleName']
+                self._operators = organization_properties.get("operators", [])
 
                 if self._organization_info.get('planDetails', []):
                     self._plan_details = self._organization_info['planDetails']
 
                 self._server_count = organization_properties['serverCount']
 
                 for file_filter in organization_properties['globalFiltersInfo']['globalFiltersInfoList']:
                     os_type_map = {1: 'Windows', 2: 'Unix'}
                     self._file_exceptions[os_type_map[file_filter['operatingSystemType']]] = \
                         file_filter['globalFilters'].get('filters', [])
+                self._theme = json.loads(organization_properties.get('customization', '{}'))
 
                 return self._organization_info
             else:
                 raise SDKException('Response', '102')
         else:
             response_string = self._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
@@ -1407,14 +1730,109 @@
             "primaryContacts": user_list
         }
 
         self._update_properties_json(req_json)
         self._update_properties()
 
     @property
+    def operators(self) -> list:
+        """
+        Returns the list of operators and roles associated to this organization
+
+        Returns:
+            list    -   list of dicts containing operator details
+
+        Example:
+            [
+                {
+                    'role': {name:'<name of role>', id:<role id>},
+                    'userGroup': {userGroupName:'<usergroupname>', userGroupId:<id>}
+                },
+                {
+                    'role':{name:'<name of role>', id:<role id>},
+                    'user':{userName:'<user name>', userId:<id>}
+                }
+            ]
+        """
+        return self._operators
+
+    @operators.setter
+    def operators(self, operator_list: list) -> None:
+        """
+        Overwrites the operator:role associations of the organization
+
+        Args:
+            operators (list): list of dicts with role and user/userGroup keys
+
+            [
+                {'role':'<name of role>','userGroup':'<usergroupname>'},
+                {'role':'<name of role>','user':'<username>'}
+            ]
+
+        Returns:
+            None
+
+        Raises:
+            SDKException:
+                if failed to update the properties of the organization
+
+                if response is empty
+
+        """
+        operators_list = []
+        for operator in operator_list:
+            operator_dict = {"role":
+                {
+                    "roleName": operator["role"],
+                    "roleId": int(self._commcell_object.roles.get(operator["role"]).role_id)
+                }
+            }
+            if 'user' in operator:
+                operator_dict['user'] = {
+                    'userName': operator['user'],
+                    'userId': int(self._commcell_object.users.get(operator['user']).user_id)
+                }
+            if 'userGroup' in operator:
+                operator_dict['userGroup'] = {
+                    'userGroupName': operator['userGroup'],
+                    'userGroupId': int(self._commcell_object.user_groups.get(operator['userGroup']).user_group_id)
+                }
+            operators_list.append(operator_dict)
+
+        request_json = {
+            "organizationInfo": {
+                "organization": {
+                    "shortName": {"domainName": self.name, "id": int(self._organization_id)}
+                },
+                "organizationProperties": {
+                    "operatorsOperationType": 1,
+                    "operators": operators_list
+                },
+            }
+        }
+        __, response = self._cvpysdk_object.make_request(
+            'PUT', self._services['UPDATE_ORGANIZATION'] % self.organization_id, request_json
+        )
+        self.refresh()
+        if response.json():
+            if 'error' in response.json():
+                error_code = response.json()['error']['errorCode']
+                error_message = response.json()['error'].get('errorMessage', '')
+            else:
+                error_code = response.json()['errorCode']
+                error_message = response.json().get('errorMessage', '')
+
+            if error_code != 0:
+                raise SDKException(
+                    'Organization', '110', 'Error: {0}'.format(error_message)
+                )
+        else:
+            raise SDKException('Response', '102')
+
+    @property
     def contacts_fullname(self):
         """ Returns Primary Contacts full name for the organization"""
         return [contact['name'] for contact in self._contacts.values()]
 
     @property
     def default_plan(self):
         """Returns the Default Plans associated to this Organization."""
@@ -2607,14 +3025,91 @@
         return self._is_authorise_for_restore_enabled
 
     @property
     def isAllowUsersToEnablePasskeyEnabled(self):
         """Returns True if it is enabled"""
         return self._is_allow_users_to_enable_passkey_enabled
 
+    @property
+    def company_theme(self)->dict:
+        """
+        Returns:
+            theme   (dict)  -   the company level theme colors set, empty dict if no company level theme set
+
+        Example:
+            {
+                loginAndBannerBg: '#0B2E44',
+                headerColor: '#DDE5ED',
+                headerTextColor: '#0B2E44',
+                navBg: '#FFFFFF',
+                navIconColor: '#0b2e44',
+                pageHeaderText: '#0B2E44',
+                actionBtnBg: '#0B2E44',
+                actionBtnText: '#eeeeee',
+                linkText: '#4B8DCC',
+                iconColor: '#0B2E44'
+            }
+        """
+        return self._theme
+
+    @company_theme.setter
+    def company_theme(self, theme_colors:dict)->None:
+        """
+        Sets company level theme for an Organisation
+
+        Args:
+            theme_colors    (dict)  -   with color setting name as key and color hex as value
+
+            example:
+                theme_colors = {
+                    loginAndBannerBg: '#0B2E44',
+                    headerColor: '#DDE5ED',
+                    headerTextColor: '#0B2E44',
+                    navBg: '#FFFFFF',
+                    navIconColor: '#0b2e44',
+                    pageHeaderText: '#0B2E44',
+                    actionBtnBg: '#0B2E44',
+                    actionBtnText: '#eeeeee',
+                    linkText: '#4B8DCC',
+                    iconColor: '#0B2E44'
+                }
+
+        Raises:
+            SDKException:
+                If it fails to Set theme for an Organisation
+        """
+        if self._theme == theme_colors:
+            return
+
+        request_json = {
+            "organizationInfo": {
+                "organizationProperties": {
+                    "customization": json.dumps(theme_colors)
+                },
+            }
+        }
+        flag, response = self._cvpysdk_object.make_request(
+            'PUT', self._services['ORGANIZATION_THEME'] % self.organization_id, request_json
+        )
+
+        if flag:
+            if response.json():
+                if 'error' in response.json():
+                    error_code = response.json()['error']['errorCode']
+                    if error_code != 0:
+                        error_message = response.json()['error']['errorMessage']
+                        raise SDKException('Organization', '110', 'Error: {0}'.format(error_message))
+            else:
+                raise SDKException('Organization', '110')
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+        self.refresh()
+
     def passkey(self, current_password, action, new_password=None):
         """"
         Updates Passkey properties of an Organisation
 
         Args:
             current_password (str) --  User Current Passkey to perform actions
             action (str)           --  'enable' | 'disable' | 'change passkey' | 'authorise'
@@ -2771,7 +3266,566 @@
 
                 self.refresh()
             else:
                 raise SDKException('Response', '102')
         else:
             response_string = self._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
+
+
+class RemoteOrganization:
+    """Class for performing remote operations on an Organization."""
+
+    def __init__(self, commcell_object, organization_name:str, organization_id:str=None, homecell:str=None):
+        """Initialise the RemoteOrganization instance.
+
+            Args:
+                commcell_object     (object)    --  instance of the Commcell class
+
+                organization_name   (str)       --  name of the organization
+
+                organization_id     (str)       --  id of the organization
+                    default: None
+
+                homecell            (str)       --  the belonging service commcell of this organization
+
+                    default: None
+
+            Returns:
+                object  -   instance of the RemoteOrganization class
+
+        """
+        self._commcell_object = commcell_object
+        self._cvpysdk_object = commcell_object._cvpysdk_object
+        self._services = commcell_object._services
+        self._update_response_ = commcell_object._update_response_
+        self._homecell = homecell
+        if not homecell:
+            self._homecell = self._get_homecell()
+
+        self._headers = self._commcell_object._headers.copy()
+        self._headers['CVContext']='Comet'
+        self._headers['_cn'] = self._homecell
+        self._headers['Comet-Commcells'] = self._homecell
+
+        self._organization_name = organization_name
+
+        if organization_id:
+            self._organization_id = str(organization_id)
+        else:
+            self._organization_id = self._get_organization_id()
+
+        self._properties = {}
+        self._reseller_enabled = None
+        self._backup_disabled = None
+        self._login_disabled = None
+        self._restore_disabled = None
+        self._domain_name = None
+        self._operators = None
+        self._parent_company = None
+
+        self.refresh()
+
+    @property
+    def reseller_enabled(self)->bool:
+        """ 
+        Returns if reseller is enabled 
+        
+        Returns:
+            bool - True if reseller mode is enabled for the company
+        """
+        return self._reseller_enabled
+
+    def __repr__(self)->str:
+        """Returns the string representation of an instance of this class."""
+        return 'Remote Organization class instance for Organization: "{0}" of "{1}"'.format(
+            self.organization_name, self._homecell
+        )
+
+    def _get_organization_id(self)->str:
+        """Gets the remote id associated with this remote organization within given commcell.
+
+            Returns:
+                str     -   remote id associated with this remote organization
+
+        """
+        organizations = Organizations(self._commcell_object)
+        organizations.fanout = True
+        return organizations.get_remote_org(self.organization_name).organization_id
+
+    def _get_homecell(self)->str:
+        """Gets the service commcell this company belongs to.
+
+            Returns:
+                str     -   service commcell where company resides
+
+        """
+        organizations = Organizations(self._commcell_object)
+        organizations.fanout = True
+        return organizations.get_remote_org(self.organization_name).homecell
+
+    def _get_properties(self)->dict:
+        """Gets the properties of this Organization.
+
+            Returns:
+                dict    -   dictionary consisting of the properties of this organization
+
+            Raises:
+                SDKException:
+                    if response is empty
+
+                    if response is not success
+
+        """
+        flag, response = self._cvpysdk_object.make_request(
+            'GET', self._services['ORGANIZATION'] % self.organization_id, headers=self._headers.copy()
+        )
+
+        if flag:
+            if response.json() and 'organizationInfo' in response.json():
+                self._organization_info = response.json().get('organizationInfo', {})
+
+                organization = self._organization_info.get('organization', {})
+                organization_properties = self._organization_info.get('organizationProperties', {})
+
+                self._description = organization.get('description')
+                self._email_domain_names = organization.get('emailDomainNames')
+                self._domain_name = organization.get('shortName', {}).get('domainName')
+                self._backup_disabled = organization.get('deactivateOptions', {}).get('disableBackup')
+                self._restore_disabled = organization.get('deactivateOptions', {}).get('disableRestore')
+                self._login_disabled = organization.get('deactivateOptions', {}).get('disableLogin')
+                self._reseller_enabled = organization_properties.get('canCreateCompanies')
+
+                self._operators = organization_properties.get("operators")
+                self._parent_company = organization_properties.get("resellerCompany")
+
+                return self._organization_info
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+    @property
+    def name(self)->str:
+        """
+        Returns the Organization display name 
+        
+        Returns:
+            str     -   name of this organization
+        """
+        return self._organization_info.get('organization', {}).get('connectName')
+
+    @property
+    def organization_id(self)->str:
+        """
+        Returns the value of the id for this Organization.
+        
+        Returns:
+            str     -   id of this organization (in given commcell)
+        
+        """
+        return self._organization_id
+
+    @property
+    def homecell(self)->str:
+        """
+        Returns the service commcell name of this Organization.
+        
+        Returns:
+            str     -   commserve name where this organization exists
+        """
+        return self._homecell
+
+    @property
+    def organization_name(self)->str:
+        """
+        Returns the value of the name for this Organization.
+        
+        Returns:
+            str     -   organization name
+        """
+        return self._organization_name.lower()
+
+    @property
+    def domain_name(self)->str:
+        """
+        Returns the value of the domain name for this Organization.
+        
+        Returns:
+            str     -   alias name/domain name of this organization
+
+        """
+        return self._domain_name
+
+    @property
+    def parent_company(self)->dict:
+        """
+        Returns the parent company details dict of this organization (if it is child company).
+
+        Returns:
+            dict    -   parent company details
+        
+        Example: {
+            '_type_': <entity type id>, 
+            'providerId': <company id>, 
+            'providerDomainName': '<company name>'
+            }
+        
+        """
+        return self._parent_company
+
+    @property
+    def is_backup_disabled(self)->bool:
+        """
+        Returns boolean whether backup is disabled for this organisation
+        
+        Returns:
+            bool    -   True if backup is disabled
+        
+        """
+        return self._backup_disabled
+
+    @property
+    def is_restore_disabled(self)->bool:
+        """
+        Returns boolean whether restore is disabled for this organisation
+        
+        Returns:
+            bool    -   True if restore is disabled
+        
+        """
+        return self._restore_disabled
+
+    @property
+    def is_login_disabled(self)->bool:
+        """
+        Returns boolean whether login is disabled for this organisation
+        
+        Returns:
+            bool    -   True if login is disabled
+        
+        """
+        return self._login_disabled
+
+    def refresh(self)->None:
+        """Refresh the properties of the Organization."""
+        self._properties = self._get_properties()
+
+    @property
+    def operators(self)->list:
+        """
+        Returns the list of operators and roles associated to this organization
+
+        Returns:
+            list    -   list of dicts containing operator details
+        
+        Example:
+            [
+                {
+                    'role': {name:'<name of role>', id:<role id>},
+                    'userGroup': {userGroupName:'<usergroupname>', userGroupId:<id>}
+                },
+                {
+                    'role':{name:'<name of role>', id:<role id>},
+                    'user':{userName:'<user name>', userId:<id>}
+                }
+            ]
+        """
+        return self._operators
+
+    @operators.setter
+    def operators(self, operator_list:list)->None:
+        """
+        Overwrites the operator:role associations of the organization remotely
+        
+        Args:
+            operators (list): list of dicts with role and user/userGroup keys
+            
+            [
+                {'role':'<name of role>','userGroup':'<usergroupname>'},
+                {'role':'<name of role>','user':'<username>'}
+            ]
+        
+        Returns:
+            None
+
+        Raises:
+            SDKException:
+                if failed to update the properties of the organization
+
+                if response is empty
+
+        """
+        operators_list = []
+        for operator in operator_list:
+            operator_dict = {"role":
+                {
+                    "roleName": operator["role"],
+                    "roleId": int(self._commcell_object.roles.get(operator["role"]).role_id)
+                }
+            }
+            if 'user' in operator:
+                operator_dict['user'] = {
+                    'userName': operator['user'],
+                    'userId': int(self._commcell_object.users.get(operator['user']).user_id)
+                }
+            if 'userGroup' in operator:
+                operator_dict['userGroup'] = {
+                    'userGroupName': operator['userGroup'],
+                    'userGroupId': int(self._commcell_object.user_groups.get(operator['userGroup']).user_group_id)
+                }
+            operators_list.append(operator_dict)
+
+        request_json = {
+            "organizationInfo": {
+                "organization": {
+                    "shortName": {"domainName": self.name, "id": int(self._organization_id)}
+                },
+                "organizationProperties": {
+                    "operatorsOperationType": 1,
+                    "operators": operators_list
+                },
+            }
+        }
+        __, response = self._cvpysdk_object.make_request(
+            'PUT', self._services['UPDATE_ORGANIZATION'] % self.organization_id, request_json, headers=self._headers.copy()
+        )
+        self.refresh()
+        if response.json():
+            if 'error' in response.json():
+                error_code = response.json()['error']['errorCode']
+                error_message = response.json()['error'].get('errorMessage', '')
+            else:
+                error_code = response.json()['errorCode']
+                error_message = response.json().get('errorMessage', '')
+
+            if error_code != 0:
+                raise SDKException(
+                    'RemoteOrganization', '101', 'Error: {0}'.format(error_message)
+                )
+        else:
+            raise SDKException('Response', '102')
+
+    def activate(self)->None:
+        """
+        To activate the organization remotely
+
+        Args:
+            None
+
+        Returns:
+            None
+
+        Raises:
+            SDKException:
+                if failed to activate the organization
+
+                if response is empty
+
+                if response is not success
+
+        """
+        flag, response = self._cvpysdk_object.make_request(
+            'POST', self._services['ACTIVATE_ORGANIZATION'] % self.organization_id, headers=self._headers.copy()
+        )
+        self.refresh()
+        if flag:
+            if response.json():
+                error_code = response.json()['response']['errorCode']
+
+                if error_code != 0:
+                    raise SDKException(
+                        'RemoteOrganization', '102', 'Error: "{0}"'.format(
+                            response.json()['error']['errorMessage']
+                        )
+                    )
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+    def deactivate(self,
+                   disable_backup=True,
+                   disable_restore=True,
+                   disable_login=True)->None:
+        """
+        To deactivate the organization remotely
+
+        Args:
+            disable_backup  (bool)      -- To disable backup
+                                            default: True
+
+            disable_restore (bool)      -- To disable restore
+                                            default: True
+
+            disable_login   (bool)      -- To disable login
+                                            default: True
+
+        Returns:
+            None
+
+        Raises:
+            SDKException:
+                if failed to deactivate the organization
+
+                if response is empty
+
+                if response is not success
+
+        """
+        request_json = {
+            "deactivateOptions": {
+                "disableBackup": disable_backup,
+                "disableRestore": disable_restore,
+                "disableLogin": disable_login
+            }
+        }
+
+        flag, response = self._cvpysdk_object.make_request(
+            'POST', self._services['DEACTIVATE_ORGANIZATION'] % self.organization_id, request_json,
+            headers=self._headers.copy()
+        )
+
+        if flag:
+            if response.json():
+                error_code = response.json()['response']['errorCode']
+
+                if error_code != 0:
+                    raise SDKException(
+                        'RemoteOrganization', '103', 'Error: "{0}"'.format(
+                            response.json()['error']['errorMessage']
+                        )
+                    )
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+        self.refresh()
+
+    @property
+    def tags(self)->list:
+        """
+        Returns:
+            tags (list)  -- List of dictionaries containing TAG values
+
+        Example:
+                [
+                    {
+                    "name": "key1",
+                    "value": "value1"
+                    },
+                    {
+                    "name": "key2",
+                    "value": "value2"
+                    }
+                ]
+
+        Raises:
+                SDKException:
+                    if response is empty
+
+                    if response is not success
+        """
+        req_url = self._services['GET_ORGANIZATION_TAGS'] % (self.organization_id)
+        flag, response = self._cvpysdk_object.make_request('GET', req_url, headers=self._headers.copy())
+
+        if flag:
+            if response.json():
+                if 'tags' in response.json():
+                    return response.json()['tags'][0]['tag']
+                else:
+                    return []
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+    @tags.setter
+    def tags(self, tag_list:list)->None:
+        """
+        Updates Tags for an Organisation
+
+        Args:
+            tag_list (list) --  List of Tag details
+
+            example:
+                tag_list = [
+                    {
+                    "name": "key1",
+                    "value": "value1"
+                    },
+                    {
+                    "name": "key2",
+                    "value": "value2"
+                    }
+                ]
+
+        Raises:
+            SDKException:
+                If it fails to Update Tags for an Organisation
+        """
+
+        req_json = {
+            "entityTag": [
+                {
+                    "entityId": int(self.organization_id),
+                    "entityType": 61,
+                    "tag": tag_list
+                }
+            ]
+        }
+
+        req_url = self._services['ORGANIZATION_TAGS']
+        flag, response = self._cvpysdk_object.make_request('PUT', req_url, req_json, headers=self._headers.copy())
+
+        if flag:
+            if response.json():
+                if 'error' in response.json():
+                    error_code = response.json()['error']['errorCode']
+                    if error_code != 0:
+                        error_message = response.json()['error']['errorMessage']
+                        raise SDKException('RemoteOrganization', '104', 'Error: {0}'.format(error_message))
+            else:
+                raise SDKException('RemoteOrganization', '104')
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+        self.refresh()
+
+    def get_entity_counts(self)->dict:
+        """Gets the entity type and counts for company's associated entities
+
+            Returns:
+                dict    -   entity as key and count as value
+
+                    {'total': 8, 'Alert definitions': 4, 'User': 1, 'User group': 2, 'Server group': 1}
+
+            Raises:
+                SDKException:
+                    if response is empty
+
+                    if response is not success
+
+        """
+        flag, response = self._cvpysdk_object.make_request(
+            'GET',
+            self._services['COMPANY_ENTITIES'] % self._organization_id,
+            headers=self._headers.copy()
+        )
+        entity_counts = {}
+        entity_types = ENTITY_TYPE_MAP
+        if flag:
+            if response.json():
+                entity_counts['total'] = response.json().get('totalCount', None)
+                for entity in response.json().get('entities',[]):
+                    entity_counts[entity_types.get(entity['name'], f'type_{entity["name"]}')] = entity['count']
+                return entity_counts
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/plan.py` & `cvpysdk-11.32/cvpysdk/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 
     delete()                    --  deletes the plan from the commcell
 
     refresh()                   --  refresh the plans associated with the commcell
 
     add_data_classification_plan()-  Adds data classification plan to the commcell
 
+    get_supported_solutions()   --  returns the supported solutions for plans
+    
 Attributes
 ----------
 
     **all_plans**   --  returns the dict consisting of plans and their details
 
 
 Plan
@@ -94,15 +96,16 @@
     disable_full_schedule()     --  disables the full schedule of a plan
 
     share()                     --  shares plan with given user by associating given role
 
     schedule()                  --  create/delete schedule on DC Plan
 
     edit_plan()                 --  edit plan options
-
+    
+    update_security_associations() -- to update security associations of a plan
 
 Plan Attributes
 ----------------
     **plan_id**                 --  returns the id of the plan
 
     **plan_name**               --  returns the name of the plan
 
@@ -125,22 +128,24 @@
     **operation_window**        --  returns the incremental operation window set by the plan
 
     **full_operation_window**   --  returns the full operation window set by the plan
 
     **associated_entities**     --  returns all the entities associated with the plan
 
     **content_indexing_props**  --  returns the DC plan related properties from the plan
+    
+    **applicable_solutions**    --  returns applicable solutions configured on server plan
 """
 from __future__ import unicode_literals
 
 import copy
 from enum import Enum
 
 from .exception import SDKException
-
+from .security.security_association import SecurityAssociation
 from .activateapps.constants import TargetApps, PlanConstants
 from functools import reduce
 
 
 class PlanTypes(Enum):
     """Class Enum to represent different plan types"""
     Any = 0
@@ -580,25 +585,29 @@
                 is_dedupe = False
 
         request_json = self._get_plan_template(plan_sub_type, "MSP")
 
         request_json['plan']['summary']['rpoInMinutes'] = sla_in_minutes
         request_json['plan']['summary']['description'] = "Created from CvPySDK."
         request_json['plan']['summary']['plan']['planName'] = plan_name
-        request_json['plan']['schedule']['subTasks'][1]['options']['commonOpts'][
-            'automaticSchedulePattern'].update({
-                'minBackupInterval': 0,
-                'maxBackupIntervalMinutes': 0,
-                'minSyncInterval': 0,
-                'minSyncIntervalMinutes': 0
-            })
-        request_json['plan']['schedule']['subTasks'][1]['options']['commonOpts'][
-            'automaticSchedulePattern']['ignoreOpWindowPastMaxInterval'] = True
+
+        template_schedules = [schedule['subTask']['subTaskName'] for schedule in request_json['plan']['schedule']['subTasks']]
+        if 'Synthetic Fulls' in template_schedules:
+            synth_full_index = template_schedules.index('Synthetic Fulls')
+            request_json['plan']['schedule']['subTasks'][synth_full_index]['options']['commonOpts'][
+                'automaticSchedulePattern'].update({
+                    'minBackupInterval': 0,
+                    'maxBackupIntervalMinutes': 0,
+                    'minSyncInterval': 0,
+                    'minSyncIntervalMinutes': 0
+                })
+            request_json['plan']['schedule']['subTasks'][synth_full_index]['options']['commonOpts'][
+                'automaticSchedulePattern']['ignoreOpWindowPastMaxInterval'] = True
         del request_json['plan']['schedule']['task']['taskName']
-        if not plan_sub_type == 'ExchangeUser':
+        if plan_sub_type != 'ExchangeUser':
             request_json['plan']['storage']['copy'][0]['useGlobalPolicy'] = {
                 "storagePolicyId": int(storage_pool_obj.storage_pool_id)
             }
             if is_dedupe:
                 request_json['plan']['storage']['copy'][0]['dedupeFlags'][
                     'useGlobalDedupStore'] = 1
             else:
@@ -753,14 +762,29 @@
                     plans[temp_name] = temp_id
 
             return plans
         else:
             response_string = self._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
 
+    def get_supported_solutions(self):
+        """Method to get supported solutions for plans"""
+        flag, response = self._cvpysdk_object.make_request(
+            'GET',
+            self._services['PLAN_SUPPORTED_SOLUTIONS']
+        )
+
+        if not flag:
+            raise SDKException('Response', '101', self._update_response_(response.text))
+        
+        if response.json() and 'id' in response.json():
+            return {solution['name']: solution['id'] for solution in response.json()['id']}
+        else:
+            raise SDKException('Response', '102')
+        
     def refresh(self):
         """Refresh the plans associated with the Commcell."""
         self._plans = self._get_plans()
 
     def add_data_classification_plan(self, plan_name, index_server, target_app=TargetApps.FSO, **kwargs):
         """Adds data classification plan to the commcell
 
@@ -995,14 +1019,16 @@
         self._client_group = None
         self._override_entities = None
         self._parent_plan_name = None
         self._addons = []
         self._associated_entities = {}
         self._dc_plan_props = {}
         self._plan_entity_type = 158
+        self._region_id = []
+        self._applicable_solutions = []
         self.refresh()
 
     def __repr__(self):
         """String representation of the instance of this class."""
         representation_string = 'Plan class instance for plan: "{0}", of Commcell: "{1}"'
 
         return representation_string.format(
@@ -1124,17 +1150,18 @@
                 else:
                     self._full_operation_window = None
 
                 if 'laptop' in self._plan_properties:
                     if 'backupContent' in self._plan_properties['laptop']['content']:
                         self._child_policies['subclientPolicyIds'].clear()
                         for ida in self._plan_properties['laptop']['content']['backupContent']:
-                            self._child_policies['subclientPolicyIds'].append(
-                                ida['subClientPolicy']['backupSetEntity']['backupsetId']
-                            )
+                            if ida['subClientPolicy'].get('backupSetEntity'):
+                                self._child_policies['subclientPolicyIds'].append(
+                                    ida['subClientPolicy']['backupSetEntity']['backupsetId']
+                                )
 
                 if ('inheritance' in self._plan_properties and
                         not self._plan_properties['inheritance']['isSealed']):
                     temp_dict = self._plan_properties['inheritance']
                     del temp_dict['isSealed']
                     if 'enforcedEntities' not in temp_dict:
                         temp_dict['enforcedEntities'] = []
@@ -1164,15 +1191,19 @@
                         self._dc_plan_props['analyticsIndexServer'] = self._plan_properties['eDiscoveryInfo']['analyticsIndexServer']
 
                 if 'options' in self._plan_properties:
                     plan_options = self._plan_properties['options']
                     if 'targetApps' in plan_options:
                         self._dc_plan_props['targetApps'] = plan_options['targetApps']
 
+                    if 'supportedWorkloads' in plan_options:
+                        self._applicable_solutions = [soln['solutionName'] for soln in plan_options['supportedWorkloads'].get('solutions', [])]
+
                 if 'securityAssociations' in self._plan_properties:
+                    self._security_associations = {}
                     for association in self._plan_properties['securityAssociations'].get('associations', []):
                         temp_key = None
                         if 'externalGroupName' in association['userOrGroup'][0]:
                             temp_key = '{0}\\{1}'.format(
                                     association['userOrGroup'][0]['providerDomainName'],
                                     association['userOrGroup'][0]['externalGroupName']
                                 )
@@ -1184,14 +1215,17 @@
                             if temp_key in self._security_associations:
                                 self._security_associations[temp_key].append(
                                     association['properties']['role']['roleName']
                                 )
                             else:
                                 self._security_associations[temp_key] = [association['properties']['role']['roleName']]
 
+                if "storageRules" in self._plan_properties:
+                    self._region_id = [x["regions"]["region"][0]["regionId"] for x in self._plan_properties["storageRules"]["rules"]]
+
                 self._get_associated_entities()
 
                 return self._plan_properties
             else:
                 raise SDKException('Response', '102')
         else:
             response_string = self._update_response_(response.text)
@@ -1924,24 +1958,61 @@
             Eg:
                 {
                     'sample_user_group_name': 'role_name'
                 }
         """
         return self._security_associations
 
+    def update_security_associations(self, associations_list, is_user = True, request_type = None, external_group = False):
+        """
+        Adds the security association on the plan object
+
+        Args:
+            associations_list   (list)  --  list of users to be associated
+                Example:
+                    associations_list = [
+                        {
+                            'user_name': user1,
+                            'role_name': role1
+                        },
+                        {
+                            'user_name': user2,
+                            'role_name': role2
+                        }
+                    ]
+ 
+            is_user (bool)           --    True or False. set is_user = False, If associations_list made up of user groups
+            request_type (str)      --    eg : 'OVERWRITE' or 'UPDATE' or 'DELETE', Default will be OVERWRITE operation
+            external_group (bool)    --    True or False, set external_group = True. If Security associations is being done on External User Groups
+
+        Raises:
+            SDKException:
+                if association is not of List type
+        """
+        if not isinstance(associations_list, list):
+            raise SDKException('Plan', '102')
+
+        SecurityAssociation(self._commcell_object, self)._add_security_association(associations_list, 
+                                        is_user, request_type, external_group)
+
     @property
     def content_indexing_props(self):
         """returns the DC plan related CI properties from Plan"""
         return self._dc_plan_props
 
     @property
     def properties(self):
         """Returns the configured properties for the Plan"""
         return self._plan_properties
 
+    @property
+    def region_id(self):
+        """Returns the Backup destination region id"""
+        return self._region_id
+
     def refresh(self):
         """Refresh the properties of the Plan."""
         self._properties = self._get_plan_properties()
 
     def associate_user(self, userlist):
         """associates the users to the plan.
             # TODO: Need to handle user groups.
@@ -2146,14 +2217,16 @@
         request_json['summary']['plan']['planId'] = int(self.plan_id)
         request_json['schedule']['associations'][0]['entityId'] = int(self.plan_id)
         request_json['schedule']['task']['taskName'] = f"Cvpysdk created Schedule policy for plan - {self.plan_name}"
         request_json['schedule']['subTasks'][0]['subTask'][
             'subTaskName'] = schedule_name
         request_json['schedule']['subTasks'][0]['pattern'] = pattern_json
         request_json['schedule']['subTasks'][0]['options']['adminOpts']['contentIndexingOption']['operationType'] = ops_type
+        if self._dc_plan_props['targetApps'][0] == TargetApps.FS.value:
+            request_json['schedule']['subTasks'][0]['subTask']['operationType'] = 5022
         self._update_plan_props(request_json)
 
     def edit_plan(self, **kwargs):
         """Edit plan options
 
                 Args:
 
@@ -2342,7 +2415,43 @@
                     errorCode = response.json()['response'][0].get('errorCode')
                     if errorCode:
                         raise SDKException('Plan', 102, 'Failed to Change Content of Plan.')
                 else:
                     raise SDKException('Plan', 102, 'Failed to get subclient Ids.')
             else:
                 raise SDKException('Plan', 102, response.text)
+
+    @property
+    def applicable_solutions(self):
+        """Method to read applicable solutions"""
+        return self._applicable_solutions
+
+    @applicable_solutions.setter
+    def applicable_solutions(self, solutions: list = list()):
+        """Method to update applicable solutions of plan
+        
+        Args:
+            solutions (list) : List of Applicable Solutions
+            
+            example: 
+                ["File Servers", "Databases"] : FS and DB will be set as a applicable solutions
+                [] : Passing empty list will reset applicable solutions to ALL
+            
+        """
+        request_url  = self._commcell_object._services['APPLICABLE_SOLNS_ENABLE' if solutions else 'APPLICABLE_SOLNS_DISABLE'] % self.plan_id
+        
+        if solutions:
+            supported_solutions =  self._commcell_object.plans.get_supported_solutions()
+            request_json = {"solutions": [{"id": supported_solutions[soln_name], "name": soln_name} for soln_name in solutions]}
+        else:
+            request_json = None
+                    
+        flag, response = self._commcell_object._cvpysdk_object.make_request('PUT', request_url, request_json)
+        
+        if not flag:
+            raise SDKException('Response', '101', self._update_response_(response.text))
+        
+        if not response.json() or response.json()['errorCode']:
+            raise SDKException('Plan', 102, 'Failed to update Applicable Solutions for Plan')
+                
+        self.refresh()
+
```

### Comparing `cvpysdk-11.30.1/cvpysdk/policies/__init__.py` & `cvpysdk-11.32/cvpysdk/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/policies/configuration_policies.py` & `cvpysdk-11.32/cvpysdk/policies/configuration_policies.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/policies/schedule_options.py` & `cvpysdk-11.32/cvpysdk/policies/schedule_options.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/policies/schedule_policies.py` & `cvpysdk-11.32/cvpysdk/policies/schedule_policies.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/policies/storage_policies.py` & `cvpysdk-11.32/cvpysdk/policies/storage_policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,44 +163,53 @@
 
     set_parallel_copy()                     --  Sets the parallel copy setting on storage policy copy
 
     is_inline_copy()                        --  Gets the inline copy setting on storage policy copy
 
     set_inline_copy()                       --  Sets the inline copy setting on storage policy copy
 
+    get_jobs_on_copy()                      --  Fetches the Details of jobs on Storage Policy Copy
+
     delete_job()                            --  delete a job from storage policy copy node
 
     _mark_jobs_on_copy()                    --  marks job(s) for given operation on a secondary copy
 
     pick_for_copy()                         --  marks job(s) to be Picked for Copy to a secondary copy
 
     recopy_jobs()                           --  marks job(s) to be picked for ReCopying to a secondary copy
 
     do_not_copy_jobs()                      --  marks job(s) as Do Not Copy to a secondary copy
 
     pick_jobs_for_data_verification()       --  marks job(s) on a copy to be Picked for Data Verification
 
     do_not_verify_data()                    --  marks job(s) on a copy to not be Picked for Data Verification
 
+    pick_jobs_for_backupcopy                --  marks job(skipped/unpicked) on a copy to be picked for backup copy
+
     mark_jobs_bad()                         --  marks job(s) on a copy as Bad
 
     is_dedupe_enabled()                     --  checks whether deduplication is enabled for the copy
 
     set_encryption_properties()                   --  configures copy encryption settings as per user input
 
     set_key_management_server()             --  sets the Key Management Server to this copy
 
+    set_multiplexing_factor()               --  sets/unset the multiplexing factor for the storage policy copy 
+
 Attributes
 ----------
+    **override_pool_retention**                 --  Returns if Override Pool Retention flag is set or not
+
+    **override_pool_retention.setter**          --  Sets/Unsets the override Pool Retention Flag
 
     **space_optimized_auxillary_copy**          --  Returns the value of space optimized auxillary copy setting
 
     **space_optimized_auxillary_copy.setter**   --  Sets the value of space optimized auxillary copy setting
 
-	**source_copy**                             --  Returns the source copy associated with the copy
+    **source_copy**                             --  Returns the source copy associated with the copy
 
     **source_copy.setter**                      --  Sets the source copy for the copy
 
     **store_priming**                    --  Sets the value of DDB store priming under copy dedupe properties
 
     ***is_active***                             --  Returns/Sets the 'Active' Property of the Copy
 
@@ -230,15 +239,15 @@
                 commcell_object (object)  --  instance of the Commcell class
 
             Returns:
                 object - instance of the StoragePolicies class
         """
         self._commcell_object = commcell_object
         self._POLICY = self._commcell_object._services['STORAGE_POLICY']
-
+        self._DELETE_POLICY =  self._commcell_object._services['DELETE_STORAGE_POLICY']
         self._policies = None
         self.refresh()
 
     def __str__(self):
         """Representation string consisting of all storage policies of the commcell.
 
             Returns:
@@ -887,28 +896,33 @@
 
                     if response is not success
         """
         if not isinstance(storage_policy_name, str):
             raise SDKException('Storage', '101')
 
         if self.has_policy(storage_policy_name):
-            policy_delete_service = self._POLICY + '/{0}'.format(storage_policy_name)
+            storagepolicy_id = self.all_storage_policies[storage_policy_name.lower()]
+            policy_delete_service = self._DELETE_POLICY + '/{0}'.format(storagepolicy_id)
 
             flag, response = self._commcell_object._cvpysdk_object.make_request(
                 'DELETE', policy_delete_service
             )
 
             if flag:
                 try:
                     if response.json():
-                        if 'errorCode' in response.json() and 'errorMessage' in response.json():
-                            error_message = response.json()['errorMessage']
-                            o_str = 'Failed to delete storage policy\nError: "{0}"'
-
-                            raise SDKException('Storage', '102', o_str.format(error_message))
+                        if 'error' in response.json():
+                            if 'errorCode' in response.json()['error'] and 'errorMessage' in response.json()['error']:
+                                error_message = response.json()['error']['errorMessage']
+                                o_str = 'Failed to delete storage policy\nError: "{0}"'
+
+                                raise SDKException('Storage', '102', o_str.format(error_message))
+                            elif 'errorCode' in response.json()['error'] and response.json()['error']['errorCode'] == 0:
+                                self.refresh()
+                                return response.text.strip()
                 except ValueError:
                     if response.text:
                         if 'errorCode' in response.text and 'errorMessage' in response.text:
                             raise SDKException('Storage', '102', response.text.strip())
                         self.refresh()
                         return response.text.strip()
                     else:
@@ -1461,14 +1475,17 @@
 
                 resource_pool       (str)   --  Name of the resource pool to add
                 default : None
 
                 is_replica_copy     (bool)   --  if true then Replica Copy will be created
                 default : None
 
+                is_c2c_target       (bool)   -- if true then NetApp Cloud target copy will be created 
+                default : False
+
                 job_retention       (bool)  -- if true job based retention will be set
                 default : False
 
             Raises:
                 SDKException:
                     if type of inputs in not string
 
@@ -1503,34 +1520,37 @@
             is_snap_copy = 1
         else:
             is_snap_copy = 0
         if provisioning_policy is None:
             provisioning_policy = ""
             resource_pool = ""
 
+        is_c2c_target = kwargs.get('is_c2c_target', False)
+        isNetAppSnapCloudTargetCopy = 1 if is_c2c_target else 0
+
         job_based_retention = kwargs.get('job_based_retention', False)
         job_retention = 1 if job_based_retention else 0
         request_xml = """
                     <App_CreateStoragePolicyCopyReq copyName="{0}">
                         <storagePolicyCopyInfo active="1" isMirrorCopy="{1}" isSnapCopy="{2}" provisioningPolicyName="{3}">
                             <StoragePolicyCopy _type_="18" copyName="{0}" storagePolicyName="{4}" />
-                            <extendedFlags arrayReplicaCopy="{5}" useOfflineArrayReplication="{6}" />
+                            <extendedFlags arrayReplicaCopy="{5}" isNetAppSnapCloudTargetCopy="{12}" useOfflineArrayReplication="{6}" />
                             <library _type_="9" libraryName="{7}" />
                             <mediaAgent _type_="11" mediaAgentName="{8}" />
                             <spareMediaGroup _type_="67" libraryName="{7}" />
                             <retentionRules jobs="8" retainArchiverDataForDays="-1" retainBackupDataForCycles="5" retainBackupDataForDays="1">
                             <retentionFlags jobBasedRetention="{11}" />
                             </retentionRules>
                             <sourceCopy _type_="18" copyName="{9}" storagePolicyName="{4}" />
                             <resourcePoolsList operation="1" resourcePoolName="{10}" />
                         </storagePolicyCopyInfo>
                     </App_CreateStoragePolicyCopyReq>
                     """.format(copy_name, is_mirror_copy, is_snap_copy, provisioning_policy,
                                self.storage_policy_name, arrayReplicaCopy, useOfflineReplication,
-                               library_name, media_agent_name, source_copy, resource_pool, job_retention)
+                               library_name, media_agent_name, source_copy, resource_pool, job_retention, isNetAppSnapCloudTargetCopy)
 
         create_copy_service = self._commcell_object._services['CREATE_STORAGE_POLICY_COPY']
 
         flag, response = self._commcell_object._cvpysdk_object.make_request(
             'POST', create_copy_service, request_xml
         )
 
@@ -1806,14 +1826,15 @@
 
             enable_snapshot_catalog          (bool)   --  Enables Snapshot Catalog if value is True
 
             source_copy_for_snapshot_catalog (str)    --  Source Copy name for Snapshot Catalog
 
             is_ocum                          (bool)   --  True if Storage policy is enabled with
                                                           ocum server
+            enable_selective_copy                 (int)   -- Enable selective copy option based on input value
 
         """
         enable_backup_copy = options['enable_backup_copy']
         enable_snapshot_catalog = options['enable_snapshot_catalog']
 
         if options['is_ocum']:
             if enable_backup_copy and enable_snapshot_catalog:
@@ -1833,29 +1854,31 @@
             source_copy_for_snap_to_tape_id = 0
         if options['source_copy_for_snapshot_catalog'] is not None:
             source_copy_for_snapshot_catalog_id = self._copies[options['source_copy_for_snapshot_catalog'].lower(
             )]['copyId']
         else:
             source_copy_for_snapshot_catalog_id = 0
 
+        selective_type = options.get('enable_selective_copy', 0)
+
         update_snapshot_tab_service = self._commcell_object._services['EXECUTE_QCOMMAND']
 
         request_xml = """
                     <EVGui_SetSnapOpPropsReq deferredCatalogOperation="{0}" snapshotToTapeOperation="{1}">
                         <header localeId="0" userId="0" />
                         <snapshotToTapeProps archGroupId="{2}" calendarId="1" dayNumber="0" deferredDays="0"
                             enable="{3}" flags="0" infoFlags="0" numOfReaders="0" numPeriod="1"
-                            sourceCopyId="{4}" startTime="0" type="0" />
+                            sourceCopyId="{4}" startTime="0" type="{7}" />
                         <deferredCatalogProps archGroupId="{2}" calendarId="1" dayNumber="0" deferredDays="0"
                             enable="{5}" flags="0" infoFlags="0" numOfReaders="0" numPeriod="1"
                             sourceCopyId="{6}" startTime="0" type="0" />
                     </EVGui_SetSnapOpPropsReq>
         """.format(defferred_catalog_value, backup_copy_value, self.storage_policy_id,
                    int(enable_backup_copy), source_copy_for_snap_to_tape_id,
-                   int(enable_snapshot_catalog), source_copy_for_snapshot_catalog_id)
+                   int(enable_snapshot_catalog), source_copy_for_snapshot_catalog_id, selective_type)
 
         flag, response = self._commcell_object._cvpysdk_object.make_request(
             'POST', update_snapshot_tab_service, request_xml
         )
 
         self.refresh()
 
@@ -2433,15 +2456,16 @@
             response_string = self._commcell_object._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
 
     def run_ddb_verification(self,
                              copy_name,
                              ver_type,
                              ddb_ver_level,
-                             use_scalable=True):
+                             use_scalable=True,
+                             orphan_chunk_listing=False):
         """
         Runs DDB verification job
 
             Args:
                 copy_name       (str)   --  name of the copy which is associated with the DDB store
 
                 ver_type        (str)   --  backup level (Full/Incremental)
@@ -2449,14 +2473,16 @@
                 ddb_ver_level   (str)   --  DDB verification type
                                             (DDB_VERIFICATION/ DDB_AND_DATA_VERIFICATION /
                                             QUICK_DDB_VERIFICATION/ DDB_DEFRAGMENTATION)
 
                 use_scalable    (bool)  --  True/False to use Scalable Resource Allocation
                                             Default: True
 
+                orphan_chunk_listing (bool) --  True/False to run orphan chunk listing phase during DDB Defragmentation
+
             Returns:
                 object - instance of the Job class for this DDB verification job
 
             Raises:
                 SDKException:
                     if type of input parameters is not string
 
@@ -2466,15 +2492,17 @@
 
                     if response is not success
         """
         if not (isinstance(copy_name, str) and
                 isinstance(ver_type, str) and
                 isinstance(ddb_ver_level, str)):
             raise SDKException('Storage', '101')
-
+        run_defrag = False
+        if ddb_ver_level == 'DDB_DEFRAGMENTATION':
+            run_defrag = True
         request = {
             "taskInfo": {
                 "associations": [
                     {
                         "copyName": copy_name, "storagePolicyName": self.storage_policy_name
                     }
                 ], "task": {
@@ -2504,15 +2532,17 @@
                                     }
                                 }
                             }, "adminOpts": {
                                 "archiveCheckOption": {
                                     "ddbVerificationLevel": ddb_ver_level,
                                     "jobsToVerify": 0,
                                     "allCopies": True,
-                                    "backupLevel": ver_type
+                                    "backupLevel": ver_type,
+                                    "ocl": orphan_chunk_listing,
+                                    "runDefrag": run_defrag
                                 }
                             }
                         }
                     }
                 ]
             }
         }
@@ -3322,14 +3352,29 @@
 
     @property
     def copy_name(self):
         """Returns the name of the copy"""
         return self._copy_name
 
     @property
+    def override_pool_retention(self):
+        """Returns if Override Pool Retention flag is set or not"""
+        return bool(self._extended_flags.get('overRideGACPRetention', 0))
+
+    @override_pool_retention.setter
+    def override_pool_retention(self, override):
+        """Sets/Unsets the override Pool Retention Flag. Not Applicable for Storage Pool Copies
+
+        Args:
+            override(bool)  :   Override the pool Retention (True/False)
+        """
+        self._extended_flags['overRideGACPRetention'] = int(override)
+        self._set_copy_properties()
+
+    @property
     def copy_retention(self):
         """Treats the copy retention as a read-only attribute."""
         retention_values = {}
         retention_values["days"] = self._retention_rules['retainBackupDataForDays']
         retention_values["cycles"] = self._retention_rules['retainBackupDataForCycles']
         retention_values["archiveDays"] = self._retention_rules['retainArchiverDataForDays']
         retention_values["jobs"] = self._retention_rules['jobs']
@@ -3724,14 +3769,76 @@
         return self.all_copies["copyPrecedence"]
 
     @property
     def media_agent(self):
         """Gets the media agent name of the copy"""
         return self._media_agent.get('mediaAgentName')
 
+    def get_jobs_on_copy(self, from_date=None, to_date=None, backup_type=None, retained_by=0,
+                         include_to_be_copied_jobs=False, list_partial_jobs_only=False):
+        """Fetches the Details of jobs on Storage Policy Copy
+
+        Args:
+            from_date      (str): Start Date Range for the Jobs
+                                    [format-'yyyy/mm/dd'] [default: from start]
+
+            to_date        (str): End Date Range for the Jobs
+                                    [format-'yyyy/mm/dd'] [default: till date]
+
+            backup_type    (str): Filter by backup type [default: None(all backup types)]
+                                    Valid values: 'full'/'incr'
+
+            retained_by    (int): Filter by retention type of jobs [default: 0]
+                                    Valid values:
+                                    1: basic retention
+                                    2: extended retention
+                                    4: manual retention
+
+            include_to_be_copied_jobs   (bool): Include details on jobs that are in to be copied state [default: False]
+
+            list_partial_jobs_only      (bool): Get details of jobs that are in partially copied state only
+                                                  [default: False]
+
+        Returns:
+            (list)  :   List of dict's with each dict containing details of a job
+        Raises:
+            SDKException:   if the response/fetch operation failed
+        """
+        command = f"qoperation execscript -sn QS_JobsinSPCopy -si @i_policyName='{self._storage_policy_name}'" \
+                  f" -si @i_copyName='{self.copy_name}'"
+        if from_date:
+            command = f"{command} -si @i_fromTime='{from_date}'"
+        if to_date:
+            command = f"{command} -si @i_toTime='{to_date}'"
+        if backup_type:
+            command = f"{command} -si @i_backupType='{backup_type.lower()}'"
+        if retained_by:
+            command = f"{command} -si @i_retention='{retained_by}'"
+        if include_to_be_copied_jobs:
+            command = f"{command} -si @i_includeToBeCopiedJobs='1'"
+        if list_partial_jobs_only:
+            command = f"{command} -si @i_includePartialJobsOnly='1'"
+
+        response = self._commcell_object.execute_qcommand(command)
+        if response.json():
+            json_response = response.json()
+            if json_response.get("ExecScriptOutput"):
+                if isinstance(json_response.get("ExecScriptOutput").get("FieldValue"), list):
+                    return json_response.get("ExecScriptOutput").get("FieldValue")
+                if isinstance(json_response.get("ExecScriptOutput").get("FieldValue"), dict):
+                    if json_response.get("ExecScriptOutput").get("FieldValue").get("@JobID"):
+                        return [json_response.get("ExecScriptOutput").get("FieldValue")]
+                return []
+            else:
+                response_string = self._commcell_object._update_response_(response.text)
+                raise SDKException('Response', '102', response_string)
+        else:
+            response_string = self._commcell_object._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
     def delete_job(self, job_id):
         """
         Deletes a job on Storage Policy
             Args:
                 job_id      (str)   --  ID for the job to be deleted
 
         Raises:
@@ -3838,14 +3945,22 @@
         """Marks job(s) on a copy as Bad
 
         Args:
             job_id      (int or str or list):   Job Id(s) that needs to be marked
         """
         self._mark_jobs_on_copy(job_id, 'markJobsBad')
 
+    def pick_jobs_for_backupcopy(self, job_id):
+        """This method is used to re-pick the job from backup which are unpick manually
+
+        Args:
+            job_id      (int or str or list):   Job Id(s) that needs to be marked
+        """
+        self._mark_jobs_on_copy(job_id, 'pickforbackupcopy')
+
     @property
     def extended_retention_rules(self):
         """Treats the extended retention rules setting as a read-only attribute."""
 
         mapping = {
             2: "EXTENDED_ALLFULL",
             4: "EXTENDED_WEEK",
@@ -4080,27 +4195,34 @@
         """
         if not isinstance(value, int):
             raise SDKException('Storage', '101')
 
         self._copy_properties['throttleNetworkBandWidthMBHR'] = value
         self._set_copy_properties()
 
-    def add_svm_association(self, src_array_id, source_array, tgt_array_id, target_array):
+    def add_svm_association(self, src_array_id, source_array, tgt_array_id,
+                            target_array, **kwargs):
         """ Method to add SVM association on Replica/vault and Mirror Copy
 
             Agrs:
                 src_array_id    (int)   --  Controlhost id of source SVM
 
                 source_array    (str)   --  Name of the source Array
 
                 tgt_array_id    (int)   --  Controlhost id of target SVM
 
                 target_array    (str)   --  Name of the Target Array
 
+                target_vendor   (str)   --  Target Vendor Name
+                
+                tgt_vendor_id   (int)   --  Target Vendor id
+
         """
+        target_vendor = kwargs.get('target_vendor', "")
+        tgt_vendor_id = kwargs.get('tgt_vendor_id', 0)
 
         request_json = {
             "EVGui_MMSMArrayReplicaPairReq": {
                 "processinginstructioninfo": {
                     "locale": {
                         "_type_": 66,
                         "localeId": 0
@@ -4129,14 +4251,22 @@
                         "copyId": 0,
                         "flags": 0,
                         "replicaPairId": 0,
                         "srcArray": {
                             "name": source_array,
                             "id": src_array_id
                         },
+                        "vendor": {
+                            "name": "",
+                            "id": 0
+                        },
+                        "tgtVendor": {
+                            "name": target_vendor,
+                            "id": tgt_vendor_id
+                        },
                         "tgtArray": {
                             "name": target_array,
                             "id": tgt_array_id
                         }
                     }
                 ]
             }
@@ -4182,7 +4312,26 @@
             raise SDKException('Storage', '101')
 
         self._copy_properties["dataEncryption"] = {
             "keyProviderName": kms_name,
             "rotateMasterKey": True
         }
         self._set_copy_properties()
+    
+    def set_multiplexing_factor(self, mux_factor):
+        """Sets/Unset the multiplexing factor for the storage policy copy
+
+            Args:
+                mux_factor  (int) -- The value for multiplexing factor
+
+            Raises SDKException:
+                If input is not valid
+
+                If API response is not successful
+        """
+        if not isinstance(mux_factor, int):
+            raise SDKException('Storage', '101')
+
+        self._copy_properties['mediaProperties'] = {
+            "multiplexingFactor" : mux_factor
+        }
+        self._set_copy_properties()
```

### Comparing `cvpysdk-11.30.1/cvpysdk/policy.py` & `cvpysdk-11.32/cvpysdk/policy.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/recovery_targets.py` & `cvpysdk-11.32/cvpysdk/recovery_targets.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,14 +248,15 @@
 
         self._recovery_target_properties = None
 
         self._policy_type = None
         self._application_type = None
         self._destination_hypervisor = None
         self._access_node = None
+        self._access_node_client_group = None
         self._users = []
         self._user_groups = []
         self._vm_prefix = ''
         self._vm_suffix = ''
 
         self._destination_host = None
         self._vm_storage_policy = None
@@ -280,16 +281,19 @@
         self._security_group = None
         self._create_public_ip = None
         self._restore_as_managed_vm = None
         self._test_virtual_network = None
         self._test_security_group = None
         self._test_vm_size = None
 
+        # AWS
         self._volume_type = None
         self._encryption_key = None
+        self._iam_role_id = None
+        self._iam_role_name = None
         self._instance_type = None
 
         self.refresh()
 
     def _get_recovery_target_id(self):
         """Gets the target id associated with this target.
 
@@ -320,22 +324,26 @@
                 vm_name_edit_string = self._recovery_target_properties.get('vmNameEditString')
                 vm_name_edit_type = self._recovery_target_properties.get('vmNameEditType', 1)
                 if vm_name_edit_string and vm_name_edit_type == 2:
                     self._vm_suffix = self._recovery_target_properties.get('vmNameEditString')
                 elif vm_name_edit_string and vm_name_edit_type == 1:
                     self._vm_prefix = self._recovery_target_properties.get('vmNameEditString')
                 self._access_node = self._recovery_target_properties.get('proxyClientEntity', {}).get('clientName')
+                self._access_node_client_group = (self._recovery_target_properties.get('proxyClientGroupEntity', {})
+                                                  .get('clientGroupName'))
                 self._users = self._recovery_target_properties.get('securityAssociations', {}).get('users')
                 self._user_groups = self._recovery_target_properties.get('securityAssociations', {}).get('userGroups')
                 self._policy_type = self._recovery_target_properties.get("entity", {}).get("policyType")
 
                 if self._policy_type == 1:
                     self._availability_zone = (self._recovery_target_properties.get('amazonPolicy',{}).get('availabilityZones', [{}])[0].get('availabilityZoneName', None))
                     self._volume_type = self._recovery_target_properties.get('amazonPolicy', {}).get('volumeType', None)
                     self._encryption_key = self._recovery_target_properties.get('amazonPolicy', {}).get('encryptionOption',{}).get('encryptionKeyName', 'Auto')
+                    self._iam_role_name = self._recovery_target_properties.get('roleInfo', {}).get('name')
+                    self._iam_role_id = self._recovery_target_properties.get('roleInfo', {}).get('id')
                     self._destination_network = self._recovery_target_properties.get('networkList', [{}])[0].get('name', None)
                     self._security_group = self._recovery_target_properties.get('securityGroups', [{}])[0].get('name', '')
                     self._instance_type = (self._recovery_target_properties.get('amazonPolicy', {}).get('instanceType', [{}])[0].get('instanceType', {}).get('vmInstanceTypeName',''))
                     
                     expiry_hours = self._recovery_target_properties.get("minutesRetainUntil", None)
                     expiry_days = self._recovery_target_properties.get("daysRetainUntil", None)
                     if expiry_hours:
@@ -439,14 +447,19 @@
 
     @property
     def access_node(self):
         """Returns: (str) the client name of the access node/proxy of the recovery target"""
         return self._access_node
 
     @property
+    def access_node_client_group(self):
+        """Returns: (str) The client group name set on the access node field of recovery target"""
+        return self._access_node_client_group
+
+    @property
     def security_user_names(self):
         """Returns: list<str> the names of the users who are used for ownership of the hypervisor and VMs"""
         return [user['userName'] for user in self._users]
 
     @property
     def vm_prefix(self):
         """Returns: (str) the prefix of the vm name to be prefixed to the destination VM"""
@@ -592,18 +605,28 @@
     @property
     def volume_type(self):
         """Returns: (str) AWS: the destination VM volume type/disk type"""
         return self._volume_type
 
     @property
     def encryption_key(self):
-        """Returns: (str) AWS: the encryption key of the destination VM. Not implemented"""
+        """Returns: (str) AWS: the encryption key of the destination VM"""
         return self._encryption_key
 
     @property
+    def iam_role_id(self):
+        """Returns: (str) AWS: the AWS IAM Role ID associated with the destination VM"""
+        return self._iam_role_id
+
+    @property
+    def iam_role_name(self):
+        """Returns: (str) AWS: the AWS IAM Role name associated with the destination VM"""
+        return self._iam_role_name
+
+    @property
     def instance_type(self):
         """Returns: (str) AWS: the AWS instance type which is used for defining hardware config"""
         return self._instance_type
 
     def refresh(self):
         """Refresh the properties of the Recovery Target."""
         self._get_recovery_target_properties()
```

### Comparing `cvpysdk-11.30.1/cvpysdk/regions.py` & `cvpysdk-11.32/cvpysdk/security/two_factor_authentication.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,158 +12,245 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # --------------------------------------------------------------------------
 
-""" File for associating Workload and Backup destination regions for various entites
+"""Helper file to manage two factor authentication settings on this commcell
 
-AssociatedEntityRegion: Class for representing all Region associations with entites
+TwoFactorAuthentication is the only class defined in this file
 
-AssociatedEntityRegion
-======================
+TwoFactorAuthentication:
 
-    __init__()                  --  initialize instance of the AssociatedEntityRegion class
+    __init__()      --      Initializes TwoFactorAuthentication class object.
 
-    set_region()                --  Associates a region to an entity
+    refresh()       --      fetches the current tfa settings.
 
-    get_region()                --  Get teh region associated to an entity
+    _get_tfa_info() --      Excutes get api on the server to fetch tfa info.
 
-    calculate_region()          --  Calculates the Region to be associated to an Entity
+    _process_response()   --  Process the response json
 
+    disable_tfa()   --      Disables tfa at commcell or organizaton level
+
+    enable_tfa()    --      Enables tfa at commcell or organization level
+
+TwoFactorAuthentication Instance Attributes
+===========================================
+
+    **is_tfa_enabled**      --      returns tfa status True or False
+
+    **tfa_enabled_user_groups** --  returns user groups on which tfa is enabled.
+                                    only if user group level tfa is enabled
 """
-from .exception import SDKException
 
-class AssociatedEntityRegion:
-    """ Class for associating Regions to all entities"""
+from ..exception import SDKException
 
-    def __init__(self, commcell_object):
-        """ Initialize object of the Regions class """
-        self._commcell_object = commcell_object
-        self._EDIT_REGION = self._commcell_object._services['EDIT_REGION']
-        self._GET_REGION = self._commcell_object._services['GET_REGION']
-        self._CALCULATE_REGION = self._commcell_object._services['CALCULATE_REGION']
 
-    def set_region(self, entity_type, entity_id, entity_region_type, region_id):
+class TwoFactorAuthentication:
+    """Class for managing the security associations roles on the commcell"""
+
+    def __init__(self, commcell_object, organization_id=None):
         """
-        Associate a region to an entity
+        Initializes TwoFactorAuthentication class object
+
         Args:
-            entity_type         (str)   :   Type of the entity
-                                            (eg:    COMMCELL,
-                                                    COMPANY,
-                                                    CLIENT,
-                                                    CLIENT_GROUP,
-                                                    MEDIAAGENT,
-                                                    STORAGE_POOL, etc
-                                            )
-            entity_id           (int)   :   unique id of the entity
-
-            entity_region_type  (str)   :   Type of the region
-                                            (WORKLOAD or BACKUP)
-
-            region_id           (int)   :   ID of the region from app_regions
-        """
-        request = {
-            "entityRegionType": entity_region_type,
-            "region":
-                {
-                    "id": region_id
-                }
-        }
+            commcell_object     --      commcell class object.
+
+            organization_id     --      id of the organization on which two factor authentication
+                                        operations to be performed.
+                default:None
+
+        Raises:
+            SDKException:
+                if invalid args are sent.
+        """
+        self._commcell = commcell_object
+        self._tfa_status = None
+        self._tfa_enabled_user_groups = None
+        self._org_id = None
+        self._cvpysdk_object = commcell_object._cvpysdk_object
+        self._services = commcell_object._services
+        self._update_response_ = commcell_object._update_response_
+        if organization_id:
+            if isinstance(organization_id, (int, str)):
+                self._org_id = organization_id
+            else:
+                raise SDKException('Security', '101')
+        self.refresh()
 
-        flag, response = self._commcell_object._cvpysdk_object.make_request(
-            'PUT', self._EDIT_REGION % (entity_type, entity_id), request
+    def refresh(self):
+        """
+        Refresh the properties of two factor authentication
+
+        Returns:
+            None
+        """
+        self._get_tfa_info()
+
+    def _get_tfa_info(self):
+        """
+        Executes api on the server and fetches commcell/organization two factor authentication info.
+
+        Returns:
+            None
+
+        Raises:
+            SDKException:
+                if failed to fetch details
+                if response is emmpty
+                if response is not success
+        """
+        url = self._services['TFA']
+
+        if self._org_id:
+            url = self._services['ORG_TFA'] % self._org_id
+
+        flag, response = self._cvpysdk_object.make_request(
+            'GET', url
         )
 
         if flag:
-            if response.json():
-                error_code = response.json()['errorCode']
-
-                if error_code != 0:
-                    if error_code == 50000:
-                        raise SDKException('Regions', '101')
-                    elif error_code == 547:
-                        raise SDKException('Regions', '102', 'Invalid regionID provided in request')
-                    else:
-                        error_string = response.json()['errorMessage']
-                        raise SDKException('Regions', '102', '{0}'.format(error_string))
+            if response.json() and 'twoFactorAuthenticationInfo' in response.json():
+                info = response.json().get('twoFactorAuthenticationInfo')
 
+                if 'error' in response.json() and 'errorCode' in response.json().get('error'):
+                    if response.json().get('error').get('errorCode') != 0:
+                        error_msg = response.json().get('error').get('errorCode').get('errorString')
+                        raise SDKException('Security',
+                                           '102',
+                                           'Failed to get the tfa info. \nError {0}'.format(error_msg))
+
+                if 'mode' in info:
+                    if info.get('mode') == 0:
+                        self._tfa_status, self._tfa_enabled_user_groups = False, []
+                    if info.get('mode') in (1, 2):
+                        self._tfa_status, self._tfa_enabled_user_groups = True, info.get('userGroups', [])
+                else:
+                    raise SDKException('Response', '102')
             else:
                 raise SDKException('Response', '102')
         else:
-            response_string = self._commcell_object._update_response_(response.text)
+            response_string = self._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
 
-    def get_region(self, entity_type, entity_id, entity_region_type):
+    def _process_response(self, flag, response):
         """
-        Gets the Region associated to an Entity
+        Processes the flag and response json
+
         Args:
-            entity_type         (str)   :   Type of the entity
-                                            (eg:    COMMCELL,
-                                                    COMPANY,
-                                                    CLIENT,
-                                                    CLIENT_GROUP,
-                                                    MEDIAAGENT,
-                                                    STORAGE_POOL, etc
-                                            )
-            entity_id           (int)   :   unique id of the entity
 
-            entity_region_type  (str)   :   Type of the region
-                                            (WORKLOAD or BACKUP)
-        """
-        flag, response = self._commcell_object._cvpysdk_object.make_request(
-            'GET', self._GET_REGION % (entity_type, entity_id, entity_region_type)
-        )
+            flag    (int)   --  status of api execution
 
-        if flag:
-            if response.json():
-                try:
-                    if response.json()['errorCode']:
-                        error_string = response.json()['errorMessage']
-                        raise SDKException('Regions', '102', '{0}'.format(error_string))
+            response    (byte)  --  data received from server
 
-                except:
-                    return response.json()['regionId']
+        Returns:
+            None
 
+        Raises:
+            SDKException:
+                if failed to get required info
+        """
+        if flag:
+            if response.json():
+                response_json = {}
+                if 'response' in response.json():
+                    response_json = response.json()['response'][0]
+                if 'error' in response.json():
+                    response_json = response.json().get('error')
+                if response_json.get('errorCode') != 0:
+                    error_msg = response_json.get('errorString')
+                    raise SDKException('Security',
+                                       '102',
+                                       'Failed to get the two factor authentication info.'
+                                       ' \nError {0}'.format(error_msg))
+                self.refresh()
             else:
-                return None
+                raise SDKException('Response', '102')
         else:
-            response_string = self._commcell_object._update_response_(response.text)
+            response_string = self._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
 
-    def calculate_region(self, entity_type, entity_id, entity_region_type):
+    def disable_tfa(self):
         """
-                Calculates the Region to be associated to an Entity
-                Args:
-                    entity_type         (str)   :   Type of the entity
-                                                    (eg:    COMMCELL,
-                                                            COMPANY,
-                                                            CLIENT,
-                                                            CLIENT_GROUP,
-                                                            MEDIAAGENT,
-                                                            STORAGE_POOL, etc
-                                                    )
-                    entity_id           (int)   :   unique id of the entity
-
-                    entity_region_type  (str)   :   Type of the region
-                                                    (WORKLOAD or BACKUP)
-                """
-        flag, response = self._commcell_object._cvpysdk_object.make_request(
-            'GET', self._CALCULATE_REGION % (entity_type, entity_id, entity_region_type)
+         Disables two factor authentication at commcell/organization level
+
+         Returns:
+             None
+
+        Raises:
+            SDKException:
+                if failed to disable tfa.
+        """
+        url = self._services['TFA_DISABLE']
+        if self._org_id:
+            url = self._services['ORG_TFA_DISABLE'] % self._org_id
+        flag, response = self._cvpysdk_object.make_request(
+            'PUT', url
         )
+        self._process_response(flag=flag, response=response)
 
-        if flag:
-            if response.json():
-                try:
-                    if response.json()['errorCode']:
-                        error_string = response.json()['errorMessage']
-                        raise SDKException('Regions', '102', '{0}'.format(error_string))
+    def enable_tfa(self, user_groups=None):
+        """
+        Enables two factor authentication at commcell/organization level.
+
+        Args:
+            user_groups     (list)  --  user group names on which two factor authentication needs to be enabled
+
+        Returns:
+            None
+
+        Raises:
+            SDKException:
+                if failed to enable tfa.
+        """
+        url = self._services['TFA_ENABLE']
 
-                except:
-                    return response.json()['regionId']
+        if self._org_id:
+            url = self._services['ORG_TFA_ENABLE'] % self._org_id
 
+        user_groups_list = []
+        if user_groups:
+            if isinstance(user_groups, list):
+                for group in user_groups:
+                    group_obj = self._commcell.user_groups.get(user_group_name=group)
+                    user_groups_list.append({"userGroupName": group_obj.name})
             else:
-                raise SDKException('Response', '102')
-        else:
-            response_string = self._commcell_object._update_response_(response.text)
-            raise SDKException('Response', '101', response_string)
+                raise SDKException('Security', '101')
+
+        payload = {
+            "twoFactorAuthenticationInfo": {
+                "mode": 2 if user_groups_list else 1,
+                "userGroups": user_groups_list
+            }
+        }
+
+        if not self._org_id:
+            payload = {
+                "commCellInfo": {
+                    "generalInfo": payload
+                }
+            }
+
+        flag, response = self._cvpysdk_object.make_request(
+            'PUT', url, payload
+        )
+        self._process_response(flag=flag, response=response)
+
+    @property
+    def is_tfa_enabled(self):
+        """Returns status of two factor authentication(True/False)"""
+        return self._tfa_status
+
+    @property
+    def tfa_enabled_user_groups(self):
+        """
+        Returns list of user group names for which two factor authentication is enabled
+            eg:-
+            [
+                {
+                "userGroupId": 1,
+                "userGroupName": "dummy"
+                }
+            ]
+        """
+        return self._tfa_enabled_user_groups
```

### Comparing `cvpysdk-11.30.1/cvpysdk/reports/__init__.py` & `cvpysdk-11.32/cvpysdk/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/reports/report.py` & `cvpysdk-11.32/cvpysdk/reports/report.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/schedules.py` & `cvpysdk-11.32/cvpysdk/schedules.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/security/__init__.py` & `cvpysdk-11.32/cvpysdk/security/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/security/role.py` & `cvpysdk-11.32/cvpysdk/security/role.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/security/security_association.py` & `cvpysdk-11.32/cvpysdk/security/security_association.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,26 +150,43 @@
 
         """
         complete_association = []
         for entity_value in entity_dictionary.values():
             for each_entity_key in entity_value:
                 for element in entity_value[each_entity_key]:
                     if each_entity_key != "role":
-                        association_blob = {
-                            "entities": {
-                                "entity": [{
-                                    each_entity_key: element
-                                }]
-                            },
-                            "properties": {
-                                "role": {
-                                    "roleName": entity_value['role'][0]
+                        if each_entity_key == "_type_":
+                            association_blob = {
+                                "entities": {
+                                    "entity": [{
+                                        each_entity_key: element,
+                                        "flags": {
+                                            "includeAll": True
+                                        }
+                                    }]
+                                },
+                                "properties": {
+                                    "role": {
+                                        "roleName": entity_value['role'][0]
+                                    }
+                                }
+                            }
+                        else:
+                            association_blob = {
+                                "entities": {
+                                    "entity": [{
+                                        each_entity_key: element
+                                    }]
+                                },
+                                "properties": {
+                                    "role": {
+                                        "roleName": entity_value['role'][0]
+                                    }
                                 }
                             }
-                        }
                         complete_association.append(association_blob)
         return complete_association
 
     @staticmethod
     def fetch_security_association(security_dict):
         """Fetches security associations from entity
         Args:
```

### Comparing `cvpysdk-11.30.1/cvpysdk/security/two_factor_authentication.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,245 +12,173 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # --------------------------------------------------------------------------
 
-"""Helper file to manage two factor authentication settings on this commcell
 
-TwoFactorAuthentication is the only class defined in this file
+"""File for operating on a Virtual Server Azure Subclient.
 
-TwoFactorAuthentication:
+AzureSubclient is the only class defined in this file.
 
-    __init__()      --      Initializes TwoFactorAuthentication class object.
+AzureSubclient: Derived class from VirtualServerSubClient  Base class, representing a
+                           Azure Subclient, and to perform operations on that Subclient
 
-    refresh()       --      fetches the current tfa settings.
+AzureSubclient:
 
-    _get_tfa_info() --      Excutes get api on the server to fetch tfa info.
+    full_vm_restore_out_of_place()                  --  restores the VM  specified in
+                                                     to the specified client, at the
+                                                        specified destination location
 
-    _process_response()   --  Process the response json
-
-    disable_tfa()   --      Disables tfa at commcell or organizaton level
-
-    enable_tfa()    --      Enables tfa at commcell or organization level
-
-TwoFactorAuthentication Instance Attributes
-===========================================
-
-    **is_tfa_enabled**      --      returns tfa status True or False
-
-    **tfa_enabled_user_groups** --  returns user groups on which tfa is enabled.
-                                    only if user group level tfa is enabled
+    full_vm_restore_in_place()              --  restores the VM specified by the
+                                                    user to the same location
 """
 
-from ..exception import SDKException
-
 
-class TwoFactorAuthentication:
-    """Class for managing the security associations roles on the commcell"""
+from ..vssubclient import VirtualServerSubclient
+from ...exception import SDKException
 
-    def __init__(self, commcell_object, organization_id=None):
-        """
-        Initializes TwoFactorAuthentication class object
-
-        Args:
-            commcell_object     --      commcell class object.
-
-            organization_id     --      id of the organization on which two factor authentication
-                                        operations to be performed.
-                default:None
-
-        Raises:
-            SDKException:
-                if invalid args are sent.
-        """
-        self._commcell = commcell_object
-        self._tfa_status = None
-        self._tfa_enabled_user_groups = None
-        self._org_id = None
-        self._cvpysdk_object = commcell_object._cvpysdk_object
-        self._services = commcell_object._services
-        self._update_response_ = commcell_object._update_response_
-        if organization_id:
-            if isinstance(organization_id, (int, str)):
-                self._org_id = organization_id
-            else:
-                raise SDKException('Security', '101')
-        self.refresh()
-
-    def refresh(self):
-        """
-        Refresh the properties of two factor authentication
 
-        Returns:
-            None
-        """
-        self._get_tfa_info()
-
-    def _get_tfa_info(self):
-        """
-        Executes api on the server and fetches commcell/organization two factor authentication info.
-
-        Returns:
-            None
-
-        Raises:
-            SDKException:
-                if failed to fetch details
-                if response is emmpty
-                if response is not success
-        """
-        url = self._services['TFA']
-
-        if self._org_id:
-            url = self._services['ORG_TFA'] % self._org_id
-
-        flag, response = self._cvpysdk_object.make_request(
-            'GET', url
+class AzureSubclient(VirtualServerSubclient):
+    """Derived class from VirtualServerSubclient  Base class, representing a
+    Azure  virtual server subclient,and to perform operations on that subclient."""
+
+    def full_vm_restore_out_of_place(self,
+                                     vm_to_restore=None,
+                                     cloud_service=None,
+                                     storage_account=None,
+                                     proxy_client=None,
+                                     restore_new_name=None,
+                                     overwrite=False,
+                                     power_on=False,
+                                     copy_precedence=0,
+                                     restore_option=None,
+                                     **kwargs):
+        """Restores the FULL Virtual machine specified  in the input  list to the client,
+            at the specified destination location.
+
+            Args:
+                cloud_service         (str)        --  provide the cloud service
+
+                storage_account     (str)          --  provide the storage account
+
+                vm_to_restore         (list)       --  provide the list of VM name(s) to restore
+
+                overwrite
+                        default:False   (bool)      --  overwrite the existing VM
+
+                poweron
+                        default:False   (bool)      --  power on the  restored VM
+
+                restore_option      (dict)     --  complete dictionary with all advanced optio
+                    default: {}
+
+                **kwargs                         : Arbitrary keyword arguments Properties as of
+                                                     full_vm_restore_out_of_place
+                    eg:
+                    v2_details          (dict)       -- details for v2 subclient
+                                                  eg: check clients.vmclient.VMClient._child_job_subclient_details
+
+
+            Returns:
+                object - instance of the Job class for this restore job
+
+            Raises:
+                SDKException:
+
+                    if destination_path is not a string
+
+                    if failed to initialize job
+
+                    if response is empty
+
+                    if response is not success
+        """
+
+        # restore options
+        if restore_option is None:
+            restore_option = {}
+        restore_option["v2_details"] = kwargs.get("v2_details", None)
+
+        # check input parameters are correct
+        if bool(restore_option):
+            if not (isinstance(overwrite, bool) and
+                    isinstance(power_on, bool)):
+                raise SDKException('Subclient', '101')     
+                
+        self._set_restore_inputs(
+            restore_option,
+            vm_to_restore=self._set_vm_to_restore(vm_to_restore),
+            unconditional_overwrite=overwrite,
+            power_on=power_on,
+            copy_precedence=copy_precedence,
+            volume_level_restore=1,
+            esx_host=cloud_service,
+            datastore=storage_account,
+            client_name=proxy_client,
+            out_place=True,
+            restore_new_name=restore_new_name
         )
 
-        if flag:
-            if response.json() and 'twoFactorAuthenticationInfo' in response.json():
-                info = response.json().get('twoFactorAuthenticationInfo')
-
-                if 'error' in response.json() and 'errorCode' in response.json().get('error'):
-                    if response.json().get('error').get('errorCode') != 0:
-                        error_msg = response.json().get('error').get('errorCode').get('errorString')
-                        raise SDKException('Security',
-                                           '102',
-                                           'Failed to get the tfa info. \nError {0}'.format(error_msg))
-
-                if 'mode' in info:
-                    if info.get('mode') == 0:
-                        self._tfa_status, self._tfa_enabled_user_groups = False, []
-                    if info.get('mode') in (1, 2):
-                        self._tfa_status, self._tfa_enabled_user_groups = True, info.get('userGroups', [])
-                else:
-                    raise SDKException('Response', '102')
-            else:
-                raise SDKException('Response', '102')
-        else:
-            response_string = self._update_response_(response.text)
-            raise SDKException('Response', '101', response_string)
-
-    def _process_response(self, flag, response):
-        """
-        Processes the flag and response json
-
-        Args:
+        # set attr for all the option in restore xml from user inputs
 
-            flag    (int)   --  status of api execution
+        request_json = self._prepare_fullvm_restore_json(restore_option)
+        return self._process_restore_response(request_json)
 
-            response    (byte)  --  data received from server
-
-        Returns:
-            None
-
-        Raises:
-            SDKException:
-                if failed to get required info
-        """
-        if flag:
-            if response.json():
-                response_json = {}
-                if 'response' in response.json():
-                    response_json = response.json()['response'][0]
-                if 'error' in response.json():
-                    response_json = response.json().get('error')
-                if response_json.get('errorCode') != 0:
-                    error_msg = response_json.get('errorString')
-                    raise SDKException('Security',
-                                       '102',
-                                       'Failed to get the two factor authentication info.'
-                                       ' \nError {0}'.format(error_msg))
-                self.refresh()
-            else:
-                raise SDKException('Response', '102')
-        else:
-            response_string = self._update_response_(response.text)
-            raise SDKException('Response', '101', response_string)
-
-    def disable_tfa(self):
-        """
-         Disables two factor authentication at commcell/organization level
-
-         Returns:
-             None
-
-        Raises:
-            SDKException:
-                if failed to disable tfa.
-        """
-        url = self._services['TFA_DISABLE']
-        if self._org_id:
-            url = self._services['ORG_TFA_DISABLE'] % self._org_id
-        flag, response = self._cvpysdk_object.make_request(
-            'PUT', url
-        )
-        self._process_response(flag=flag, response=response)
-
-    def enable_tfa(self, user_groups=None):
-        """
-        Enables two factor authentication at commcell/organization level.
-
-        Args:
-            user_groups     (list)  --  user group names on which two factor authentication needs to be enabled
-
-        Returns:
-            None
-
-        Raises:
-            SDKException:
-                if failed to enable tfa.
-        """
-        url = self._services['TFA_ENABLE']
-
-        if self._org_id:
-            url = self._services['ORG_TFA_ENABLE'] % self._org_id
-
-        user_groups_list = []
-        if user_groups:
-            if isinstance(user_groups, list):
-                for group in user_groups:
-                    group_obj = self._commcell.user_groups.get(user_group_name=group)
-                    user_groups_list.append({"userGroupName": group_obj.name})
-            else:
-                raise SDKException('Security', '101')
-
-        payload = {
-            "twoFactorAuthenticationInfo": {
-                "mode": 2 if user_groups_list else 1,
-                "userGroups": user_groups_list
-            }
-        }
-
-        if not self._org_id:
-            payload = {
-                "commCellInfo": {
-                    "generalInfo": payload
-                }
-            }
-
-        flag, response = self._cvpysdk_object.make_request(
-            'PUT', url, payload
+    def full_vm_restore_in_place(self,
+                                 vm_to_restore=None,
+                                 overwrite=True,
+                                 power_on=True,
+                                 copy_precedence=0,
+                                 **kwargs):
+        """Restores the FULL Virtual machine specified  in the input  list to the client,
+            to the location same as source .
+
+            Args:
+                vm_to_restore         (list)       --  provide the list of VM name(s) to restore
+
+                overwrite
+                        default:true   (bool)      --  overwrite the existing VM
+
+                power_on                (bool)      --  power on the  restored VM
+                                                        default: True
+
+                copy_precedence       (int)         --  copy precedence value
+                                                        default: 0
+
+                **kwargs                         : Arbitrary keyword arguments Properties as of
+                                                     full_vm_restore_in_place
+                    eg:
+                    v2_details          (dict)       -- details for v2 subclient
+                                                    eg: check clients.vmclient.VMClient._child_job_subclient_details
+
+            Returns:
+                object - instance of the Job class for this restore job
+
+            Raises:
+                SDKException:
+
+                    if failed to initialize job
+
+                    if response is empty
+
+                    if response is not success
+        """
+        restore_option = {"v2_details": kwargs.get("v2_details", None)}
+        # check mandatory input parameters are correct
+        if not (isinstance(overwrite, bool) and
+                isinstance(power_on, bool)):
+            raise SDKException('Subclient', '101')
+        # set attr for all the option in restore xml from user inputs
+        self._set_restore_inputs(
+            restore_option,
+            vm_to_restore=self._set_vm_to_restore(vm_to_restore),
+            unconditional_overwrite=overwrite,
+            power_on=power_on,
+            copy_preceedence=copy_precedence,
+            volume_level_restore=1,
+            out_place=False
         )
-        self._process_response(flag=flag, response=response)
-
-    @property
-    def is_tfa_enabled(self):
-        """Returns status of two factor authentication(True/False)"""
-        return self._tfa_status
-
-    @property
-    def tfa_enabled_user_groups(self):
-        """
-        Returns list of user group names for which two factor authentication is enabled
-            eg:-
-            [
-                {
-                "userGroupId": 1,
-                "userGroupName": "dummy"
-                }
-            ]
-        """
-        return self._tfa_enabled_user_groups
+        request_json = self._prepare_fullvm_restore_json(restore_option)
+        return self._process_restore_response(request_json)
+
```

### Comparing `cvpysdk-11.30.1/cvpysdk/security/user.py` & `cvpysdk-11.32/cvpysdk/security/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,17 @@
 
     user_guid()                         --  returns user GUID
 
     age_password_days()                 --  returns age password days for user
 
     user_company_name()                 -- returns company name if user is a company user else returns empty str
 
+    get_account_lock_info()             -- returns account lock information
+
+    unlock()                            --  Unlocks user account
 """
 
 from base64 import b64encode
 from .security_association import SecurityAssociation
 from ..exception import SDKException
 
 
@@ -368,14 +371,15 @@
                 },
                 "securityAssociations": security_json,
                 "associatedUserGroups": groups_json
             }]
         }
         response_json = self._add_user(create_user_request)
 
+
         created_user_username = response_json.get("response", [{}])[0].get("entity", {}).get("userName")
 
         return self.get(created_user_username)
 
     def has_user(self, user_name):
         """Checks if any user with specified name exists on this commcell
 
@@ -626,33 +630,45 @@
                     self._associated_external_usergroups = self._properties['associatedExternalUserGroups']
             else:
                 raise SDKException('Response', '102')
         else:
             response_string = self._commcell_object._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
 
-    def _update_user_props(self, properties_dict):
+    def _update_user_props(self, properties_dict, **kwargs):
         """Updates the properties of this user
 
             Args:
                 properties_dict (dict)  --  user property dict which is to be updated
                     e.g.: {
                             "description": "My description"
                         }
+                ** kwargs(dict)         --  Key value pairs for supported arguments
+                Supported arguments values:
+                    new_username (str)  -- New login name for the user
             Returns:
                 User Properties update dict
+            Raises:
+                SDKException:
+                    If invalid type arguments are passed
+                    Response was not success.
+                    Response was empty.
         """
         request_json = {
             "users": [{
                 "userEntity": {
                     "userName": self.user_name
                 }
             }]
         }
-
+        new_username = kwargs.get("new_username", None)
+        if new_username is not None:
+            if not isinstance(new_username, str):
+                raise SDKException("USER", "101")
+            request_json["users"][0]["userEntity"]["userName"] = new_username
         request_json['users'][0].update(properties_dict)
 
         flag, response = self._commcell_object._cvpysdk_object.make_request(
             'POST', self._user, request_json
         )
 
         if flag:
@@ -723,14 +739,19 @@
 
     @property
     def name(self):
         """Returns the User display name"""
         return self._properties['userEntity']['userName']
 
     @property
+    def full_name(self):
+        """Returns the full name of this commcell user"""
+        return self._properties.get('fullName','')
+
+    @property
     def user_name(self):
         """Returns the user name of this commcell user"""
         return self._user_name
 
     @property
     def user_id(self):
         """Returns the user id of this commcell user"""
@@ -742,14 +763,19 @@
         return self._description
 
     @property
     def email(self):
         """Returns the email associated with this commcell user"""
         return self._email
 
+    @user_name.setter
+    def user_name(self, value):
+        """Sets the new username for this commcell user"""
+        self._update_user_props("", new_username=value)
+
     @email.setter
     def email(self, value):
         """""Sets the description for this commcell user"""
         props_dict = {
             "email": value
         }
         self._update_user_props(props_dict)
@@ -1024,7 +1050,56 @@
     def is_tfa_enabled(self):
         """
         Returns the status of two factor authentication for this user
 
         bool    --  tfa status
         """
         return self._tfa_status
+
+    @property
+    def get_account_lock_info(self):
+        """
+        Returns user account lock status
+        dict     --  account lock info
+        example:
+            {
+                "isAccountLocked" : True,
+                "lockStartTime" : 1646640752,
+                "lockEndTime" : 1646727152
+            }
+        """
+        lock_info = dict()
+        lock_info['isAccountLocked'] = self._properties.get('isAccountLocked', False)
+        lock_info['lockStartTime'] = self._properties.get('lockStartTime', 0)
+        lock_info['lockEndTime'] = self._properties.get('lockEndTime', 0)
+        return lock_info
+
+    def unlock(self):
+        """
+        Unlocks user account.
+        Returns:
+            status      (str)   --      unlock operation status
+                Example:-
+                "Unlock successful for user account"
+                "Logged in user cannot unlock their own account"
+                "Unlock failed for user account"
+                "User account is not locked"
+                "Logged in user does not have rights to unlock this user account"
+            statusCode
+        Raises:
+            SDKException:
+                if response is empty
+                if response is not success
+        """
+        payload = {"lockedAccounts": [{"user": {"userName": self._user_name, "userId": self._user_id}}]}
+        service = self._commcell_object._services['UNLOCK']
+        flag, response = self._commcell_object._cvpysdk_object.make_request(
+            'POST', service, payload
+        )
+        if flag:
+            if response and response.json() and 'lockedAccounts' in response.json():
+                return response.json().get('lockedAccounts')[0].get('status'), response.json().get('lockedAccounts')[0].get('statusCode')
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._commcell_object._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/security/usergroup.py` & `cvpysdk-11.32/cvpysdk/security/usergroup.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,23 +263,30 @@
                 entity_dictionary(dict)     --  combination of entity_type, entity
                                                 names and role
                 e.g.: security_dict={
                                 'assoc1':
                                     {
                                         'entity_type':['entity_name'],
                                         'entity_type':['entity_name', 'entity_name'],
+                                        '_type_':['entity_type1', 'entity_type2']
                                         'role': ['role1']
                                     },
                                 'assoc2':
                                     {
                                         'mediaAgentName': ['networktestcs', 'standbycs'],
                                         'clientName': ['Linux1'],
                                         'role': ['New1']
                                         }
-                                    }
+                                    },
+                                'assoc3':
+                                    {
+                                        '_type_': ['CLIENT_ENTITY', 'STORAGE_POLICIES_ENTITY'],
+                                        'role': ['Alert Owner']
+                                        }
+                                    },
                 entity_type         --      key for the entity present in dictionary
                                             on which user will have access
                 entity_name         --      Value of the key
                 role                --      key for role name you specify
                 e.g:   e.g.: {"clientName":"Linux1"}
                 Entity Types are:   clientName, mediaAgentName, libraryName, userName,
                                     userGroupName, storagePolicyName, clientGroupName,
```

### Comparing `cvpysdk-11.30.1/cvpysdk/services.py` & `cvpysdk-11.32/cvpysdk/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,21 +49,23 @@
     'WHO_AM_I': '{0}WhoAmI',
 
     'TFA': '{0}Commcell/Properties/TwoFactorAuth',
     'TFA_ENABLE': '{0}Commcell/Properties/TwoFactorAuth/Action/Enable',
     'TFA_DISABLE': '{0}Commcell/Properties/TwoFactorAuth/Action/Disable',
     'PRIVACY_ENABLE': '{0}Commcell/Properties/Privacy/Action/Enable',
     'PRIVACY_DISABLE': '{0}Commcell/Properties/Privacy/Action/Disable',
+    'ACCOUNT_lOCK_SETTINGS': '{0}Commcell/Properties/AccountLockSettings',
     'ORG_TFA': '{0}Organization/%s/TwoFactorAuth',
     'ORG_TFA_ENABLE': '{0}Organization/%s/TwoFactorAuth/Action/Enable',
     'ORG_TFA_DISABLE': '{0}Organization/%s/TwoFactorAuth/Action/Disable',
     'TFA_STATUS_OF_USER': '{0}Security/TwoFactorAuth/Status?username=%s',
 
     'GET_ALL_CLIENTS': '{0}Client',
     'GET_VIRTUAL_CLIENTS': '{0}Client?PseudoClientType=VSPseudo',
+    'GET_VIRTUALIZATION_ACCESS_NODES': '{0}VSAClientAndClientGroupList',
     'GET_FILE_SERVER_CLIENTS': '{0}/v4/FileServers',
     'CLIENTFORCEDELETE':'{0}Client/%s?forceDelete=1',
     'CLIENT': '{0}Client/%s',
     'FILTER_CLIENTS':'{0}Client?%s',
     'GET_ALL_CLIENTS_PLUS_HIDDEN': '{0}Client?hiddenclients=true',
     'GET_ALL_PSEUDO_CLIENTS': '{0}Client?PseudoClientType',
     'CHECK_READINESS': '{0}Client/%s/CheckReadiness?network=%s&resourceCapacity=%s'
@@ -106,19 +108,23 @@
     'DISABLE_SHARED_LAPTOP': '{0}Commcell/Properties/SharedLaptopUsage/Action/Disable',
 
     'GET_MEDIA_AGENTS': '{0}V2/MediaAgents',
     'LIBRARY': '{0}Library',
     'GET_LIBRARY_PROPERTIES': '{0}Library/%s',
     'DETECT_TAPE_LIBRARY': '{0}Library?Action=detect',
     'CONFIGURE_TAPE_LIBRARY': '{0}Library?Action=configureTape',
-    
+
+    'GET_MOVE_MOUNTPATH_DETAILS': '{0}MountPath/%s/Move',
+    'MOVE_MOUNTPATH': '{0}MountPath/Move',
+
     'LOCK_MM_CONFIGURATION': '{0}LockMMConfiguration',
 
     'STORAGE_POLICY': '{0}StoragePolicy',
     'GET_STORAGE_POLICY': '{0}StoragePolicy/%s',
+    'DELETE_STORAGE_POLICY': '{0}V2/StoragePolicy',
     'GET_STORAGE_POLICY_ADVANCED': '{0}v2/StoragePolicy/%s?propertyLevel=10',
     'CREATE_STORAGE_POLICY_COPY': '{0}StoragePolicy?Action=createCopy',
     'DELETE_STORAGE_POLICY_COPY': '{0}StoragePolicy?Action=deleteCopy',
     'SCHEDULE_POLICY': '{0}SchedulePolicy',
     'CREATE_UPDATE_SCHEDULE_POLICY': '{0}Task',
     'GET_SCHEDULE_POLICY': '{0}SchedulePolicy/%s',
     'MEDIA_AGENT': '{0}MediaAgent/%s',
@@ -246,17 +252,21 @@
     'ADD_CONTAINER': '{0}PerformContainerOperation',
     'DELETE_CONTAINER': '{0}Containers/Action/Delete',
     'CA_UPLOAD_FILE': '{0}ContentAnalyzer/%s/action/uploadFile',
     'GET_CLASSIFIERS': '{0}dcube/classifiers?getDisabled=True',
     'START_TRAINING': '{0}ContentAnalyzer/%s/%s/ml/action/train',
     'CANCEL_TRAINING': '{0}ContentAnalyzer/%s/%s/training/cancel',
 
-    'EDISCOVERY_INVENTORIES': '{0}EDiscoveryClients/Inventories',
-    'EDISCOVERY_INVENTORY': '{0}EDiscoveryClients/Inventories/%s',
-    'EDISCOVERY_ASSETS': '{0}EDiscoveryClients/Inventories/%s/Assets',
+    'V4_ACTIVATE_DS_PERMISSION': '{0}V4/Activate/SEA_DATASOURCE_ENTITY/%s/Permissions',
+    'V4_INVENTORY_CRAWL': '{0}V4/InventoryManager/Inventory/%s/Crawl',
+    'EDISCOVERY_INVENTORIES': '{0}V4/InventoryManager/Inventory',
+    'EDISCOVERY_INVENTORY': '{0}V4/InventoryManager/Inventory/%s',
+    'EDISCOVERY_ASSETS': '{0}V4/InventoryManager/Inventory/%s/Assets',
+    'EDISCOVERY_ASSET': '{0}V4/InventoryManager/Inventory/%s/Assets/%s',
+    'EDISCOVERY_ASSET_JOBS': '{0}V4/InventoryManager/Inventory/%s/Assets/%s/jobs',
     'EDISCOVERY_CRAWL': '{0}EDiscoveryClients/Clients/%s/Jobs?datasourceId=%s&type=%s&operation=%s',
     'EDISCOVERY_JOBS_HISTORY': '{0}EDiscoveryClients/Clients/%s/Jobs/History?type=%s&datasourceId=%s',
     'EDISCOVERY_JOB_STATUS': '{0}EDiscoveryClients/Clients/%s/Jobs/Status?type=%s&datasourceId=%s',
     'EDISCOVERY_GET_DEFAULT_HANDLER': '{0}dcube/getdefaulthandler/%s',
     'EDISCOVERY_V2_GET_CLIENTS': '{0}V2/EDiscoveryClients/Clients?datasourceType=%s&clientGroup=%s&limit=%s&offset=%s&sortBy=%s&sortDir=%s',
     'EDISCOVERY_V2_GET_CLIENT_DETAILS': '{0}V2/EDiscoveryClients/Clients/%s?includeDocCount=%s&limit=%s&offset=%s&sortBy=%s&sortDir=%s&datasourceType=%s',
     'EDISCOVERY_V2_GET_CLIENT_GROUP_DETAILS': '{0}V2/EDiscoveryClients/ClientGroups/%s?includeDocCount=%s',
@@ -293,30 +303,35 @@
     'PLAN': '{0}V2/Plan/%s',
     'DELETE_PLAN': '{0}V2/Plan/%s?confirmDelete=True',
     'ADD_USERS_TO_PLAN': '{0}V2/Plan/%s/Users',
     'GET_PLAN_TEMPLATE': '{0}V2/Plan/template?type=%s&subType=%s',
     'ELIGIBLE_PLANS': '{0}V2/Plan/Eligible?%s',
     'ASSOCIATED_ENTITIES': '{0}V2/Plan/%s/AssociatedEntities',
     'GET_PLANS': '{0}V2/Plan?type=%s&subType=%s',
+    'APPLICABLE_SOLNS_ENABLE': '{0}V4/ServerPlan/%s/ApplicableSolutions/Restrict/Enable',
+    'APPLICABLE_SOLNS_DISABLE': '{0}V4/ServerPlan/%s/ApplicableSolutions/Restrict/Disable',
+    'PLAN_SUPPORTED_SOLUTIONS': '{0}V4/Solutions?filter=PLAN_SUPPORTED_SOLUTIONS',
 
     'DOMAIN_CONTROLER': '{0}CommCell/DomainController',
     'DELETE_DOMAIN_CONTROLER': '{0}CommCell/DomainController/%s',
     'DOMAIN_PROPERTIES': '{0}CommCell/DomainController?domainId=%s',
 
     'DRBACKUP': '{0}/CommServ/DRBackup',
     'DISASTER_RECOVERY_PROPERTIES': '{0}/Commcell/DRBackup/Properties',
     'CVDRBACKUP_STATUS': '{0}/cvdrbackup/status?commcellid=%s',
     'CVDRBACKUP_INFO': '{0}/cvdrbackup/info',
     'CVDRBACKUP_DOWNLOAD': '{0}/cvdrbackup/download',
-    'CVDRBACKUP_REQUEST': '{0}cvdrbackup/requests',
+    'CVDRBACKUP_REQUEST': '{0}/cvdrbackup/requests',
+    'CVDRBACKUP_REQUEST_HISTORY': '{0}/cr/reportsplusengine/datasets/%s/data/?parameter.duration=%s',
 
     'ORACLE_INSTANCE_BROWSE': '{0}Instance/DBBrowse/%s',
 
     'METRICS': '{0}CommServ/MetricsReporting',
     'GET_METRICS': '{0}CommServ/MetricsReporting?isPrivateCloud=%s',
+    'LOCAL_METRICS': '{0}CommServ/MetricsReporting?isLocalMetrics=%s',
 
     'INTERNET_PROXY': '{0}/Commcell/InternetOptions/Proxy',
 
     'PASSWORD_ENCRYPTION_CONFIG': '{0}/Commcell/PasswordEncryptionConfig',
 
     'VM_ALLOCATION_POLICY': '{0}VMAllocationPolicy',
     'ALL_VM_ALLOCATION_POLICY': '{0}VMAllocationPolicy?showResourceGroupPolicy=true&deep=false&hiddenpolicies=true',
@@ -324,14 +339,16 @@
     'PROTECTED_VMS': "{0}VM?propertyLevel=AllProperties&status=1&fromTime=%s&toTime=%s&Limit=%s",
     'CONTINUOUS_REPLICATION_MONITOR': "{0}Replications/Monitors/continuous",
     'USERS': '{0}User',
     'USER': '{0}User/%s?Level=50',
     'DELETE_USER': '{0}User/%s?newUserId=%s&newUserGroupId=%s',
     'OTP': '{0}User/%s/preferences/OTP',
 
+    'UNLOCK': '{0}User/Unlock',
+
     'ROLES': '{0}Role',
     'ROLE': '{0}Role/%s',
 
     'ALL_CREDENTIALS': '{0}/CommCell/Credentials?propertyLevel=30',
     'ONE_CREDENTIAL': '{0}/CommCell/Credentials/%s?propertyLevel=30',
     'CREDENTIAL':   '{0}/Commcell/Credentials',
     'DELETE_RECORD': '{0}/Commcell/Credentials/action/delete',
@@ -355,20 +372,22 @@
     'UPDATE_ORGANIZATION': '{0}Organization?organizationId=%s',
     'GENERATE_AUTH_CODE': '{0}Organization/%s/Authtoken',
     'ACTIVATE_ORGANIZATION': '{0}Organization/%s/action/activate',
     'DEACTIVATE_ORGANIZATION': '{0}Organization/%s/action/deactivate',
     'ORGANIZATION_ASSOCIATION': '{0}company/%s/company-association',
     'ENABLE_PRIVACY_COMPANY_DATA': '{0}V2/Organization/%s/Privacy/Action/Lock',
     'DISABLE_PRIVACY_COMPANY_DATA': '{0}V2/Organization/%s/Privacy/Action/Unlock',
+    'ORGANIZATION_THEME': '{0}V2/Organization/%s/Customization',
     'ORGANIZATION_TAGS' : '{0}Tags',
     'GET_ORGANIZATION_TAGS' : '{0}Tags/PROVIDER_ENTITY/%s',
     'COMPANY_PASSKEY' : '{0}Company/%s/Passkey',
     'COMPANY_AUTH_RESTORE' : '{0}Company/%s/AuthRestore',
     'EDIT_COMPANY_DETAILS': '{0}v4/company/%s',
     'CHECK_ELIGIBILITY_MIGRATION' : '{0}Company/%s/migration-entities',
+    'COMPANY_ENTITIES': '{0}Company/%s/AssociatedEntities',
     'MIGRATE_CLIENTS' : '{0}Company/%s/company-association',
 
     'STORAGE_POOL': '{0}StoragePool',
     'GET_STORAGE_POOL': '{0}StoragePool/%s',
     'ADD_STORAGE_POOL': '{0}StoragePool?Action=create',
     'DELETE_STORAGE_POOL': '{0}StoragePool/%s',
     'EDIT_STORAGE_POOL': '{0}StoragePool?Action=edit',
@@ -392,14 +411,20 @@
 
     'DR_GROUPS': '{0}DRGroups',
     'GET_DR_GROUP': '{0}DRGroups/%s',
     'DR_GROUP_MACHINES': '{0}DRGroups/ClientList?source=1&entityType=3&entityId=%s',
     'DR_GROUP_JOB_STATS': '{0}DRGroups/JobStats?jobId=%s&drGroupId=%s&replicationId=%s&clientId=0',
     'DR_JOB_STATS': '{0}DRGroups/JobStats?jobId=%s',
 
+    'FAILOVER_GROUPS': '{0}FailoverGroups',
+    'GET_FAILOVER_GROUP': '{0}FailoverGroups/%s',
+    'FAILOVER_GROUP_MACHINES': '{0}FailoverGroups/ClientList?source=1&entityType=3&entityId=%s',
+    'FAILOVER_GROUP_JOB_STATS': '{0}DR/JobStats?jobId=%s&failoverGroupId=%s&replicationId=%s&clientId=0',
+    'DRORCHESTRATION_JOB_STATS': '{0}DR/JobStats?jobId=%s',
+
     'REVERSE_REPLICATION_TASK': '{0}Replications/Monitors/streaming/Operation',
     'REPLICATION_MONITOR': '{0}Replications/Monitors/streaming?subclientId=0',
     'RPSTORE': '{0}Replications/RPStore',
 
     'CREATE_PSEUDO_CLIENT': '{0}pseudoClient',
     'CREATE_NAS_CLIENT': '{0}NASClient',
     'GET_OFFICE_365_ENTITIES': '{0}Office365/entities',
@@ -448,16 +473,16 @@
     'GET_CLOUDAPPS_USERS': '{0}Instance/%s/CloudDiscovery?clientId=%s&eDiscoverType=%s',
     'GET_CLOUDAPPS_ONEDRIVE_USERS': '{0}Instance/%s/CloudDiscovery?clientId=%s&eDiscoverType=%s&subclientId=%s',
     'ENABLE_CLIENT_PRIVACY': '{0}/V3/Client/%s/Lock',
     'DISABLE_CLIENT_PRIVACY': '{0}/V3/Client/%s/Unlock',
 
     'IDENTITY_APPS': '{0}ThirdParty/App',
 
-    'GLOBAL_PARAM': '{0}/setGlobalParam',
-    'GET_GLOBAL_PARAM': '{0}/CommServ/AddRemoveSoftware/CommServeSoftwareCache',
+    'SET_GLOBAL_PARAM': '{0}/setGlobalParam',
+    'GET_GLOBAL_PARAM': '{0}/CommServ/GlobalParams',
 
     'SNAP_OPERATIONS': '{0}/Snaps/Operations',
     'STORAGE_ARRAYS': '{0}/StorageArrays',
 
     'GET_NETWORK_SUMMARY' :'{0}/FirewallSummary/%s',
     'NETWORK_TOPOLOGIES': '{0}FirewallTopology',
     'NETWORK_TOPOLOGY': '{0}FirewallTopology/%s',
@@ -486,14 +511,15 @@
     'DASHBOARD_ENVIRONMENT_TILE': '{0}clients/count?type=fileserver,vm,laptop',
     'DASHBOARD_NEEDS_ATTENTION_TILE': '{0}CommServ/Anomaly/Entity/Count?anomalousEntityType=14',
 
     'GET_ALL_LIVE_SYNC_PAIRS': '{0}Replications/Monitors/streaming?subclientId=%s',
     'GET_ALL_LIVE_SYNC_VM_PAIRS': '{0}Replications/Monitors/streaming?subclientId=%s&taskId=%s',
     'GET_LIVE_SYNC_VM_PAIR': '{0}Replications/Monitors/streaming?subclientId=%s&replicationPairId=%s',
     'GET_REPLICATION_PAIR': '{0}Replications/Monitors/streaming?replicationPairId=%s',
+    'GET_REPLICATION_PAIRS': '{0}Replications/Monitors/streaming?',
 
     'BACKUP_NETWORK_PAIRS': '{0}CommServ/DataInterfacePairs?ClientId=%s',
     'BACKUP_NETWORK_PAIR': '{0}CommServ/DataInterfacePairs',
 
     'GET_ALL_RECOVERY_TARGETS':
         '{0}/VMAllocationPolicy?showResourceGroupPolicy=true&showNonResourceGroupPolicy=false&deep=true',
     'GET_RECOVERY_TARGET': '{0}/VMAllocationPolicy/%s',
@@ -516,19 +542,34 @@
     'METALLIC_COMPLETED_SETUPS': '{0}CloudService/CompletedSetups',
     'USER_MAPPINGS': '{0}GetUserMappings',
     'METALLIC_REGISTERED': '{0}CloudServices/Registered',
     'METALLIC_UNLINK': '{0}CloudService/Unsubscribe',
     'ADD_OR_GET_SAML': '{0}/v4/SAML',
     'EDIT_SAML': '{0}/v4/SAML/%s',
 
+    'REGIONS': '{0}/v4/Regions',
     'EDIT_REGION': '{0}/entity/%s/%s/region',
     'GET_REGION': '{0}/entity/%s/%s/region?entityRegionType=%s',
     'CALCULATE_REGION': '{0}/entity/%s/%s/region?calculate=True&entityRegionType=%s',
     
-    'GET_OEM_ID': '{0}/GetOemId'
+    'GET_OEM_ID': '{0}/GetOemId',
+
+    'DO_WEB_SEARCH': '{0}/Search',
+
+    
+    'GET_SLA': '{0}GetSLAConfiguration',
+    'WORKLOAD_REGION': '{0}entity/COMMCELL/%s/region?entityRegionType=WORKLOAD',
+
+    'GET_USER_SUGGESTIONS': '{0}getADUserSuggestions?namePattern=%s&getDomainUsers=true&getCommcellUsers=true&'
+                            'getDomainGroups=true&returnDomain=true&getCommCellGroups=true&searchOnDisplayName=true'
+                            '&searchOnAliasName=true&searchOnSmtp=1&ignoreSmtpRule=1&getOrganizationUsers=false&'
+                            'getOrganizationGroups=false',
+    'DOMAIN_SSO': '{0}V4/LDAP/%s',
+
+    'VM_GROUP': '{0}V4/VmGroup/%s'
 }
 
 
 def get_services(web_service):
     """Initializes the SERVICES DICT with the web service for APIs.
 
         Args:
```

### Comparing `cvpysdk-11.30.1/cvpysdk/storage.py` & `cvpysdk-11.32/cvpysdk/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # limitations under the License.
 # --------------------------------------------------------------------------
 
 """Main file for performing storage related operations on the commcell.
 
 This file has all the classes related to Storage operations.
 
+
 MediaAgents:      Class for representing all the media agents attached to the commcell.
 
 MediaAgent:       Class for representing a single media agent attached to the commcell.
 
 DiskLibraries:    Class for representing all the disk libraries attached to the commcell.
 
 DiskLibrary:      Class for representing a single disk library associated with the commcell.
@@ -94,14 +95,17 @@
 
     set_state()                    -- enables/disables media agent
 
     mark_for_maintenance() -- marks/unmarks media agent offline for maintenance
 
     set_ransomware_protection()  -- set / unset ransomware protection on Windows MA
 
+    set_concurrent_lan()        --  set / unset concurrent LAN backup in Media agent properties.
+
+    is_power_management_enabled() -- returns of power management is enabled or not
 
 Libraries:
 
     __init__()               --  initialize the instance of Libraries class
     
     _get_libraries           --  Gets all the libraries associated to the commcell specified by commcell object
     
@@ -373,15 +377,15 @@
                 return MediaAgent(self._commcell_object,
                                   media_agent_name,
                                   self._media_agents[media_agent_name]['id'])
 
             raise SDKException(
                 'Storage', '102', 'No media agent exists with name: {0}'.format(media_agent_name)
             )
-    
+
     def delete(self, media_agent, force=False):
         """Deletes the media agent from the commcell.
 
             Args:
                 media_agent (str)  --  name of the Mediaagent to remove from the commcell
                 
                 force       (bool)     --  True if you want to delete media agent forcefully.
@@ -411,24 +415,24 @@
                     mediagent_delete_service += "?forceDelete=1"
 
                 flag, response = self._commcell_object._cvpysdk_object.make_request('DELETE', mediagent_delete_service)
 
                 error_code = 0
                 if flag:
                     if 'errorCode' in response.json():
-                        o_str = 'Failed to delete mediaagent' 
-                        error_code = response.json()['errorCode'] 
+                        o_str = 'Failed to delete mediaagent'
+                        error_code = response.json()['errorCode']
                         if error_code == 0:
                             # initialize the mediaagents again
                             # so the mediaagents object has all the mediaagents
                             self.refresh()
-                        else:                                
+                        else:
                             error_message = response.json()['errorMessage']
                             if error_message:
-                                o_str += '\nError: "{0}"'.format(error_message)                        
+                                o_str += '\nError: "{0}"'.format(error_message)
                             raise SDKException('Storage', '102', o_str)
                     else:
                         raise SDKException('Response', '102')
                 else:
                     raise SDKException('Response', '101', self._commcell_object._update_response_(response.text))
             else:
                 raise SDKException(
@@ -949,14 +953,61 @@
                 if response.get('error', {}).get('errorCode', -1) != 0:
                     error_message = response.get('error', {}).get('errorString', '')
                     raise SDKException('Storage', '102', error_message)
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101')
+    
+    def set_concurrent_lan(self, enable=True):
+        """
+        disable / enable concurrent LAN backup in Media agent properties.
+            Args:
+            enable      -   (bool)
+                            True        - Enable concurent LAN Backup
+                            False       - Disable concurent LAN Backup
+
+        Returns:
+            None                   --   if operation performed successfully.
+
+        Raises:
+            SDKException:
+                - if there is failure in executing the operation
+
+        """
+
+        if type(enable) != bool:
+            raise SDKException('Storage', '101')
+
+        media_id = int(self.media_agent_id)
+        request_json = {
+            "mediaAgentInfo": {
+                "mediaAgent": {
+                    "mediaAgentId": media_id
+                },
+                "mediaAgentProps": {
+                    "optimizeForConcurrentLANBackups": enable
+                }
+            }
+        }
+
+        flag, response = self._commcell_object._cvpysdk_object.make_request(
+            'PUT', self._MEDIA_AGENTS, request_json
+        )
+
+        if flag:
+            if response and response.json():
+                response = response.json()
+                if response.get('error', {}).get('errorCode', -1) != 0:
+                    error_message = response.get('error', {}).get('errorString', '')
+                    raise SDKException('Storage', '102', error_message)
+            else:
+                raise SDKException('Response', '102')
+        else:
+            raise SDKException('Response', '101')
 
     @property
     def name(self):
         """Returns the media agent display name"""
         return self._media_agent_info['mediaAgent']['displayName']
 
     @property
@@ -986,14 +1037,19 @@
 
     @property
     def index_cache_enabled(self):
         """Treats the cache enabled value as a read-only attribute"""
         return self._index_cache_enabled
 
     @property
+    def is_power_management_enabled(self):
+        """ Returns power management enable status"""
+        return self._is_power_management_enabled
+
+    @property
     def current_power_status(self):
         """
                 Returns the power state of the MA.
 
                     Args :
                             self : Object
                     Returns :
@@ -1012,15 +1068,15 @@
     def refresh(self):
         """Refresh the properties of the MediaAgent."""
         self._initialize_media_agent_properties()
 
 
 class Libraries(object):
     """ Class for libraries"""
-    
+
     def __init__(self, commcell_object):
         """Initialize object of the DiskLibraries class.
 
             Args:
                 commcell_object (object)  --  instance of the Commcell class
 
             Returns:
@@ -1372,28 +1428,31 @@
         """String representation of the instance of this class."""
         representation_string = 'DiskLibrary class instance for library: "{0}" of Commcell: "{1}"'
         return representation_string.format(
             self.library_name, self._commcell_object.commserv_name
         )
 
     def move_mountpath(self, mountpath_id, source_device_path,
-                       source_mediaagent_id, target_device_path, target_mediaagent_id):
+                       source_mediaagent_id, target_device_path, target_mediaagent_id,
+                       target_device_id=0):
 
         """ To perform move mountpath operation
         Args:
             mountpath_id  (int)   --  Mountpath Id that need to be moved.
 
             source_device_path (str)   -- Present Mountpath location
 
             source_mediaagent_id    (int)   -- MediaAgent Id on which present mountpath exists
 
             target_device_path    (str)   -- New Mountpath location
 
             target_mediaagent_id    (int)   -- MediaAgent Id on which new mountpath exists
 
+            target_device_id        (int)   --  Device Id of target path if already exists
+
         Returns:
             instance of the Job class for this move mountpath job
 
         Raises
             Exception:
                 - if argument datatype is invalid
 
@@ -1403,57 +1462,73 @@
 
                 - if response code is not as expected
         """
 
         if not (isinstance(mountpath_id, int) and
                 isinstance(source_mediaagent_id, int) and
                 isinstance(target_mediaagent_id, int) and
-                isinstance(target_device_path, str) and
+                (isinstance(target_device_path, str) or target_device_id > 0) and
                 isinstance(source_device_path, str)):
             raise SDKException('Storage', '101')
 
-        request_xml = """<TMMsg_CreateTaskReq>
-                        <taskInfo>
-                            <task initiatedFrom="1" ownerId="1" sequenceNumber="0" taskId="0" taskType="1">
-                                <taskFlags disabled="0" />
-                            </task>
-                            <associations mountPathId="{1}" />
-                            <subTasks subTaskOperation="1">
-                                <subTask operationType="5017" subTaskType="1" />
-                                <options> <adminOpts> <libraryOption>
-                                    <library libraryId="{0}" />
-                                    <moveMPOption>
-                                        <mountPathMoveList mountPathId="{1}" sourceDevicePath="{2}" 
-                                        sourcemediaAgentId="{3}" targetDevicePath="{4}" targetMediaAgentId="{5}">
-                                        <credential credentialId="0" credentialName=" " />
-                                        </mountPathMoveList>
-                                    </moveMPOption>
-                                </libraryOption> </adminOpts> </options>
-                            </subTasks>
-                        </taskInfo>
-                    </TMMsg_CreateTaskReq>""".format(self.library_id, mountpath_id, source_device_path,
-                                                     source_mediaagent_id, target_device_path, target_mediaagent_id)
+        MOVE_MOUNTPATH_DETAILS = self._commcell_object._services['GET_MOVE_MOUNTPATH_DETAILS'] % (mountpath_id)
+
+        flag, response = self._commcell_object._cvpysdk_object.make_request('GET', MOVE_MOUNTPATH_DETAILS)
+
+        source_device_id = None
+
+        if flag:
+            if response.json():
+                if 'sourceDeviceInfo' in response.json():
+                    source_device_id = response.json().get('sourceDeviceInfo').get('deviceId', None)
+                if not source_device_id:
+                    raise SDKException('Storage', '102', 'Failed to get details of the mountpath for move')
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._commcell_object._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+        request_json = {
+            'MPMoveOption': {
+                'mountPathMoveList': [{
+                    'sourceDeviceId': source_device_id,
+                    'sourcemediaAgentId': source_mediaagent_id,
+                    'targetMediaAgentId': target_mediaagent_id,
+                }]
+            }
+        }
+        if target_device_id > 0:
+            request_json['MPMoveOption']['mountPathMoveList'][0]['targetDeviceId'] = target_device_id
+        else:
+            request_json['MPMoveOption']['mountPathMoveList'][0]['targetDevicePath'] = target_device_path
 
         flag, response = self._commcell_object._cvpysdk_object.make_request(
-            'POST', self._commcell_object._services['CREATE_TASK'], request_xml)
+            'POST', self._commcell_object._services['MOVE_MOUNTPATH'], request_json)
 
         if flag:
             if response.json():
                 if "jobIds" in response.json():
-                    from cvpysdk.job import Job
-                    return Job(self._commcell_object, response.json()['jobIds'][0])
+                    if len(response.json()['jobIds']) == 1:
+                        from cvpysdk.job import Job
+                        return Job(self._commcell_object, response.json()['jobIds'][0])
+                    else:
+                        from cvpysdk.job import Job
+                        mp_move_job_list = []
+                        for job_id in response.json()['jobIds']:
+                            mp_move_job_list.append(Job(self._commcell_object, job_id))
+                        return mp_move_job_list
 
                 if "errorCode" in response.json():
                     error_message = response.json()['errorMessage']
                     o_str = 'Error: "{0}"'.format(error_message)
                     raise SDKException('Commcell', '105', o_str)
 
                 else:
                     raise SDKException('Commcell', '105')
-
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101', self._commcell_object._update_response_(response.text))
 
     def validate_mountpath(self, mountpath_drive_id, media_agent):
 
@@ -1923,21 +1998,17 @@
                 }
         }
         self._commcell_object.qoperation_execute(request_json)
 
     @property
     def media_agents_associated(self):
         """ Returns the media agents associated with the disk library """
-        media_agents = self._library_properties['magLibSummary'].get(
-            'associatedMediaAgents', None)
-        if media_agents is None:
-            mount_paths = self._library_properties.get('MountPathList')
-            media_agents = [mount_path.get('mediaAgents') for mount_path in mount_paths if "mediaAgents" in mount_path]
-            return media_agents
-        return media_agents.strip().split(",")
+        mount_paths = self._library_properties.get('MountPathList')
+        media_agents = [mount_path.get('mountPathName').split('[')[1].split(']')[0] for mount_path in mount_paths if "mountPathName" in mount_path]
+        return list(set(media_agents))
 
     @property
     def name(self):
         """Returns library display name."""
         return self._library_properties['MountPathList'][0]['mountPathSummary']['libraryName']
 
     @property
@@ -1971,15 +2042,15 @@
         """Treats the library id as a read-only attribute."""
         return self.mediaagent
 
     @media_agent.setter
     def media_agent(self, media_agent):
         """setter for media agent"""
         self.mediaagent = media_agent
-        
+
     def share_mount_path(self, new_media_agent, new_mount_path, **kwargs):
         """
         Method to share a mountpath to a disklibrary
 
         Args:
         
             new_media_agent (str)   -- Media agent which is accessing the shared mount path
@@ -2036,22 +2107,22 @@
 
                 - if API response error code is not 0
 
                 - if response is empty
 
                 - if response code is not as expected
         """
-        
+
         media_agent = kwargs.get('media_agent', self.mediaagent)
         library_name = kwargs.get('library_name', self.library_name)
         mount_path = kwargs.get('mount_path', self.mountpath)
         access_type = kwargs.get('access_type', 22)
         username = kwargs.get('username', '')
         password = kwargs.get('password', '')
-       
+
         self._EXECUTE = self._commcell_object._services['EXECUTE_QCOMMAND']
         self.library = {
             "opType": 64,
             "mediaAgentName": media_agent,
             "libraryName": library_name,
             "mountPath": "%s" %
                          mount_path}
@@ -2104,16 +2175,18 @@
         self.refresh()
 
     def _get_rp_stores(self):
         xml = '<?xml version="1.0" encoding="UTF-8"?><EVGui_GetLibraryListWCReq libraryType="RPSTORE"/>'
         response = self._commcell.execute_qcommand("qoperation execute", xml)
 
         try:
-            return {library["library"]["libraryName"].lower(): library["MountPathList"][0]["rpStoreLibraryInfo"]
-                    ["rpStoreId"] for library in response.json()["libraryList"]}
+            if response.json().get('libraryList'):
+                return {library["library"]["libraryName"].lower(): library["MountPathList"][0]["rpStoreLibraryInfo"]
+                        ["rpStoreId"] for library in response.json()["libraryList"]}
+            return {}
         except (KeyError, ValueError):
             generic_msg = "Unable to fetch RPStore"
             err_msg = response.json().get("errorMessage", generic_msg) if response.status_code == 200 else generic_msg
             raise SDKException('Storage', '102', '{0}'.format(err_msg))
 
     def add(self, name, path, storage, media_agent_name):
         """
@@ -2440,17 +2513,17 @@
                 }
                 flag, response = self._commcell_object._cvpysdk_object.make_request('POST', self._CONFIGURE_TAPE_LIBRARY,
                                                                                     pay_load)
                 break
 
         if not flag:
             raise SDKException('Storage', '102', "Failed to configure the library")
-            
+
         self.refresh()
-        
+
         tape_library_name = tape_library_name.lower()
         for lib_name, lib_id in self._libraries.items():
             if lib_name.startswith(tape_library_name + " "):
                 return self.get(lib_name)
 
 
 
@@ -2514,20 +2587,20 @@
     def get_drive_list(self):
         """
             Returns the tape drive list of this tape library
 
             Returns:
                 list - List of the drives of this tape library
         """
-        
+
         self.refresh()
-        
-        drive_list=[]
 
-        if self.library_properties["DriveList"]:
+        drive_list=[]
+        
+        if 'DriveList' in self.library_properties:
             for drive in self.library_properties["DriveList"]:
                 drive_list.append(drive["driveName"])
 
         return drive_list
 
 
     def _get_library_properties(self):
@@ -2557,15 +2630,15 @@
         response_string = self._commcell_object._update_response_(response.text)
         raise SDKException('Response', '101', response_string)
 
 
     def refresh(self):
         """Refresh the properties of this tape library."""
         self.library_properties = self._get_library_properties()
-        
+
 
     @property
     def library_name(self):
         """Treats the library name as a read-only attribute."""
         return self._name
 
     @property
```

### Comparing `cvpysdk-11.30.1/cvpysdk/storage_pool.py` & `cvpysdk-11.32/cvpysdk/storage_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
     get()                       --  returns StoragePool object of the storage pool for the
                                     specified input name
 
     add()                       --  Adds a storage pool, according to given input and returns
                                     StoragePool object
 
+    add_azure_storage_pool()    --  Adds new storage pool with provided name to the commcell
+
     delete()                    --  deletes the specified storage pool
 
     refresh()                   --  refresh the list of storage pools associated with the commcell
 
 
 Attributes
 ----------
@@ -80,24 +82,26 @@
 **storage_policy_id**           --  returns the storage pool id
 
 
 # TODO: check with MM API team to get the response in JSON
 
 
 """
+import copy
 
 import xmltodict
 
 from .exception import SDKException
 
 # from .job import Job
 
 from .storage import DiskLibrary
 from .storage import MediaAgent
 from .security.security_association import SecurityAssociation
+from .constants import StoragePoolConstants
 
 
 class StoragePools:
     """Class for doing operations on Storage Pools, like get storage poo ID."""
 
     def __init__(self, commcell_object):
         """Initializes instance of the StoragePools class to perform operations on a storage pool.
@@ -267,47 +271,47 @@
 
         """
         name = name.lower()
 
         if self.has_storage_pool(name):
             return StoragePool(self._commcell_object, name, storage_pool_id=self._storage_pools[name])
         else:
-            raise SDKException('StoragePool', '103')    
-    
+            raise SDKException('StoragePool', '103')
+
     def hyperscale_create_storage_pool(self, storage_pool_name, media_agents):
         """
             Create new storage pool for hyperscale
             Args:
                 storage_pool_name (string) -- Name of the storage pools to create
                 
                 media_agents      (List)   -- List of 3 media agents with name's(str)
                                                 or instance of media agent's(object)
                                                 
                 Example: ["ma1","ma2","ma3"]
 
             Return:
                  flag, response -- response returned by the REST API call
         """
-        
+
         if not isinstance(media_agents, list):
             raise SDKException('Storage', '101')
         if not isinstance(storage_pool_name, str):
             raise SDKException('Storage', '101')
-        
+
         mediagent_obj = []
         for media_agent in media_agents:
             if isinstance(media_agent, MediaAgent):
                 mediagent_obj.append(media_agent)
             elif isinstance(media_agent, str):
                 mediagent_obj.append(self._commcell_object.media_agents.get(media_agent))
             else:
                 raise SDKException('Storage', '103')
         if len(mediagent_obj) <= 2:
             raise SDKException('Storage', '102', "minimum 3 media agents are required")
-        
+
         request_xml = """<App_CreateStoragePolicyReq storagePolicyName="{0}" copyName="{0}_Primary" type="1"
                                      numberOfCopies="1">
                                     <storagePolicyCopyInfo>
                                         <storagePolicyFlags scaleOutStoragePolicy="1"/>
                                     </storagePolicyCopyInfo>
                                     <storage>
                                         <mediaAgent mediaAgentId="{4}" mediaAgentName="{1}" displayName="{1}"/>
@@ -320,15 +324,15 @@
                                     </storage>
                                     <scaleoutConfiguration configurationType="1"/>
                                 </App_CreateStoragePolicyReq>
                                 """.format(storage_pool_name, mediagent_obj[0].media_agent_name,
                                            mediagent_obj[1].media_agent_name, mediagent_obj[2].media_agent_name,
                                            mediagent_obj[0].media_agent_id, mediagent_obj[1].media_agent_id,
                                            mediagent_obj[2].media_agent_id)
-        
+
         flag, response = self._commcell_object._cvpysdk_object.make_request(
             'POST', self._add_storage_pool_api, request_xml
         )
         if flag:
             if response.json():
                 error_code = response.json()['error']['errorCode']
 
@@ -467,14 +471,98 @@
         else:
             response_string = self._commcell_object._update_response_(response.text)
             raise SDKException('Response', '101', response_string)
 
         self.refresh()
         return self.get(storage_pool_name)
 
+    def add_azure_storage_pool(self, storage_pool_name, container_name, media_agents, dedup_paths, **kwargs):
+        """ Adds new storage pool with provided name to the commcell
+                 Args:
+                     storage_pool_name (str)     --  name of the storage pool to be created
+
+                     container_name (str)        --  container name to be used with storage pool
+
+                     media_agents (list)         --  list of media agent names to be used for storage pool
+
+                     dedup_paths (list)          --  list of paths for storing deduplication data
+
+                     **kwargs (dict)             --  dict of keyword arguments as follows
+                         username        (str)   --  azure storage credential username
+                         password        (str)   --  azure storage credential password
+                         credential_name (str)   --  Credential name to be used
+
+                 Returns:
+                     Azure storage policy object
+
+                 Raises:
+                     SDKException:
+                         If invalid type arguments are passed
+                         If Storage Pool with given name already exist
+                         Response was not success.
+                         Response was empty.
+
+        """
+        username = kwargs.get("username", "")
+        password = kwargs.get("password", "")
+        credential_name = kwargs.get("credential_name", "")
+        if not (isinstance(storage_pool_name, str) and isinstance(container_name, str)
+                and isinstance(media_agents, list) and isinstance(dedup_paths, list)
+                and isinstance(username, str) and isinstance(password, str)
+                and isinstance(credential_name, str)):
+            raise SDKException('StoragePool', '101')
+        storage_pools = self._commcell_object.storage_pools
+        if storage_pools.has_storage_pool(storage_pool_name):
+            raise SDKException('StoragePool', '103')
+        request_json = copy.deepcopy(StoragePoolConstants.AZURE_STORAGE_REQ_JSON)
+        request_json["storagePolicyName"] = storage_pool_name
+        storage_policy_info = request_json["storagePolicyCopyInfo"]
+        storage_ma = self._commcell_object.media_agents.get(media_agents[0])
+        storage_policy_info["library"]["libraryName"] = container_name
+        storage_policy_info["mediaAgent"]["mediaAgentId"] = int(storage_ma.media_agent_id)
+        storage_policy_info["mediaAgent"]["mediaAgentName"] = storage_ma.media_agent_name
+        ddb_info = []
+        for (ma, ddb_path) in zip(media_agents, dedup_paths):
+            ma_ddb = copy.deepcopy(StoragePoolConstants.MA_INFO_LIST)
+            ma_info = self._commcell_object.media_agents.get(ma)
+            ma_ddb["mediaAgent"]["mediaAgentId"] = int(ma_info.media_agent_id)
+            ma_ddb["mediaAgent"]["mediaAgentName"] = ma_info.media_agent_name
+            ma_ddb["subStoreList"][0]["accessPath"]["path"] = ddb_path
+            ddb_info.append(ma_ddb)
+        storage_policy_info["DDBPartitionInfo"]["maInfoList"] = ddb_info
+        storage_info = request_json["storage"][0]
+        storage_info["path"] = container_name
+        storage_info["mediaAgent"]["mediaAgentId"] = int(storage_ma.media_agent_id)
+        storage_info["mediaAgent"]["mediaAgentName"] = storage_ma.media_agent_name
+        storage_info["credentials"]["userName"] = username
+        storage_info["credentials"]["password"] = password
+        credential = self._commcell_object.credentials.get(credential_name)
+        storage_info["savedCredential"]["credentialId"] = credential.credential_id
+        storage_info["savedCredential"]["credentialName"] = credential.credential_name
+        flag, response = self._commcell_object._cvpysdk_object.make_request(
+            'POST', self._add_storage_pool_api, request_json
+        )
+
+        if flag:
+            if response.json():
+                error_code = response.json().get('error', {}).get('errorCode', 0)
+                if int(error_code) != 0:
+                    error_message = response.json()['error']['errorMessage']
+                    o_str = 'Failed to create storage policy\nError: "{0}"'
+
+                    raise SDKException('StoragePool', '102', o_str.format(error_message))
+            else:
+                raise SDKException('Response', '102')
+        else:
+            response_string = self._commcell_object._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+        self.refresh()
+        return self.get(request_json["storagePolicyName"])
+
     def delete(self, storage_pool_name):
         """deletes the specified storage pool.
 
             Args:
                 storage_pool_name (str)  --  name of the storage pool to delete
 
             Raises:
@@ -525,15 +613,16 @@
                     '102',
                     'No storage pool exists with name: {0}'.format(storage_pool_name)
                 )
 
     def refresh(self):
         """Refresh the list of storage pools associated to the Commcell."""
         self._storage_pools = self._get_storage_pools()
-        
+
+
 class StoragePool(object):
     """Class for individual storage pools"""
 
     def __init__(self, commcell_object, storage_pool_name, storage_pool_id=None):
         """
         Intitalise the Storage Pool classs instance
 
@@ -601,15 +690,15 @@
         """Treats the storage_pool_properties as a read only attribute"""
         return self._storage_pool_properties
 
     @property
     def global_policy_name(self):
         """Returns the global policy corresponding to the storage pool"""
         return self._storage_pool_properties["storagePoolDetails"]["copyInfo"]["StoragePolicyCopy"]["storagePolicyName"]
-    
+
     def hyperscale_add_nodes(self, media_agents):
         """
         Add 3 new nodes to an existing storage pool
 
         args:
             media_agents      (List)   -- List of 3 media agents with name's(str)
                                             or instance of media agent's(object)
@@ -618,28 +707,27 @@
 
         Raises:
                 SDKException:
                     if add nodes to an existing storage pool fails
         """
         if not isinstance(media_agents, list):
             raise SDKException('Storage', '101')
-        
+
         mediagent_obj = []
-        for media_agent in media_agents:        
+        for media_agent in media_agents:
             if isinstance(media_agent, MediaAgent):
                 mediagent_obj.append(media_agent)
             elif isinstance(media_agent, str):
                 mediagent_obj.append(self._commcell_object.media_agents.get(media_agent))
             else:
                 raise SDKException('Storage', '103')
-                    
+
         if len(mediagent_obj) <= 2:
             raise SDKException('Storage', '102', "Minimum 3 MediaAgents required")
-        
-        
+
         request_json = {
             "scaleoutOperationType": 2,
             "StoragePolicy": {
                 "storagePolicyName": "{0}".format(self.storage_pool_name),
             },
             "storage": [
                 {
@@ -668,15 +756,15 @@
 
         self._edit_storage_pool_api = self._commcell_object._services[
             'EDIT_STORAGE_POOL']
 
         flag, response = self._commcell_object._cvpysdk_object.make_request(
             'POST', self._edit_storage_pool_api, request_json
         )
-        
+
         if flag:
             if response.json():
                 error_code = response.json()['errorCode']
 
                 if int(error_code) != 0:
                     error_message = response.json()['errorMessage']
                     o_str = 'Failed to add nodes to storage pool\nError: "{0}"'
@@ -699,25 +787,24 @@
         Raises:
                 SDKException:
                     if reconfigure fails
         """
         if not isinstance(storage_pool_name, str):
             raise SDKException('Storage', '101')
 
-
         request_json = {
 
             "scaleoutOperationType": 4,
             "StoragePolicy":
                 {
                     "storagePolicyName": "{0}".format(storage_pool_name),
                     "storagePolicyId": int("{0}".format(self.storage_pool_id))
 
                 }
-            }
+        }
 
         self._edit_storage_pool_api = self._commcell_object._services[
             'EDIT_STORAGE_POOL']
 
         flag, response = self._commcell_object._cvpysdk_object.make_request(
             'POST', self._edit_storage_pool_api, request_json
         )
@@ -806,15 +893,15 @@
 
         self.refresh()
 
     def refresh(self):
         """Refreshes propery of the class object"""
         self._get_storage_pool_properties()
 
-    def update_security_associations(self, associations_list, isUser = True, request_type = None, externalGroup = False):
+    def update_security_associations(self, associations_list, isUser=True, request_type=None, externalGroup=False):
         """
         Adds the security association on the storage pool object
 
         Args:
             associations_list   (list)  --  list of users to be associated
                 Example:
                     associations_list = [
@@ -823,21 +910,23 @@
                             'role_name': role1
                         },
                         {
                             'user_name': user2,
                             'role_name': role2
                         }
                     ]
- 
+
             isUser (bool)           --    True or False. set isUser = False, If associations_list made up of user groups
             request_type (str)      --    eg : 'OVERWRITE' or 'UPDATE' or 'DELETE', Default will be OVERWRITE operation
             externalGroup (bool)    --    True or False, set externalGroup = True. If Security associations is being done on External User Groups
 
         Raises:
             SDKException:
                 if association is not of List type
         """
         if not isinstance(associations_list, list):
             raise SDKException('StoragePool', '101')
 
-        SecurityAssociation(self._commcell_object, self)._add_security_association(associations_list, 
-                                        user= isUser, request_type = request_type, externalGroup = externalGroup)
+        SecurityAssociation(self._commcell_object, self)._add_security_association(associations_list,
+                                                                                   user=isUser,
+                                                                                   request_type=request_type,
+                                                                                   externalGroup=externalGroup)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclient.py` & `cvpysdk-11.32/cvpysdk/subclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 
     add()                       --  adds a new subclient to the backupset
 
     add_oracle_logical_dump_subclient()  --  add subclient for oracle logical dump
 
     add_postgresql_subclient()  --  Adds a new postgresql subclient to the backupset.
 
+     add_mysql_subclient()  --  Adds a new mysql subclient to the instance.
+
     add_virtual_server_subclient()  -- adds a new virtual server subclient to the backupset
 
     add_onedrive_subclient()   --  adds a new onedrive subclient to the instance
 
     get(subclient_name)         --  returns the subclient object of the input subclient name
 
     delete(subclient_name)      --  deletes the subclient (subclient name) from the backupset
@@ -537,25 +539,27 @@
                     return self.get(subclient_name)
 
             else:
                 raise SDKException('Response', '102')
         else:
             raise SDKException('Response', '101', self._update_response_(response.text))
 
-    def add(self, subclient_name, storage_policy,
+    def add(self, subclient_name, storage_policy=None,
             subclient_type=None, description='', advanced_options=None,
             pre_scan_cmd=None):
         """Adds a new subclient to the backupset.
 
             Args:
                 subclient_name      (str)   --  name of the new subclient to add
 
                 storage_policy      (str)   --  name of the storage policy to be associated
                 with the subclient
 
+                    default: None
+
                 subclient_type      (str)   --  type of subclient for sql server
 
                     default: None
 
                     Valid Values are:
 
                         - DATABASE
@@ -595,15 +599,14 @@
 
                     if response is not success
 
                     if subclient already exists with the given name
 
         """
         if not (isinstance(subclient_name, str) and
-                isinstance(storage_policy, str) and
                 isinstance(description, str)):
             raise SDKException('Subclient', '101')
 
         if self.has_subclient(subclient_name):
             raise SDKException(
                 'Subclient', '102', 'Subclient "{0}" already exists.'.format(
                     subclient_name)
@@ -615,15 +618,15 @@
                 self._backupset_object = self._instance_object.backupsets.get(
                     'defaultBackupSet')
             else:
                 self._backupset_object = self._instance_object.backupsets.get(
                     sorted(self._instance_object.backupsets.all_backupsets)[0]
                 )
 
-        if not self._commcell_object.storage_policies.has_policy(
+        if storage_policy and not self._commcell_object.storage_policies.has_policy(
                 storage_policy):
             raise SDKException(
                 'Subclient',
                 '102',
                 'Storage Policy: "{0}" does not exist in the Commcell'.format(
                     storage_policy)
             )
@@ -654,37 +657,41 @@
                         "dataBackupStoragePolicy": {
                             "storagePolicyName": storage_policy
                         }
                     },
                 }
             }
         }
+
+        if storage_policy is None:
+            del request_json["subClientProperties"]["commonProperties"]["storageDevice"]
+
         if pre_scan_cmd is not None:
             request_json["subClientProperties"]["commonProperties"]["prepostProcess"] = {
                 "runAs": 1,
                 "preScanCommand": pre_scan_cmd
             }
 
         if self._agent_object.agent_name == 'sql server':
             request_json['subClientProperties']['mssqlSubClientProp'] = {
                 'sqlSubclientType': self._sqlsubclient_type_dict[subclient_type]
             }
 
         return self._process_add_request(request_json)
 
     def add_oracle_logical_dump_subclient(
-                                 self,
-                                 subclient_name,
-                                 storage_policy,
-                                 dump_dir,
-                                 user_name,
-                                 domain_name,
-                                 password,
-                                 full_mode,
-                                 schema_value = None):
+            self,
+            subclient_name,
+            storage_policy,
+            dump_dir,
+            user_name,
+            domain_name,
+            password,
+            full_mode,
+            schema_value=None):
         """
         Method to add subclient for oracle logical dump.
         This method add two type of subclient full mode
         and schema mode. For full mode full_mode should be
         true and schema_value should be none and for schema
         mode full_mode should be false and schema_value should
         be list of values.Rest of thing should be same for both.
@@ -720,23 +727,22 @@
 
                     if storage policy does not exist
 
         """
         if not (isinstance(subclient_name, str) and
                 isinstance(storage_policy, str) and
                 isinstance(dump_dir, str) and
-                isinstance(user_name,str) and
+                isinstance(user_name, str) and
                 isinstance(domain_name, str) and
                 isinstance(password, str) and
                 isinstance(full_mode, bool)):
             raise SDKException('Subclient', '101')
         if (full_mode == False and not
-                isinstance(schema_value, list)):
-            raise SDKException('Subclient','101')
-
+        isinstance(schema_value, list)):
+            raise SDKException('Subclient', '101')
 
         if self.has_subclient(subclient_name):
             raise SDKException(
                 'Subclient', '102', 'Subclient "{0}" already exists.'.format(
                     subclient_name)
             )
 
@@ -756,69 +762,68 @@
                 'Subclient',
                 '102',
                 'Storage Policy: "{0}" does not exist in the Commcell'.format(
                     storage_policy)
             )
 
         request_json = {
-                "subClientProperties": {
-                    "subClientEntity": {
-                        "clientName": self._client_object.client_name,
-                        "instanceName": self._instance_object.instance_name,
-                        "appName": self._agent_object.agent_name,
-                        "backupsetName": self._backupset_object.backupset_name,
-                        "subclientName": subclient_name
+            "subClientProperties": {
+                "subClientEntity": {
+                    "clientName": self._client_object.client_name,
+                    "instanceName": self._instance_object.instance_name,
+                    "appName": self._agent_object.agent_name,
+                    "backupsetName": self._backupset_object.backupset_name,
+                    "subclientName": subclient_name
+                },
+                "oracleSubclientProp": {
+                    "data": False,
+                    "archiveDelete": False,
+                    "useSQLConntect": False,
+                    "dbSubclientType": 2,
+                    "mergeIncImageCopies": False,
+                    "selectiveOnlineFull": False,
+                    "protectBackupRecoveryArea": False,
+                    "selectArchiveLogDestForBackup": False,
+                    "backupSPFile": False,
+                    "backupControlFile": False,
+                    "backupArchiveLog": False,
+                    "validate": False,
+                },
+                "commonProperties": {
+                    "snapCopyInfo": {
+                        "useSeparateProxyForSnapToTape": False,
+                        "checkProxyForSQLIntegrity": False,
+                        "snapToTapeProxyToUseSource": False,
+                        "isSnapBackupEnabled": False,
+                        "IsOracleSposDriverEnabled": False,
+                        "isRMANEnableForTapeMovement": False
                     },
-                    "oracleSubclientProp": {
-                        "data": False,
-                        "archiveDelete": False,
-                        "useSQLConntect": False,
-                        "dbSubclientType": 2,
-                        "mergeIncImageCopies": False,
-                        "selectiveOnlineFull": False,
-                        "protectBackupRecoveryArea": False,
-                        "selectArchiveLogDestForBackup": False,
-                        "backupSPFile": False,
-                        "backupControlFile": False,
-                        "backupArchiveLog": False,
-                        "validate": False,
+                    "dbDumpConfig": {
+                        "fullMode": True,
+                        "database": "",
+                        "dumpDir": dump_dir,
+                        "parallelism": 2,
+                        "overrideInstanceUser": True,
+                        "sqlConnect": {
+                            "password": b64encode(password.encode()).decode(),
+                            "domainName": domain_name,
+                            "userName": user_name
+                        }
                     },
-                    "commonProperties": {
-                        "snapCopyInfo": {
-                            "useSeparateProxyForSnapToTape": False,
-                            "checkProxyForSQLIntegrity": False,
-                            "snapToTapeProxyToUseSource": False,
-                            "isSnapBackupEnabled": False,
-                            "IsOracleSposDriverEnabled": False,
-                            "isRMANEnableForTapeMovement": False
-                        },
-                        "dbDumpConfig": {
-                            "fullMode": True,
-                            "database": "",
-                            "dumpDir": dump_dir,
-                            "parallelism": 2,
-                            "overrideInstanceUser": True,
-                            "sqlConnect": {
-                                "password": b64encode(password.encode()).decode(),
-                                "domainName": domain_name,
-                                "userName": user_name
-                            }
+                    "storageDevice": {
+                        "dataBackupStoragePolicy": {
+                            "storagePolicyName": storage_policy
                         },
-                        "storageDevice": {
-                            "dataBackupStoragePolicy": {
-                                "storagePolicyName": storage_policy
-                            },
-                            "deDuplicationOptions": {
-                                "enableDeduplication": True
-                            }
+                        "deDuplicationOptions": {
+                            "enableDeduplication": True
                         }
                     }
                 }
             }
-
+        }
 
         if (full_mode == False):
             request_json["subClientProperties"]["commonProperties"]["dbDumpConfig"]["fullMode"] = False
             request_json["subClientProperties"]["commonProperties"]["dbDumpConfig"]["schema"] = schema_value
 
         return self._process_add_request(request_json)
 
@@ -921,14 +926,123 @@
                 },
                 "content": content_list
             }
         }
 
         return self._process_add_request(request_json)
 
+    def add_mysql_subclient(
+            self,
+            subclient_name,
+            storage_policy,
+            contents,
+            **kwargs
+    ):
+        """Adds a new mysql subclient to the instance.
+
+            Args:
+                subclient_name          (str)   --  name of the new subclient to add
+
+                storage_policy          (str)   --  name of the storage policy to be associated
+                with the subclient
+
+                contents                (list)  --  database list to be added as subclient content
+
+                kwargs      (dict)  -- dict of keyword arguments as follows
+
+                    no_of_backup_streams    (int)   --  No of backup streams to be used
+                    default: 1
+
+                    no_of_log_backup_streams    (int)   -- No of Transaction log backup streams
+                    default: 1
+
+                    full_instance_xtrabackup    (bool)  -- True if XtraBackup is selected for subclient
+                    default: False
+
+            Returns:
+                object  -   instance of the Subclient class
+
+            Raises:
+                SDKException:
+                    if subclient name argument is not of type string
+
+                    if storage policy argument is not of type string
+
+                    if conetnts argument is not of type list
+
+                    if contents is empty list
+
+                    if failed to create subclient
+
+                    if response is empty
+
+                    if response is not success
+
+                    if subclient already exists with the given name
+
+        """
+        if not (isinstance(subclient_name, str) and
+                isinstance(storage_policy, str) and
+                isinstance(contents, list)):
+            raise SDKException('Subclient', '101')
+
+        if self.has_subclient(subclient_name):
+            raise SDKException(
+                'Subclient', '102', 'Subclient "{0}" already exists.'.format(
+                    subclient_name)
+            )
+
+        if not self._commcell_object.storage_policies.has_policy(
+                storage_policy):
+            raise SDKException(
+                'Subclient',
+                '102',
+                'Storage Policy: "{0}" does not exist in the Commcell'.format(
+                    storage_policy)
+            )
+
+        if not contents:
+            raise SDKException(
+                'Subclient',
+                '102',
+                'Content list cannot be empty'
+            )
+
+        content_list = []
+        for content in contents:
+            content_list.append({"mySQLContent": {"databaseName": content}})
+
+        request_json = {
+            "subClientProperties": {
+                "contentOperationType": 2,
+                "subClientEntity": {
+                    "clientName": self._client_object.client_name,
+                    "appName": self._agent_object.agent_name,
+                    "instanceName": self._instance_object.instance_name,
+                    "backupsetName": "defaultDummyBackupSet",
+                    "subclientName": subclient_name
+                },
+                "commonProperties": {
+                    "storageDevice": {
+                        "dataBackupStoragePolicy": {
+                            "storagePolicyName": storage_policy
+                        }
+                    },
+                },
+                "mySqlSubclientProp": {
+                    "numberOfBackupStreams": kwargs.get('no_of_backup_streams'),
+                    "numberOfTransactionLogStreams": kwargs.get('no_of_log_backup_streams'),
+                    "fullInstanceXtraBackup": kwargs.get('full_instance_xtrabackup')
+                },
+                "content": content_list
+            }
+        }
+
+        return self._process_add_request(request_json)
+
     def add_virtual_server_subclient(
             self,
             subclient_name,
             subclient_content,
             **kwargs
     ):
         """Adds a new virtual server subclient to the backupset.
@@ -1046,22 +1160,23 @@
                         'display_name': 'sample1',
                         'type':  < VSAObjects.VMName: 10 >
                     }
 
             Returns:
 
             """
-            return{
+            return {
                 "equalsOrNotEquals": item_content.get('equal_value', True),
                 "name": item_content.get('id', ''),
                 "displayName": item_content.get('display_name', ''),
                 "path": item_content.get('path', ''),
                 "allOrAnyChildren": item.get('allOrAnyChildren', True),
                 "type": item_content['type'] if isinstance(item_content['type'], int) else item_content['type'].value
             }
+
         for item in subclient_content:
             _temp_list = []
             _temp_dict = {}
             allOrAnyChildren = item.get('allOrAnyChildren', None)
             if 'content' in item:
                 nested_content = item['content']
                 for each_condition in nested_content:
@@ -1109,18 +1224,18 @@
             if not self._commcell_object.storage_policies.has_policy(kwargs.get('storage_policy')):
                 raise SDKException(
                     'Subclient',
                     '102',
                     'Storage Policy: "{0}" does not exist in the Commcell'.format(kwargs.get('storage_policy'))
                 )
             request_json['subClientProperties']['commonProperties']['storageDevice'] = {
-                        "dataBackupStoragePolicy": {
-                            "storagePolicyName": kwargs.get('storage_policy')
-                        }
-                    }
+                "dataBackupStoragePolicy": {
+                    "storagePolicyName": kwargs.get('storage_policy')
+                }
+            }
         else:
             raise SDKException('Subclient', '102', 'Either Plan or Storage policy should be given as input')
 
         return self._process_add_request(request_json)
 
     def add_onedrive_subclient(self,
                                subclient_name,
@@ -1365,16 +1480,16 @@
         # the appropriate class object will be initialized based on the agent
         _subclients_dict = {
             'big data apps': BigDataAppsSubclient,
             'file system': FileSystemSubclient,
             'virtual server': [VirtualServerSubclient, VMInstanceSubclient],
             'cloud apps': CloudAppsSubclient,
             'sql server': SQLServerSubclient,
-            'nas': NASSubclient,        # SP11 or lower CS honors NAS as the Agent Name
-            'ndmp': NASSubclient,       # SP12 and above honors NDMP as the Agent Name
+            'nas': NASSubclient,  # SP11 or lower CS honors NAS as the Agent Name
+            'ndmp': NASSubclient,  # SP12 and above honors NDMP as the Agent Name
             'sap hana': SAPHANASubclient,
             'oracle': OracleSubclient,
             'oracle rac': OracleSubclient,
             'notes database': LNDbSubclient,
             'notes document': LNDocSubclient,
             'domino mailbox archiver': LNDmSubclient,
             'sybase': SybaseSubclient,
@@ -1382,15 +1497,15 @@
             "exchange mailbox": [ExchangeSubclient, CaseSubclient],
             'mysql': MYSQLSubclient,
             'exchange database': ExchangeDatabaseSubclient,
             'postgresql': PostgresSubclient,
             'db2': DB2Subclient,
             'informix': InformixSubclient,
             'active directory': ADSubclient,
-            'sharepoint server': [SharepointV1Subclient,SharepointSubclient],
+            'sharepoint server': [SharepointV1Subclient, SharepointSubclient],
             "azure ad": AzureAdSubclient
         }
 
         agent_object = backupset_object._agent_object
         instance_object = backupset_object._instance_object
         client_object = agent_object._client_object
 
@@ -1560,19 +1675,19 @@
             Raises:
                 SDKException:
                     if failed to update number properties for subclient
 
 
         """
         try:
-            backup = eval('self.%s' % attr_name)        # Take backup of old value
+            backup = eval('self.%s' % attr_name)  # Take backup of old value
         except (AttributeError, KeyError):
             backup = None
 
-        exec("self.%s = %s" % (attr_name, 'value'))     # set new value
+        exec("self.%s = %s" % (attr_name, 'value'))  # set new value
 
         request_json = self._get_subclient_properties_json()
 
         flag, response = self._cvpysdk_object.make_request('POST', self._SUBCLIENT, request_json)
 
         output = self._process_update_response(flag, response)
 
@@ -1877,15 +1992,15 @@
     def display_name(self):
         """Returns the Subclient display name"""
         return self.name
 
     @property
     def subclient_guid(self):
         """Returns the SubclientGUID"""
-        return self._subclient_properties.get('subClientEntity' , {}).get('subclientGUID')
+        return self._subclient_properties.get('subClientEntity', {}).get('subclientGUID')
 
     @display_name.setter
     def display_name(self, display_name):
         """Sets the display name for the subclient
         Args:
             display_name    (str)   -- Display name for the subclient
 
@@ -2201,15 +2316,15 @@
                 SDKException:
                     if failed to enable backup of subclient
         """
         self._set_subclient_properties("_commonProperties['enableBackup']", True)
 
     def enable_trueup(self):
         """Setter for the TrueUp Option for a Subclient"""
-        if 'isTrueUpOptionEnabled'in self._commonProperties:
+        if 'isTrueUpOptionEnabled' in self._commonProperties:
             self._set_subclient_properties("_commonProperties['isTrueUpOptionEnabled']", True)
 
     def enable_trueup_days(self, days=30):
         """Setter for the TrueUp Option with reconcile after x days"""
         self.enable_trueup()
         self._set_subclient_properties("_commonProperties['runTrueUpJobAfterDays']", days)
 
@@ -2413,15 +2528,15 @@
         Raise Exception:
                 if unable to get MA names
         """
         storage = self._subclient_properties['commonProperties']['storageDevice']
         if 'performanceMode' in storage:
             data_backup_storage_device = storage['performanceMode']["perfCRCDetails"]
             malist = []
-            for each_ma in data_backup_storage_device :
+            for each_ma in data_backup_storage_device:
                 malist.append(each_ma['perfMa'])
             return malist
 
     def browse(self, *args, **kwargs):
         """Browses the content of the Subclient.
 
             Args:
@@ -2611,20 +2726,20 @@
 
                 restore_data_and_acl    (bool)  --  restore data and ACL files
                     default: True
 
                 copy_precedence         (int)   --  copy precedence value of storage policy copy
                     default: None
 
-                from_time           (str)       --  time to retore the contents after
+                from_time           (str)       --  time to restore the contents after
                         format: YYYY-MM-DD HH:MM:SS
 
                     default: None
 
-                to_time           (str)         --  time to retore the contents before
+                to_time           (str)         --  time to restore the contents before
                         format: YYYY-MM-DD HH:MM:SS
 
                     default: None
 
                 fs_options      (dict)          -- dictionary that includes all advanced options
                     options:
                         all_versions        : if set to True restores all the versions of the
@@ -2715,20 +2830,20 @@
 
                 restore_data_and_acl  (bool)       --  restore data and ACL files
                     default: True
 
                 copy_precedence         (int)   --  copy precedence value of storage policy copy
                     default: None
 
-                from_time           (str)       --  time to retore the contents after
+                from_time           (str)       --  time to restore the contents after
                         format: YYYY-MM-DD HH:MM:SS
 
                     default: None
 
-                to_time           (str)         --  time to retore the contents before
+                to_time           (str)         --  time to restore the contents before
                         format: YYYY-MM-DD HH:MM:SS
 
                     default: None
 
                 fs_options      (dict)          -- dictionary that includes all advanced options
                     options:
                         preserve_level      : preserve level option to set in restore
@@ -3167,23 +3282,23 @@
             if self._commcell_object.plans.has_plan(value.plan_name):
                 self.update_properties({
                     'planEntity': {
                         'planName': value.plan_name
                     }
                 })
             else:
-                raise SDKException('Subclient','102', 'Plan does not exist')
+                raise SDKException('Subclient', '102', 'Plan does not exist')
         elif isinstance(value, str):
             if self._commcell_object.plans.has_plan(value):
                 self.update_properties({
                     'planEntity': {
                         'planName': value
                     }
                 })
             else:
-                raise SDKException('Subclient','102', 'Plan does not exist')
+                raise SDKException('Subclient', '102', 'Plan does not exist')
         elif value is None:
             self.update_properties({
                 'removePlanAssociation': True
             })
         else:
             raise SDKException('Subclient', '101')
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/__init__.py` & `cvpysdk-11.32/cvpysdk/subclients/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/aadsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/aadsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/adsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/adsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/bigdataappssubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/bigdataappssubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/casesubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/casesubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/casubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/casubclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,29 +49,29 @@
         from .cloudapps.teams_subclient import TeamsSubclient
         from .cloudapps.spanner_subclient import GoogleSpannerSubclient
 
         instance_types = {
             1: GoogleSubclient,
             2: GoogleSubclient,
             3: SalesforceSubclient,
-            4: CloudDatabaseSubclient, # Amazon RDS Subclient
+            4: CloudDatabaseSubclient,  # Amazon RDS Subclient
             5: CloudStorageSubclient,  # AmazonS3 Subclient
             6: CloudStorageSubclient,  # AzureBlob Subclient
             7: GoogleSubclient,  # OneDrive Subclient. GoogleSuclient class is used for OneDrive too
             14: CloudStorageSubclient,  # OracleCloud Subclient
             15: CloudStorageSubclient,  # Openstack Subclient
             20: CloudStorageSubclient,  # Google Cloud Instance
             21: CloudStorageSubclient,  # azure data lake gen2
-            26: CloudDatabaseSubclient, # Amazon Redshift subclient
-            27: CloudDatabaseSubclient, # Amazon Document DB subclient
+            26: CloudDatabaseSubclient,  # Amazon Redshift subclient
+            27: CloudDatabaseSubclient,  # Amazon Document DB subclient
             25: CloudStorageSubclient,  # AliBaba
-            24: CloudStorageSubclient,  #IBM
+            24: CloudStorageSubclient,  # IBM
             22: CloudDatabaseSubclient,  # Amazon DynamoDB subclient
-            35: MSDynamics365Subclient,  # MS Dynamics 365 Subclient
-            36: TeamsSubclient, # Office 365 Teams
+            35: MSDynamics365Subclient,  # Office 365 Apps -> MS Dynamics 365 Subclient
+            36: TeamsSubclient,  # Office 365 Apps -> MS Teams
             37: GoogleSpannerSubclient  # Google Cloud Spanner Subclient
         }
 
         cloud_apps_instance_type = backupset_object._instance_object._properties[
             'cloudAppsInstance']['instanceType']
 
         if cloud_apps_instance_type in instance_types:
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/__init__.py` & `cvpysdk-11.32/cvpysdk/subclients/cloudapps/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/cloud_database_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/cloudapps/cloud_database_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/cloud_storage_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/cloudapps/cloud_storage_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/dynamics365_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/cloudapps/dynamics365_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/google_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/cloudapps/google_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/salesforce_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/cloudapps/salesforce_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/spanner_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/cloudapps/spanner_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/cloudapps/teams_constants.py` & `cvpysdk-11.32/cvpysdk/subclients/cloudapps/teams_constants.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/db2subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/db2subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/dbsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/dbsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/exchange/__init__.py` & `cvpysdk-11.32/cvpysdk/subclients/exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/exchange/contentstoremailbox_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/exchange/contentstoremailbox_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/exchange/exchange_database_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/exchange/exchange_database_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/exchange/journalmailbox_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/exchange/journalmailbox_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/exchange/usermailbox_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/exchange/usermailbox_subclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,62 +16,80 @@
 # limitations under the License.
 # --------------------------------------------------------------------------
 
 """File for operating on a UserMailbox Subclient.
 
 UsermailboxSubclient is the only class defined in this file.
 
-UsermailboxSubclient:   Derived class from ExchangeMailboxSubclient Base class, representing a
+UsermailboxSubclient:       Derived class from ExchangeMailboxSubclient Base class, representing a
                             UserMailbox subclient, and to perform operations on that subclient
 
 UsermailboxSubclient:
+======================
 
     _get_subclient_properties()         --  gets the properties of UserMailbox Subclient
-
     _get_subclient_properties_json()    --  gets the properties JSON of UserMailbox Subclient
+    _get_discover_adgroups()            --  Get the discovered AD Groups
+    _get_discover_users()               --  Get the discovered users
+    _association_json_with_plan()       --  Create the Association JSON for
+                                            associations using Exchange Plan
+    _association_mailboxes_json()       --  Association for particular mailboxes
+    _task_json_for_backup()             --  JSON for backup task for Exchange User mailbox Subclient
+    _backup_generic_items_json()        --  JSON to backup generic items
 
-    users()                             --  creates users association for subclient
-
-    Databases()                         --  creates Db association for  the subclient
-
-    Adgroups()                          --  creates Adgroup association for subclient
-
-    restore_in_place()                  --  runs in-place restore for the subclient
+Content Association Methods:
+==============================
 
+    set_user_assocaition()              --  Set exchange users association
     set_pst_association()               --  Create PST association for UserMailboxSubclient
-
     set_fs_association_for_pst()        --  Helper method to create pst association for
                                             PST Ingestion by FS association
+    set_adgroup_associations()          --  Create Association for ADGroups
+    set_o365group_asscoiations()        --  Create O365 group association
 
-    _association_json_with_plan()       --  Create the Association JSON for
-                                            associations using Exchange Plan
+    delete_user_assocaition()           --  Delete User Association from content
+    delete_o365group_association()      --  Delete Office 365 Group Association
+    delete_database_assocaition()       --  Delete Exchange DB Association
+    delete_adgroup_assocaition          --  Delete association for an AD Group
 
-    _association_mailboxes_json()       --  Association for particular mailboxes
 
-    backup_mailboxes()                  --  Backup specific mailboxes
+    enable_allusers_association()       --  Enable association for all mailboxes
+    disable_allusers_association()      --  Disable All Users Association
 
-    _backup_generic_items_json()        --  JSON to backup generic items
+    enable_auto_discover_association    --  Enable Association for Auto Discovered Content
+                                            viz. All Public Folders/
+                                                All Mailboxes/
+                                                All Group Mailboxes
+    delete_auto_discover_association    --  Delete Association for Auto Discovered Content
+                                           `viz. All Public Folders/
+                                                All Mailboxes/
+                                                All Group Mailboxes
+    enable_ews_support()                --  Enables EWS Support for backup for ON_PREM Mailboxes
 
+Browse/ Restore/ Backup Methods:
+==============================
+
+    browse_mailboxes()                  --  Backup specific mailboxes
     backup_generic_items()              --  Backup Generic Items
                                             viz. All Public Folders/
                                                 All User Mailboxes/
                                                 All Group Mailboxes
+    backup_mailboxes()                  --  Backup selected mailboxes
+    restore_in_place()                  --  runs in-place restore for the subclient
+    create_recovery_point()             --  Create a recovery point for a mailbox
 
-    set_adgroup_associations()          --  Create Association for ADGroups
-
-    _get_discover_adgroups()            --  Get the discovered AD Groups
-
-    _get_discover_users()               --  Get the discovered users
-
-    set_o365group_asscoiations()        --  Create O365 group association for UsermailboxSubclient
 
-    delete_o365group_association()      --  delete O365 group association for UsermailboxSubclient
 
-    enable_ews_support()                -- Enables EWS Support for backup for ON_PREM Mailboxes
+User Mailbox Subclient Instance Attributes:
+==============================
 
+    discover_users                          --  Dictionary of users discovered
+    discover_databases                      --  Dictionary of databases discovered
+    adgroups                                --  Dictionary of discovered AD Groups
+    o365groups                              --  Dictionary of discovered Office 365 Groups
 """
 
 from __future__ import unicode_literals
 
 from ...exception import SDKException
 
 from ..exchsubclient import ExchangeSubclient
@@ -154,15 +172,15 @@
         return policy_json
 
     def _association_json(self, subclient_content, is_o365group=False):
         """Constructs association json to create assocaition in UserMailbox Subclient.
 
             Args:
                 subclient_content (dict)  --  dict of the Users to add to the subclient
-                                             (dict of only policies in case of office 365 groups)
+                                             (dict of only policies in case of Office 365 groups)
                 subclient_content = {
 
                         'archive_policy' : "CIPLAN Archiving policy",
 
                         'cleanup_policy' : 'CIPLAN Clean-up policy',
 
                         'retention_policy': 'CIPLAN Retention policy'
@@ -299,15 +317,16 @@
             "createNewIndex": False
         }
         task_json['taskInfo']['subTasks'][0]['options']['backupOpts'] = backup_options
         task_json['taskInfo']['subTasks'][0]['options']['dataOpt'] = data_options
         return task_json
 
     def _set_association_request(self, associations_json):
-        """Runs the emailAssociation ass API to set association
+        """
+            Runs the emailAssociation POST API to set association
 
             Args:
                 associations_json    (dict)  -- request json sent as payload
 
             Returns:
                 (str, str):
                     str  -  error code received in the response
@@ -649,14 +668,68 @@
                         'retention_policy': retention_policy
                     }
 
                     adgroups.append(temp_dict)
 
         return adgroups
 
+    def _backup_generic_items_json(self, subclient_content):
+        """
+            Create the JSON for Backing Up the Generic Items of any Exchange Online Client
+
+            Args:
+                subclient_content   (list)  List having dictionary of items to be backed up
+
+                subclient_content = [
+                    {
+                    "associationName" : "All Public Folders",
+                    "associationType":12
+                    },
+                    {
+                    "associationName" : "All Users",
+                    "associationType":12
+                    }
+                ]
+
+            Returns:
+                The JSON to create a backup task
+        """
+
+        task_dict = {
+            "taskInfo": {
+                "associations": [
+                    self._subClientEntity
+                ],
+                "task": {
+                    "taskType": 1
+                },
+                "subTasks": [
+                    {
+                        "subTask": {
+                            "subTaskType": 2,
+                            "operationType": 2
+                        },
+                        "options": {
+                            "backupOpts": {
+                                "backupLevel": 1,
+                                "incLevel": 1,
+                                "exchOnePassOptions": {
+                                    "genericAssociations": [
+                                    ]
+                                }
+                            }
+                        }
+                    }
+                ]
+            }
+        }
+        task_dict["taskInfo"]["subTasks"][0]["options"]["backupOpts"]["exchOnePassOptions"][
+            "genericAssociations"] = subclient_content
+        return task_dict
+
     @property
     def discover_users(self):
         """"Returns the list of discovered users for the UserMailbox subclient."""
         return self._discover_users
 
     @property
     def discover_databases(self):
@@ -737,15 +810,15 @@
                             'mailBoxType': mb_item['mailBoxType'],
                             'displayName': mb_item['displayName'],
                             'exchangeServer': mb_item['exchangeServer'],
                             'isAutoDiscoveredUser': mb_item['isAutoDiscoveredUser'],
                             "associated": False,
                             'databaseName': mb_item['databaseName'],
                             "exchangeVersion": mb_item['exchangeVersion'],
-                            "msExchRecipientTypeDetails": mb_item['msExchRecipientTypeDetails'],
+                            # "msExchRecipientTypeDetails": mb_item['msExchRecipientTypeDetails'],
                             'user': {
                                 '_type_': 13,
                                 'userGUID': mb_item['user']['userGUID']
                             }
                         }
                         users.append(mailbox_dict)
                         break
@@ -1008,134 +1081,14 @@
             "discoverByType": 3,
             "adGroups": adgroups
         }
         _assocaition_json_ = self._association_json(subclient_content)
         _assocaition_json_["emailAssociation"]["emailDiscoverinfo"] = discover_info
         self._set_association_request(_assocaition_json_)
 
-    def _backup_generic_items_json(self, subclient_content):
-        """
-            Create the JSON for Backing Up the Generic Items of any Exchange Online Client
-
-            Args:
-                subclient_content   (list)  List having dictionary of items to be backed up
-
-                subclient_content = [
-                    {
-                    "associationName" : "All Public Folders",
-                    "associationType":12
-                    },
-                    {
-                    "associationName" : "All Users",
-                    "associationType":12
-                    }
-                ]
-
-            Returns:
-                The JSON to create a backup task
-        """
-
-        task_dict = {
-            "taskInfo": {
-                "associations": [
-                    self._subClientEntity
-                ],
-                "task": {
-                    "taskType": 1
-                },
-                "subTasks": [
-                    {
-                        "subTask": {
-                            "subTaskType": 2,
-                            "operationType": 2
-                        },
-                        "options": {
-                            "backupOpts": {
-                                "backupLevel": 1,
-                                "incLevel": 1,
-                                "exchOnePassOptions": {
-                                    "genericAssociations": [
-                                    ]
-                                }
-                            }
-                        }
-                    }
-                ]
-            }
-        }
-        task_dict["taskInfo"]["subTasks"][0]["options"]["backupOpts"]["exchOnePassOptions"][
-            "genericAssociations"] = subclient_content
-        return task_dict
-
-    def enable_ews_support(self, service_url):
-        """This function provides support for EWS protocol to backup on-prem mailboxes
-            Args:
-                service_url (string) -- EWS Connection URL for your exchange server
-            Returns: None
-        """
-        self.agentproperties = self._agent_object.properties
-        self.agentproperties["onePassProperties"]["onePassProp"]["ewsDetails"]["bUseEWS"] = True
-        self.agentproperties["onePassProperties"]["onePassProp"]["ewsDetails"]["ewsConnectionUrl"] = service_url
-        self._agent_object.update_properties(self.agentproperties)
-
-    def browse_mailboxes(self, retry_attempts=0):
-        """
-        This function returns the mailboxes available for OOP restore
-        return: dictionary containing mailbox info
-        """
-        BROWSE_MAILBOXES = self._commcell_object._services['EMAIL_DISCOVERY_WITHOUT_REFRESH'] % (
-            int(self._backupset_object.backupset_id), 'User'
-        )
-        flag, response = self._commcell_object._cvpysdk_object.make_request('GET', BROWSE_MAILBOXES)
-        if flag:
-            if response and response.json():
-                discover_content = response.json()
-                if discover_content.get('resp', {}).get('errorCode', 0) == 469762468:
-                    time.sleep(10)
-                    if retry_attempts > 10:
-                        raise SDKException('Subclient', '102', 'Failed to perform browse operation.')
-                    return self.browse_mailboxes(retry_attempts + 1)
-                if 'discoverInfo' in discover_content.keys():
-                    if 'mailBoxes' in discover_content['discoverInfo']:
-                        mailboxes = discover_content["discoverInfo"]["mailBoxes"]
-                        return mailboxes
-            else:
-                raise SDKException("Response", "102")
-        else:
-            response_string = self.commcell._update_response_(response.text)
-            raise SDKException('Response', '101', response_string)
-
-    def backup_generic_items(self, subclient_content):
-        """
-            Backups the Generic Items for any Exchange Online Client
-            GGeneric Items:
-                All Public Folders/ All O365 Group ailboxes/ All Users
-
-            Args:
-                subclient_content   (list)  List having dictionary of items to be backed up
-
-                subclient_content = [
-                    {
-                    "associationName" : "All Public Folders",
-                    "associationType":12
-                    },
-                    {
-                    "associationName" : "All Users",
-                    "associationType":12
-                    }
-                ]
-        """
-        task_dict = self._backup_generic_items_json(subclient_content=subclient_content)
-
-        flag, response = self._commcell_object._cvpysdk_object.make_request(
-            'POST', self._services['CREATE_TASK'], task_dict
-        )
-
-        return self._process_backup_response(flag, response)
-
     def set_o365group_asscoiations(self, subclient_content):
         """Create O365 Group association for UserMailboxSubclient.
             Args:
                 subclient_content   (dict)  --  dict of the policies to associate
 
                     subclient_content = {
 
@@ -1201,15 +1154,15 @@
                             'mailBoxType': mb_item['mailBoxType'],
                             'displayName': mb_item['displayName'],
                             'exchangeServer': mb_item['exchangeServer'],
                             'isAutoDiscoveredUser': mb_item['isAutoDiscoveredUser'],
                             "associated": False,
                             'databaseName': mb_item['databaseName'],
                             "exchangeVersion": mb_item['exchangeVersion'],
-                            "msExchRecipientTypeDetails": mb_item['msExchRecipientTypeDetails'],
+                            # "msExchRecipientTypeDetails": mb_item['msExchRecipientTypeDetails'],
                             "exchangeServer": mb_item['exchangeServer'],
                             'user': {
                                 '_type_': 13,
                                 'userGUID': mb_item['user']['userGUID']
                             }
                         }
                         users.append(mailbox_dict)
@@ -1548,14 +1501,80 @@
             ]
         }
         _association_json_["emailAssociation"]["advanceOptions"]["enableAutoDiscovery"] = True
         _association_json_["emailAssociation"]["emailStatus"] = 1
         _association_json_["emailAssociation"]["emailDiscoverinfo"] = discover_info
         self._set_association_request(_association_json_)
 
+    def enable_ews_support(self, service_url):
+        """This function provides support for EWS protocol to backup on-prem mailboxes
+            Args:
+                service_url (string) -- EWS Connection URL for your exchange server
+            Returns: None
+        """
+        self.agentproperties = self._agent_object.properties
+        self.agentproperties["onePassProperties"]["onePassProp"]["ewsDetails"]["bUseEWS"] = True
+        self.agentproperties["onePassProperties"]["onePassProp"]["ewsDetails"]["ewsConnectionUrl"] = service_url
+        self._agent_object.update_properties(self.agentproperties)
+
+    def browse_mailboxes(self, retry_attempts=0):
+        """
+        This function returns the mailboxes available for OOP restore
+        return: dictionary containing mailbox info
+        """
+        BROWSE_MAILBOXES = self._commcell_object._services['EMAIL_DISCOVERY_WITHOUT_REFRESH'] % (
+            int(self._backupset_object.backupset_id), 'User'
+        )
+        flag, response = self._commcell_object._cvpysdk_object.make_request('GET', BROWSE_MAILBOXES)
+        if flag:
+            if response and response.json():
+                discover_content = response.json()
+                if discover_content.get('resp', {}).get('errorCode', 0) == 469762468:
+                    time.sleep(10)
+                    if retry_attempts > 10:
+                        raise SDKException('Subclient', '102', 'Failed to perform browse operation.')
+                    return self.browse_mailboxes(retry_attempts + 1)
+                if 'discoverInfo' in discover_content.keys():
+                    if 'mailBoxes' in discover_content['discoverInfo']:
+                        mailboxes = discover_content["discoverInfo"]["mailBoxes"]
+                        return mailboxes
+            else:
+                raise SDKException("Response", "102")
+        else:
+            response_string = self.commcell._update_response_(response.text)
+            raise SDKException('Response', '101', response_string)
+
+    def backup_generic_items(self, subclient_content):
+        """
+            Backups the Generic Items for any Exchange Online Client
+            GGeneric Items:
+                All Public Folders/ All O365 Group ailboxes/ All Users
+
+            Args:
+                subclient_content   (list)  List having dictionary of items to be backed up
+
+                subclient_content = [
+                    {
+                    "associationName" : "All Public Folders",
+                    "associationType":12
+                    },
+                    {
+                    "associationName" : "All Users",
+                    "associationType":12
+                    }
+                ]
+        """
+        task_dict = self._backup_generic_items_json(subclient_content=subclient_content)
+
+        flag, response = self._commcell_object._cvpysdk_object.make_request(
+            'POST', self._services['CREATE_TASK'], task_dict
+        )
+
+        return self._process_backup_response(flag, response)
+
     def backup_mailboxes(self, mailbox_alias_names):
         """
         Backup specific mailboxes.
         Args:
             mailbox_alias_names(list): alias names of all the mailboxes to backup
                 Sample Values:
                     ['aj', 'tkumar']
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/exchsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/exchsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/fssubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/fssubclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,18 @@
   
     **block_level_backup_option**         --  Enable/Disable Blocklevel Option on subclient
 
     **create_file_level_index_option**    --  Enable/Disable Metadata collection Option on subclient
 
     **system_state_option**               --  Enable/Disable System state option for the subclient
 
+    **_dc_options_dict**                  --   Data Classification plan  Options
+
+    **enable_dc_content_indexing**        -- Enable Dataclassification Indexing option.
+
     **onetouch_option**                   --  Enable/Disable One-Touch option for the subclient
 
     **onetouch_server**                   --  Provides the 1-touch server name
 
     **onetouch_server_directory**         --  Provides the 1-touch server directory
     
     **catalog_acl**                       --  To enable/disable ACL on the subclient
@@ -231,15 +235,16 @@
                     "proxyClient": self._proxyClient,
                     "subClientEntity": self._subClientEntity,
                     "fsSubClientProp": self._fsSubClientProp,
 
                     "content": self._content,
                     "commonProperties": self._commonProperties,
                     "fsContentOperationType": "OVERWRITE",
-                    "fsExcludeFilterOperationType": "OVERWRITE" if not hasattr(self, '_fsExcludeFilterOperationType') else self._fsExcludeFilterOperationType
+                    "fsExcludeFilterOperationType": "OVERWRITE" if not hasattr(self, '_fsExcludeFilterOperationType') else self._fsExcludeFilterOperationType,
+                    "fsIncludeFilterOperationType": "OVERWRITE" if not hasattr(self, '_fsIncludeFilterOperationType') else self._fsIncludeFilterOperationType
                 }
         }
 
         if 'isDDBSubclient' in self._fs_subclient_prop:
             if self._fs_subclient_prop['isDDBSubclient']:
                 del subclient_json["subClientProperties"]["content"]
         return subclient_json
@@ -312,14 +317,15 @@
             exception_dict = {
                 "includePath": path
             }
             update_content.append(exception_dict)
 
         self._set_subclient_properties("_content", update_content)
         self._fsExcludeFilterOperationType = "OVERWRITE"  # RESET THE OPERATION TYPE TO ITS DEFAULT
+        self._fsIncludeFilterOperationType = "OVERWRITE"  # RESET THE OPERATION TYPE TO ITS DEFAULT
 
 
     def _common_backup_options(self, options):
         """
          Generates the advanced job options dict
 
             Args:
@@ -532,15 +538,18 @@
                 SDKException:
                     if failed to update exception content of subclient
 
                     if the type of value input is not list
 
                     if value list is empty
         """
-        if isinstance(value, list) and value != []:
+        if isinstance(value, list):
+            if value == []:
+                value = self.exception_content
+                self._fsIncludeFilterOperationType = "DELETE"
             self._set_content(exception_content=value)
         else:
             raise SDKException(
                 'Subclient',
                 '102',
                 'Subclient exception content should be a list value and not empty')
 
@@ -746,14 +755,33 @@
                 block_level_backup_value (bool)  --  Specifies to enable or disable blocklevel option
         """
 
         self._set_subclient_properties(
             "_fsSubClientProp['blockLevelBackup']",
             block_level_backup_value)
 
+
+    @property
+    def _dc_options_dict(self):
+        """ Constructs Data classification Property"""
+        dc_options = {'dcPlanEntity': {'planType': 7, 'planSubtype': 117506053, 'planName': ''}}
+        return dc_options
+
+    def enable_dc_content_indexing(self, dcplan_name):
+        """Creates the JSON with the specified dataclassification plan to pass to API to
+            update  file system Subclient
+
+            Args:
+                dcplan_name (String)  --  DC plan name
+
+        """
+        temp_dc = self._dc_options_dict
+        temp_dc['dcPlanEntity']['planName'] = dcplan_name
+        self.update_properties(temp_dc)
+
     @property
     def create_file_level_index_option(self):
         """Gets the value of Metadata collection Option
 
             Returns:
                 true - if metadata collection is enabled on the subclient
                 false - if metadata collection is not enabled on the subclient
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/hanasubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/hanasubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/index_server_subclient.py` & `cvpysdk-11.32/cvpysdk/subclients/index_server_subclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,14 +334,16 @@
                 find_options['operation'] = 'browse'
 
             find_options['path'] = roles_path
         if job_id != 0:
             find_options['job_id'] = job_id
         if include_files:
             find_options['include_meta_data'] = True
+        else:
+            find_options['hide_user_hidden'] = True
 
         return self.find(find_options)
 
     def configure_backup(self, storage_policy, role_content):
         """Edit the default subclient for modifying role content or storage policy.
 
                     Args:
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/informixsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/informixsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/lndbsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/lndbsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/__init__.py` & `cvpysdk-11.32/cvpysdk/subclients/lotusnotes/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/lndbsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndbsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/lndmsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndmsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/lndocsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndocsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/lotusnotes/lnsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lnsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/mysqlsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/mysqlsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/nassubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/fusioncompute.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-﻿#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # --------------------------------------------------------------------------
 # Copyright Commvault Systems, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -13,228 +12,229 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # --------------------------------------------------------------------------
 
-"""File for operating on a NAS Subclient
+"""File for operating on a Virtual Server FusionCompute Subclient.
 
-NASSubclient is the only class defined in this file.
+FusionComputeVirtualServerSubclient is the only class defined in this file.
 
-NASSubclient: Derived class from Subclient Base class, representing a nas subclient,
-                        and to perform operations on that subclient
+FusionComputeVirtualServerSubclient: Derived class from VirtualServerSubClient  Base class,
+                            representing a FusionCompute Subclient, and
+                            to perform operations on that Subclient
 
-NASSubclient:
-    _get_subclient_properties()          --  gets the subclient  related properties of NAS subclient.
-    
-    _get_subclient_properties_json()     --  gets all the subclient  related properties of NAS subclient.
-    
-    content()                            --  update the content of the subclient
+FusionComputeVirtualServerSubclient:
 
-    filter_content()                    --  update the filter content of the subclient
+    __init__(,backupset_object, subclient_name, subclient_id)--  initialize object of FusionCompute
+                                                                             subclient object
+                                                                                 associated with
+                                                                        the VirtualServer subclient
 
-    content()                           --  update the content of the subclient
-
-    backup()                            --  run a backup job for the subclient
-    
-    restore_in_place()                  -- run a restore in place for the subclient
+    full_vm_restore_out_of_place()                  --  restores the VM  specified in
+                                                     to the specified client, at the
+                                                        specified destination location
 
+    full_vm_restore_in_place()              --  restores the VM specified by the
+                                                    user to the same location
 """
+from cvpysdk.exception import SDKException
+from ..vssubclient import VirtualServerSubclient
 
-from __future__ import unicode_literals
 
-from .fssubclient import FileSystemSubclient
-from ..exception import SDKException
+class FusionComputeVirtualServerSubclient(VirtualServerSubclient):
+    """Derived class from VirtualServerSubclient Base class.
+       This represents a Fusion Compute virtual server subclient,
+       and can perform restore operations on only that subclient.
+
+    """
+    def __init__(self, backupset_object, subclient_name, subclient_id=None):
+        """Initialize the Instance object for the given Virtual Server instance.
+        Args
+        class_object (backupset_object, subclient_name, subclient_id)  --  instance of the
+                                         backupset class, subclient name, subclient id
 
+        """
+        super(FusionComputeVirtualServerSubclient, self).__init__(
+            backupset_object, subclient_name, subclient_id)
+        self.diskExtension = ["none"]
+
+        self._disk_option = {
+            'original': 0,
+            'thicklazyzero': 1,
+            'thin': 2,
+            'common': 3
+        }
 
-class NASSubclient(FileSystemSubclient):
-    """Derived class from Subclient Base class, representing a nas subclient,
-        and to perform operations on that subclient."""
-    
-   
-    def backup(
+    def full_vm_restore_in_place(
             self,
-            backup_level="Incremental",
-            incremental_backup=False,
-            incremental_level='BEFORE_SYNTH', on_demand_input=None, snap_name=None):
-        """Runs a backup job for the subclient of the level specified.
+            vm_to_restore=None,
+            overwrite=True,
+            power_on=True,
+            proxy_client=None,
+            copy_precedence=0,
+            **kwargs):
+        """Restores the FULL Virtual machine specified in the input list
+            to the location same as the actual location of the VM in VCenter.
 
             Args:
-                backup_level        (str)   --  level of backup the user wish to run
-                        Full / Incremental / Differential / Synthetic_full
-                    default: Incremental
-
-                incremental_backup  (bool)  --  run incremental backup
-                        only applicable in case of Synthetic_full backup
-                    default: False
-
-                incremental_level   (str)   --  run incremental backup before/after synthetic full
-                        BEFORE_SYNTH / AFTER_SYNTH
-
-                        only applicable in case of Synthetic_full backup
-                    default: BEFORE_SYNTH
-
-                on_demand_input     (str)   --  input file location for on demand backupset
-                    default: None
+                vm_to_restore       (list)     --  provide the VM name to
+                                                   restore
+                                                   default: None
+
+                overwrite           (bool)     --  overwrite the existing VM
+                                                   default: True
+
+                power_on            (bool)     --  power on the  restored VM
+                                                   default: True
+
+                copy_precedence     (int)      --  copy precedence value
+                                                   default: 0
+
+                proxy_client          (str)  --  proxy client to be used for restore
+                                                        default: proxy added in subclient
+
+                **kwargs                         : Arbitrary keyword arguments Properties as of
+                                                     full_vm_restore_out_of_place
+                    eg:
+                    v2_details          (dict)       -- details for v2 subclient
+                                                    eg: check clients.vmclient.VMClient._child_job_subclient_details
 
             Returns:
-                object - instance of the Job class for this backup job
+                object - instance of the Job class for this restore job
 
             Raises:
                 SDKException:
-                    if backup level specified is not correct
+                    if inputs are not of correct type as per definition
+
+                    if failed to initialize job
 
                     if response is empty
 
                     if response is not success
-        """
-        
-        if snap_name is None:
-            return super(NASSubclient, self).backup(
-                backup_level, incremental_backup, incremental_level, on_demand_input=on_demand_input
-            )
-        else:
-            request_json = self._backup_json(backup_level, incremental_backup, incremental_level)
 
-            if not isinstance(snap_name, str):
-                raise SDKException('Subclient', '101')
+        """
+        restore_option = {"v2_details": kwargs.get("v2_details", None)}
 
-            if snap_name:
-                nas_options = {
-                    "nasOptions": {
-                        "backupFromSnap": snap_name,
-                        "backupQuotas": True,
-                        "backupFromSnapshot": True,
-                        "backupFromSnapshotYes": True,
-                        "replicationVolumeId": 0
-                    }
-                }
-                request_json["taskInfo"]["subTasks"][0]["options"]["backupOpts"].update(
-                    nas_options
-                )
-
-            bakup_service = self._commcell_object._services['CREATE_TASK']
-
-            flag, response = self._commcell_object._cvpysdk_object.make_request(
-                'POST', bakup_service, request_json
-            )
+        # set attr for all the option in restore xml from user inputs
+        self._set_restore_inputs(
+            restore_option,
+            unconditional_overwrite=overwrite,
+            power_on=power_on,
+            copy_precedence=copy_precedence,
+            vm_to_restore=self._set_vm_to_restore(vm_to_restore),
+            volume_level_restore=1,
+            client_name=proxy_client,
+            in_place=True
+        )
 
-            return self._process_backup_response(flag, response)
+        request_json = self._prepare_fullvm_restore_json(restore_option)
+        return self._process_restore_response(request_json)
 
-    def restore_in_place(
+    def full_vm_restore_out_of_place(
             self,
-            paths,
-            overwrite=True,
-            restore_data_and_acl=True,
-            copy_precedence=None,
-            from_time=None,
-            to_time=None,
-            fs_options=None,
-            schedule_pattern=None,
+            vm_to_restore=None,
+            destination_client=None,
             proxy_client=None,
-            advanced_options=None,
-            synthRestore=False):
-        """Runs a restore job for the subclient .
+            new_name=None,
+            host=None,
+            datastore=None,
+            overwrite=True,
+            power_on=True,
+            copy_precedence=0,
+            disk_provisioning='original',
+            **kwargs):
+        """Restores the FULL Virtual machine specified in the input list
+            to the provided vcenter client along with the ESX and the datastores.
+            If the provided client name is none then it restores the Full Virtual
+            Machine to the source client and corresponding ESX and datastore.
 
             Args:
-                            paths                   (list)  --  list of full paths of files/folders to restore
-
-                overwrite               (bool)  --  unconditional overwrite files during restore
-                    default: True
-
-                restore_data_and_acl    (bool)  --  restore data and ACL files
-                    default: True
-
-                copy_precedence         (int)   --  copy precedence value of storage policy copy
-                    default: None
+                vm_to_restore     (list)  --  provide the VM name to restore
+                                              default: None
 
-                from_time           (str)       --  time to retore the contents after
-                        format: YYYY-MM-DD HH:MM:SS
+                destination_client    (str) -- name of the Pseudo client
+                                                  where the VM should be
+                                                    restored.
+
+                new_name          (str) -- new name to be given to the
+                                                    restored VM
+
+                host          (str) -- destination cluster or  host
+                                                    restores to the source VM
+                                                    esx if this value is not
+                                                    specified
+
+                datastore         (str) -- datastore where the
+                                                  restored VM should be located
+                                                  restores to the source VM
+                                                  datastore if this value is
+                                                  not specified
+
+                overwrite         (bool)       -- overwrite the existing VM
+                                                  default: True
+
+                power_on          (bool)       -- power on the  restored VM
+                                                  default: True
+
+                copy_precedence   (int)        -- copy precedence value
+                                                  default: 0
+
+                disk_provisioning       (str) -- disk provisioning for the
+                                                  restored vm
+                                                  default: 0 which is equivalent
+                                                  to Original
+                proxy_client     (str)  --  proxy client to be used for restore
+                                                        default: proxy added in subclient
+
+                **kwargs                         : Arbitrary keyword arguments Properties as of
+                                                     full_vm_restore_out_of_place
+                    eg:
+                    v2_details          (dict)       -- details for v2 subclient
+                                                    eg: check clients.vmclient.VMClient._child_job_subclient_details
 
-                    default: None
-
-                to_time           (str)         --  time to retore the contents before
-                        format: YYYY-MM-DD HH:MM:SS
-
-                    default: None
-
-                fs_options      (dict)          -- dictionary that includes all advanced options
-                    options:
-                        all_versions        : if set to True restores all the versions of the
-                                                specified file
-                        versions            : list of version numbers to be backed up
-                        validate_only       : To validate data backed up for restore
-
-
-                schedule_pattern (dict) -- scheduling options to be included for the task
-
-                        Please refer schedules.schedulePattern.createSchedule()
-                                                                    doc for the types of Jsons
-
-                proxy_client    (str)          -- Proxy client used during FS under NAS operations
-
-                advanced_options    (dict)  -- Advanced restore options
-                
-                synthRestore (bool)     -- Advance NAS restore option SynthRestore
-
-                    Options:
-
-                        job_description (str)   --  Restore job description
-
-                        timezone        (str)   --  Timezone to be used for restore
-
-                            **Note** make use of TIMEZONES dict in constants.py to pass timezone
 
             Returns:
-                object - instance of the Job class for this restore job if its an immediate Job
-                         instance of the Schedule class for this restore job if its a scheduled Job
+                object - instance of the Job class for this restore job
 
             Raises:
                 SDKException:
-                    if paths is not a list
+                    if inputs are not of correct type as per definition
 
                     if failed to initialize job
 
                     if response is empty
 
                     if response is not success
-                
+
         """
-        self._backupset_object._instance_object._restore_association = self._subClientEntity
-        if synthRestore == False:
-            return super(NASSubclient, self).restore_in_place(
-                paths,
-                overwrite,
-                restore_data_and_acl,
-                copy_precedence,
-                from_time,
-                to_time,
-                fs_options,
-                schedule_pattern,
-                proxy_client,
-                advanced_options
-            )
-        else:
-            request_json = self._restore_json(
-                paths=paths,
-                overwrite=overwrite,
-                restore_data_and_acl=restore_data_and_acl,
-                copy_precedence=copy_precedence,
-                from_time=from_time,
-                to_time=to_time,
-                fs_options=None,
-                schedule_pattern=None,
-                proxy_client=None,
-                advanced_options=None
-            )
-            
-            nas_option = {
-                "nasOption": {
-                     "synthRestore": 1
-                }
-            }
+        restore_option = {"v2_details": kwargs.get("v2_details", None)}
+
+        if vm_to_restore:
+            vm_to_restore = [vm_to_restore]
+
+        if new_name:
+            if not(isinstance(vm_to_restore, str) or
+                   isinstance(new_name, str)):
+                raise SDKException('Subclient', '101')
+            restore_option['restore_new_name'] = new_name
 
-            request_json["taskInfo"]["subTasks"][0]["options"]["restoreOptions"].update(nas_option)
+        # set attr for all the option in restore xml from user inputs
+        self._set_restore_inputs(
+            restore_option,
+            vm_to_restore=self._set_vm_to_restore(vm_to_restore),
+            unconditional_overwrite=overwrite,
+            power_on=power_on,
+            disk_option=self._disk_option[disk_provisioning],
+            copy_precedence=copy_precedence,
+            volume_level_restore=1,
+            client_name=proxy_client,
+            vcenter_client=destination_client,
+            esx_host=host,
+            datastore=datastore,
+            in_place=False,
+            restore_new_name=new_name
+        )
 
-            
-            return self._process_restore_response(request_json)
+        request_json = self._prepare_fullvm_restore_json(restore_option)
+        return self._process_restore_response(request_json)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/oraclesubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/oraclesubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/postgressubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/postgressubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/saporaclesubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/saporaclesubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/sharepointsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/sharepointsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/splunksubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/splunksubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/sqlsubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/sqlsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/sybasesubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/sybasesubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/__init__.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/alibaba_cloud.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/alibaba_cloud.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/amazon_web_services.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/amazon_web_services.py`

 * *Files 5% similar despite different names*

```diff
@@ -317,15 +317,16 @@
             amazon_options=None,
             overwrite=True,
             copy_precedence=0,
             destination_vm_guid=None,
             disk_prefix=None,
             availability_zone=None,
             media_agent=None,
-            disk_name=None
+            disk_name=None,
+            **kwargs,
     ):
         """Restores the Attach Disk restore with  specified in the input list
             to the provided instance.
 
             Args:
                 vm_to_restore         (str)  --  provide the source vm name
 
@@ -407,18 +408,26 @@
         src_item_list = []
         for each_disk in disk_name:
             src_item_list.append("\\" + vm_ids[vm_to_restore] + "\\" + each_disk.split("\\")[-1])
         _attach_disk_restore_option['paths'] = src_item_list
         if proxy_client is not None:
             _attach_disk_restore_option['client'] = proxy_client
         if not destination_vm:
-            destination_vm = vm_to_restore
+            destination_vm = 'del' + vm_to_restore
         instance_dict = self._backupset_object._instance_object._properties['instance']
         _attach_disk_restore_option = self.amazon_defaults(vm_to_restore, _attach_disk_restore_option)
 
+        if kwargs.get('new_instance', False):
+            _attach_disk_restore_option['keyPairList'][0] = {}
+            _attach_disk_restore_option['keyPairList'][0]['KeyId'] = kwargs.get('key_pair', None)
+            _attach_disk_restore_option['keyPairList'][0]['KeyName'] = kwargs.get('key_pair', None)
+            _attach_disk_restore_option['new_instance'] = True
+            _attach_disk_restore_option['ami'] = {'templateId': kwargs.get('ami_id', None)}
+            _attach_disk_restore_option['os_id'] = kwargs['os_id']
+
         # set attr for all the option in restore xml from user inputs
         self._set_restore_inputs(
             _attach_disk_restore_option,
             vm_to_restore=vm_to_restore,
             esx_server_name=instance_dict["clientName"],
             volume_level_restore=6,
             unconditional_overwrite=overwrite,
@@ -428,15 +437,17 @@
             resourcePoolPath=None,
             availability_zone=availability_zone,
             esx_host=availability_zone,
             newName=destination_vm,
             newGUID=destination_vm_guid,
             disk_name_prefix=disk_prefix,
             ami=_attach_disk_restore_option.get('ami', None),
-            vmSize=_attach_disk_restore_option.get('instance_type', None)
+            vmSize=_attach_disk_restore_option.get('instance_type', None),
+            new_instance=_attach_disk_restore_option.get('new_instance', None),
+            os_id=_attach_disk_restore_option.get('os_id', None)
         )
 
         request_json = self._prepare_attach_disk_restore_json(_attach_disk_restore_option)
         return self._process_restore_response(request_json)
 
     def full_vm_conversion_azurerm(
             self,
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/azure.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure_stack.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,78 +12,104 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # --------------------------------------------------------------------------
 
+"""File for operating on a Virtual Server AzureStack Subclient.
 
-"""File for operating on a Virtual Server Azure Subclient.
+AzureStackSubclient is the only class defined in this file.
 
-AzureSubclient is the only class defined in this file.
+AzureStackSubclient: Derived class from VirtualServerSubClient  Base class, representing a
+                           AzureStack Subclient, and to perform operations on that Subclient
 
-AzureSubclient: Derived class from VirtualServerSubClient  Base class, representing a
-                           Azure Subclient, and to perform operations on that Subclient
-
-AzureSubclient:
+AzureStackSubclient:
 
     full_vm_restore_out_of_place()                  --  restores the VM  specified in
-                                                     to the specified client, at the
+                                                        to the specified client, at the
                                                         specified destination location
 
-    full_vm_restore_in_place()              --  restores the VM specified by the
-                                                    user to the same location
+    full_vm_restore_in_place()                      --  restores the VM specified by the
+                                                        user to the same location
 """
 
-
 from ..vssubclient import VirtualServerSubclient
-from ...exception import SDKException
+from .azure_resource_manager import AzureRMSubclient
 
 
-class AzureSubclient(VirtualServerSubclient):
+class AzureStackSubclient(VirtualServerSubclient):
     """Derived class from VirtualServerSubclient  Base class, representing a
-    Azure  virtual server subclient,and to perform operations on that subclient."""
+    AzureStack virtual server subclient,and to perform operations on that subclient."""
+
+    def __init__(self, backupset_object, subclient_name, subclient_id=None):
+        """Initialize the Instance object for the given Virtual Server instance.
+        Args
+        class_object (backupset_object, subclient_name, subclient_id)  --  instance of the
+                                         backupset class, subclient name, subclient id
+
+        """
+        self.diskExtension = [".vhd", ".avhd"]
+        super(AzureStackSubclient, self).__init__(
+            backupset_object, subclient_name, subclient_id)
 
     def full_vm_restore_out_of_place(self,
                                      vm_to_restore=None,
-                                     cloud_service=None,
+                                     resource_group=None,
                                      storage_account=None,
                                      proxy_client=None,
                                      restore_new_name=None,
                                      overwrite=False,
                                      power_on=False,
+                                     instance_size=None,
+                                     public_ip=True,
+                                     restore_as_managed=True,
                                      copy_precedence=0,
                                      restore_option=None,
                                      **kwargs):
         """Restores the FULL Virtual machine specified  in the input  list to the client,
             at the specified destination location.
 
             Args:
-                cloud_service         (str)        --  provide the cloud service
 
-                storage_account     (str)          --  provide the storage account
+                vm_to_restore         (list)       --  provide the list of VM name(s) to restore
+
+                resource_group        (str)        -- provide the resource group to restore
+
+                storage_account       (str)        -- provide the storage account to restore
+
+                proxy_client          (str)        -- provide the proxy client to restore
+
+                restore_new_name      (str)        -- provide the new restore name
+
+                instance_size         (str)        -- provide the instance size of the restore VM
+
+                createPublicIP
+                        default:True   (bool)      --  creates the Public IP of the new VM
+
+                restoreAsManagedVM
+                        default:False   (bool)      --  new VM will be restored as unmanaged VM
 
-                vm_to_restore         (list)       --  provide the VM name to restore
 
                 overwrite
                         default:False   (bool)      --  overwrite the existing VM
 
                 poweron
                         default:False   (bool)      --  power on the  restored VM
 
+
                 restore_option      (dict)     --  complete dictionary with all advanced optio
                     default: {}
 
                 **kwargs                         : Arbitrary keyword arguments Properties as of
                                                      full_vm_restore_out_of_place
                     eg:
                     v2_details          (dict)       -- details for v2 subclient
                                                     eg: check clients.vmclient.VMClient._child_job_subclient_details
 
-
             Returns:
                 object - instance of the Job class for this restore job
 
             Raises:
                 SDKException:
 
                     if destination_path is not a string
@@ -91,94 +117,59 @@
                     if failed to initialize job
 
                     if response is empty
 
                     if response is not success
         """
 
-        # restore options
-        if restore_option is None:
+        if not restore_option:
             restore_option = {}
         restore_option["v2_details"] = kwargs.get("v2_details", None)
 
-        # check input parameters are correct
-        if bool(restore_option):
-            if not (isinstance(overwrite, bool) and
-                    isinstance(power_on, bool)):
-                raise SDKException('Subclient', '101')     
-                
-        self._set_restore_inputs(
-            restore_option,
-            vm_to_restore=self._set_vm_to_restore(vm_to_restore),
-            unconditional_overwrite=overwrite,
-            power_on=power_on,
-            copy_precedence=copy_precedence,
-            volume_level_restore=1,
-            esx_host=cloud_service,
-            datastore=storage_account,
-            client_name=proxy_client,
-            out_place=True,
-            restore_new_name=restore_new_name
-        )
-
-        # set attr for all the option in restore xml from user inputs
-
-        request_json = self._prepare_fullvm_restore_json(restore_option)
-        return self._process_restore_response(request_json)
+        AzureRMSubclient.full_vm_restore_out_of_place(
+            self, vm_to_restore, resource_group, storage_account,
+            proxy_client, restore_new_name, restore_option, overwrite, power_on,
+            instance_size, public_ip, restore_as_managed,
+            copy_precedence)
 
     def full_vm_restore_in_place(self,
                                  vm_to_restore=None,
                                  overwrite=True,
                                  power_on=True,
-                                 copy_precedence=0,
-                                 **kwargs):
+                                 public_ip=True,
+                                 restore_as_managed=False,
+                                 copy_precedence=0):
         """Restores the FULL Virtual machine specified  in the input  list to the client,
             to the location same as source .
 
             Args:
-                vm_to_restore         (list)       --  provide the VM name to restore
+                vm_to_restore         (list)       --  provide the of list VM name(s) to restore
+
+                createPublicIP
+                        default:True   (bool)      --  creates the Public IP of the new VM
+
+                restoreAsManagedVM
+                        default:False   (bool)      --  new VM will be restored as unmanaged VM
 
                 overwrite
                         default:true   (bool)      --  overwrite the existing VM
 
-                power_on                (bool)      --  power on the  restored VM
-                                                        default: True
-
-                copy_precedence       (int)         --  copy precedence value
-                                                        default: 0
+                poweron
+                        default:true   (bool)      --  power on the  restored VM
 
-                **kwargs                         : Arbitrary keyword arguments Properties as of
-                                                     full_vm_restore_in_place
-                    eg:
-                    v2_details          (dict)       -- details for v2 subclient
-                                                    eg: check clients.vmclient.VMClient._child_job_subclient_details
 
             Returns:
                 object - instance of the Job class for this restore job
 
             Raises:
                 SDKException:
 
                     if failed to initialize job
 
                     if response is empty
 
                     if response is not success
         """
-        restore_option = {"v2_details": kwargs.get("v2_details", None)}
-        # check mandatory input parameters are correct
-        if not (isinstance(overwrite, bool) and
-                isinstance(power_on, bool)):
-            raise SDKException('Subclient', '101')
-        # set attr for all the option in restore xml from user inputs
-        self._set_restore_inputs(
-            restore_option,
-            vm_to_restore=self._set_vm_to_restore(vm_to_restore),
-            unconditional_overwrite=overwrite,
-            power_on=power_on,
-            copy_preceedence=copy_precedence,
-            volume_level_restore=1,
-            out_place=False
-        )
-        request_json = self._prepare_fullvm_restore_json(restore_option)
-        return self._process_restore_response(request_json)
-    
+
+        AzureRMSubclient.full_vm_restore_in_place(
+            self, overwrite, power_on,
+            public_ip, restore_as_managed, copy_precedence)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/azure_resource_manager.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure_resource_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                                      restore_option=None,
                                      **kwargs):
         """Restores the FULL Virtual machine specified  in the input  list to the client,
             at the specified destination location.
 
             Args:
 
-                vm_to_restore         (list)       --  provide the VM name to restore
+                vm_to_restore         (list)       --  provide the list of VM name(s) to restore
 
                 resource_group        (str)        -- provide the resource group to restore
 
                 storage_account       (str)        -- provide the storage account to restore
 
                 proxy_client          (str)        -- provide the proxy client to restore
 
@@ -174,15 +174,15 @@
                                  restore_as_managed=False,
                                  copy_precedence=0,
                                  **kwargs):
         """Restores the FULL Virtual machine specified  in the input  list to the client,
             to the location same as source .
 
             Args:
-                vm_to_restore         (list)       --  provide the VM name to restore
+                vm_to_restore         (list)       --  provide the list of VM name(s) to restore
 
                 createPublicIP
                         default:True   (bool)      --  creates the Public IP of the new VM
 
                 restoreAsManagedVM
                         default:False   (bool)      --  new VM will be restored as unmanaged VM
 
@@ -244,15 +244,15 @@
             public_ip=False,
             restore_as_managed=False,
             copy_precedence=0,
             restore_option=None):
         """
                 This converts the AzureRM to Azurestack
                 Args:
-                        vm_to_restore          (list):     provide the VM names to restore
+                        vm_to_restore          (list):     provide the list of VM name(s) to restore
 
                         azure_client    (str):      name of the AzureRM client
                                                            where the VM should be
                                                            restored.
 
                         resource_group   (str):      destination Resource group
                                                             in the AzureRM
@@ -338,15 +338,15 @@
             amazon_bucket=None,
             overwrite=True,
             power_on=True,
             copy_precedence=0):
         """
                 This converts the AzureRM to Amazon
                 Args:
-                        vm_to_restore          (list):     provide the VM names to restore
+                        vm_to_restore          (list):     provide the list of VM name(s) to restore
 
                         amazon_client    (str):     name of the Amazon client
                                                            where the VM should be
                                                            restored.
 
                         overwrite              (bool):     overwrite the existing VM
                                                            default: True
@@ -523,18 +523,20 @@
             destination_network=destination_network,
             volume_level_restore=0,
             destination_instance=instance.instance_name,
             backupset_client_name=instance._agent_object._client_object.client_name
         )
 
         request_json = self._prepare_fullvm_restore_json(restore_option)
-        disk_options = request_json['taskInfo']['subTasks'][0]['options']['restoreOptions']['virtualServerRstOption']['diskLevelVMRestoreOption']
+        disk_options = request_json['taskInfo']['subTasks'][0]['options']['restoreOptions'][
+            'virtualServerRstOption']['diskLevelVMRestoreOption']
         for disk_info in disk_options['advancedRestoreOptions'][0]['disks']:
             disk_info['newName'] = ''
-        request_json['taskInfo']['subTasks'][0]['options']['restoreOptions']['volumeRstOption']['volumeLevelRestoreType'] = 1
+        request_json['taskInfo']['subTasks'][0]['options']['restoreOptions'][
+            'volumeRstOption']['volumeLevelRestoreType'] = 1
 
         return self._process_restore_response(request_json)
 
 
     def full_vm_conversion_vmware(
             self,
             vcenter_client,
@@ -648,12 +650,13 @@
             destination_instance=instance.instance_name,
             backupset_client_name=instance._agent_object._client_object.client_name,
             destination_network=destination_network,
             destination_os_name=destination_os_name
         )
 
         request_json = self._prepare_fullvm_restore_json(restore_option)
-        disk_options = request_json['taskInfo']['subTasks'][0]['options']['restoreOptions']['virtualServerRstOption']['diskLevelVMRestoreOption']
+        disk_options = request_json['taskInfo']['subTasks'][0]['options']['restoreOptions'][
+            'virtualServerRstOption']['diskLevelVMRestoreOption']
         for disk_info in disk_options['advancedRestoreOptions'][0]['disks']:
             disk_info['newName'] = ''
 
         return self._process_restore_response(request_json)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/azure_stack.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/hyperv_live_sync.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,164 +12,161 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # --------------------------------------------------------------------------
 
-"""File for operating on a Virtual Server AzureStack Subclient.
+"""File for configuring and monitoring live sync on the Hyper-V subclient.
 
-AzureStackSubclient is the only class defined in this file.
+HyperVLiveSync is the only class defined in this file.
 
-AzureStackSubclient: Derived class from VirtualServerSubClient  Base class, representing a
-                           AzureStack Subclient, and to perform operations on that Subclient
+HyperVLiveSync: Class for configuring and monitoring Hyper-V subclient live sync
 
-AzureStackSubclient:
+HyperVLiveSync:
 
-    full_vm_restore_out_of_place()                  --  restores the VM  specified in
-                                                        to the specified client, at the
-                                                        specified destination location
+    generate_restore_options_json()     -- To generate the restore options json for Hyper-V live sync
 
-    full_vm_restore_in_place()                      --  restores the VM specified by the
-                                                        user to the same location
 """
 
-from ..vssubclient import VirtualServerSubclient
-from .azure_resource_manager import AzureRMSubclient
+from .vsa_live_sync import VsaLiveSync
+from ....exception import SDKException
 
 
-class AzureStackSubclient(VirtualServerSubclient):
-    """Derived class from VirtualServerSubclient  Base class, representing a
-    AzureStack virtual server subclient,and to perform operations on that subclient."""
-
-    def __init__(self, backupset_object, subclient_name, subclient_id=None):
-        """Initialize the Instance object for the given Virtual Server instance.
-        Args
-        class_object (backupset_object, subclient_name, subclient_id)  --  instance of the
-                                         backupset class, subclient name, subclient id
+class HyperVLiveSync(VsaLiveSync):
+    """Class for configuring and monitoring Hyper-V live sync operations"""
 
-        """
-        self.diskExtension = [".vhd", ".avhd"]
-        super(AzureStackSubclient, self).__init__(
-            backupset_object, subclient_name, subclient_id)
-
-    def full_vm_restore_out_of_place(self,
-                                     vm_to_restore=None,
-                                     resource_group=None,
-                                     storage_account=None,
-                                     proxy_client=None,
-                                     restore_new_name=None,
-                                     overwrite=False,
-                                     power_on=False,
-                                     instance_size=None,
-                                     public_ip=True,
-                                     restore_as_managed=True,
-                                     copy_precedence=0,
-                                     restore_option=None,
-                                     **kwargs):
-        """Restores the FULL Virtual machine specified  in the input  list to the client,
-            at the specified destination location.
-
-            Args:
-
-                vm_to_restore         (list)       --  provide the VM name to restore
-
-                resource_group        (str)        -- provide the resource group to restore
-
-                storage_account       (str)        -- provide the storage account to restore
-
-                proxy_client          (str)        -- provide the proxy client to restore
-
-                restore_new_name      (str)        -- provide the new restore name
-
-                instance_size         (str)        -- provide the instance size of the restore VM
-
-                createPublicIP
-                        default:True   (bool)      --  creates the Public IP of the new VM
-
-                restoreAsManagedVM
-                        default:False   (bool)      --  new VM will be restored as unmanaged VM
-
-
-                overwrite
-                        default:False   (bool)      --  overwrite the existing VM
-
-                poweron
-                        default:False   (bool)      --  power on the  restored VM
-
-
-                restore_option      (dict)     --  complete dictionary with all advanced optio
-                    default: {}
-
-                **kwargs                         : Arbitrary keyword arguments Properties as of
-                                                     full_vm_restore_out_of_place
-                    eg:
-                    v2_details          (dict)       -- details for v2 subclient
-                                                    eg: check clients.vmclient.VMClient._child_job_subclient_details
+    def configure_live_sync(self,
+                            schedule_name=None,
+                            destination_client=None,
+                            proxy_client=None,
+                            copy_precedence=0,
+                            vm_to_restore=None,
+                            destination_path=None,
+                            destination_network=None,
+                            power_on=True,
+                            overwrite=False,
+                            distribute_vm_workload=None,
+                            restored_vm_name=None,
+                            restore_option=None,
+                            pattern_dict=None
+                            ):
+        """To configure live
+
+        Args:
+
+            schedule_name               (str)   -- Name of the Live sync schedule to be created
+
+            destination_client          (str)   -- Hyperv Host Client Name where VM needs to be restored
+
+            proxy_client                (str)   -- Name of the proxy client to be used
+
+            copy_precedence             (int)   -- Copy id from which restore needs to be performed
+                                                    default: 0
+
+            vm_to_restore               (list)  -- VM's to be restored
+
+            destination_path            (str)   -- Full path of the restore location on client
+
+            destination_network         (str)   -- Network card name on the destination machine
+
+            power_on                    (bool)  -- To validate destination VM power on and off
+                                                    default: True
+
+            overwrite                   (bool)  -- To overwrite VM and VHDs in destination path
+                                                    default: False
+
+            distribute_vm_workload      (int)   -- Virtual machines to be used per job
+
+            restored_vm_name            (str)   -- Name used for the VM when restored
+
+            restore_option              (dict)  -- Restore options dictionary with advanced options
+
+            pattern_dict                (dict)  -- Dictionary to generate the live sync schedule
+
+                Sample:
+
+                    for after_job_completes :
+                    {
+                        "freq_type": 'after_job_completes',
+                        "active_start_date": date_in_%m/%d/%y (str),
+                        "active_start_time": time_in_%H/%S (str),
+                        "repeat_days": days_to_repeat (int)
+                    }
+
+                    for daily:
+                    {
+                         "freq_type": 'daily',
+                         "active_start_time": time_in_%H/%S (str),
+                         "repeat_days": days_to_repeat (int)
+                    }
+
+                    for weekly:
+                    {
+                         "freq_type": 'weekly',
+                         "active_start_time": time_in_%H/%S (str),
+                         "repeat_weeks": weeks_to_repeat (int)
+                         "weekdays": list of weekdays ['Monday','Tuesday']
+                    }
+
+                    for monthly:
+                    {
+                         "freq_type": 'monthly',
+                         "active_start_time": time_in_%H/%S (str),
+                         "repeat_months": weeks_to_repeat (int)
+                         "on_day": Day to run schedule (int)
+                    }
+
+                    for yearly:
+                    {
+                         "active_start_time": time_in_%H/%S (str),
+                         "on_month": month to run schedule (str) January, Febuary...
+                         "on_day": Day to run schedule (int)
+                    }
 
-            Returns:
-                object - instance of the Job class for this restore job
+        Returns:
+            object - instance of the Schedule class for this Live sync
 
-            Raises:
-                SDKException:
-
-                    if destination_path is not a string
-
-                    if failed to initialize job
-
-                    if response is empty
-
-                    if response is not success
         """
-
-        if not restore_option:
+        # restore options
+        if restore_option is None:
             restore_option = {}
-        restore_option["v2_details"] = kwargs.get("v2_details", None)
-
-        AzureRMSubclient.full_vm_restore_out_of_place(
-            self, vm_to_restore, resource_group, storage_account,
-            proxy_client, restore_new_name, restore_option, overwrite, power_on,
-            instance_size, public_ip, restore_as_managed,
-            copy_precedence)
-
-    def full_vm_restore_in_place(self,
-                                 vm_to_restore=None,
-                                 overwrite=True,
-                                 power_on=True,
-                                 public_ip=True,
-                                 restore_as_managed=False,
-                                 copy_precedence=0):
-        """Restores the FULL Virtual machine specified  in the input  list to the client,
-            to the location same as source .
-
-            Args:
-                vm_to_restore         (list)       --  provide the VM name to restore
-
-                createPublicIP
-                        default:True   (bool)      --  creates the Public IP of the new VM
 
-                restoreAsManagedVM
-                        default:False   (bool)      --  new VM will be restored as unmanaged VM
+        if vm_to_restore and not isinstance(vm_to_restore, str):
+            raise SDKException('Subclient', '101')
 
-                overwrite
-                        default:true   (bool)      --  overwrite the existing VM
-
-                poweron
-                        default:true   (bool)      --  power on the  restored VM
-
-
-            Returns:
-                object - instance of the Job class for this restore job
-
-            Raises:
-                SDKException:
-
-                    if failed to initialize job
-
-                    if response is empty
-
-                    if response is not success
-        """
+        if not restored_vm_name and isinstance(vm_to_restore, str):
+            restored_vm_name = "LiveSync_"
+        restore_option['restore_new_name'] = restored_vm_name
+
+        if copy_precedence:
+            restore_option["copy_precedence_applicable"] = True
+
+        if vm_to_restore:
+            vm_to_restore = [vm_to_restore]
+
+        # check mandatory input parameters are correct
+        if bool(restore_option):
+            if not (isinstance(destination_path, str) and
+                    isinstance(overwrite, bool) and
+                    isinstance(power_on, bool)):
+                raise SDKException('Subclient', '101')
+
+        # set attr for all the option in restore xml from user inputs
+        self._subclient_object._set_restore_inputs(
+            restore_option,
+            vm_to_restore=self._subclient_object._set_vm_to_restore(vm_to_restore),
+            unconditional_overwrite=overwrite,
+            power_on=power_on,
+            distribute_vm_workload=distribute_vm_workload,
+            copy_precedence=copy_precedence,
+            volume_level_restore=1,
+            vcenter_client=destination_client,
+            client_name=proxy_client,
+            esx_server=proxy_client,
+            esx_host=proxy_client,
+            datastore=destination_path,
+            destination_network=destination_network,
+            in_place=False
+        )
 
-        AzureRMSubclient.full_vm_restore_in_place(
-            self, overwrite, power_on,
-            public_ip, restore_as_managed, copy_precedence)
+        return self._configure_live_sync(schedule_name, restore_option, pattern_dict)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/fusioncompute.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/google_cloud_platform.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,77 +12,72 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # --------------------------------------------------------------------------
 
-"""File for operating on a Virtual Server FusionCompute Subclient.
+"""File for operating on a Virtual Server Googlecloud Subclient.
 
-FusionComputeVirtualServerSubclient is the only class defined in this file.
+GooglecloudVirtualServerSubclient is the only class defined in this file.
 
-FusionComputeVirtualServerSubclient: Derived class from VirtualServerSubClient  Base class,
-                            representing a FusionCompute Subclient, and
-                            to perform operations on that Subclient
+GooglecloudVirtualServerSubclient: Derived class from VirtualServerSubClient  Base class,
+                                   representing a FusionCompute Subclient, and
+                                   to perform operations on that Subclient
 
-FusionComputeVirtualServerSubclient:
+GooglecloudVirtualServerSubclient:
 
-    __init__(,backupset_object, subclient_name, subclient_id)--  initialize object of FusionCompute
+    __init__(,backupset_object, subclient_name, subclient_id)--  initialize object of googlecloud
                                                                              subclient object
                                                                                  associated with
                                                                         the VirtualServer subclient
 
     full_vm_restore_out_of_place()                  --  restores the VM  specified in
                                                      to the specified client, at the
                                                         specified destination location
 
     full_vm_restore_in_place()              --  restores the VM specified by the
                                                     user to the same location
 """
-from cvpysdk.exception import SDKException
+
 from ..vssubclient import VirtualServerSubclient
+from ...exception import SDKException
 
 
-class FusionComputeVirtualServerSubclient(VirtualServerSubclient):
+class GooglecloudVirtualServerSubclient(VirtualServerSubclient):
     """Derived class from VirtualServerSubclient Base class.
-       This represents a Fusion Compute virtual server subclient,
+       This represents a Google cloud virtual server subclient,
        and can perform restore operations on only that subclient.
 
     """
     def __init__(self, backupset_object, subclient_name, subclient_id=None):
         """Initialize the Instance object for the given Virtual Server instance.
         Args
         class_object (backupset_object, subclient_name, subclient_id)  --  instance of the
                                          backupset class, subclient name, subclient id
 
         """
-        super(FusionComputeVirtualServerSubclient, self).__init__(
+        super(GooglecloudVirtualServerSubclient, self).__init__(
             backupset_object, subclient_name, subclient_id)
         self.diskExtension = ["none"]
 
-        self._disk_option = {
-            'original': 0,
-            'thicklazyzero': 1,
-            'thin': 2,
-            'common': 3
-        }
-
     def full_vm_restore_in_place(
             self,
             vm_to_restore=None,
             overwrite=True,
             power_on=True,
             proxy_client=None,
             copy_precedence=0,
+            zone=None,
             **kwargs):
         """Restores the FULL Virtual machine specified in the input list
             to the location same as the actual location of the VM in VCenter.
 
             Args:
-                vm_to_restore       (list)     --  provide the VM name to
+                vm_to_restore       (list)     --  provide the list of VM name to
                                                    restore
                                                    default: None
 
                 overwrite           (bool)     --  overwrite the existing VM
                                                    default: True
 
                 power_on            (bool)     --  power on the  restored VM
@@ -91,15 +86,15 @@
                 copy_precedence     (int)      --  copy precedence value
                                                    default: 0
 
                 proxy_client          (str)  --  proxy client to be used for restore
                                                         default: proxy added in subclient
 
                 **kwargs                         : Arbitrary keyword arguments Properties as of
-                                                     full_vm_restore_out_of_place
+                                                     full_vm_restore_in_place
                     eg:
                     v2_details          (dict)       -- details for v2 subclient
                                                     eg: check clients.vmclient.VMClient._child_job_subclient_details
 
             Returns:
                 object - instance of the Job class for this restore job
 
@@ -110,15 +105,15 @@
                     if failed to initialize job
 
                     if response is empty
 
                     if response is not success
 
         """
-        restore_option = {"v2_details": kwargs.get("v2_details", None)}
+        restore_option = {"v2_details": kwargs.get("v2_details", None), "datacenter": zone[:-2]}
 
         # set attr for all the option in restore xml from user inputs
         self._set_restore_inputs(
             restore_option,
             unconditional_overwrite=overwrite,
             power_on=power_on,
             copy_precedence=copy_precedence,
@@ -130,73 +125,57 @@
 
         request_json = self._prepare_fullvm_restore_json(restore_option)
         return self._process_restore_response(request_json)
 
     def full_vm_restore_out_of_place(
             self,
             vm_to_restore=None,
-            destination_client=None,
             proxy_client=None,
             new_name=None,
-            host=None,
-            datastore=None,
+            zone=None,
+            machine_type=None,
             overwrite=True,
             power_on=True,
+            public_ip=False,
             copy_precedence=0,
-            disk_provisioning='original',
+            project_id=None,
+            restore_option=None,
             **kwargs):
-        """Restores the FULL Virtual machine specified in the input list
-            to the provided vcenter client along with the ESX and the datastores.
-            If the provided client name is none then it restores the Full Virtual
-            Machine to the source client and corresponding ESX and datastore.
+
+        """Restores the FULL Virtual machine specified  in the input  list to the client,
+            at the specified destination location.
+
 
             Args:
-                vm_to_restore     (list)  --  provide the VM name to restore
-                                              default: None
+                vm_to_restore     (list):       provide the list of VM name to restore
+                                                default: None
 
-                destination_client    (str) -- name of the Pseudo client
-                                                  where the VM should be
-                                                    restored.
-
-                new_name          (str) -- new name to be given to the
-                                                    restored VM
-
-                host          (str) -- destination cluster or  host
-                                                    restores to the source VM
-                                                    esx if this value is not
-                                                    specified
-
-                datastore         (str) -- datastore where the
-                                                  restored VM should be located
-                                                  restores to the source VM
-                                                  datastore if this value is
-                                                  not specified
+                proxy_client     (str):         proxy client to be used for restore
+                                                default: proxy added in subclient
 
-                overwrite         (bool)       -- overwrite the existing VM
-                                                  default: True
+                new_name         (str):         new name to be given to the
+                                                restored VM
 
-                power_on          (bool)       -- power on the  restored VM
+                overwrite         (bool):        overwrite the existing VM
+                                                 default: True
+
+                power_on          (bool):        power on the  restored VM
                                                   default: True
 
                 copy_precedence   (int)        -- copy precedence value
                                                   default: 0
 
-                disk_provisioning       (str) -- disk provisioning for the
-                                                  restored vm
-                                                  default: 0 which is equivalent
-                                                  to Original
-                proxy_client     (str)  --  proxy client to be used for restore
-                                                        default: proxy added in subclient
-
                 **kwargs                         : Arbitrary keyword arguments Properties as of
                                                      full_vm_restore_out_of_place
                     eg:
                     v2_details          (dict)       -- details for v2 subclient
                                                     eg: check clients.vmclient.VMClient._child_job_subclient_details
-
+                    destination_network (string)     -- Name of the destination network
+                    networks_nic        (string)     -- Link for the destination network
+                    subnetwork_nic      (string)    -- Link for the destination subnetwork
 
             Returns:
                 object - instance of the Job class for this restore job
 
             Raises:
                 SDKException:
                     if inputs are not of correct type as per definition
@@ -204,37 +183,51 @@
                     if failed to initialize job
 
                     if response is empty
 
                     if response is not success
 
         """
-        restore_option = {"v2_details": kwargs.get("v2_details", None)}
+        restore_option = {}
+        extra_options = ['destination_network', 'networks_nic', 'subnetwork_nic']
+        for key in extra_options:
+            if key in kwargs:
+                restore_option[key] = kwargs[key]
+            else:
+                restore_option[key] = None
 
         if vm_to_restore:
             vm_to_restore = [vm_to_restore]
 
         if new_name:
-            if not(isinstance(vm_to_restore, str) or
-                   isinstance(new_name, str)):
-                raise SDKException('Subclient', '101')
             restore_option['restore_new_name'] = new_name
 
+        if bool(restore_option):
+            if not (isinstance(overwrite, bool) and
+                    isinstance(power_on, bool)):
+                raise SDKException('Subclient', '101')
+        restore_option["datacenter"] = zone[:-2]
+        if kwargs.get("replica_zone"):
+            restore_option["replicaZones"] = []
+            restore_option["replicaZones"].append(zone)
+            restore_option["replicaZones"].append(kwargs.get("replica_zone"))
+
         # set attr for all the option in restore xml from user inputs
         self._set_restore_inputs(
             restore_option,
             vm_to_restore=self._set_vm_to_restore(vm_to_restore),
             unconditional_overwrite=overwrite,
             power_on=power_on,
-            disk_option=self._disk_option[disk_provisioning],
             copy_precedence=copy_precedence,
             volume_level_restore=1,
             client_name=proxy_client,
-            vcenter_client=destination_client,
-            esx_host=host,
-            datastore=datastore,
+            esx_host=zone,
+            vm_size=machine_type,
+            datacenter=zone,
             in_place=False,
+            createPublicIP=public_ip,
+            project_id=project_id,
             restore_new_name=new_name
         )
 
         request_json = self._prepare_fullvm_restore_json(restore_option)
         return self._process_restore_response(request_json)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/google_cloud_platform.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/xen.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,91 +12,84 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # --------------------------------------------------------------------------
 
-"""File for operating on a Virtual Server Googlecloud Subclient.
+"""File for operating on a Virtual Server FusionCompute Subclient.
 
-GooglecloudVirtualServerSubclient is the only class defined in this file.
+XenSubclient is the only class defined in this file.
 
-GooglecloudVirtualServerSubclient: Derived class from VirtualServerSubClient  Base class,
-                                   representing a FusionCompute Subclient, and
-                                   to perform operations on that Subclient
+XenSubclient: Derived class from VirtualServerSubClient  Base class,
+                            representing a FusionCompute Subclient, and
+                            to perform operations on that Subclient
 
-GooglecloudVirtualServerSubclient:
+XenSubclient:
 
-    __init__(,backupset_object, subclient_name, subclient_id)--  initialize object of googlecloud
+    __init__(,backupset_object, subclient_name, subclient_id)--  initialize object of FusionCompute
                                                                              subclient object
                                                                                  associated with
                                                                         the VirtualServer subclient
 
     full_vm_restore_out_of_place()                  --  restores the VM  specified in
                                                      to the specified client, at the
                                                         specified destination location
 
     full_vm_restore_in_place()              --  restores the VM specified by the
                                                     user to the same location
 """
-
+from cvpysdk.exception import SDKException
 from ..vssubclient import VirtualServerSubclient
-from ...exception import SDKException
 
 
-class GooglecloudVirtualServerSubclient(VirtualServerSubclient):
+class Xen(VirtualServerSubclient):
     """Derived class from VirtualServerSubclient Base class.
-       This represents a Google cloud virtual server subclient,
+       This represents a Fusion Compute virtual server subclient,
        and can perform restore operations on only that subclient.
 
     """
     def __init__(self, backupset_object, subclient_name, subclient_id=None):
         """Initialize the Instance object for the given Virtual Server instance.
         Args
         class_object (backupset_object, subclient_name, subclient_id)  --  instance of the
                                          backupset class, subclient name, subclient id
 
         """
-        super(GooglecloudVirtualServerSubclient, self).__init__(
+        super(Xen, self).__init__(
             backupset_object, subclient_name, subclient_id)
         self.diskExtension = ["none"]
 
     def full_vm_restore_in_place(
             self,
             vm_to_restore=None,
             overwrite=True,
             power_on=True,
             proxy_client=None,
-            copy_precedence=0,
-            **kwargs):
+            copy_precedence=0):
         """Restores the FULL Virtual machine specified in the input list
             to the location same as the actual location of the VM in VCenter.
 
             Args:
                 vm_to_restore       (list)     --  provide the VM name to
                                                    restore
                                                    default: None
 
                 overwrite           (bool)     --  overwrite the existing VM
                                                    default: True
 
                 power_on            (bool)     --  power on the  restored VM
                                                    default: True
 
-                copy_precedence     (int)      --  copy precedence value
-                                                   default: 0
 
                 proxy_client          (str)  --  proxy client to be used for restore
                                                         default: proxy added in subclient
 
-                **kwargs                         : Arbitrary keyword arguments Properties as of
-                                                     full_vm_restore_in_place
-                    eg:
-                    v2_details          (dict)       -- details for v2 subclient
-                                                    eg: check clients.vmclient.VMClient._child_job_subclient_details
+                copy_precedence       (int)         --  copy precedence value
+                                                        default: 0
 
             Returns:
                 object - instance of the Job class for this restore job
 
             Raises:
                 SDKException:
                     if inputs are not of correct type as per definition
@@ -104,15 +97,15 @@
                     if failed to initialize job
 
                     if response is empty
 
                     if response is not success
 
         """
-        restore_option = {"v2_details": kwargs.get("v2_details", None)}
+        restore_option = {}
 
         # set attr for all the option in restore xml from user inputs
         self._set_restore_inputs(
             restore_option,
             unconditional_overwrite=overwrite,
             power_on=power_on,
             copy_precedence=copy_precedence,
@@ -124,57 +117,62 @@
 
         request_json = self._prepare_fullvm_restore_json(restore_option)
         return self._process_restore_response(request_json)
 
     def full_vm_restore_out_of_place(
             self,
             vm_to_restore=None,
+            destination_client=None,
             proxy_client=None,
             new_name=None,
-            zone=None,
-            machine_type=None,
+            xen_server=None,
+            storage=None,
             overwrite=True,
             power_on=True,
-            public_ip=False,
             copy_precedence=0,
-            project_id=None,
-            restore_option=None,
             **kwargs):
-
-        """Restores the FULL Virtual machine specified  in the input  list to the client,
-            at the specified destination location.
-
+        """Restores the FULL Virtual machine specified in the input list
+            to the provided vcenter client along with the ESX and the datastores.
+            If the provided client name is none then it restores the Full Virtual
+            Machine to the source client and corresponding ESX and datastore.
 
             Args:
-                vm_to_restore     (list):       provide the VM name to restore
-                                                default: None
-
-                proxy_client     (str):         proxy client to be used for restore
-                                                default: proxy added in subclient
+                vm_to_restore     (list)  --  provide the VM name to restore
+                                              default: None
 
-                new_name         (str):         new name to be given to the
-                                                restored VM
+                destination_client    (str) -- name of the Pseudo client
+                                                  where the VM should be
+                                                    restored.
+
+                new_name          (str) -- new name to be given to the
+                                                    restored VM
+
+                xen_server          (str) -- destination cluster or  host
+                                                    restores to the source VM
+                                                    esx if this value is not
+                                                    specified
+
+                storage         (str) -- datastore where the
+                                                  restored VM should be located
+                                                  restores to the source VM
+                                                  datastore if this value is
+                                                  not specified
 
-                overwrite         (bool):        overwrite the existing VM
-                                                 default: True
+                overwrite         (bool)       -- overwrite the existing VM
+                                                  default: True
 
-                power_on          (bool):        power on the  restored VM
+                power_on          (bool)       -- power on the  restored VM
                                                   default: True
 
                 copy_precedence   (int)        -- copy precedence value
                                                   default: 0
 
-                **kwargs                         : Arbitrary keyword arguments Properties as of
-                                                     full_vm_restore_out_of_place
-                    eg:
-                    v2_details          (dict)       -- details for v2 subclient
-                                                    eg: check clients.vmclient.VMClient._child_job_subclient_details
-                    destination_network (string)     -- Name of the destination network
-                    networks_nic        (string)     -- Link for the destination network
-                    subnetwork_nic      (string)    -- Link for the destination subnetwork
+                proxy_client     (str)  --  proxy client to be used for restore
+                                                        default: proxy added in subclient
+
 
             Returns:
                 object - instance of the Job class for this restore job
 
             Raises:
                 SDKException:
                     if inputs are not of correct type as per definition
@@ -183,45 +181,39 @@
 
                     if response is empty
 
                     if response is not success
 
         """
         restore_option = {}
-        extra_options = ['destination_network', 'networks_nic', 'subnetwork_nic']
+        extra_options = ['v2_details']
+
         for key in extra_options:
-            if key in kwargs:
-                restore_option[key] = kwargs[key]
-            else:
-                restore_option[key] = None
+            restore_option[key] = kwargs[key] if key in kwargs else None
 
         if vm_to_restore:
             vm_to_restore = [vm_to_restore]
 
         if new_name:
-            restore_option['restore_new_name'] = new_name
-
-        if bool(restore_option):
-            if not (isinstance(overwrite, bool) and
-                    isinstance(power_on, bool)):
+            if not(isinstance(vm_to_restore, str) or
+                   isinstance(new_name, str)):
                 raise SDKException('Subclient', '101')
+            restore_option['restore_new_name'] = new_name
 
         # set attr for all the option in restore xml from user inputs
         self._set_restore_inputs(
             restore_option,
             vm_to_restore=self._set_vm_to_restore(vm_to_restore),
             unconditional_overwrite=overwrite,
             power_on=power_on,
             copy_precedence=copy_precedence,
             volume_level_restore=1,
             client_name=proxy_client,
-            esx_host=zone,
-            vm_size=machine_type,
-            datacenter=zone,
+            vcenter_client=destination_client,
+            esx_host=xen_server,
+            datastore=storage,
             in_place=False,
-            createPublicIP=public_ip,
-            project_id=project_id,
             restore_new_name=new_name
         )
 
         request_json = self._prepare_fullvm_restore_json(restore_option)
         return self._process_restore_response(request_json)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/hyperv.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/hyperv.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 
             Args:
                 client                (str/object) --  either the name of the client or
                                                            the instance of the Client
 
                 destination_path      (str)        --  full path of the restore location on client
 
-                vm_to_restore         (list)       --  provide the VM name to restore
+                vm_to_restore         (list)       --  provide the list of VM name(s) to restore
 
                 overwrite
                         default:False   (bool)      --  overwrite the existing VM
 
                 poweron
                         default:False   (bool)      --  power on the  restored VM
 
@@ -360,15 +360,15 @@
                                  add_to_failover=False,
                                  snap_proxy=None,
                                  **kwargs):
         """Restores the FULL Virtual machine specified  in the input  list to the client,
             to the location same as source .
 
             Args:
-                vm_to_restore         (list)       --  provide the VM name to restore
+                vm_to_restore         (list)       --  provide the list of VM name(s) to restore
 
                 overwrite
                         default:true   (bool)      --  overwrite the existing VM
 
                 poweron
                         default:true   (bool)      --  power on the  restored VM
 
@@ -583,18 +583,19 @@
             networkDisplayName=None,
             networkrsg=None,
             destsubid=None,
             subnetId=None):
         """
                 This converts the Hyperv VM to AzureRM
                 Args:
-                        vm_to_restore          (dict):     dict containing the VM name(s) to restore as
-                                                           keys and the new VM name(s) as their values.
-                                                           Input empty string for default VM name for
-                                                           restored VM.
+                        vm_to_restore          (dict):     dict containing the VM name(s)
+                                                           to restore as keys and the new
+                                                           VM name(s) as their values.
+                                                           Input empty string for default
+                                                           VM name for restored VM.
                                                            default: {}
 
                         azure_client    (str):      name of the AzureRM client
                                                            where the VM should be
                                                            restored.
 
                         resource_group   (str):      destination Resource group
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/kubernetes.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/kubernetes.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/__init__.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/amazon_live_sync.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/amazon_live_sync.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/azure_live_sync.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/azure_live_sync.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/hyperv_live_sync.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/vmware_live_sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,75 +12,74 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # --------------------------------------------------------------------------
 
-"""File for configuring and monitoring live sync on the Hyper-V subclient.
+"""File for configuring and monitoring live sync on the VMW subclient.
 
-HyperVLiveSync is the only class defined in this file.
+VMWareLiveSync is the only class defined in this file.
 
-HyperVLiveSync: Class for configuring and monitoring Hyper-V subclient live sync
+VMWareLiveSync: Class for configuring and monitoring VMWare subclient live sync
 
-HyperVLiveSync:
+VMWareLiveSync:
 
-    generate_restore_options_json()     -- To generate the restore options json for Hyper-V live sync
+    configure_live_sync()     -- To configure live sync from supplied parameters
 
 """
 
 from .vsa_live_sync import VsaLiveSync
 from ....exception import SDKException
 
 
-class HyperVLiveSync(VsaLiveSync):
-    """Class for configuring and monitoring Hyper-V live sync operations"""
-
+class VMWareLiveSync(VsaLiveSync):
+    """Class for configuring and monitoring VMWare live sync operations"""
     def configure_live_sync(self,
                             schedule_name=None,
                             destination_client=None,
                             proxy_client=None,
                             copy_precedence=0,
                             vm_to_restore=None,
-                            destination_path=None,
                             destination_network=None,
                             power_on=True,
                             overwrite=False,
                             distribute_vm_workload=None,
+                            datastore=None,
                             restored_vm_name=None,
                             restore_option=None,
-                            pattern_dict=None
+                            pattern_dict=None,
                             ):
         """To configure live
 
         Args:
 
             schedule_name               (str)   -- Name of the Live sync schedule to be created
 
-            destination_client          (str)   -- Hyperv Host Client Name where VM needs to be restored
+            destination_client          (str)   -- VMWare Host Client Name where VM needs to be restored
 
             proxy_client                (str)   -- Name of the proxy client to be used
 
             copy_precedence             (int)   -- Copy id from which restore needs to be performed
                                                     default: 0
 
             vm_to_restore               (list)  -- VM's to be restored
 
-            destination_path            (str)   -- Full path of the restore location on client
-
             destination_network         (str)   -- Network card name on the destination machine
 
             power_on                    (bool)  -- To validate destination VM power on and off
                                                     default: True
 
             overwrite                   (bool)  -- To overwrite VM and VHDs in destination path
                                                     default: False
 
             distribute_vm_workload      (int)   -- Virtual machines to be used per job
 
+            datastore                   (str)   -- Datastore to restore the VM
+
             restored_vm_name            (str)   -- Name used for the VM when restored
 
             restore_option              (dict)  -- Restore options dictionary with advanced options
 
             pattern_dict                (dict)  -- Dictionary to generate the live sync schedule
 
                 Sample:
@@ -127,46 +126,40 @@
             object - instance of the Schedule class for this Live sync
 
         """
         # restore options
         if restore_option is None:
             restore_option = {}
 
-        if vm_to_restore and not isinstance(vm_to_restore, str):
-            raise SDKException('Subclient', '101')
-
-        if not restored_vm_name and isinstance(vm_to_restore, str):
+        if not restored_vm_name:
             restored_vm_name = "LiveSync_"
         restore_option['restore_new_name'] = restored_vm_name
 
         if copy_precedence:
             restore_option["copy_precedence_applicable"] = True
 
         if vm_to_restore:
             vm_to_restore = [vm_to_restore]
 
         # check mandatory input parameters are correct
         if bool(restore_option):
-            if not (isinstance(destination_path, str) and
-                    isinstance(overwrite, bool) and
+            if not (isinstance(overwrite, bool) and
                     isinstance(power_on, bool)):
                 raise SDKException('Subclient', '101')
 
         # set attr for all the option in restore xml from user inputs
         self._subclient_object._set_restore_inputs(
             restore_option,
             vm_to_restore=self._subclient_object._set_vm_to_restore(vm_to_restore),
             unconditional_overwrite=overwrite,
             power_on=power_on,
             distribute_vm_workload=distribute_vm_workload,
             copy_precedence=copy_precedence,
             volume_level_restore=1,
             vcenter_client=destination_client,
             client_name=proxy_client,
-            esx_server=proxy_client,
-            esx_host=proxy_client,
-            datastore=destination_path,
+            datastore=datastore,
             destination_network=destination_network,
             in_place=False
         )
 
         return self._configure_live_sync(schedule_name, restore_option, pattern_dict)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/livesync/vsa_live_sync.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/vsa_live_sync.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/null.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/null.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/nutanix_ahv.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/nutanix_ahv.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/openstack.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/openstack.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/oracle_cloud.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/oracle_cloud.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/oracle_cloud_infrastructure.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/oracle_cloud_infrastructure.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 # --------------------------------------------------------------------------
 # Copyright  Commvault Systems, Inc.
 # See LICENSE.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
-"""File for operating on a Virtual Server OracleCloud Subclient.
+"""
+File for operating on a Virtual Server OracleCloud Subclient.
 
 OracleCloudeVirtualServerSubclient is the only class defined in this file.
 
 OracleCloudVirtualServerSubclient: Derived class from VirtualServerSubClient  Base class,
                             representing a OracleCloud Subclient, and
                             to perform operations on that Subclient
 
@@ -18,28 +19,30 @@
 
     full_vm_restore_out_of_place()  --  restores the VM specified in to the specified client,
                                         at the specified destination location
 
     full_vm_restore_in_place()  --  restores the VM specified in to the source client,
 
 """
+
 import time
 from ..vssubclient import VirtualServerSubclient
 from ...exception import SDKException
 
 
 class OCIVirtualServerSubclient(VirtualServerSubclient):
-    """Derived class from VirtualServerSubclient Base class.
+    """
+       Derived class from VirtualServerSubclient Base class.
        This represents a OracleCloud virtual server subclient,
        and can perform restore operations on only that subclient.
-
     """
 
     def __init__(self, backupset_object, subclient_name, subclient_id=None):
-        """Initialize the Instance object for the given Virtual Server instance.
+        """
+        Initialize the Instance object for the given Virtual Server instance.
         Args
         class_object (backupset_object, subclient_name, subclient_id)  --  instance of the
                                          backupset class, subclient name, subclient id
 
         """
         super(OCIVirtualServerSubclient, self).__init__(
             backupset_object, subclient_name, subclient_id)
@@ -56,69 +59,56 @@
             new_name='AutomationRestored_'+str(int(time.time())),
             copy_preceedence=0,
             power_on=True,
             source_vm_details=None,
             restore_option=None,
             indexing_v2=True,
             **kwargs):
-        """Restores the FULL Virtual machine specified in the input list
-            to the provided vcenter client along with the ESX and the datastores.
-            If the provided client name is none then it restores the Full Virtual
-            Machine to the source client and corresponding ESX and datastore.
-
-            Args:
-                vm_to_restore           (list)  --  list of all VMs to restore
-
-                destination_client      (str)   --  name of the pseudo client where VM should be
+        """
+        Restores the FULL Virtual machine specified in the input list
+        to the provided vcenter client along with the ESX and the datastores.
+        If the provided client name is none then it restores the Full Virtual
+        Machine to the source client and corresponding ESX and datastore.
+        Args:
+            vm_to_restore           (list)  --  list of all VMs to restore
+             destination_client      (str)   --  name of the pseudo client where VM should be
                                                         restored
-
-                proxy_client            (str)   --  the proxy to be used for restore
-
-                new_name                (str)   --  new name to be given to the restored VM
-
-                power_on                (bool)  --  power on the restored VM
+             proxy_client            (str)   --  the proxy to be used for restore
+             new_name                (str)   --  new name to be given to the restored VM
+             power_on                (bool)  --  power on the restored VM
                                                         default: True
-
-                copy_precedence         (int)   --  copy precedence to restored from
+             copy_precedence         (int)   --  copy precedence to restored from
                                                         default: 0
-
-                restore_option          (dict)  --  dictionary with all the advanced restore
+             restore_option          (dict)  --  dictionary with all the advanced restore
                                                         options.
-
-                **kwargs                         : Arbitrary keyword arguments Properties as of
-                                                     full_vm_restore_out_of_place
-                    eg:
-                    v2_details          (dict)       -- details for v2 subclient
-                                                    eg: check clients.vmclient.VMClient._child_job_subclient_details
-
-            Returns:
+             **kwargs                         : Arbitrary keyword arguments Properties as of
+                                                 full_vm_restore_out_of_place
+                eg:
+                v2_details          (dict)       -- details for v2 subclient
+                                                eg: check clients.vmclient.VMClient._child_job_subclient_details
+         Returns:
                 object - instance of the Job class for this restore job
 
             Raises:
                 SDKException:
                     if inputs are not of correct type as per definition
 
                     if failed to initialize job
 
                     if response is empty
 
                     if response is not success
 
         """
-        #self.hvobj = hvobj
-        #self.vm_obj = self.hvobj.get_vm_property(vm_to_restore)
-        #vm_ip = self.hvobj['oci_vm_ip'],
-        #vm_guid = self.hvobj['oci_vm_guid'],
-        #vm_guidip = self.hvobj['oci_vm_ip'],
         copy_precedence = 0
         self.source_vm_details = source_vm_details
         if not restore_option:
             restore_option = {}
         restore_option["v2_details"] = kwargs.get("v2_details", None)
-    # set attr for all the option in restore xml from user inputs
+        # set attr for all the option in restore xml from user inputs
         self._set_restore_inputs(
             restore_option,
             vm_to_restore=self._set_vm_to_restore(),
             power_on=True,
             copy_precedence=copy_precedence,
             indexing_v2=indexing_v2,
             restore_new_name=new_name,
@@ -176,23 +166,20 @@
                     if response is empty
 
                     if response is not success
 
 
         """
         self.source_vm_details = source_vm_details
-        #self.hvobj = hvobj
-        #self.vm_obj = self.hvobj.get_vm_property(vm_to_restore)
         restore_option = {"v2_details": kwargs.get("v2_details", None)}
-    # check mandatory input parameters are correct
+        # check mandatory input parameters are correct
         if not (isinstance(overwrite, bool) and
                 isinstance(power_on, bool)):
             raise SDKException('Subclient', '101')
         # set attr for all the option in restore xml from user inputs
-        #copy_precedence = 0
         self._set_restore_inputs(
             restore_option,
             vm_to_restore=self._set_vm_to_restore(),
             copy_precedence=copy_precedence,
             volume_level_restore=1,
             out_place=False,
             in_place=True,
@@ -243,29 +230,27 @@
         restore_option['guid'] = self.source_vm_details['guid']#self.vm_obj['guid']
         restore_option["FolderPath"] = folder_path
         restore_option["ResourcePool"] = "/"
 
         # populate restore disk and datastore
         vm_disks = []
         disk_list, disk_info_dict = self.disk_level_browse("\\\\" + vm_ids[vm_to_restore])
-
         for disk, data in disk_info_dict.items():
             if ((restore_option["in_place"]) or ("datastore" not in restore_option)):
                 restore_option["datastore"] = data["advanced_data"]["browseMetaData"][
                                              "virtualServerMetaData"]["datastore"]
                 restore_option['vmSize'] = self.source_vm_details['vmSize']
             _disk_dict = self._disk_dict_pattern(disk.split('\\')[-1], restore_option["datastore"])
             vm_disks.append(_disk_dict)
         if not vm_disks:
             raise SDKException('Subclient', 104)
         restore_option["disks"] = vm_disks
 
         # prepare nics info json
         nics_list = self._json_nics_advancedRestoreOptions(vm_to_restore, restore_option)
-
         restore_option["nics"] = nics_list
         if restore_option["source_ip"] and restore_option["destination_ip"]:
             vm_ip = self._json_vmip_advanced_restore_options(restore_option)
             restore_option["vm_ip_address_options"] = vm_ip
         if restore_option["in_place"]:
             restore_option['createPublicIP'] = False
             if "hyper" in restore_option["destination_instance"]:
@@ -287,21 +272,16 @@
         temp_dict = self._json_restore_advancedRestoreOptions(restore_option)
         self._advanced_restore_option_list.append(temp_dict)
 
 
     def _json_nics_advancedRestoreOptions(self, vm_to_restore, value):
         """
             Setter for nics list for advanced restore option json
-
         """
-
-        #nics_dict_from_browse = self.get_nics_from_browse()
         nics_list = []
-        #vm_nics_list = nics_dict_from_browse[vm_to_restore]
-
         for key, val in self.source_vm_details['vcn'].items():
             nics = {
                 "subnetId": val['subnet_id'],
                 "sourceNetwork": val['display_name'],
                 "sourceNetworkId": val['subnet_id'],
                 "name": val['network_id'],
                 "networkName": val['display_name'],
@@ -327,12 +307,11 @@
 
     def _json_vcenter_instance(self, value):
         """ Setter for vcenter_instance JSON """
 
         if not isinstance(value, dict):
             raise SDKException('Subclient', '101')
 
-
         self._vcenter_instance_json = {
             "clientName": value.get("destination_client_name", ""),
             "instanceName": value.get("destination_instance", "")
         }
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/oraclevm.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/oraclevm.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/red_hat_openshift.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/red_hat_openshift.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/red_hat_virtualization.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/red_hat_virtualization.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/vcloud_director.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/vcloud_director.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/virtualserver/vmware.py` & `cvpysdk-11.32/cvpysdk/subclients/virtualserver/vmware.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,32 @@
             'Auto': 0,
             'SAN': 1,
             'Hot Add': 2,
             'NBD': 5,
             'NBD SSL': 4
         }
 
+    def add_revert_option(self, request_json, revert):
+        """
+        Add revert in restore json
+
+        Args:
+
+            request_json            (dict)  :       restore dict
+
+            revert                  (bool)  :       revert option
+
+        Returns:
+            request_json            (dict)  :       restore dict
+
+        """
+        if revert:
+            request_json['taskInfo']['subTasks'][0]['options']['restoreOptions']['commonOptions']['revert'] = True
+        return request_json
+
     def full_vm_restore_in_place(
             self,
             vm_to_restore=None,
             overwrite=True,
             power_on=True,
             copy_precedence=0,
             disk_option='Original',
@@ -130,14 +148,16 @@
                                                      full_vm_restore_in_place
                     eg:
                     media_agent         (str)   -- media agent
 
                     v2_details          (dict)       -- details for v2 subclient
                                                     eg: check clients.vmclient.VMClient._child_job_subclient_details
 
+                    revert              (bool)      --  Revert option
+
 
             Returns:
                 object - instance of the Job class for this restore job
 
             Raises:
                 SDKException:
                     if inputs are not of correct type as per definition
@@ -146,15 +166,16 @@
 
                     if response is empty
 
                     if response is not success
 
         """
 
-        restore_option = {"media_agent": kwargs.get("media_agent", None), "v2_details": kwargs.get("v2_details", None)}
+        restore_option = {"media_agent": kwargs.get("media_agent", None), "v2_details": kwargs.get("v2_details", None),
+                          "revert": kwargs.get("revert", False)}
 
         # check input parameters are correct
         if vm_to_restore and not isinstance(vm_to_restore, str):
             raise SDKException('Subclient', '101')
 
         disk_option_value = self._disk_option[disk_option]
         transport_mode_value = self._transport_mode[transport_mode]
@@ -181,14 +202,15 @@
             disk_option=disk_option_value,
             transport_mode=transport_mode_value,
             copy_precedence=copy_precedence,
             to_time=to_time
         )
 
         request_json = self._prepare_fullvm_restore_json(restore_option)
+        request_json = self.add_revert_option(request_json, restore_option.get('revert', False))
         return self._process_restore_response(request_json)
 
     def full_vm_restore_out_of_place(
             self,
             vm_to_restore=None,
             restored_vm_name=None,
             vcenter_client=None,
@@ -269,14 +291,16 @@
 
                     restore_option      (dict)     --  complete dictionary with all advanced options
                         default: {}
 
                     v2_details          (dict)       -- details for v2 jobs
                                                     eg: check clients.vmclient.VMClient._child_job_subclient_details
 
+                    revert              (bool)      --  Revert option
+
 
             Returns:
                 object - instance of the Job class for this restore job
 
             Raises:
                 SDKException:
                     if inputs are not of correct type as per definition
@@ -288,15 +312,15 @@
                     if response is not success
 
         """
 
         restore_option = {}
         extra_options = ['source_ip', 'destination_ip', 'network', 'destComputerName',
                          'source_subnet', 'source_gateway', 'destination_subnet',
-                         'destination_gateway', 'folder_path', 'media_agent', 'v2_details']
+                         'destination_gateway', 'folder_path', 'media_agent', 'v2_details', 'revert']
         for key in extra_options:
             if key in kwargs:
                 restore_option[key] = kwargs[key]
             else:
                 restore_option[key] = None
         # check mandatory input parameters are correct
         if vm_to_restore and not isinstance(vm_to_restore, str):
@@ -336,14 +360,15 @@
             copy_precedence=copy_precedence,
             volume_level_restore=1,
             source_item=[],
             to_time=to_time
         )
 
         request_json = self._prepare_fullvm_restore_json(restore_option)
+        request_json = self.add_revert_option(request_json, restore_option.get('revert', False))
         return self._process_restore_response(request_json)
 
     def disk_restore(self,
                      vm_name,
                      destination_path,
                      disk_name=None,
                      proxy_client=None,
@@ -543,15 +568,15 @@
 
         # fetching all disks from the vm
         disk_list, disk_info_dict = self.disk_level_browse(
             "\\" + vm_ids[vm_name])
 
         if not disk_name:  # if disk names are not provided, restore all vmdk disks
             for each_disk_path in disk_list:
-                disk_name.append(each_disk_path.split('\\')[-1])
+                disk_name.append(disk_info_dict[each_disk_path]['snap_display_name'])
 
         else:  # else, check if the given VM has a disk with the list of disks in disk_name.
             for each_disk in disk_name:
                 each_disk_path = "\\" + str(vm_name) + "\\" + each_disk
                 if each_disk_path not in disk_list:
                     raise SDKException('Subclient', '111')
```

### Comparing `cvpysdk-11.30.1/cvpysdk/subclients/vssubclient.py` & `cvpysdk-11.32/cvpysdk/subclients/vssubclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 from inspect import getmembers, isclass, isabstract
 
 import xmltodict
 
 from cvpysdk.plan import Plans
 from ..exception import SDKException
 from ..subclient import Subclient
-from ..constants import VSAObjects
+from ..constants import VSAObjects, HypervisorType
 
 
 class VirtualServerSubclient(Subclient):
     """Derived class from Subclient Base class, representing a virtual server subclient,
         and to perform operations on that subclient."""
 
     def __new__(cls, backupset_object, subclient_name, subclient_id=None):
@@ -409,15 +409,15 @@
                 for item in entity:
                     temp = {
                         'allOrAnyChildren': item.get('allOrAnyChildren', True),
                         'equalsOrNotEquals': item.get('equalsOrNotEquals', True),
                         'name': item.get('name',""),
                         'displayName': item.get('display_name',''),
                         'path': '',
-                        'type': item['type'] if isinstance(item['type'], int) else item['type'].value
+                        'type': item['type'] if (isinstance(item['type'], int) or isinstance(item['type'], str)) else item['type'].value
                     }
                     if item['type'] == VSAObjects.VMNotes:
                         temp['value'] = item['display_name']
                         temp['displayName'] = item['display_name']
                         temp['name'] = "Notes"
                     if (item['type'] ==
                             VSAObjects.VMPowerState and
@@ -722,15 +722,15 @@
 
             Returns:
 
                 disk dictionary(dict)       -- Dictionary with key name, new name , datastore
                                                 and corresponding
         """
 
-        if not new_name and not self._instance_object.instance_name == 'google cloud platform':
+        if not new_name and not self._instance_object.instance_name == HypervisorType.GOOGLE_CLOUD.value.lower():
             new_name = name
         temp_disk_dict = {}
         temp_disk_dict[self.disk_pattern.name.value] = name
         temp_disk_dict[self.disk_pattern.datastore.value] = datastore
         temp_disk_dict[self.disk_pattern.new_name.value] = new_name
         return temp_disk_dict
 
@@ -803,30 +803,32 @@
             Setter for nics list for advanced restore option json
         """
 
         nics_dict_from_browse = self.get_nics_from_browse(copy_precedence=value.get('copy_precedence', 0))
         nics_list = []
         vm_nics_list = nics_dict_from_browse[vm_to_restore]
         for network_card_dict in vm_nics_list:
-            if self._instance_object.instance_name == 'google cloud platform':
+            if self._instance_object.instance_name == HypervisorType.GOOGLE_CLOUD.value.lower():
                 current_project = network_card_dict.get('subnetId').split('/')[6]
                 if value.get('project_id') is not None:
                     network_card_dict['subnetId'] = value.get('subnetwork_nic')
                     network_card_dict['sourceNetwork'] = value.get('networks_nic')
 
             _destnetwork = value.get("destination_network",
                                      value.get('network',
                                                network_card_dict['name']))
 
             nics = {
                 "subnetId": network_card_dict.get('subnetId', ""),
                 "sourceNetwork": network_card_dict['name'],
                 "sourceNetworkId": network_card_dict.get('sourceNetwork', ""),
-                "name": network_card_dict.get('sourceNetwork', "")+_destnetwork if self._instance_object.instance_name
-                == 'google cloud platform' else '' ,
+                "name": (network_card_dict.get('sourceNetwork',
+                                               "") + _destnetwork) if self._instance_object.instance_name ==
+                                                                      HypervisorType.GOOGLE_CLOUD.value.lower() and _destnetwork else
+                network_card_dict['label'],
                 "networkName": _destnetwork if _destnetwork else '',
                 "destinationNetwork": _destnetwork if _destnetwork else network_card_dict['name']
             }
 
             # setting nics for azureRM instance
             if value.get('destination_instance') == 'azure resource manager':
                 if "networkDisplayName" in value and 'networkrsg' in value and 'destsubid' in value:
@@ -957,15 +959,16 @@
                 self._advanced_option_restore_json[inner_key] = value.get(val1, val2)
 
         if "vmSize" in value:
             val1, val2 = ("instanceSize", "") if not value["vmSize"] else ("vmSize", "vmSize")
             self._advanced_option_restore_json["vmSize"] = value.get(val1, val2)
         if "ami" in value and value["ami"] is not None:
             self._advanced_option_restore_json["templateId"] = value["ami"]["templateId"]
-            self._advanced_option_restore_json["templateName"] = value["ami"]["templateName"]
+            if value.get('ami', {}).get('templateName'):
+                self._advanced_option_restore_json["templateName"] = value["ami"]["templateName"]
         if "iamRole" in value and value["iamRole"] is not None:
             self._advanced_option_restore_json["roleInfo"] = {
                 "name": value["iamRole"]
             }
         if self._instance_object.instance_name == 'openstack':
             if "securityGroups" in value and value["securityGroups"] is not None:
                 self._advanced_option_restore_json["securityGroups"] = [{"groupName": value["securityGroups"]}]
@@ -1900,14 +1903,16 @@
         # set vms to restore
         if not vm_to_restore:
             vm_to_restore = restore_option.get("vm_to_restore", self._vm_ids_browse)
             _temp_res_list = vm_to_restore
 
         else:
             _temp_res_list = []
+            if not isinstance(vm_to_restore, list):
+                vm_to_restore = [vm_to_restore]
             for each_vm in vm_to_restore:
                 _temp_res_list.append(each_vm)
 
         vm_to_restore = list(set(self._vm_names_browse) & set(_temp_res_list))
 
         if not vm_to_restore:
             raise SDKException('Subclient', '104')
@@ -2117,29 +2122,31 @@
                     if restore_option.get("availability_zone") is not None:
                         ds = restore_option.get("availability_zone")
                     else:
                         ds = vs_metadata["esxHost"]
             new_name_prefix = restore_option.get("disk_name_prefix")
             new_name = data["name"] if new_name_prefix is None \
                 else new_name_prefix + "_" + data["name"]
-            if self._instance_object.instance_name == 'google cloud platform':
+            if self._instance_object.instance_name == HypervisorType.GOOGLE_CLOUD.value.lower():
                 new_name = ""
+                if data["advanced_data"]["browseMetaData"]["virtualServerMetaData"].get('replicaZones', False):
+                    replicaZones = restore_option.get("replicaZones")
             if restore_option['destination_instance'].lower() == 'vmware':
                 _disk_dict = self._disk_dict_pattern(data['snap_display_name'], ds, new_name)
             else:
                 _disk_dict = self._disk_dict_pattern(disk.split('\\')[-1], ds, new_name)
             if 'is_aws_proxy' in restore_option and not restore_option['is_aws_proxy']:
                 _disk_dict['Datastore'] = restore_option["datastore"]
             vm_disks.append(_disk_dict)
         if not vm_disks:
             raise SDKException('Subclient', '104')
         restore_option["disks"] = vm_disks
 
         # prepare nics info json
-        if "nics" not in restore_option or self._instance_object.instance_name == 'google cloud platform':
+        if "nics" not in restore_option or self._instance_object.instance_name == HypervisorType.GOOGLE_CLOUD.value.lower():
             nics_list = self._json_nics_advancedRestoreOptions(vm_to_restore, restore_option)
             restore_option["nics"] = nics_list
             if restore_option.get('source_ip') and restore_option.get('destination_ip'):
                 vm_ip = self._json_vmip_advanced_restore_options(restore_option)
                 restore_option["vm_ip_address_options"] = vm_ip
             if restore_option["in_place"]:
                 if "hyper" in restore_option["destination_instance"].lower():
@@ -2206,15 +2213,15 @@
 
         for disk, data in disk_info_dict.items():
             ds = ""
             if "datastore" in restore_option:
                 ds = restore_option["datastore"]
             new_name_prefix = restore_option.get("disk_name_prefix")
             if self._instance_object.instance_name != 'openstack':
-                new_name = data["name"].replace("/", "_").replace(" ", "_")
+                new_name = data["snap_display_name"].replace("/", "_").replace(" ", "_")
                 new_name = "del_" + new_name if new_name_prefix is None \
                     else new_name_prefix + "_" + new_name
             else:
                 new_name = data["name"]
             _disk_dict = self._disk_dict_pattern(data['snap_display_name'], ds, new_name)
             vm_disks.append(_disk_dict)
         if not vm_disks:
@@ -2428,17 +2435,47 @@
         self._virtualserver_option_restore_json["diskLevelVMRestoreOption"][
             "advancedRestoreOptions"] = self._advanced_restore_option_list
         self._advanced_restore_option_list = []
         request_json["taskInfo"]["subTasks"][0]["options"]["restoreOptions"][
             "virtualServerRstOption"] = self._virtualserver_option_restore_json
         request_json["taskInfo"]["subTasks"][0]["options"][
             "restoreOptions"]["volumeRstOption"] = self._json_restore_volumeRstOption(_disk_restore_option)
-
+        if _disk_restore_option.get('new_instance'):
+            request_json = self._update_attach_disk_restore_new_instance(request_json, _disk_restore_option)
         return request_json
 
+    @staticmethod
+    def _update_attach_disk_restore_new_instance(json_to_be_edited, _disk_restore_option):
+        """
+        Updates teh Json for attach disk restore as a new instance
+
+        Args:
+            json_to_be_edited               (dict): Request json to be edited
+
+            _disk_restore_option:           (dict): Attach dsik restore options
+
+        Returns:
+            json_to_be_edited               (dict): Dictionary after its edited
+
+        """
+        json_to_be_edited['taskInfo']['subTasks'][0]['options']['restoreOptions'][
+            'virtualServerRstOption']['diskLevelVMRestoreOption']['powerOnVmAfterRestore'] = True
+        adv_options = json_to_be_edited['taskInfo']['subTasks'][0]['options']['restoreOptions'][
+            'virtualServerRstOption']['diskLevelVMRestoreOption']['advancedRestoreOptions'][0]
+        del adv_options['newGuid']
+        del adv_options['nics'][0]['destinationNetwork']
+        _nic2 = adv_options['nics'][0].copy()
+        adv_options['nics'].append(_nic2)
+        adv_options['nics'][1]['networkName'] = 'New Network Interface'
+        _region = adv_options['esxHost']
+        for disks in adv_options['disks']:
+            disks['availabilityZone'] = _region
+        adv_options['guestOperatingSystemId'] = _disk_restore_option.get('os_id', 0)
+        return json_to_be_edited
+
     def _prepare_fullvm_restore_json(self, restore_option=None):
         """
         Prepare Full VM restore Json with all getters
 
         Args:
             restore_option - dictionary with all VM restore options
 
@@ -2873,7 +2910,31 @@
             return self._parse_preview_vms(response.json()['scList'])
         else:
             raise SDKException(
                 'Subclient',
                 '102',
                 self._update_response_(
                     response.text))
+
+    @property
+    def quiesce_file_system(self):
+        """
+            Gets the quiesce value set for the vsa subclient
+
+        Returns:
+            (Boolean)    True/False
+        """
+        quiesce_file_system = r'quiesceGuestFileSystemAndApplications'
+        return self._vsaSubclientProp.get(quiesce_file_system)
+
+    @quiesce_file_system.setter
+    def quiesce_file_system(self, value):
+        """
+        Sets the quiesce value for the vsa subclient
+
+        Args:
+            value   (Boolean)   True/False
+
+        """
+        update_properties = self.properties
+        update_properties['vsaSubclientProp']['quiesceGuestFileSystemAndApplications'] = value
+        self.update_properties(update_properties)
```

### Comparing `cvpysdk-11.30.1/cvpysdk/system.py` & `cvpysdk-11.32/cvpysdk/system.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/virtualmachinepolicies.py` & `cvpysdk-11.32/cvpysdk/virtualmachinepolicies.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.30.1/cvpysdk/workflow.py` & `cvpysdk-11.32/cvpysdk/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,31 +564,35 @@
         if flag is False:
             raise SDKException(
                 'Workflow',
                 '102',
                 'Getting Pacakge id for workflow failed. {0}'.format(response.text)
             )
 
-        if response.json():
-            if "packageId" in response.json():
-                package_id = response.json()["packageId"]
-            else:
-                raise SDKException(
-                    'Workflow', '102', response.json()['errorDetail']['errorMessage']
-                )
-        else:
+        if not response.json():
             raise SDKException('Response', '102')
+        
+        if "packageId" not in response.json():
+            raise SDKException(
+                'Workflow', '102', response.json()['errorDetail']['errorMessage']
+            )
+        package_id = response.json()["packageId"]
+        platform_id = 1
+        if "platforms" in response.json():
+            platforms = response.json()["platforms"]
+            if isinstance(platforms, list) and platforms:
+                platform_id = platforms[0]["id"]
 
         download_xml = """
         <DM2ContentIndexing_OpenFileReq>
             <fileParams id="3" name="Package"/>
             <fileParams id="2" name="{0}"/>
-            <fileParams id="9" name="1"/>
+            <fileParams id="9" name="{1}"/>
         </DM2ContentIndexing_OpenFileReq>
-        """.format(package_id)
+        """.format(package_id, platform_id)
 
         flag, response = cvpysdk_object.make_request(
             'POST', services['SOFTWARESTORE_DOWNLOADITEM'], download_xml
         )
 
         if flag:
             if response.json():
@@ -599,15 +603,15 @@
                     try:
                         os.makedirs(download_location)
                     except FileExistsError:
                         pass
 
                 download_path = os.path.join(download_location, workflow_name + ".xml")
 
-                with open(download_path, "w") as file_pointer:
+                with open(download_path, "w", encoding="utf-8") as file_pointer:
                     file_pointer.write(file_content)
 
                 return download_path
 
             else:
                 raise SDKException('Response', '102')
         else:
@@ -1251,15 +1255,15 @@
 
                 if "jobId" in response.json():
                     if response.json()["jobId"] == 0:
                         return output, 'Workflow Execution Finished Successfully'
                     else:
                         return output, Job(self._commcell_object, response.json()['jobId'])
                 elif "errorCode" in response.json():
-                    if response.json()['errorCode'] == 0:
+                    if int(response.json()['errorCode']) == 0:
                         return output, 'Workflow Execution Finished Successfully'
                     else:
                         error_message = response.json()['errorMessage']
                         o_str = 'Executing Workflow failed\nError: "{0}"'.format(error_message)
 
                         raise SDKException('Workflow', '102', o_str)
                 else:
```

### Comparing `cvpysdk-11.30.1/cvpysdk.egg-info/PKG-INFO` & `cvpysdk-11.32/cvpysdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvpysdk
-Version: 11.30.1
+Version: 11.32
 Summary: Commvault SDK for Python
 Home-page: https://github.com/Commvault/cvpysdk
 Author: Commvault Systems Inc.
 Author-email: Dev-PythonSDK@commvault.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Commvault/cvpysdk/issues
 Project-URL: Documentation, https://commvault.github.io/cvpysdk/
@@ -35,15 +35,15 @@
 ------------------
 
 CVPySDK can be installed directly from PyPI using pip:
 
     >>> pip install cvpysdk
 
 
-CVPySDK is available on GitHub `here <https://github.com/Commvault/cvpysdk>`_
+CVPySDK is available on GitHub `here <https://github.com/Commvault/cvpysdk>`__
 
 It can also be installed from source.
 
 After downloading, from within the ``cvpysdk`` directory, execute:
 
     >>> python setup.py install
 
@@ -205,14 +205,19 @@
 
 - All python code should be **PEP8** compliant.
 - All changes should be consistent with the design of the SDK.
 - The code should be formatted using **autopep8** with line-length set to **99** instead of default **79**.
 - All changes and any new methods/classes should be properly documented.
 - The doc strings should be of the same format as existing docs.
 
+Questions/Comments/Suggestions
+------------------------------
+If you have any questions or comments, please contact us `here <https://ma.commvault.com/>`__.
+Also Check out our community for `Automation <https://community.commvault.com/developer-tools-integration-and-automation-workflow-rest-powershell-etc-50>`_ incase of queries.
+
 Code of Conduct
 ***************
 
 Everyone interacting in the **CVPySDK** project's codebases, issue trackers,
 chat rooms, and mailing lists is expected to follow the
 `PyPA Code of Conduct`_.
```

### Comparing `cvpysdk-11.30.1/cvpysdk.egg-info/SOURCES.txt` & `cvpysdk-11.32/cvpysdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -191,14 +191,15 @@
 cvpysdk/subclients/fssubclient.py
 cvpysdk/subclients/hanasubclient.py
 cvpysdk/subclients/index_server_subclient.py
 cvpysdk/subclients/informixsubclient.py
 cvpysdk/subclients/lndbsubclient.py
 cvpysdk/subclients/mysqlsubclient.py
 cvpysdk/subclients/nassubclient.py
+cvpysdk/subclients/o365apps_subclient.py
 cvpysdk/subclients/oraclesubclient.py
 cvpysdk/subclients/postgressubclient.py
 cvpysdk/subclients/saporaclesubclient.py
 cvpysdk/subclients/sharepointsubclient.py
 cvpysdk/subclients/splunksubclient.py
 cvpysdk/subclients/sqlsubclient.py
 cvpysdk/subclients/sybasesubclient.py
```

### Comparing `cvpysdk-11.30.1/setup.py` & `cvpysdk-11.32/setup.py`

 * *Files identical despite different names*

