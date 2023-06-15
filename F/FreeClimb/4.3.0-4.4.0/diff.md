# Comparing `tmp/FreeClimb-4.3.0.tar.gz` & `tmp/FreeClimb-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeClimb-4.3.0.tar", last modified: Tue May  2 00:01:36 2023, max compression
+gzip compressed data, was "FreeClimb-4.4.0.tar", last modified: Thu Jun 15 17:52:16 2023, max compression
```

## Comparing `FreeClimb-4.3.0.tar` & `FreeClimb-4.4.0.tar`

### file list

```diff
@@ -1,286 +1,306 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:01:36.289751 FreeClimb-4.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:01:36.229751 FreeClimb-4.3.0/FreeClimb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-02 00:01:36.000000 FreeClimb-4.3.0/FreeClimb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-05-02 00:01:36.000000 FreeClimb-4.3.0/FreeClimb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:01:36.000000 FreeClimb-4.3.0/FreeClimb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-02 00:01:36.000000 FreeClimb-4.3.0/FreeClimb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 00:01:36.000000 FreeClimb-4.3.0/FreeClimb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-02 00:01:36.289751 FreeClimb-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22557 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:01:36.229751 FreeClimb-4.3.0/freeclimb/
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:01:36.233751 FreeClimb-4.3.0/freeclimb/api/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   248913 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39832 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:01:36.233751 FreeClimb-4.3.0/freeclimb/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17499 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:01:36.261751 FreeClimb-4.3.0/freeclimb/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/account_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    17946 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/account_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/account_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/account_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/account_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/add_to_conference.py
--rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/add_to_conference_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/answered_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/application_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/application_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/application_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/application_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/application_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/available_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/available_number_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/available_number_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/buy_incoming_number_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/call_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/call_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/call_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/call_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/call_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/call_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/conference_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/conference_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    16372 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/conference_participant_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/conference_participant_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/conference_participant_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/conference_participant_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/conference_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    15408 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/conference_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/conference_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    19853 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/create_conference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/create_conference_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/create_conference_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/dequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    19031 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/enqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/enqueue_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/filter_logs_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    22828 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/get_digits.py
--rw-r--r--   0 runner    (1001) docker     (123)    17786 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/get_digits_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    24968 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/get_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/get_speech_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/get_speech_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/grammar_file_built_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/grammar_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/hangup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/hangup_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/if_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/incoming_number_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/incoming_number_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/incoming_number_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    20378 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/incoming_number_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    16495 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/incoming_number_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/log_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/log_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/log_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/log_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/machine_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/make_call_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/message_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/message_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/message_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17944 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/message_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/message_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/message_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/messages_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/messages_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/mutable_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/out_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/out_dial_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/park.py
--rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/park_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/pause.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/pause_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/percl_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/percl_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/play.py
--rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/play_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/play_beep.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/play_early_media.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/play_early_media_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/queue_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/queue_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/queue_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/queue_member_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/queue_member_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/queue_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/queue_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14212 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/queue_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/queue_result_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    19905 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/record_utterance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/record_utterance_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/record_utterance_term_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/recording_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/recording_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/recording_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/recording_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/redirect_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/reject.py
--rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/reject_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/remove_from_conference.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/remove_from_conference_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/say.py
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/say_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    18199 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/send_digits.py
--rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/send_digits_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17505 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/set_listen.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/set_listen_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/set_talk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/set_talk_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/sms_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/start_record_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/terminate_conference.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/terminate_conference_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/unpark.py
--rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/update_call_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/update_call_request_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/update_conference_participant_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/update_conference_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model/update_conference_request_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    83184 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:01:36.261751 FreeClimb-4.3.0/freeclimb/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/freeclimb/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 00:01:36.289751 FreeClimb-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:01:36.289751 FreeClimb-4.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_account_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_account_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_account_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_account_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_account_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_add_to_conference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_add_to_conference_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_answered_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_application_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_application_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_application_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_application_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_application_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_available_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_available_number_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_available_number_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_buy_incoming_number_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_call_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_call_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_call_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_call_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_call_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_call_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_conference_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_conference_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_conference_participant_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_conference_participant_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_conference_participant_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_conference_participant_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_conference_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_conference_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_conference_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_create_conference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_create_conference_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_create_conference_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_dequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_enqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_enqueue_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_filter_logs_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_get_digits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_get_digits_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_get_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_get_speech_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_get_speech_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_grammar_file_built_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_grammar_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_hangup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_hangup_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_if_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_incoming_number_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_incoming_number_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_incoming_number_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_incoming_number_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_incoming_number_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_log_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_log_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_log_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_log_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_make_call_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_message_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_message_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_message_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_message_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_message_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_message_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_messages_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_messages_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_mutable_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_out_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_out_dial_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_park.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_park_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_pause.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_pause_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_percl_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_percl_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_play.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_play_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_play_beep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_play_early_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_play_early_media_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_queue_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_queue_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_queue_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_queue_member_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_queue_member_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_queue_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_queue_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_queue_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_queue_result_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_record_utterance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_record_utterance_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_record_utterance_term_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_recording_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_recording_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_recording_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_recording_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_redirect_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_reject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_reject_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_remove_from_conference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_remove_from_conference_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_request_verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_say.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_say_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_send_digits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_send_digits_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_set_listen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_set_listen_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_set_talk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_set_talk_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_signature_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_sms_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_start_record_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_terminate_conference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_terminate_conference_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_unpark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_update_call_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_update_call_request_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_update_conference_participant_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_update_conference_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-02 00:01:21.000000 FreeClimb-4.3.0/test/test_update_conference_request_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:52:16.567041 FreeClimb-4.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:52:16.531039 FreeClimb-4.4.0/FreeClimb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 17:52:16.000000 FreeClimb-4.4.0/FreeClimb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-15 17:52:16.000000 FreeClimb-4.4.0/FreeClimb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:52:16.000000 FreeClimb-4.4.0/FreeClimb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 17:52:16.000000 FreeClimb-4.4.0/FreeClimb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 17:52:16.000000 FreeClimb-4.4.0/FreeClimb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 17:52:16.567041 FreeClimb-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21635 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:52:16.535039 FreeClimb-4.4.0/freeclimb/
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:52:16.535039 FreeClimb-4.4.0/freeclimb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   279487 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39832 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:52:16.535039 FreeClimb-4.4.0/freeclimb/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17499 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:52:16.551040 FreeClimb-4.4.0/freeclimb/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/account_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17946 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/account_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/account_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/account_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/add_to_conference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/add_to_conference_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/answered_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/application_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/application_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/application_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/application_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/application_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/available_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/available_number_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/available_number_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/buy_incoming_number_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/call_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/call_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/call_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/call_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/call_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/call_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/conference_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/conference_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16372 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/conference_participant_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/conference_participant_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/conference_participant_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/conference_participant_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/conference_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15408 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/conference_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/conference_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19853 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/create_conference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/create_conference_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/create_conference_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/dequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19031 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/enqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/enqueue_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/filter_logs_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22828 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/get_digits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17786 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/get_digits_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24968 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/get_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/get_speech_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/get_speech_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/grammar_file_built_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/grammar_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/hangup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/hangup_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/if_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/incoming_number_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/incoming_number_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/incoming_number_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20378 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/incoming_number_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16495 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/incoming_number_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/log_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/log_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/log_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/log_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/make_call_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/message_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/message_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/message_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17944 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/message_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/message_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/message_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/messages_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/messages_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/mutable_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/out_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/out_dial_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/park.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/park_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/pause.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/pause_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/percl_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/percl_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/play.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/play_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/play_beep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/play_early_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/play_early_media_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/queue_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/queue_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/queue_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/queue_member_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/queue_member_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/queue_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/queue_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14212 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/queue_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/queue_result_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19905 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/record_utterance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/record_utterance_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/record_utterance_term_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/recording_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/recording_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/recording_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/recording_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/redirect_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/reject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/reject_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/remove_from_conference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/remove_from_conference_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/say.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/say_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18199 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/send_digits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/send_digits_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17505 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/set_listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/set_listen_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/set_talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/set_talk_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25173 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16255 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_brands_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_brands_list_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24818 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_campaigns_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_campaigns_list_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_partner_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_partner_campaign_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_partner_campaigns_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_partner_campaigns_list_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/start_record_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/terminate_conference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/terminate_conference_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/unpark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/update_call_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/update_call_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/update_conference_participant_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/update_conference_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model/update_conference_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83184 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:52:16.551040 FreeClimb-4.4.0/freeclimb/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/freeclimb/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 17:52:16.567041 FreeClimb-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:52:16.567041 FreeClimb-4.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_account_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_account_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_account_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_add_to_conference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_add_to_conference_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_answered_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_application_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_application_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_application_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_application_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_application_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_available_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_available_number_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_available_number_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_buy_incoming_number_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_call_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_call_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_call_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_call_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_call_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_call_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_conference_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_conference_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_conference_participant_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_conference_participant_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_conference_participant_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_conference_participant_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_conference_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_conference_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_conference_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_create_conference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_create_conference_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_create_conference_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37893 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_dequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_enqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_enqueue_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_filter_logs_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_get_digits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_get_digits_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_get_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_get_speech_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_get_speech_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_grammar_file_built_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_grammar_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_hangup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_hangup_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_if_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_incoming_number_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_incoming_number_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_incoming_number_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_incoming_number_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_incoming_number_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_log_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_log_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_log_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_log_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_make_call_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_message_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_message_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_message_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_message_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_message_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_messages_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_messages_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_mutable_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_out_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_out_dial_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_park.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_park_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_pause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_pause_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_percl_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_percl_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_play_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_play_beep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_play_early_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_play_early_media_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_queue_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_queue_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_queue_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_queue_member_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_queue_member_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_queue_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_queue_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_queue_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_queue_result_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_record_utterance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_record_utterance_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_record_utterance_term_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_recording_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_recording_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_recording_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_recording_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_redirect_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_reject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_reject_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_remove_from_conference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_remove_from_conference_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_request_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_say.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_say_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_send_digits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_send_digits_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_set_listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_set_listen_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_set_talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_set_talk_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_signature_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_ten_dlc_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_ten_dlc_brands_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_ten_dlc_brands_list_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_ten_dlc_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_ten_dlc_campaigns_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_ten_dlc_campaigns_list_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_ten_dlc_partner_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_ten_dlc_partner_campaign_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_ten_dlc_partner_campaigns_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_sms_ten_dlc_partner_campaigns_list_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_start_record_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_terminate_conference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_terminate_conference_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_unpark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_update_call_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_update_call_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_update_conference_participant_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_update_conference_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-15 17:52:06.000000 FreeClimb-4.4.0/test/test_update_conference_request_status.py
```

### Comparing `FreeClimb-4.3.0/FreeClimb.egg-info/PKG-INFO` & `FreeClimb-4.4.0/FreeClimb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeClimb
-Version: 4.3.0
+Version: 4.4.0
 Summary: FreeClimb API
 Home-page: https://freeclimb.com
 Author: FreeClimb API Support
 Author-email: support@freeclimb.com
 Keywords: OpenAPI,OpenAPI-Generator,FreeClimb API
 Requires-Python: >=3.6
 License-File: LICENSE
```

### Comparing `FreeClimb-4.3.0/FreeClimb.egg-info/SOURCES.txt` & `FreeClimb-4.4.0/FreeClimb.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -131,14 +131,24 @@
 freeclimb/model/send_digits_all_of.py
 freeclimb/model/set_listen.py
 freeclimb/model/set_listen_all_of.py
 freeclimb/model/set_talk.py
 freeclimb/model/set_talk_all_of.py
 freeclimb/model/sms.py
 freeclimb/model/sms_all_of.py
+freeclimb/model/sms_ten_dlc_brand.py
+freeclimb/model/sms_ten_dlc_brands_list_result.py
+freeclimb/model/sms_ten_dlc_brands_list_result_all_of.py
+freeclimb/model/sms_ten_dlc_campaign.py
+freeclimb/model/sms_ten_dlc_campaigns_list_result.py
+freeclimb/model/sms_ten_dlc_campaigns_list_result_all_of.py
+freeclimb/model/sms_ten_dlc_partner_campaign.py
+freeclimb/model/sms_ten_dlc_partner_campaign_brand.py
+freeclimb/model/sms_ten_dlc_partner_campaigns_list_result.py
+freeclimb/model/sms_ten_dlc_partner_campaigns_list_result_all_of.py
 freeclimb/model/start_record_call.py
 freeclimb/model/terminate_conference.py
 freeclimb/model/terminate_conference_all_of.py
 freeclimb/model/unpark.py
 freeclimb/model/update_call_request.py
 freeclimb/model/update_call_request_status.py
 freeclimb/model/update_conference_participant_request.py
@@ -262,14 +272,24 @@
 test/test_set_listen.py
 test/test_set_listen_all_of.py
 test/test_set_talk.py
 test/test_set_talk_all_of.py
 test/test_signature_information.py
 test/test_sms.py
 test/test_sms_all_of.py
+test/test_sms_ten_dlc_brand.py
+test/test_sms_ten_dlc_brands_list_result.py
+test/test_sms_ten_dlc_brands_list_result_all_of.py
+test/test_sms_ten_dlc_campaign.py
+test/test_sms_ten_dlc_campaigns_list_result.py
+test/test_sms_ten_dlc_campaigns_list_result_all_of.py
+test/test_sms_ten_dlc_partner_campaign.py
+test/test_sms_ten_dlc_partner_campaign_brand.py
+test/test_sms_ten_dlc_partner_campaigns_list_result.py
+test/test_sms_ten_dlc_partner_campaigns_list_result_all_of.py
 test/test_start_record_call.py
 test/test_terminate_conference.py
 test/test_terminate_conference_all_of.py
 test/test_unpark.py
 test/test_update_call_request.py
 test/test_update_call_request_status.py
 test/test_update_conference_participant_request.py
```

### Comparing `FreeClimb-4.3.0/LICENSE` & `FreeClimb-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/PKG-INFO` & `FreeClimb-4.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeClimb
-Version: 4.3.0
+Version: 4.4.0
 Summary: FreeClimb API
 Home-page: https://freeclimb.com
 Author: FreeClimb API Support
 Author-email: support@freeclimb.com
 Keywords: OpenAPI,OpenAPI-Generator,FreeClimb API
 Requires-Python: >=3.6
 License-File: LICENSE
```

### Comparing `FreeClimb-4.3.0/README.md` & `FreeClimb-4.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,58 @@
 # FreeClimb
-
 FreeClimb is a cloud-based application programming interface (API) that puts the power of the Vail platform in your hands. FreeClimb simplifies the process of creating applications that can use a full range of telephony features without requiring specialized or on-site telephony equipment. Using the FreeClimb REST API to write applications is easy! You have the option to use the language of your choice or hit the API directly. Your application can execute a command by issuing a RESTful request to the FreeClimb API. The base URL to send HTTP requests to the FreeClimb REST API is: /apiserver. FreeClimb authenticates and processes your request.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 4.3.0
+- Package version: 4.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
-  For more information, please visit [https://www.freeclimb.com/support/](https://www.freeclimb.com/support/)
+For more information, please visit [https://www.freeclimb.com/support/](https://www.freeclimb.com/support/)
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
-
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
 pip install git+https://github.com/freeclimbapi/python-sdk.git
 ```
-
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/freeclimbapi/python-sdk.git`)
 
 Then import the package:
-
 ```python
 import freeclimb
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
-
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
-
 ```python
 import freeclimb
 ```
 
 ### Running Tests
-
 Ensure the test dependencies have been installed
 
 ```sh
 pip install -r test-requirements.txt
 ```
 
 Run tests with command:
-
 ```sh
 pytest
 ```
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
@@ -98,15 +90,15 @@
     # Create an instance of the API class
     api_instance = DefaultApi(api_client)
     buy_incoming_number_request = BuyIncomingNumberRequest(
         phone_number="phone_number_example",
         alias="alias_example",
         application_id="application_id_example",
     ) # BuyIncomingNumberRequest | Incoming Number transaction details
-
+    
 
     try:
         # Buy a Phone Number
         api_response = api_instance.buy_a_phone_number(buy_incoming_number_request)
         pprint(api_response)
     except freeclimb.ApiException as e:
         print("Exception when calling DefaultApi->buy_a_phone_number: %s\n" % e)
@@ -129,199 +121,219 @@
 print(percl_script.to_json())
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://www.freeclimb.com/apiserver*
 
-| Class        | Method                                                                        | HTTP request                                                                      | Description               |
-| ------------ | ----------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | ------------------------- |
-| _DefaultApi_ | [**buy_a_phone_number**](docs/DefaultApi.md#buy_a_phone_number)               | **POST** /Accounts/{accountId}/IncomingPhoneNumbers                               | Buy a Phone Number        |
-| _DefaultApi_ | [**create_a_conference**](docs/DefaultApi.md#create_a_conference)             | **POST** /Accounts/{accountId}/Conferences                                        | Create a Conference       |
-| _DefaultApi_ | [**create_a_queue**](docs/DefaultApi.md#create_a_queue)                       | **POST** /Accounts/{accountId}/Queues                                             | Create a Queue            |
-| _DefaultApi_ | [**create_an_application**](docs/DefaultApi.md#create_an_application)         | **POST** /Accounts/{accountId}/Applications                                       | Create an application     |
-| _DefaultApi_ | [**delete_a_recording**](docs/DefaultApi.md#delete_a_recording)               | **DELETE** /Accounts/{accountId}/Recordings/{recordingId}                         | Delete a Recording        |
-| _DefaultApi_ | [**delete_an_application**](docs/DefaultApi.md#delete_an_application)         | **DELETE** /Accounts/{accountId}/Applications/{applicationId}                     | Delete an application     |
-| _DefaultApi_ | [**delete_an_incoming_number**](docs/DefaultApi.md#delete_an_incoming_number) | **DELETE** /Accounts/{accountId}/IncomingPhoneNumbers/{phoneNumberId}             | Delete an Incoming Number |
-| _DefaultApi_ | [**dequeue_a_member**](docs/DefaultApi.md#dequeue_a_member)                   | **POST** /Accounts/{accountId}/Queues/{queueId}/Members/{callId}                  | Dequeue a Member          |
-| _DefaultApi_ | [**dequeue_head_member**](docs/DefaultApi.md#dequeue_head_member)             | **POST** /Accounts/{accountId}/Queues/{queueId}/Members/Front                     | Dequeue Head Member       |
-| _DefaultApi_ | [**download_a_recording_file**](docs/DefaultApi.md#download_a_recording_file) | **GET** /Accounts/{accountId}/Recordings/{recordingId}/Download                   | Download a Recording File |
-| _DefaultApi_ | [**filter_logs**](docs/DefaultApi.md#filter_logs)                             | **POST** /Accounts/{accountId}/Logs                                               | Filter Logs               |
-| _DefaultApi_ | [**get_a_call**](docs/DefaultApi.md#get_a_call)                               | **GET** /Accounts/{accountId}/Calls/{callId}                                      | Get a Call                |
-| _DefaultApi_ | [**get_a_conference**](docs/DefaultApi.md#get_a_conference)                   | **GET** /Accounts/{accountId}/Conferences/{conferenceId}                          | Get a Conference          |
-| _DefaultApi_ | [**get_a_member**](docs/DefaultApi.md#get_a_member)                           | **GET** /Accounts/{accountId}/Queues/{queueId}/Members/{callId}                   | Get a Member              |
-| _DefaultApi_ | [**get_a_participant**](docs/DefaultApi.md#get_a_participant)                 | **GET** /Accounts/{accountId}/Conferences/{conferenceId}/Participants/{callId}    | Get a Participant         |
-| _DefaultApi_ | [**get_a_queue**](docs/DefaultApi.md#get_a_queue)                             | **GET** /Accounts/{accountId}/Queues/{queueId}                                    | Get a Queue               |
-| _DefaultApi_ | [**get_a_recording**](docs/DefaultApi.md#get_a_recording)                     | **GET** /Accounts/{accountId}/Recordings/{recordingId}                            | Get a Recording           |
-| _DefaultApi_ | [**get_an_account**](docs/DefaultApi.md#get_an_account)                       | **GET** /Accounts/{accountId}                                                     | Get an Account            |
-| _DefaultApi_ | [**get_an_application**](docs/DefaultApi.md#get_an_application)               | **GET** /Accounts/{accountId}/Applications/{applicationId}                        | Get an Application        |
-| _DefaultApi_ | [**get_an_incoming_number**](docs/DefaultApi.md#get_an_incoming_number)       | **GET** /Accounts/{accountId}/IncomingPhoneNumbers/{phoneNumberId}                | Get an Incoming Number    |
-| _DefaultApi_ | [**get_an_sms_message**](docs/DefaultApi.md#get_an_sms_message)               | **GET** /Accounts/{accountId}/Messages/{messageId}                                | Get an SMS Message        |
-| _DefaultApi_ | [**get_head_member**](docs/DefaultApi.md#get_head_member)                     | **GET** /Accounts/{accountId}/Queues/{queueId}/Members/Front                      | Get Head Member           |
-| _DefaultApi_ | [**list_active_queues**](docs/DefaultApi.md#list_active_queues)               | **GET** /Accounts/{accountId}/Queues                                              | List Active Queues        |
-| _DefaultApi_ | [**list_all_account_logs**](docs/DefaultApi.md#list_all_account_logs)         | **GET** /Accounts/{accountId}/Logs                                                | List All Account Logs     |
-| _DefaultApi_ | [**list_applications**](docs/DefaultApi.md#list_applications)                 | **GET** /Accounts/{accountId}/Applications                                        | List applications         |
-| _DefaultApi_ | [**list_available_numbers**](docs/DefaultApi.md#list_available_numbers)       | **GET** /AvailablePhoneNumbers                                                    | List available numbers    |
-| _DefaultApi_ | [**list_call_logs**](docs/DefaultApi.md#list_call_logs)                       | **GET** /Accounts/{accountId}/Calls/{callId}/Logs                                 | List Call Logs            |
-| _DefaultApi_ | [**list_call_recordings**](docs/DefaultApi.md#list_call_recordings)           | **GET** /Accounts/{accountId}/Calls/{callId}/Recordings                           | List Call Recordings      |
-| _DefaultApi_ | [**list_calls**](docs/DefaultApi.md#list_calls)                               | **GET** /Accounts/{accountId}/Calls                                               | List Calls                |
-| _DefaultApi_ | [**list_conferences**](docs/DefaultApi.md#list_conferences)                   | **GET** /Accounts/{accountId}/Conferences                                         | List Conferences          |
-| _DefaultApi_ | [**list_incoming_numbers**](docs/DefaultApi.md#list_incoming_numbers)         | **GET** /Accounts/{accountId}/IncomingPhoneNumbers                                | List Incoming Numbers     |
-| _DefaultApi_ | [**list_members**](docs/DefaultApi.md#list_members)                           | **GET** /Accounts/{accountId}/Queues/{queueId}/Members                            | List Members              |
-| _DefaultApi_ | [**list_participants**](docs/DefaultApi.md#list_participants)                 | **GET** /Accounts/{accountId}/Conferences/{conferenceId}/Participants             | List Participants         |
-| _DefaultApi_ | [**list_recordings**](docs/DefaultApi.md#list_recordings)                     | **GET** /Accounts/{accountId}/Recordings                                          | List Recordings           |
-| _DefaultApi_ | [**list_sms_messages**](docs/DefaultApi.md#list_sms_messages)                 | **GET** /Accounts/{accountId}/Messages                                            | List SMS Messages         |
-| _DefaultApi_ | [**make_a_call**](docs/DefaultApi.md#make_a_call)                             | **POST** /Accounts/{accountId}/Calls                                              | Make a Call               |
-| _DefaultApi_ | [**remove_a_participant**](docs/DefaultApi.md#remove_a_participant)           | **DELETE** /Accounts/{accountId}/Conferences/{conferenceId}/Participants/{callId} | Remove a Participant      |
-| _DefaultApi_ | [**send_an_sms_message**](docs/DefaultApi.md#send_an_sms_message)             | **POST** /Accounts/{accountId}/Messages                                           | Send an SMS Message       |
-| _DefaultApi_ | [**stream_a_recording_file**](docs/DefaultApi.md#stream_a_recording_file)     | **GET** /Accounts/{accountId}/Recordings/{recordingId}/Stream                     | Stream a Recording File   |
-| _DefaultApi_ | [**update_a_conference**](docs/DefaultApi.md#update_a_conference)             | **POST** /Accounts/{accountId}/Conferences/{conferenceId}                         | Update a Conference       |
-| _DefaultApi_ | [**update_a_live_call**](docs/DefaultApi.md#update_a_live_call)               | **POST** /Accounts/{accountId}/Calls/{callId}                                     | Update a Live Call        |
-| _DefaultApi_ | [**update_a_participant**](docs/DefaultApi.md#update_a_participant)           | **POST** /Accounts/{accountId}/Conferences/{conferenceId}/Participants/{callId}   | Update a Participant      |
-| _DefaultApi_ | [**update_a_queue**](docs/DefaultApi.md#update_a_queue)                       | **POST** /Accounts/{accountId}/Queues/{queueId}                                   | Update a Queue            |
-| _DefaultApi_ | [**update_an_account**](docs/DefaultApi.md#update_an_account)                 | **POST** /Accounts/{accountId}                                                    | Manage an account         |
-| _DefaultApi_ | [**update_an_application**](docs/DefaultApi.md#update_an_application)         | **POST** /Accounts/{accountId}/Applications/{applicationId}                       | Update an application     |
-| _DefaultApi_ | [**update_an_incoming_number**](docs/DefaultApi.md#update_an_incoming_number) | **POST** /Accounts/{accountId}/IncomingPhoneNumbers/{phoneNumberId}               | Update an Incoming Number |
+Class | Method | HTTP request | Description
+------------ | ------------- | ------------- | -------------
+*DefaultApi* | [**buy_a_phone_number**](docs/DefaultApi.md#buy_a_phone_number) | **POST** /Accounts/{accountId}/IncomingPhoneNumbers | Buy a Phone Number
+*DefaultApi* | [**create_a_conference**](docs/DefaultApi.md#create_a_conference) | **POST** /Accounts/{accountId}/Conferences | Create a Conference
+*DefaultApi* | [**create_a_queue**](docs/DefaultApi.md#create_a_queue) | **POST** /Accounts/{accountId}/Queues | Create a Queue
+*DefaultApi* | [**create_an_application**](docs/DefaultApi.md#create_an_application) | **POST** /Accounts/{accountId}/Applications | Create an application
+*DefaultApi* | [**delete_a_recording**](docs/DefaultApi.md#delete_a_recording) | **DELETE** /Accounts/{accountId}/Recordings/{recordingId} | Delete a Recording
+*DefaultApi* | [**delete_an_application**](docs/DefaultApi.md#delete_an_application) | **DELETE** /Accounts/{accountId}/Applications/{applicationId} | Delete an application
+*DefaultApi* | [**delete_an_incoming_number**](docs/DefaultApi.md#delete_an_incoming_number) | **DELETE** /Accounts/{accountId}/IncomingPhoneNumbers/{phoneNumberId} | Delete an Incoming Number
+*DefaultApi* | [**dequeue_a_member**](docs/DefaultApi.md#dequeue_a_member) | **POST** /Accounts/{accountId}/Queues/{queueId}/Members/{callId} | Dequeue a Member
+*DefaultApi* | [**dequeue_head_member**](docs/DefaultApi.md#dequeue_head_member) | **POST** /Accounts/{accountId}/Queues/{queueId}/Members/Front | Dequeue Head Member
+*DefaultApi* | [**download_a_recording_file**](docs/DefaultApi.md#download_a_recording_file) | **GET** /Accounts/{accountId}/Recordings/{recordingId}/Download | Download a Recording File
+*DefaultApi* | [**filter_logs**](docs/DefaultApi.md#filter_logs) | **POST** /Accounts/{accountId}/Logs | Filter Logs
+*DefaultApi* | [**get_a_call**](docs/DefaultApi.md#get_a_call) | **GET** /Accounts/{accountId}/Calls/{callId} | Get a Call
+*DefaultApi* | [**get_a_conference**](docs/DefaultApi.md#get_a_conference) | **GET** /Accounts/{accountId}/Conferences/{conferenceId} | Get a Conference
+*DefaultApi* | [**get_a_member**](docs/DefaultApi.md#get_a_member) | **GET** /Accounts/{accountId}/Queues/{queueId}/Members/{callId} | Get a Member
+*DefaultApi* | [**get_a_participant**](docs/DefaultApi.md#get_a_participant) | **GET** /Accounts/{accountId}/Conferences/{conferenceId}/Participants/{callId} | Get a Participant
+*DefaultApi* | [**get_a_queue**](docs/DefaultApi.md#get_a_queue) | **GET** /Accounts/{accountId}/Queues/{queueId} | Get a Queue
+*DefaultApi* | [**get_a_recording**](docs/DefaultApi.md#get_a_recording) | **GET** /Accounts/{accountId}/Recordings/{recordingId} | Get a Recording
+*DefaultApi* | [**get_an_account**](docs/DefaultApi.md#get_an_account) | **GET** /Accounts/{accountId} | Get an Account
+*DefaultApi* | [**get_an_application**](docs/DefaultApi.md#get_an_application) | **GET** /Accounts/{accountId}/Applications/{applicationId} | Get an Application
+*DefaultApi* | [**get_an_incoming_number**](docs/DefaultApi.md#get_an_incoming_number) | **GET** /Accounts/{accountId}/IncomingPhoneNumbers/{phoneNumberId} | Get an Incoming Number
+*DefaultApi* | [**get_an_sms_message**](docs/DefaultApi.md#get_an_sms_message) | **GET** /Accounts/{accountId}/Messages/{messageId} | Get an SMS Message
+*DefaultApi* | [**get_head_member**](docs/DefaultApi.md#get_head_member) | **GET** /Accounts/{accountId}/Queues/{queueId}/Members/Front | Get Head Member
+*DefaultApi* | [**get_ten_dlc_sms_brand**](docs/DefaultApi.md#get_ten_dlc_sms_brand) | **GET** /Accounts/{accountId}/Messages/10DLC/Brands/{brandId} | Get a 10DLC SMS Brand
+*DefaultApi* | [**get_ten_dlc_sms_brands**](docs/DefaultApi.md#get_ten_dlc_sms_brands) | **GET** /Accounts/{accountId}/Messages/10DLC/Brands | Get list of SMS 10DLC Brands
+*DefaultApi* | [**get_ten_dlc_sms_campaign**](docs/DefaultApi.md#get_ten_dlc_sms_campaign) | **GET** /Accounts/{accountId}/Messages/10DLC/Campaigns/{campaignId} | Get a 10DLC SMS Campaign
+*DefaultApi* | [**get_ten_dlc_sms_campaigns**](docs/DefaultApi.md#get_ten_dlc_sms_campaigns) | **GET** /Accounts/{accountId}/Messages/10DLC/Campaigns | Get list of SMS 10DLC Campaigns
+*DefaultApi* | [**get_ten_dlc_sms_partner_campaign**](docs/DefaultApi.md#get_ten_dlc_sms_partner_campaign) | **GET** /Accounts/{accountId}/Messages/10DLC/PartnerCampaigns/{campaignId} | Get a 10DLC SMS Partner Campaign
+*DefaultApi* | [**get_ten_dlc_sms_partner_campaigns**](docs/DefaultApi.md#get_ten_dlc_sms_partner_campaigns) | **GET** /Accounts/{accountId}/Messages/10DLC/PartnerCampaigns | Get list of SMS 10DLC Partner Campaigns
+*DefaultApi* | [**list_active_queues**](docs/DefaultApi.md#list_active_queues) | **GET** /Accounts/{accountId}/Queues | List Active Queues
+*DefaultApi* | [**list_all_account_logs**](docs/DefaultApi.md#list_all_account_logs) | **GET** /Accounts/{accountId}/Logs | List All Account Logs
+*DefaultApi* | [**list_applications**](docs/DefaultApi.md#list_applications) | **GET** /Accounts/{accountId}/Applications | List applications
+*DefaultApi* | [**list_available_numbers**](docs/DefaultApi.md#list_available_numbers) | **GET** /AvailablePhoneNumbers | List available numbers
+*DefaultApi* | [**list_call_logs**](docs/DefaultApi.md#list_call_logs) | **GET** /Accounts/{accountId}/Calls/{callId}/Logs | List Call Logs
+*DefaultApi* | [**list_call_recordings**](docs/DefaultApi.md#list_call_recordings) | **GET** /Accounts/{accountId}/Calls/{callId}/Recordings | List Call Recordings
+*DefaultApi* | [**list_calls**](docs/DefaultApi.md#list_calls) | **GET** /Accounts/{accountId}/Calls | List Calls
+*DefaultApi* | [**list_conferences**](docs/DefaultApi.md#list_conferences) | **GET** /Accounts/{accountId}/Conferences | List Conferences
+*DefaultApi* | [**list_incoming_numbers**](docs/DefaultApi.md#list_incoming_numbers) | **GET** /Accounts/{accountId}/IncomingPhoneNumbers | List Incoming Numbers
+*DefaultApi* | [**list_members**](docs/DefaultApi.md#list_members) | **GET** /Accounts/{accountId}/Queues/{queueId}/Members | List Members
+*DefaultApi* | [**list_participants**](docs/DefaultApi.md#list_participants) | **GET** /Accounts/{accountId}/Conferences/{conferenceId}/Participants | List Participants
+*DefaultApi* | [**list_recordings**](docs/DefaultApi.md#list_recordings) | **GET** /Accounts/{accountId}/Recordings | List Recordings
+*DefaultApi* | [**list_sms_messages**](docs/DefaultApi.md#list_sms_messages) | **GET** /Accounts/{accountId}/Messages | List SMS Messages
+*DefaultApi* | [**make_a_call**](docs/DefaultApi.md#make_a_call) | **POST** /Accounts/{accountId}/Calls | Make a Call
+*DefaultApi* | [**remove_a_participant**](docs/DefaultApi.md#remove_a_participant) | **DELETE** /Accounts/{accountId}/Conferences/{conferenceId}/Participants/{callId} | Remove a Participant
+*DefaultApi* | [**send_an_sms_message**](docs/DefaultApi.md#send_an_sms_message) | **POST** /Accounts/{accountId}/Messages | Send an SMS Message
+*DefaultApi* | [**stream_a_recording_file**](docs/DefaultApi.md#stream_a_recording_file) | **GET** /Accounts/{accountId}/Recordings/{recordingId}/Stream | Stream a Recording File
+*DefaultApi* | [**update_a_conference**](docs/DefaultApi.md#update_a_conference) | **POST** /Accounts/{accountId}/Conferences/{conferenceId} | Update a Conference
+*DefaultApi* | [**update_a_live_call**](docs/DefaultApi.md#update_a_live_call) | **POST** /Accounts/{accountId}/Calls/{callId} | Update a Live Call
+*DefaultApi* | [**update_a_participant**](docs/DefaultApi.md#update_a_participant) | **POST** /Accounts/{accountId}/Conferences/{conferenceId}/Participants/{callId} | Update a Participant
+*DefaultApi* | [**update_a_queue**](docs/DefaultApi.md#update_a_queue) | **POST** /Accounts/{accountId}/Queues/{queueId} | Update a Queue
+*DefaultApi* | [**update_an_account**](docs/DefaultApi.md#update_an_account) | **POST** /Accounts/{accountId} | Manage an account
+*DefaultApi* | [**update_an_application**](docs/DefaultApi.md#update_an_application) | **POST** /Accounts/{accountId}/Applications/{applicationId} | Update an application
+*DefaultApi* | [**update_an_incoming_number**](docs/DefaultApi.md#update_an_incoming_number) | **POST** /Accounts/{accountId}/IncomingPhoneNumbers/{phoneNumberId} | Update an Incoming Number
+
 
 ## Documentation For Models
 
-- [AccountRequest](docs/AccountRequest.md)
-- [AccountResult](docs/AccountResult.md)
-- [AccountResultAllOf](docs/AccountResultAllOf.md)
-- [AccountStatus](docs/AccountStatus.md)
-- [AccountType](docs/AccountType.md)
-- [AddToConference](docs/AddToConference.md)
-- [AddToConferenceAllOf](docs/AddToConferenceAllOf.md)
-- [AnsweredBy](docs/AnsweredBy.md)
-- [ApplicationList](docs/ApplicationList.md)
-- [ApplicationListAllOf](docs/ApplicationListAllOf.md)
-- [ApplicationRequest](docs/ApplicationRequest.md)
-- [ApplicationResult](docs/ApplicationResult.md)
-- [ApplicationResultAllOf](docs/ApplicationResultAllOf.md)
-- [AvailableNumber](docs/AvailableNumber.md)
-- [AvailableNumberList](docs/AvailableNumberList.md)
-- [AvailableNumberListAllOf](docs/AvailableNumberListAllOf.md)
-- [BuyIncomingNumberRequest](docs/BuyIncomingNumberRequest.md)
-- [CallDirection](docs/CallDirection.md)
-- [CallList](docs/CallList.md)
-- [CallListAllOf](docs/CallListAllOf.md)
-- [CallResult](docs/CallResult.md)
-- [CallResultAllOf](docs/CallResultAllOf.md)
-- [CallStatus](docs/CallStatus.md)
-- [Capabilities](docs/Capabilities.md)
-- [ConferenceList](docs/ConferenceList.md)
-- [ConferenceListAllOf](docs/ConferenceListAllOf.md)
-- [ConferenceParticipantList](docs/ConferenceParticipantList.md)
-- [ConferenceParticipantListAllOf](docs/ConferenceParticipantListAllOf.md)
-- [ConferenceParticipantResult](docs/ConferenceParticipantResult.md)
-- [ConferenceParticipantResultAllOf](docs/ConferenceParticipantResultAllOf.md)
-- [ConferenceResult](docs/ConferenceResult.md)
-- [ConferenceResultAllOf](docs/ConferenceResultAllOf.md)
-- [ConferenceStatus](docs/ConferenceStatus.md)
-- [CreateConference](docs/CreateConference.md)
-- [CreateConferenceAllOf](docs/CreateConferenceAllOf.md)
-- [CreateConferenceRequest](docs/CreateConferenceRequest.md)
-- [Dequeue](docs/Dequeue.md)
-- [Enqueue](docs/Enqueue.md)
-- [EnqueueAllOf](docs/EnqueueAllOf.md)
-- [FilterLogsRequest](docs/FilterLogsRequest.md)
-- [GetDigits](docs/GetDigits.md)
-- [GetDigitsAllOf](docs/GetDigitsAllOf.md)
-- [GetSpeech](docs/GetSpeech.md)
-- [GetSpeechAllOf](docs/GetSpeechAllOf.md)
-- [GetSpeechReason](docs/GetSpeechReason.md)
-- [GrammarFileBuiltIn](docs/GrammarFileBuiltIn.md)
-- [GrammarType](docs/GrammarType.md)
-- [Hangup](docs/Hangup.md)
-- [HangupAllOf](docs/HangupAllOf.md)
-- [IfMachine](docs/IfMachine.md)
-- [IncomingNumberList](docs/IncomingNumberList.md)
-- [IncomingNumberListAllOf](docs/IncomingNumberListAllOf.md)
-- [IncomingNumberRequest](docs/IncomingNumberRequest.md)
-- [IncomingNumberResult](docs/IncomingNumberResult.md)
-- [IncomingNumberResultAllOf](docs/IncomingNumberResultAllOf.md)
-- [Language](docs/Language.md)
-- [LogLevel](docs/LogLevel.md)
-- [LogList](docs/LogList.md)
-- [LogListAllOf](docs/LogListAllOf.md)
-- [LogResult](docs/LogResult.md)
-- [MachineType](docs/MachineType.md)
-- [MakeCallRequest](docs/MakeCallRequest.md)
-- [MessageDirection](docs/MessageDirection.md)
-- [MessageRequest](docs/MessageRequest.md)
-- [MessageRequestAllOf](docs/MessageRequestAllOf.md)
-- [MessageResult](docs/MessageResult.md)
-- [MessageResultAllOf](docs/MessageResultAllOf.md)
-- [MessageStatus](docs/MessageStatus.md)
-- [MessagesList](docs/MessagesList.md)
-- [MessagesListAllOf](docs/MessagesListAllOf.md)
-- [MutableResourceModel](docs/MutableResourceModel.md)
-- [OutDial](docs/OutDial.md)
-- [OutDialAllOf](docs/OutDialAllOf.md)
-- [PaginationModel](docs/PaginationModel.md)
-- [Park](docs/Park.md)
-- [ParkAllOf](docs/ParkAllOf.md)
-- [Pause](docs/Pause.md)
-- [PauseAllOf](docs/PauseAllOf.md)
-- [PerclCommand](docs/PerclCommand.md)
-- [PerclScript](docs/PerclScript.md)
-- [Play](docs/Play.md)
-- [PlayAllOf](docs/PlayAllOf.md)
-- [PlayBeep](docs/PlayBeep.md)
-- [PlayEarlyMedia](docs/PlayEarlyMedia.md)
-- [PlayEarlyMediaAllOf](docs/PlayEarlyMediaAllOf.md)
-- [QueueList](docs/QueueList.md)
-- [QueueListAllOf](docs/QueueListAllOf.md)
-- [QueueMember](docs/QueueMember.md)
-- [QueueMemberList](docs/QueueMemberList.md)
-- [QueueMemberListAllOf](docs/QueueMemberListAllOf.md)
-- [QueueRequest](docs/QueueRequest.md)
-- [QueueResult](docs/QueueResult.md)
-- [QueueResultAllOf](docs/QueueResultAllOf.md)
-- [QueueResultStatus](docs/QueueResultStatus.md)
-- [RecordUtterance](docs/RecordUtterance.md)
-- [RecordUtteranceAllOf](docs/RecordUtteranceAllOf.md)
-- [RecordUtteranceTermReason](docs/RecordUtteranceTermReason.md)
-- [RecordingList](docs/RecordingList.md)
-- [RecordingListAllOf](docs/RecordingListAllOf.md)
-- [RecordingResult](docs/RecordingResult.md)
-- [RecordingResultAllOf](docs/RecordingResultAllOf.md)
-- [Redirect](docs/Redirect.md)
-- [RedirectAllOf](docs/RedirectAllOf.md)
-- [Reject](docs/Reject.md)
-- [RejectAllOf](docs/RejectAllOf.md)
-- [RemoveFromConference](docs/RemoveFromConference.md)
-- [RemoveFromConferenceAllOf](docs/RemoveFromConferenceAllOf.md)
-- [RequestType](docs/RequestType.md)
-- [Say](docs/Say.md)
-- [SayAllOf](docs/SayAllOf.md)
-- [SendDigits](docs/SendDigits.md)
-- [SendDigitsAllOf](docs/SendDigitsAllOf.md)
-- [SetListen](docs/SetListen.md)
-- [SetListenAllOf](docs/SetListenAllOf.md)
-- [SetTalk](docs/SetTalk.md)
-- [SetTalkAllOf](docs/SetTalkAllOf.md)
-- [Sms](docs/Sms.md)
-- [SmsAllOf](docs/SmsAllOf.md)
-- [StartRecordCall](docs/StartRecordCall.md)
-- [TerminateConference](docs/TerminateConference.md)
-- [TerminateConferenceAllOf](docs/TerminateConferenceAllOf.md)
-- [Unpark](docs/Unpark.md)
-- [UpdateCallRequest](docs/UpdateCallRequest.md)
-- [UpdateCallRequestStatus](docs/UpdateCallRequestStatus.md)
-- [UpdateConferenceParticipantRequest](docs/UpdateConferenceParticipantRequest.md)
-- [UpdateConferenceRequest](docs/UpdateConferenceRequest.md)
-- [UpdateConferenceRequestStatus](docs/UpdateConferenceRequestStatus.md)
+ - [AccountRequest](docs/AccountRequest.md)
+ - [AccountResult](docs/AccountResult.md)
+ - [AccountResultAllOf](docs/AccountResultAllOf.md)
+ - [AccountStatus](docs/AccountStatus.md)
+ - [AccountType](docs/AccountType.md)
+ - [AddToConference](docs/AddToConference.md)
+ - [AddToConferenceAllOf](docs/AddToConferenceAllOf.md)
+ - [AnsweredBy](docs/AnsweredBy.md)
+ - [ApplicationList](docs/ApplicationList.md)
+ - [ApplicationListAllOf](docs/ApplicationListAllOf.md)
+ - [ApplicationRequest](docs/ApplicationRequest.md)
+ - [ApplicationResult](docs/ApplicationResult.md)
+ - [ApplicationResultAllOf](docs/ApplicationResultAllOf.md)
+ - [AvailableNumber](docs/AvailableNumber.md)
+ - [AvailableNumberList](docs/AvailableNumberList.md)
+ - [AvailableNumberListAllOf](docs/AvailableNumberListAllOf.md)
+ - [BuyIncomingNumberRequest](docs/BuyIncomingNumberRequest.md)
+ - [CallDirection](docs/CallDirection.md)
+ - [CallList](docs/CallList.md)
+ - [CallListAllOf](docs/CallListAllOf.md)
+ - [CallResult](docs/CallResult.md)
+ - [CallResultAllOf](docs/CallResultAllOf.md)
+ - [CallStatus](docs/CallStatus.md)
+ - [Capabilities](docs/Capabilities.md)
+ - [ConferenceList](docs/ConferenceList.md)
+ - [ConferenceListAllOf](docs/ConferenceListAllOf.md)
+ - [ConferenceParticipantList](docs/ConferenceParticipantList.md)
+ - [ConferenceParticipantListAllOf](docs/ConferenceParticipantListAllOf.md)
+ - [ConferenceParticipantResult](docs/ConferenceParticipantResult.md)
+ - [ConferenceParticipantResultAllOf](docs/ConferenceParticipantResultAllOf.md)
+ - [ConferenceResult](docs/ConferenceResult.md)
+ - [ConferenceResultAllOf](docs/ConferenceResultAllOf.md)
+ - [ConferenceStatus](docs/ConferenceStatus.md)
+ - [CreateConference](docs/CreateConference.md)
+ - [CreateConferenceAllOf](docs/CreateConferenceAllOf.md)
+ - [CreateConferenceRequest](docs/CreateConferenceRequest.md)
+ - [Dequeue](docs/Dequeue.md)
+ - [Enqueue](docs/Enqueue.md)
+ - [EnqueueAllOf](docs/EnqueueAllOf.md)
+ - [FilterLogsRequest](docs/FilterLogsRequest.md)
+ - [GetDigits](docs/GetDigits.md)
+ - [GetDigitsAllOf](docs/GetDigitsAllOf.md)
+ - [GetSpeech](docs/GetSpeech.md)
+ - [GetSpeechAllOf](docs/GetSpeechAllOf.md)
+ - [GetSpeechReason](docs/GetSpeechReason.md)
+ - [GrammarFileBuiltIn](docs/GrammarFileBuiltIn.md)
+ - [GrammarType](docs/GrammarType.md)
+ - [Hangup](docs/Hangup.md)
+ - [HangupAllOf](docs/HangupAllOf.md)
+ - [IfMachine](docs/IfMachine.md)
+ - [IncomingNumberList](docs/IncomingNumberList.md)
+ - [IncomingNumberListAllOf](docs/IncomingNumberListAllOf.md)
+ - [IncomingNumberRequest](docs/IncomingNumberRequest.md)
+ - [IncomingNumberResult](docs/IncomingNumberResult.md)
+ - [IncomingNumberResultAllOf](docs/IncomingNumberResultAllOf.md)
+ - [Language](docs/Language.md)
+ - [LogLevel](docs/LogLevel.md)
+ - [LogList](docs/LogList.md)
+ - [LogListAllOf](docs/LogListAllOf.md)
+ - [LogResult](docs/LogResult.md)
+ - [MachineType](docs/MachineType.md)
+ - [MakeCallRequest](docs/MakeCallRequest.md)
+ - [MessageDirection](docs/MessageDirection.md)
+ - [MessageRequest](docs/MessageRequest.md)
+ - [MessageRequestAllOf](docs/MessageRequestAllOf.md)
+ - [MessageResult](docs/MessageResult.md)
+ - [MessageResultAllOf](docs/MessageResultAllOf.md)
+ - [MessageStatus](docs/MessageStatus.md)
+ - [MessagesList](docs/MessagesList.md)
+ - [MessagesListAllOf](docs/MessagesListAllOf.md)
+ - [MutableResourceModel](docs/MutableResourceModel.md)
+ - [OutDial](docs/OutDial.md)
+ - [OutDialAllOf](docs/OutDialAllOf.md)
+ - [PaginationModel](docs/PaginationModel.md)
+ - [Park](docs/Park.md)
+ - [ParkAllOf](docs/ParkAllOf.md)
+ - [Pause](docs/Pause.md)
+ - [PauseAllOf](docs/PauseAllOf.md)
+ - [PerclCommand](docs/PerclCommand.md)
+ - [PerclScript](docs/PerclScript.md)
+ - [Play](docs/Play.md)
+ - [PlayAllOf](docs/PlayAllOf.md)
+ - [PlayBeep](docs/PlayBeep.md)
+ - [PlayEarlyMedia](docs/PlayEarlyMedia.md)
+ - [PlayEarlyMediaAllOf](docs/PlayEarlyMediaAllOf.md)
+ - [QueueList](docs/QueueList.md)
+ - [QueueListAllOf](docs/QueueListAllOf.md)
+ - [QueueMember](docs/QueueMember.md)
+ - [QueueMemberList](docs/QueueMemberList.md)
+ - [QueueMemberListAllOf](docs/QueueMemberListAllOf.md)
+ - [QueueRequest](docs/QueueRequest.md)
+ - [QueueResult](docs/QueueResult.md)
+ - [QueueResultAllOf](docs/QueueResultAllOf.md)
+ - [QueueResultStatus](docs/QueueResultStatus.md)
+ - [RecordUtterance](docs/RecordUtterance.md)
+ - [RecordUtteranceAllOf](docs/RecordUtteranceAllOf.md)
+ - [RecordUtteranceTermReason](docs/RecordUtteranceTermReason.md)
+ - [RecordingList](docs/RecordingList.md)
+ - [RecordingListAllOf](docs/RecordingListAllOf.md)
+ - [RecordingResult](docs/RecordingResult.md)
+ - [RecordingResultAllOf](docs/RecordingResultAllOf.md)
+ - [Redirect](docs/Redirect.md)
+ - [RedirectAllOf](docs/RedirectAllOf.md)
+ - [Reject](docs/Reject.md)
+ - [RejectAllOf](docs/RejectAllOf.md)
+ - [RemoveFromConference](docs/RemoveFromConference.md)
+ - [RemoveFromConferenceAllOf](docs/RemoveFromConferenceAllOf.md)
+ - [RequestType](docs/RequestType.md)
+ - [SMSTenDLCBrand](docs/SMSTenDLCBrand.md)
+ - [SMSTenDLCBrandsListResult](docs/SMSTenDLCBrandsListResult.md)
+ - [SMSTenDLCBrandsListResultAllOf](docs/SMSTenDLCBrandsListResultAllOf.md)
+ - [SMSTenDLCCampaign](docs/SMSTenDLCCampaign.md)
+ - [SMSTenDLCCampaignsListResult](docs/SMSTenDLCCampaignsListResult.md)
+ - [SMSTenDLCCampaignsListResultAllOf](docs/SMSTenDLCCampaignsListResultAllOf.md)
+ - [SMSTenDLCPartnerCampaign](docs/SMSTenDLCPartnerCampaign.md)
+ - [SMSTenDLCPartnerCampaignBrand](docs/SMSTenDLCPartnerCampaignBrand.md)
+ - [SMSTenDLCPartnerCampaignsListResult](docs/SMSTenDLCPartnerCampaignsListResult.md)
+ - [SMSTenDLCPartnerCampaignsListResultAllOf](docs/SMSTenDLCPartnerCampaignsListResultAllOf.md)
+ - [Say](docs/Say.md)
+ - [SayAllOf](docs/SayAllOf.md)
+ - [SendDigits](docs/SendDigits.md)
+ - [SendDigitsAllOf](docs/SendDigitsAllOf.md)
+ - [SetListen](docs/SetListen.md)
+ - [SetListenAllOf](docs/SetListenAllOf.md)
+ - [SetTalk](docs/SetTalk.md)
+ - [SetTalkAllOf](docs/SetTalkAllOf.md)
+ - [Sms](docs/Sms.md)
+ - [SmsAllOf](docs/SmsAllOf.md)
+ - [StartRecordCall](docs/StartRecordCall.md)
+ - [TerminateConference](docs/TerminateConference.md)
+ - [TerminateConferenceAllOf](docs/TerminateConferenceAllOf.md)
+ - [Unpark](docs/Unpark.md)
+ - [UpdateCallRequest](docs/UpdateCallRequest.md)
+ - [UpdateCallRequestStatus](docs/UpdateCallRequestStatus.md)
+ - [UpdateConferenceParticipantRequest](docs/UpdateConferenceParticipantRequest.md)
+ - [UpdateConferenceRequest](docs/UpdateConferenceRequest.md)
+ - [UpdateConferenceRequestStatus](docs/UpdateConferenceRequestStatus.md)
+
 
 ## Documentation For Authorization
 
+
 ## fc
 
 - **Type**: HTTP basic authentication
 
+
 <a name="documentation-for-verify-request-signature"></a>
 
 ## Documentation for verifying request signature
 
 - To verify the request signature, we will need to use the verify_request_signature method within the Request Verifier class
 
   RequestVerifier.verify_request_signature(requestBody, requestHeader, signingSecret, tolerance)
@@ -344,28 +356,26 @@
             RequestVerifier.verify_request_signature(request_body, request_header, signing_secret, tolerance)
   ```
 
 ## Author
 
 support@freeclimb.com
 
-## Notes for Large OpenAPI documents
 
+## Notes for Large OpenAPI documents
 If the OpenAPI document is large, imports in freeclimb.apis and freeclimb.models may fail with a
 RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
 
 Solution 1:
 Use specific imports for apis and models like:
-
 - `from freeclimb.api.default_api import DefaultApi`
 - `from freeclimb.model.pet import Pet`
 
 Solution 2:
 Before importing the package, adjust the maximum recursion limit as shown below:
-
 ```
 import sys
 sys.setrecursionlimit(1500)
 import freeclimb
 from freeclimb.apis import *
 from freeclimb.models import *
 ```
```

### Comparing `FreeClimb-4.3.0/freeclimb/__init__.py` & `FreeClimb-4.4.0/freeclimb/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,17 @@
 # flake8: noqa
 
-"""
-    FreeClimb API
-
-    FreeClimb is a cloud-based application programming interface (API) that puts the power of the Vail platform in your hands. FreeClimb simplifies the process of creating applications that can use a full range of telephony features without requiring specialized or on-site telephony equipment. Using the FreeClimb REST API to write applications is easy! You have the option to use the language of your choice or hit the API directly. Your application can execute a command by issuing a RESTful request to the FreeClimb API. The base URL to send HTTP requests to the FreeClimb REST API is: /apiserver. FreeClimb authenticates and processes your request.  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Contact: support@freeclimb.com
-    Generated by: https://openapi-generator.tech
-"""
-
-
-__version__ = "4.3.0"
-
-# import ApiClient
-from freeclimb.api_client import ApiClient
-
-# import Configuration
-from freeclimb.configuration import Configuration
-
-# import exceptions
-from freeclimb.exceptions import OpenApiException
-from freeclimb.exceptions import ApiAttributeError
-from freeclimb.exceptions import ApiTypeError
-from freeclimb.exceptions import ApiValueError
-from freeclimb.exceptions import ApiKeyError
-from freeclimb.exceptions import ApiException
+# import all models into this package
+# if you have many models here with many references from one model to another this may
+# raise a RecursionError
+# to avoid this, import only the models that you directly need like:
+# from from freeclimb.model.pet import Pet
+# or import this package, but before doing it, use:
+# import sys
+# sys.setrecursionlimit(n)
 
 from freeclimb.model.account_request import AccountRequest
 from freeclimb.model.account_result import AccountResult
 from freeclimb.model.account_result_all_of import AccountResultAllOf
 from freeclimb.model.account_status import AccountStatus
 from freeclimb.model.account_type import AccountType
 from freeclimb.model.add_to_conference import AddToConference
@@ -131,14 +113,24 @@
 from freeclimb.model.redirect import Redirect
 from freeclimb.model.redirect_all_of import RedirectAllOf
 from freeclimb.model.reject import Reject
 from freeclimb.model.reject_all_of import RejectAllOf
 from freeclimb.model.remove_from_conference import RemoveFromConference
 from freeclimb.model.remove_from_conference_all_of import RemoveFromConferenceAllOf
 from freeclimb.model.request_type import RequestType
+from freeclimb.model.sms_ten_dlc_brand import SMSTenDLCBrand
+from freeclimb.model.sms_ten_dlc_brands_list_result import SMSTenDLCBrandsListResult
+from freeclimb.model.sms_ten_dlc_brands_list_result_all_of import SMSTenDLCBrandsListResultAllOf
+from freeclimb.model.sms_ten_dlc_campaign import SMSTenDLCCampaign
+from freeclimb.model.sms_ten_dlc_campaigns_list_result import SMSTenDLCCampaignsListResult
+from freeclimb.model.sms_ten_dlc_campaigns_list_result_all_of import SMSTenDLCCampaignsListResultAllOf
+from freeclimb.model.sms_ten_dlc_partner_campaign import SMSTenDLCPartnerCampaign
+from freeclimb.model.sms_ten_dlc_partner_campaign_brand import SMSTenDLCPartnerCampaignBrand
+from freeclimb.model.sms_ten_dlc_partner_campaigns_list_result import SMSTenDLCPartnerCampaignsListResult
+from freeclimb.model.sms_ten_dlc_partner_campaigns_list_result_all_of import SMSTenDLCPartnerCampaignsListResultAllOf
 from freeclimb.model.say import Say
 from freeclimb.model.say_all_of import SayAllOf
 from freeclimb.model.send_digits import SendDigits
 from freeclimb.model.send_digits_all_of import SendDigitsAllOf
 from freeclimb.model.set_listen import SetListen
 from freeclimb.model.set_listen_all_of import SetListenAllOf
 from freeclimb.model.set_talk import SetTalk
```

### Comparing `FreeClimb-4.3.0/freeclimb/api/default_api.py` & `FreeClimb-4.4.0/freeclimb/api/default_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,20 @@
 from freeclimb.model.queue_list import QueueList
 from freeclimb.model.queue_member import QueueMember
 from freeclimb.model.queue_member_list import QueueMemberList
 from freeclimb.model.queue_request import QueueRequest
 from freeclimb.model.queue_result import QueueResult
 from freeclimb.model.recording_list import RecordingList
 from freeclimb.model.recording_result import RecordingResult
+from freeclimb.model.sms_ten_dlc_brand import SMSTenDLCBrand
+from freeclimb.model.sms_ten_dlc_brands_list_result import SMSTenDLCBrandsListResult
+from freeclimb.model.sms_ten_dlc_campaign import SMSTenDLCCampaign
+from freeclimb.model.sms_ten_dlc_campaigns_list_result import SMSTenDLCCampaignsListResult
+from freeclimb.model.sms_ten_dlc_partner_campaign import SMSTenDLCPartnerCampaign
+from freeclimb.model.sms_ten_dlc_partner_campaigns_list_result import SMSTenDLCPartnerCampaignsListResult
 from freeclimb.model.update_call_request import UpdateCallRequest
 from freeclimb.model.update_conference_participant_request import UpdateConferenceParticipantRequest
 from freeclimb.model.update_conference_request import UpdateConferenceRequest
 
 
 class DefaultApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
@@ -1331,14 +1337,348 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_ten_dlc_sms_brand_endpoint = _Endpoint(
+            settings={
+                'response_type': (SMSTenDLCBrand,),
+                'auth': [
+                    'fc'
+                ],
+                'endpoint_path': '/Accounts/{accountId}/Messages/10DLC/Brands/{brandId}',
+                'operation_id': 'get_ten_dlc_sms_brand',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'account_id',
+                    'brand_id',
+                ],
+                'required': [
+                    'account_id',
+                    'brand_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'account_id':
+                        (str,),
+                    'brand_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'account_id': 'accountId',
+                    'brand_id': 'brandId',
+                },
+                'location_map': {
+                    'account_id': 'path',
+                    'brand_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_ten_dlc_sms_brands_endpoint = _Endpoint(
+            settings={
+                'response_type': (SMSTenDLCBrandsListResult,),
+                'auth': [
+                    'fc'
+                ],
+                'endpoint_path': '/Accounts/{accountId}/Messages/10DLC/Brands',
+                'operation_id': 'get_ten_dlc_sms_brands',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'account_id',
+                ],
+                'required': [
+                    'account_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'account_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'account_id': 'accountId',
+                },
+                'location_map': {
+                    'account_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_ten_dlc_sms_campaign_endpoint = _Endpoint(
+            settings={
+                'response_type': (SMSTenDLCCampaign,),
+                'auth': [
+                    'fc'
+                ],
+                'endpoint_path': '/Accounts/{accountId}/Messages/10DLC/Campaigns/{campaignId}',
+                'operation_id': 'get_ten_dlc_sms_campaign',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'account_id',
+                    'campaign_id',
+                ],
+                'required': [
+                    'account_id',
+                    'campaign_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'account_id':
+                        (str,),
+                    'campaign_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'account_id': 'accountId',
+                    'campaign_id': 'campaignId',
+                },
+                'location_map': {
+                    'account_id': 'path',
+                    'campaign_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_ten_dlc_sms_campaigns_endpoint = _Endpoint(
+            settings={
+                'response_type': (SMSTenDLCCampaignsListResult,),
+                'auth': [
+                    'fc'
+                ],
+                'endpoint_path': '/Accounts/{accountId}/Messages/10DLC/Campaigns',
+                'operation_id': 'get_ten_dlc_sms_campaigns',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'account_id',
+                    'brand_id',
+                ],
+                'required': [
+                    'account_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'account_id':
+                        (str,),
+                    'brand_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'account_id': 'accountId',
+                    'brand_id': 'brandId',
+                },
+                'location_map': {
+                    'account_id': 'path',
+                    'brand_id': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_ten_dlc_sms_partner_campaign_endpoint = _Endpoint(
+            settings={
+                'response_type': (SMSTenDLCPartnerCampaign,),
+                'auth': [
+                    'fc'
+                ],
+                'endpoint_path': '/Accounts/{accountId}/Messages/10DLC/PartnerCampaigns/{campaignId}',
+                'operation_id': 'get_ten_dlc_sms_partner_campaign',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'account_id',
+                    'campaign_id',
+                ],
+                'required': [
+                    'account_id',
+                    'campaign_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'account_id':
+                        (str,),
+                    'campaign_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'account_id': 'accountId',
+                    'campaign_id': 'campaignId',
+                },
+                'location_map': {
+                    'account_id': 'path',
+                    'campaign_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_ten_dlc_sms_partner_campaigns_endpoint = _Endpoint(
+            settings={
+                'response_type': (SMSTenDLCPartnerCampaignsListResult,),
+                'auth': [
+                    'fc'
+                ],
+                'endpoint_path': '/Accounts/{accountId}/Messages/10DLC/PartnerCampaigns',
+                'operation_id': 'get_ten_dlc_sms_partner_campaigns',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'account_id',
+                    'brand_id',
+                ],
+                'required': [
+                    'account_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'account_id':
+                        (str,),
+                    'brand_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'account_id': 'accountId',
+                    'brand_id': 'brandId',
+                },
+                'location_map': {
+                    'account_id': 'path',
+                    'brand_id': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.list_active_queues_endpoint = _Endpoint(
             settings={
                 'response_type': (QueueList,),
                 'auth': [
                     'fc'
                 ],
                 'endpoint_path': '/Accounts/{accountId}/Queues',
@@ -1897,26 +2237,26 @@
                     'alias',
                     'region',
                     'country',
                     'application_id',
                     'has_application',
                     'voice_enabled',
                     'sms_enabled',
+                    'has_campaign',
                     'capabilities_voice',
                     'capabilities_sms',
                     'capabilities_toll_free',
                     'capabilities_ten_dlc',
                     'capabilities_short_code',
                     'offnet',
                 ],
                 'required': [
                     'account_id',
                 ],
                 'nullable': [
-                    'offnet',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -1939,37 +2279,40 @@
                         (str,),
                     'has_application':
                         (bool,),
                     'voice_enabled':
                         (bool,),
                     'sms_enabled':
                         (bool,),
+                    'has_campaign':
+                        (bool,),
                     'capabilities_voice':
                         (bool,),
                     'capabilities_sms':
                         (bool,),
                     'capabilities_toll_free':
                         (bool,),
                     'capabilities_ten_dlc':
                         (bool,),
                     'capabilities_short_code':
                         (bool,),
                     'offnet':
-                        (bool, none_type,),
+                        (bool,),
                 },
                 'attribute_map': {
                     'account_id': 'accountId',
                     'phone_number': 'phoneNumber',
                     'alias': 'alias',
                     'region': 'region',
                     'country': 'country',
                     'application_id': 'applicationId',
                     'has_application': 'hasApplication',
                     'voice_enabled': 'voiceEnabled',
                     'sms_enabled': 'smsEnabled',
+                    'has_campaign': 'hasCampaign',
                     'capabilities_voice': 'capabilities.voice',
                     'capabilities_sms': 'capabilities.sms',
                     'capabilities_toll_free': 'capabilities.tollFree',
                     'capabilities_ten_dlc': 'capabilities.tenDLC',
                     'capabilities_short_code': 'capabilities.shortCode',
                     'offnet': 'offnet',
                 },
@@ -1979,14 +2322,15 @@
                     'alias': 'query',
                     'region': 'query',
                     'country': 'query',
                     'application_id': 'query',
                     'has_application': 'query',
                     'voice_enabled': 'query',
                     'sms_enabled': 'query',
+                    'has_campaign': 'query',
                     'capabilities_voice': 'query',
                     'capabilities_sms': 'query',
                     'capabilities_toll_free': 'query',
                     'capabilities_ten_dlc': 'query',
                     'capabilities_short_code': 'query',
                     'offnet': 'query',
                 },
@@ -4841,14 +5185,514 @@
             self.account_id
 
         kwargs['queue_id'] = \
             queue_id
 
         return self.get_head_member_endpoint.call_with_http_info(**kwargs)
 
+    def get_ten_dlc_sms_brand(
+        self,
+        brand_id, 
+        **kwargs
+        ):
+        """Get a 10DLC SMS Brand  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_ten_dlc_sms_brand(brand_id, async_req=True)
+        >>> result = thread.get()
+
+
+        Args:
+
+
+            brand_id (str): String that uniquely identifies this brand resource.
+
+
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SMSTenDLCBrand
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['account_id'] = \
+            self.account_id
+
+        kwargs['brand_id'] = \
+            brand_id
+
+        return self.get_ten_dlc_sms_brand_endpoint.call_with_http_info(**kwargs)
+
+    def get_ten_dlc_sms_brands(
+        self,
+         
+        **kwargs
+        ):
+        """Get list of SMS 10DLC Brands  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_ten_dlc_sms_brands(async_req=True)
+        >>> result = thread.get()
+
+
+
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SMSTenDLCBrandsListResult
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['account_id'] = \
+            self.account_id
+
+        return self.get_ten_dlc_sms_brands_endpoint.call_with_http_info(**kwargs)
+
+    def get_ten_dlc_sms_campaign(
+        self,
+        campaign_id, 
+        **kwargs
+        ):
+        """Get a 10DLC SMS Campaign  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_ten_dlc_sms_campaign(campaign_id, async_req=True)
+        >>> result = thread.get()
+
+
+        Args:
+
+
+            campaign_id (str): String that uniquely identifies this campaign resource.
+
+
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SMSTenDLCCampaign
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['account_id'] = \
+            self.account_id
+
+        kwargs['campaign_id'] = \
+            campaign_id
+
+        return self.get_ten_dlc_sms_campaign_endpoint.call_with_http_info(**kwargs)
+
+    def get_ten_dlc_sms_campaigns(
+        self,
+         
+        **kwargs
+        ):
+        """Get list of SMS 10DLC Campaigns  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_ten_dlc_sms_campaigns(async_req=True)
+        >>> result = thread.get()
+
+
+
+
+
+        Keyword Args:
+            brand_id (str): The unique identifier for a brand. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SMSTenDLCCampaignsListResult
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['account_id'] = \
+            self.account_id
+
+        return self.get_ten_dlc_sms_campaigns_endpoint.call_with_http_info(**kwargs)
+
+    def get_ten_dlc_sms_partner_campaign(
+        self,
+        campaign_id, 
+        **kwargs
+        ):
+        """Get a 10DLC SMS Partner Campaign  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_ten_dlc_sms_partner_campaign(campaign_id, async_req=True)
+        >>> result = thread.get()
+
+
+        Args:
+
+
+            campaign_id (str): String that uniquely identifies this campaign resource.
+
+
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SMSTenDLCPartnerCampaign
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['account_id'] = \
+            self.account_id
+
+        kwargs['campaign_id'] = \
+            campaign_id
+
+        return self.get_ten_dlc_sms_partner_campaign_endpoint.call_with_http_info(**kwargs)
+
+    def get_ten_dlc_sms_partner_campaigns(
+        self,
+         
+        **kwargs
+        ):
+        """Get list of SMS 10DLC Partner Campaigns  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_ten_dlc_sms_partner_campaigns(async_req=True)
+        >>> result = thread.get()
+
+
+
+
+
+        Keyword Args:
+            brand_id (str): The unique identifier for a brand. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SMSTenDLCPartnerCampaignsListResult
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['account_id'] = \
+            self.account_id
+
+        return self.get_ten_dlc_sms_partner_campaigns_endpoint.call_with_http_info(**kwargs)
+
     def list_active_queues(
         self,
          
         **kwargs
         ):
         """List Active Queues  # noqa: E501
 
@@ -5538,20 +6382,21 @@
             alias (str): Only show incoming phone numbers with aliases that exactly match this value.. [optional]
             region (str): State or province of this phone number.. [optional]
             country (str): Country of this phone number.. [optional]
             application_id (str): ID of the Application that FreeClimb should contact if a Call or SMS arrives for this phone number or a Call from this number is placed. An incoming phone number is not useful until associated with an applicationId.. [optional]
             has_application (bool): Indication of whether the phone number has an application linked to it.. [optional] if omitted the server will use the default value of False
             voice_enabled (bool): Indicates whether the phone number can handle Calls. Typically set to true for all numbers.. [optional] if omitted the server will use the default value of True
             sms_enabled (bool): Indication of whether the phone number can handle sending and receiving SMS messages. Typically set to true for all numbers.. [optional] if omitted the server will use the default value of True
+            has_campaign (bool): Indication of whether the phone number has a campaign associated with it. [optional]
             capabilities_voice (bool): [optional]
             capabilities_sms (bool): [optional]
             capabilities_toll_free (bool): [optional]
             capabilities_ten_dlc (bool): [optional]
             capabilities_short_code (bool): [optional]
-            offnet (bool, none_type): Indication of whether the phone number was registered as an offnet number. This field will be rendered only for requests to the IncomingPhone number resource.. [optional]
+            offnet (bool): Indication of whether the phone number was registered as an offnet number. This field will be rendered only for requests to the IncomingPhone number resource.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `FreeClimb-4.3.0/freeclimb/api_client.py` & `FreeClimb-4.4.0/freeclimb/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/4.3.0/python'
+        self.user_agent = 'OpenAPI-Generator/4.4.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `FreeClimb-4.3.0/freeclimb/configuration.py` & `FreeClimb-4.4.0/freeclimb/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 4.3.0".\
+               "SDK Package Version: 4.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `FreeClimb-4.3.0/freeclimb/exceptions.py` & `FreeClimb-4.4.0/freeclimb/exceptions.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/account_request.py` & `FreeClimb-4.4.0/freeclimb/model/account_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/account_result.py` & `FreeClimb-4.4.0/freeclimb/model/account_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/account_result_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/account_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/account_status.py` & `FreeClimb-4.4.0/freeclimb/model/account_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/account_type.py` & `FreeClimb-4.4.0/freeclimb/model/account_type.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/add_to_conference.py` & `FreeClimb-4.4.0/freeclimb/model/add_to_conference.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/add_to_conference_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/add_to_conference_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/answered_by.py` & `FreeClimb-4.4.0/freeclimb/model/answered_by.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/application_list.py` & `FreeClimb-4.4.0/freeclimb/model/application_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/application_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/application_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/application_request.py` & `FreeClimb-4.4.0/freeclimb/model/application_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/application_result.py` & `FreeClimb-4.4.0/freeclimb/model/application_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/application_result_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/application_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/available_number.py` & `FreeClimb-4.4.0/freeclimb/model/available_number.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/available_number_list.py` & `FreeClimb-4.4.0/freeclimb/model/available_number_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/available_number_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/available_number_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/buy_incoming_number_request.py` & `FreeClimb-4.4.0/freeclimb/model/buy_incoming_number_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/call_direction.py` & `FreeClimb-4.4.0/freeclimb/model/call_direction.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/call_list.py` & `FreeClimb-4.4.0/freeclimb/model/call_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/call_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/call_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/call_result.py` & `FreeClimb-4.4.0/freeclimb/model/call_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/call_result_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/call_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/call_status.py` & `FreeClimb-4.4.0/freeclimb/model/call_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/capabilities.py` & `FreeClimb-4.4.0/freeclimb/model/capabilities.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/conference_list.py` & `FreeClimb-4.4.0/freeclimb/model/conference_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/conference_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/conference_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/conference_participant_list.py` & `FreeClimb-4.4.0/freeclimb/model/conference_participant_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/conference_participant_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/conference_participant_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/conference_participant_result.py` & `FreeClimb-4.4.0/freeclimb/model/conference_participant_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/conference_participant_result_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/conference_participant_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/conference_result.py` & `FreeClimb-4.4.0/freeclimb/model/conference_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/conference_result_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/conference_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/conference_status.py` & `FreeClimb-4.4.0/freeclimb/model/conference_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/create_conference.py` & `FreeClimb-4.4.0/freeclimb/model/create_conference.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/create_conference_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/create_conference_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/create_conference_request.py` & `FreeClimb-4.4.0/freeclimb/model/create_conference_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/dequeue.py` & `FreeClimb-4.4.0/freeclimb/model/dequeue.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/enqueue.py` & `FreeClimb-4.4.0/freeclimb/model/enqueue.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/enqueue_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/enqueue_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/filter_logs_request.py` & `FreeClimb-4.4.0/freeclimb/model/filter_logs_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/get_digits.py` & `FreeClimb-4.4.0/freeclimb/model/get_digits.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/get_digits_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/get_digits_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/get_speech.py` & `FreeClimb-4.4.0/freeclimb/model/get_speech.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/get_speech_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/get_speech_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/get_speech_reason.py` & `FreeClimb-4.4.0/freeclimb/model/get_speech_reason.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/grammar_file_built_in.py` & `FreeClimb-4.4.0/freeclimb/model/grammar_file_built_in.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/grammar_type.py` & `FreeClimb-4.4.0/freeclimb/model/grammar_type.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/hangup.py` & `FreeClimb-4.4.0/freeclimb/model/hangup.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/hangup_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/hangup_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/if_machine.py` & `FreeClimb-4.4.0/freeclimb/model/if_machine.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/incoming_number_list.py` & `FreeClimb-4.4.0/freeclimb/model/incoming_number_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/incoming_number_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/incoming_number_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/incoming_number_request.py` & `FreeClimb-4.4.0/freeclimb/model/queue_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     OpenApiModel
 )
 from freeclimb.exceptions import ApiAttributeError
 
 
 
 
-class IncomingNumberRequest(ModelNormal):
+class QueueRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -79,37 +79,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'application_id': (str,),  # noqa: E501
             'alias': (str,),  # noqa: E501
+            'max_size': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'application_id': 'applicationId',  # noqa: E501
         'alias': 'alias',  # noqa: E501
+        'max_size': 'maxSize',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """IncomingNumberRequest - a model defined in OpenAPI
+        """QueueRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,16 +134,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            application_id (str): ID of the Application that should handle calls to this number.. [optional]  # noqa: E501
-            alias (str): Description for this phone number.. [optional]  # noqa: E501
+            alias (str): Description for this Queue. Max length is 64 characters.. [optional]  # noqa: E501
+            max_size (int): Maximum number of calls this queue can hold. Default is 100. Maximum is 1000. **Note:** Reducing the maxSize of a Queue causes the Queue to reject incoming requests until it shrinks below the new value of maxSize.. [optional] if omitted the server will use the default value of 100  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,15 +184,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """IncomingNumberRequest - a model defined in OpenAPI
+        """QueueRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,16 +217,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            application_id (str): ID of the Application that should handle calls to this number.. [optional]  # noqa: E501
-            alias (str): Description for this phone number.. [optional]  # noqa: E501
+            alias (str): Description for this Queue. Max length is 64 characters.. [optional]  # noqa: E501
+            max_size (int): Maximum number of calls this queue can hold. Default is 100. Maximum is 1000. **Note:** Reducing the maxSize of a Queue causes the Queue to reject incoming requests until it shrinks below the new value of maxSize.. [optional] if omitted the server will use the default value of 100  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `FreeClimb-4.3.0/freeclimb/model/incoming_number_result.py` & `FreeClimb-4.4.0/freeclimb/model/incoming_number_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/incoming_number_result_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/incoming_number_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/language.py` & `FreeClimb-4.4.0/freeclimb/model/language.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/log_level.py` & `FreeClimb-4.4.0/freeclimb/model/log_level.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/log_list.py` & `FreeClimb-4.4.0/freeclimb/model/log_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/log_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/log_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/log_result.py` & `FreeClimb-4.4.0/freeclimb/model/log_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/machine_type.py` & `FreeClimb-4.4.0/freeclimb/model/machine_type.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/make_call_request.py` & `FreeClimb-4.4.0/freeclimb/model/make_call_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/message_direction.py` & `FreeClimb-4.4.0/freeclimb/model/message_direction.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/message_request.py` & `FreeClimb-4.4.0/freeclimb/model/message_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/message_request_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/message_request_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/message_result.py` & `FreeClimb-4.4.0/freeclimb/model/message_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/message_result_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/message_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/message_status.py` & `FreeClimb-4.4.0/freeclimb/model/message_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/messages_list.py` & `FreeClimb-4.4.0/freeclimb/model/messages_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/messages_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/messages_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/mutable_resource_model.py` & `FreeClimb-4.4.0/freeclimb/model/mutable_resource_model.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/out_dial.py` & `FreeClimb-4.4.0/freeclimb/model/out_dial.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/out_dial_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/out_dial_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/pagination_model.py` & `FreeClimb-4.4.0/freeclimb/model/pagination_model.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/park.py` & `FreeClimb-4.4.0/freeclimb/model/park.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/park_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/park_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/pause.py` & `FreeClimb-4.4.0/freeclimb/model/pause.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/pause_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/pause_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/percl_command.py` & `FreeClimb-4.4.0/freeclimb/model/percl_command.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/percl_script.py` & `FreeClimb-4.4.0/freeclimb/model/percl_script.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/play.py` & `FreeClimb-4.4.0/freeclimb/model/play.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/play_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/play_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/play_beep.py` & `FreeClimb-4.4.0/freeclimb/model/play_beep.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/play_early_media.py` & `FreeClimb-4.4.0/freeclimb/model/play_early_media.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/play_early_media_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/play_early_media_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/queue_list.py` & `FreeClimb-4.4.0/freeclimb/model/queue_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/queue_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/queue_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/queue_member.py` & `FreeClimb-4.4.0/freeclimb/model/queue_member.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/queue_member_list.py` & `FreeClimb-4.4.0/freeclimb/model/queue_member_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/queue_member_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/queue_member_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/queue_request.py` & `FreeClimb-4.4.0/freeclimb/model/set_listen_all_of.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     OpenApiModel
 )
 from freeclimb.exceptions import ApiAttributeError
 
 
 
 
-class QueueRequest(ModelNormal):
+class SetListenAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -79,37 +79,40 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'alias': (str,),  # noqa: E501
-            'max_size': (int,),  # noqa: E501
+            'call_id': (str,),  # noqa: E501
+            'listen': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'alias': 'alias',  # noqa: E501
-        'max_size': 'maxSize',  # noqa: E501
+        'call_id': 'callId',  # noqa: E501
+        'listen': 'listen',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """QueueRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, call_id, *args, **kwargs):  # noqa: E501
+        """SetListenAllOf - a model defined in OpenAPI
+
+        Args:
+            call_id (str): ID of the call leg that is to be assigned the listen privilege. The Call must be in a Conference or an error will be triggered.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,16 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            alias (str): Description for this Queue. Max length is 64 characters.. [optional]  # noqa: E501
-            max_size (int): Maximum number of calls this queue can hold. Default is 100. Maximum is 1000. **Note:** Reducing the maxSize of a Queue causes the Queue to reject incoming requests until it shrinks below the new value of maxSize.. [optional] if omitted the server will use the default value of 100  # noqa: E501
+            listen (bool): Specifying `false` will silence the Conference for this Participant.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -163,14 +165,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.call_id = call_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -183,16 +186,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """QueueRequest - a model defined in OpenAPI
+    def __init__(self, call_id, *args, **kwargs):  # noqa: E501
+        """SetListenAllOf - a model defined in OpenAPI
+
+        Args:
+            call_id (str): ID of the call leg that is to be assigned the listen privilege. The Call must be in a Conference or an error will be triggered.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,16 +223,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            alias (str): Description for this Queue. Max length is 64 characters.. [optional]  # noqa: E501
-            max_size (int): Maximum number of calls this queue can hold. Default is 100. Maximum is 1000. **Note:** Reducing the maxSize of a Queue causes the Queue to reject incoming requests until it shrinks below the new value of maxSize.. [optional] if omitted the server will use the default value of 100  # noqa: E501
+            listen (bool): Specifying `false` will silence the Conference for this Participant.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -244,14 +249,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.call_id = call_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `FreeClimb-4.3.0/freeclimb/model/queue_result.py` & `FreeClimb-4.4.0/freeclimb/model/queue_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/queue_result_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/queue_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/queue_result_status.py` & `FreeClimb-4.4.0/freeclimb/model/queue_result_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/record_utterance.py` & `FreeClimb-4.4.0/freeclimb/model/record_utterance.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/record_utterance_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/record_utterance_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/record_utterance_term_reason.py` & `FreeClimb-4.4.0/freeclimb/model/record_utterance_term_reason.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/recording_list.py` & `FreeClimb-4.4.0/freeclimb/model/recording_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/recording_list_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/recording_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/recording_result.py` & `FreeClimb-4.4.0/freeclimb/model/recording_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/recording_result_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/recording_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/redirect.py` & `FreeClimb-4.4.0/freeclimb/model/redirect.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/redirect_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/redirect_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/reject.py` & `FreeClimb-4.4.0/freeclimb/model/reject.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/reject_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/reject_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/remove_from_conference.py` & `FreeClimb-4.4.0/freeclimb/model/remove_from_conference.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/remove_from_conference_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/remove_from_conference_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/request_type.py` & `FreeClimb-4.4.0/freeclimb/model/request_type.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/say.py` & `FreeClimb-4.4.0/freeclimb/model/say.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/say_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/say_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/send_digits.py` & `FreeClimb-4.4.0/freeclimb/model/send_digits.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/send_digits_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/send_digits_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/set_listen.py` & `FreeClimb-4.4.0/freeclimb/model/set_listen.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/set_listen_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/update_conference_participant_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     OpenApiModel
 )
 from freeclimb.exceptions import ApiAttributeError
 
 
 
 
-class SetListenAllOf(ModelNormal):
+class UpdateConferenceParticipantRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -79,40 +79,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'call_id': (str,),  # noqa: E501
+            'talk': (bool,),  # noqa: E501
             'listen': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'call_id': 'callId',  # noqa: E501
+        'talk': 'talk',  # noqa: E501
         'listen': 'listen',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, call_id, *args, **kwargs):  # noqa: E501
-        """SetListenAllOf - a model defined in OpenAPI
-
-        Args:
-            call_id (str): ID of the call leg that is to be assigned the listen privilege. The Call must be in a Conference or an error will be triggered.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """UpdateConferenceParticipantRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +134,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            listen (bool): Specifying `false` will silence the Conference for this Participant.. [optional]  # noqa: E501
+            talk (bool): (Optional) Default is `true`. Setting to `false` mutes the Participant. FreeClimb returns an error and ignores any other value.. [optional]  # noqa: E501
+            listen (bool): (Optional) Default is `true`. Setting to `false` silences the Conference for this Participant. FreeClimb returns an error and ignores any other value.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -165,15 +163,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.call_id = call_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +183,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, call_id, *args, **kwargs):  # noqa: E501
-        """SetListenAllOf - a model defined in OpenAPI
-
-        Args:
-            call_id (str): ID of the call leg that is to be assigned the listen privilege. The Call must be in a Conference or an error will be triggered.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """UpdateConferenceParticipantRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,15 +217,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            listen (bool): Specifying `false` will silence the Conference for this Participant.. [optional]  # noqa: E501
+            talk (bool): (Optional) Default is `true`. Setting to `false` mutes the Participant. FreeClimb returns an error and ignores any other value.. [optional]  # noqa: E501
+            listen (bool): (Optional) Default is `true`. Setting to `false` silences the Conference for this Participant. FreeClimb returns an error and ignores any other value.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -249,15 +244,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.call_id = call_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `FreeClimb-4.3.0/freeclimb/model/set_talk.py` & `FreeClimb-4.4.0/freeclimb/model/set_talk.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/set_talk_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/set_talk_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/sms.py` & `FreeClimb-4.4.0/freeclimb/model/sms.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/sms_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/sms_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/start_record_call.py` & `FreeClimb-4.4.0/freeclimb/model/start_record_call.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/terminate_conference.py` & `FreeClimb-4.4.0/freeclimb/model/terminate_conference.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/terminate_conference_all_of.py` & `FreeClimb-4.4.0/freeclimb/model/terminate_conference_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/unpark.py` & `FreeClimb-4.4.0/freeclimb/model/unpark.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/update_call_request.py` & `FreeClimb-4.4.0/freeclimb/model/update_call_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/update_call_request_status.py` & `FreeClimb-4.4.0/freeclimb/model/update_call_request_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/update_conference_participant_request.py` & `FreeClimb-4.4.0/freeclimb/model/sms_ten_dlc_brands_list_result_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,20 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from freeclimb.exceptions import ApiAttributeError
 
 
 
+def lazy_import():
+    from freeclimb.model.sms_ten_dlc_brand import SMSTenDLCBrand
+    globals()['SMSTenDLCBrand'] = SMSTenDLCBrand
 
-class UpdateConferenceParticipantRequest(ModelNormal):
+
+class SMSTenDLCBrandsListResultAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -64,52 +68,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'talk': (bool,),  # noqa: E501
-            'listen': (bool,),  # noqa: E501
+            'brands': ([SMSTenDLCBrand], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'talk': 'talk',  # noqa: E501
-        'listen': 'listen',  # noqa: E501
+        'brands': 'brands',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateConferenceParticipantRequest - a model defined in OpenAPI
+        """SMSTenDLCBrandsListResultAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,16 +138,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            talk (bool): (Optional) Default is `true`. Setting to `false` mutes the Participant. FreeClimb returns an error and ignores any other value.. [optional]  # noqa: E501
-            listen (bool): (Optional) Default is `true`. Setting to `false` silences the Conference for this Participant. FreeClimb returns an error and ignores any other value.. [optional]  # noqa: E501
+            brands ([SMSTenDLCBrand], none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UpdateConferenceParticipantRequest - a model defined in OpenAPI
+        """SMSTenDLCBrandsListResultAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,16 +220,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            talk (bool): (Optional) Default is `true`. Setting to `false` mutes the Participant. FreeClimb returns an error and ignores any other value.. [optional]  # noqa: E501
-            listen (bool): (Optional) Default is `true`. Setting to `false` silences the Conference for this Participant. FreeClimb returns an error and ignores any other value.. [optional]  # noqa: E501
+            brands ([SMSTenDLCBrand], none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `FreeClimb-4.3.0/freeclimb/model/update_conference_request.py` & `FreeClimb-4.4.0/freeclimb/model/update_conference_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model/update_conference_request_status.py` & `FreeClimb-4.4.0/freeclimb/model/update_conference_request_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/model_utils.py` & `FreeClimb-4.4.0/freeclimb/model_utils.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/freeclimb/rest.py` & `FreeClimb-4.4.0/freeclimb/rest.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/setup.py` & `FreeClimb-4.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "FreeClimb"
-VERSION = "4.3.0"
+VERSION = "4.4.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `FreeClimb-4.3.0/test/test_account_request.py` & `FreeClimb-4.4.0/test/test_account_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_account_result.py` & `FreeClimb-4.4.0/test/test_account_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_account_result_all_of.py` & `FreeClimb-4.4.0/test/test_account_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_account_status.py` & `FreeClimb-4.4.0/test/test_account_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_account_type.py` & `FreeClimb-4.4.0/test/test_account_type.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_add_to_conference.py` & `FreeClimb-4.4.0/test/test_add_to_conference.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_add_to_conference_all_of.py` & `FreeClimb-4.4.0/test/test_add_to_conference_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_answered_by.py` & `FreeClimb-4.4.0/test/test_answered_by.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_application_list.py` & `FreeClimb-4.4.0/test/test_application_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_application_list_all_of.py` & `FreeClimb-4.4.0/test/test_application_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_application_request.py` & `FreeClimb-4.4.0/test/test_application_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_application_result.py` & `FreeClimb-4.4.0/test/test_application_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_application_result_all_of.py` & `FreeClimb-4.4.0/test/test_application_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_available_number.py` & `FreeClimb-4.4.0/test/test_available_number.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_available_number_list.py` & `FreeClimb-4.4.0/test/test_available_number_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_available_number_list_all_of.py` & `FreeClimb-4.4.0/test/test_available_number_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_buy_incoming_number_request.py` & `FreeClimb-4.4.0/test/test_buy_incoming_number_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_call_direction.py` & `FreeClimb-4.4.0/test/test_call_direction.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_call_list.py` & `FreeClimb-4.4.0/test/test_call_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_call_list_all_of.py` & `FreeClimb-4.4.0/test/test_call_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_call_result.py` & `FreeClimb-4.4.0/test/test_call_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_call_result_all_of.py` & `FreeClimb-4.4.0/test/test_call_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_call_status.py` & `FreeClimb-4.4.0/test/test_call_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_capabilities.py` & `FreeClimb-4.4.0/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_conference_list.py` & `FreeClimb-4.4.0/test/test_conference_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_conference_list_all_of.py` & `FreeClimb-4.4.0/test/test_conference_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_conference_participant_list.py` & `FreeClimb-4.4.0/test/test_conference_participant_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_conference_participant_list_all_of.py` & `FreeClimb-4.4.0/test/test_conference_participant_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_conference_participant_result.py` & `FreeClimb-4.4.0/test/test_conference_participant_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_conference_participant_result_all_of.py` & `FreeClimb-4.4.0/test/test_conference_participant_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_conference_result.py` & `FreeClimb-4.4.0/test/test_conference_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_conference_result_all_of.py` & `FreeClimb-4.4.0/test/test_conference_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_conference_status.py` & `FreeClimb-4.4.0/test/test_conference_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_create_conference.py` & `FreeClimb-4.4.0/test/test_create_conference.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_create_conference_all_of.py` & `FreeClimb-4.4.0/test/test_create_conference_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_create_conference_request.py` & `FreeClimb-4.4.0/test/test_create_conference_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_default_api.py` & `FreeClimb-4.4.0/test/test_default_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,20 @@
 from freeclimb.model.queue_list import QueueList
 from freeclimb.model.queue_member import QueueMember
 from freeclimb.model.queue_member_list import QueueMemberList
 from freeclimb.model.queue_request import QueueRequest
 from freeclimb.model.queue_result import QueueResult
 from freeclimb.model.recording_list import RecordingList
 from freeclimb.model.recording_result import RecordingResult
+from freeclimb.model.sms_ten_dlc_brand import SMSTenDLCBrand
+from freeclimb.model.sms_ten_dlc_brands_list_result import SMSTenDLCBrandsListResult
+from freeclimb.model.sms_ten_dlc_campaign import SMSTenDLCCampaign
+from freeclimb.model.sms_ten_dlc_campaigns_list_result import SMSTenDLCCampaignsListResult
+from freeclimb.model.sms_ten_dlc_partner_campaign import SMSTenDLCPartnerCampaign
+from freeclimb.model.sms_ten_dlc_partner_campaigns_list_result import SMSTenDLCPartnerCampaignsListResult
 from freeclimb.model.update_call_request import UpdateCallRequest
 from freeclimb.model.update_conference_participant_request import UpdateConferenceParticipantRequest
 from freeclimb.model.update_conference_request import UpdateConferenceRequest
 
 import json
 
 class TestDefaultApi(unittest.TestCase):
@@ -394,14 +400,91 @@
         queue_id = queue_id_get_head_member_test_value
 
 
         api_response = self.api.get_head_member(queue_id=queue_id)
         
         assert isinstance(api_response, QueueMember)
 
+    def test_get_ten_dlc_sms_brand(self):
+        """Test case for get_ten_dlc_sms_brand
+
+        Get a 10DLC SMS Brand  # noqa: E501
+        """
+
+        brand_id = brand_id_get_ten_dlc_sms_brand_test_value
+
+
+        api_response = self.api.get_ten_dlc_sms_brand(brand_id=brand_id)
+        
+        assert isinstance(api_response, SMSTenDLCBrand)
+
+    def test_get_ten_dlc_sms_brands(self):
+        """Test case for get_ten_dlc_sms_brands
+
+        Get list of SMS 10DLC Brands  # noqa: E501
+        """
+
+
+
+        api_response = self.api.get_ten_dlc_sms_brands()
+        
+        assert isinstance(api_response, SMSTenDLCBrandsListResult)
+
+    def test_get_ten_dlc_sms_campaign(self):
+        """Test case for get_ten_dlc_sms_campaign
+
+        Get a 10DLC SMS Campaign  # noqa: E501
+        """
+
+        campaign_id = campaign_id_get_ten_dlc_sms_campaign_test_value
+
+
+        api_response = self.api.get_ten_dlc_sms_campaign(campaign_id=campaign_id)
+        
+        assert isinstance(api_response, SMSTenDLCCampaign)
+
+    def test_get_ten_dlc_sms_campaigns(self):
+        """Test case for get_ten_dlc_sms_campaigns
+
+        Get list of SMS 10DLC Campaigns  # noqa: E501
+        """
+
+        brand_id = brand_id_get_ten_dlc_sms_campaigns_test_value
+
+
+        api_response = self.api.get_ten_dlc_sms_campaigns(brand_id=brand_id)
+        
+        assert isinstance(api_response, SMSTenDLCCampaignsListResult)
+
+    def test_get_ten_dlc_sms_partner_campaign(self):
+        """Test case for get_ten_dlc_sms_partner_campaign
+
+        Get a 10DLC SMS Partner Campaign  # noqa: E501
+        """
+
+        campaign_id = campaign_id_get_ten_dlc_sms_partner_campaign_test_value
+
+
+        api_response = self.api.get_ten_dlc_sms_partner_campaign(campaign_id=campaign_id)
+        
+        assert isinstance(api_response, SMSTenDLCPartnerCampaign)
+
+    def test_get_ten_dlc_sms_partner_campaigns(self):
+        """Test case for get_ten_dlc_sms_partner_campaigns
+
+        Get list of SMS 10DLC Partner Campaigns  # noqa: E501
+        """
+
+        brand_id = brand_id_get_ten_dlc_sms_partner_campaigns_test_value
+
+
+        api_response = self.api.get_ten_dlc_sms_partner_campaigns(brand_id=brand_id)
+        
+        assert isinstance(api_response, SMSTenDLCPartnerCampaignsListResult)
+
     def test_list_active_queues(self):
         """Test case for list_active_queues
 
         List Active Queues  # noqa: E501
         """
 
         alias = alias_list_active_queues_test_value
@@ -531,23 +614,24 @@
         alias = alias_list_incoming_numbers_test_value
         region = region_list_incoming_numbers_test_value
         country = country_list_incoming_numbers_test_value
         application_id = application_id_list_incoming_numbers_test_value
         has_application = has_application_list_incoming_numbers_test_value
         voice_enabled = voice_enabled_list_incoming_numbers_test_value
         sms_enabled = sms_enabled_list_incoming_numbers_test_value
+        has_campaign = has_campaign_list_incoming_numbers_test_value
         capabilities_voice = capabilities_voice_list_incoming_numbers_test_value
         capabilities_sms = capabilities_sms_list_incoming_numbers_test_value
         capabilities_toll_free = capabilities_toll_free_list_incoming_numbers_test_value
         capabilities_ten_dlc = capabilities_ten_dlc_list_incoming_numbers_test_value
         capabilities_short_code = capabilities_short_code_list_incoming_numbers_test_value
         offnet = offnet_list_incoming_numbers_test_value
 
 
-        api_response = self.api.list_incoming_numbers(phone_number=phone_number,alias=alias,region=region,country=country,application_id=application_id,has_application=has_application,voice_enabled=voice_enabled,sms_enabled=sms_enabled,capabilities_voice=capabilities_voice,capabilities_sms=capabilities_sms,capabilities_toll_free=capabilities_toll_free,capabilities_ten_dlc=capabilities_ten_dlc,capabilities_short_code=capabilities_short_code,offnet=offnet)
+        api_response = self.api.list_incoming_numbers(phone_number=phone_number,alias=alias,region=region,country=country,application_id=application_id,has_application=has_application,voice_enabled=voice_enabled,sms_enabled=sms_enabled,has_campaign=has_campaign,capabilities_voice=capabilities_voice,capabilities_sms=capabilities_sms,capabilities_toll_free=capabilities_toll_free,capabilities_ten_dlc=capabilities_ten_dlc,capabilities_short_code=capabilities_short_code,offnet=offnet)
         
         assert isinstance(api_response, IncomingNumberList)
 
     def test_list_members(self):
         """Test case for list_members
 
         List Members  # noqa: E501
@@ -952,14 +1036,26 @@
 
 call_id_list_recordings_test_value = "callId_example"
 
 conference_id_list_recordings_test_value = "conferenceId_example"
 
 date_created_list_recordings_test_value = "dateCreated_example"
 
+brand_id_get_ten_dlc_sms_campaigns_test_value = "BX56XX4"
+
+brand_id_get_ten_dlc_sms_partner_campaigns_test_value = "BX56XX4"
+
+brand_id_get_ten_dlc_sms_brand_test_value = "BX56XX4"
+
+campaign_id_get_ten_dlc_sms_campaign_test_value = "CX56XX4"
+
+campaign_id_get_ten_dlc_sms_partner_campaign_test_value = "CX56XX4"
+
+has_campaign_list_incoming_numbers_test_value = True
+
 queue_request_update_a_queue_test_value = QueueRequest(
         alias="alias_example",
         max_size=100,
 )
 
 application_request_update_an_application_test_value = ApplicationRequest(
             alias="alias_example",
```

### Comparing `FreeClimb-4.3.0/test/test_dequeue.py` & `FreeClimb-4.4.0/test/test_dequeue.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_enqueue.py` & `FreeClimb-4.4.0/test/test_enqueue.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_enqueue_all_of.py` & `FreeClimb-4.4.0/test/test_enqueue_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_filter_logs_request.py` & `FreeClimb-4.4.0/test/test_filter_logs_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_get_digits.py` & `FreeClimb-4.4.0/test/test_get_digits.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_get_digits_all_of.py` & `FreeClimb-4.4.0/test/test_get_digits_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_get_speech.py` & `FreeClimb-4.4.0/test/test_get_speech.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_get_speech_all_of.py` & `FreeClimb-4.4.0/test/test_get_speech_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_get_speech_reason.py` & `FreeClimb-4.4.0/test/test_get_speech_reason.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_grammar_file_built_in.py` & `FreeClimb-4.4.0/test/test_grammar_file_built_in.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_grammar_type.py` & `FreeClimb-4.4.0/test/test_grammar_type.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_hangup.py` & `FreeClimb-4.4.0/test/test_hangup.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_hangup_all_of.py` & `FreeClimb-4.4.0/test/test_hangup_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_if_machine.py` & `FreeClimb-4.4.0/test/test_if_machine.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_incoming_number_list.py` & `FreeClimb-4.4.0/test/test_incoming_number_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_incoming_number_list_all_of.py` & `FreeClimb-4.4.0/test/test_incoming_number_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_incoming_number_request.py` & `FreeClimb-4.4.0/test/test_incoming_number_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_incoming_number_result.py` & `FreeClimb-4.4.0/test/test_incoming_number_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_incoming_number_result_all_of.py` & `FreeClimb-4.4.0/test/test_incoming_number_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_language.py` & `FreeClimb-4.4.0/test/test_language.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_log_level.py` & `FreeClimb-4.4.0/test/test_log_level.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_log_list.py` & `FreeClimb-4.4.0/test/test_log_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_log_list_all_of.py` & `FreeClimb-4.4.0/test/test_log_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_log_result.py` & `FreeClimb-4.4.0/test/test_log_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_machine_type.py` & `FreeClimb-4.4.0/test/test_machine_type.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_make_call_request.py` & `FreeClimb-4.4.0/test/test_make_call_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_message_direction.py` & `FreeClimb-4.4.0/test/test_message_direction.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_message_request.py` & `FreeClimb-4.4.0/test/test_message_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_message_request_all_of.py` & `FreeClimb-4.4.0/test/test_message_request_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_message_result.py` & `FreeClimb-4.4.0/test/test_message_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_message_result_all_of.py` & `FreeClimb-4.4.0/test/test_message_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_message_status.py` & `FreeClimb-4.4.0/test/test_message_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_messages_list.py` & `FreeClimb-4.4.0/test/test_messages_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_messages_list_all_of.py` & `FreeClimb-4.4.0/test/test_messages_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_mutable_resource_model.py` & `FreeClimb-4.4.0/test/test_mutable_resource_model.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_out_dial.py` & `FreeClimb-4.4.0/test/test_out_dial.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_out_dial_all_of.py` & `FreeClimb-4.4.0/test/test_out_dial_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_pagination_model.py` & `FreeClimb-4.4.0/test/test_pagination_model.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_park.py` & `FreeClimb-4.4.0/test/test_park.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_park_all_of.py` & `FreeClimb-4.4.0/test/test_park_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_pause.py` & `FreeClimb-4.4.0/test/test_pause.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_pause_all_of.py` & `FreeClimb-4.4.0/test/test_pause_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_percl_command.py` & `FreeClimb-4.4.0/test/test_percl_command.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_percl_script.py` & `FreeClimb-4.4.0/test/test_percl_script.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_play.py` & `FreeClimb-4.4.0/test/test_play.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_play_all_of.py` & `FreeClimb-4.4.0/test/test_play_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_play_beep.py` & `FreeClimb-4.4.0/test/test_play_beep.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_play_early_media.py` & `FreeClimb-4.4.0/test/test_play_early_media.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_play_early_media_all_of.py` & `FreeClimb-4.4.0/test/test_play_early_media_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_queue_list.py` & `FreeClimb-4.4.0/test/test_queue_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_queue_list_all_of.py` & `FreeClimb-4.4.0/test/test_queue_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_queue_member.py` & `FreeClimb-4.4.0/test/test_queue_member.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_queue_member_list.py` & `FreeClimb-4.4.0/test/test_queue_member_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_queue_member_list_all_of.py` & `FreeClimb-4.4.0/test/test_queue_member_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_queue_request.py` & `FreeClimb-4.4.0/test/test_queue_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_queue_result.py` & `FreeClimb-4.4.0/test/test_queue_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_queue_result_all_of.py` & `FreeClimb-4.4.0/test/test_queue_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_queue_result_status.py` & `FreeClimb-4.4.0/test/test_queue_result_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_record_utterance.py` & `FreeClimb-4.4.0/test/test_record_utterance.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_record_utterance_all_of.py` & `FreeClimb-4.4.0/test/test_record_utterance_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_record_utterance_term_reason.py` & `FreeClimb-4.4.0/test/test_record_utterance_term_reason.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_recording_list.py` & `FreeClimb-4.4.0/test/test_recording_list.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_recording_list_all_of.py` & `FreeClimb-4.4.0/test/test_recording_list_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_recording_result.py` & `FreeClimb-4.4.0/test/test_recording_result.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_recording_result_all_of.py` & `FreeClimb-4.4.0/test/test_recording_result_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_redirect.py` & `FreeClimb-4.4.0/test/test_redirect.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_redirect_all_of.py` & `FreeClimb-4.4.0/test/test_redirect_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_reject.py` & `FreeClimb-4.4.0/test/test_reject.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_reject_all_of.py` & `FreeClimb-4.4.0/test/test_reject_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_remove_from_conference.py` & `FreeClimb-4.4.0/test/test_remove_from_conference.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_remove_from_conference_all_of.py` & `FreeClimb-4.4.0/test/test_remove_from_conference_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_request_type.py` & `FreeClimb-4.4.0/test/test_request_type.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_request_verifier.py` & `FreeClimb-4.4.0/test/test_request_verifier.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_say.py` & `FreeClimb-4.4.0/test/test_say.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_say_all_of.py` & `FreeClimb-4.4.0/test/test_say_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_send_digits.py` & `FreeClimb-4.4.0/test/test_send_digits.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_send_digits_all_of.py` & `FreeClimb-4.4.0/test/test_send_digits_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_set_listen.py` & `FreeClimb-4.4.0/test/test_set_listen.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_set_listen_all_of.py` & `FreeClimb-4.4.0/test/test_set_listen_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_set_talk.py` & `FreeClimb-4.4.0/test/test_set_talk.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_set_talk_all_of.py` & `FreeClimb-4.4.0/test/test_set_talk_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_signature_information.py` & `FreeClimb-4.4.0/test/test_signature_information.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_sms.py` & `FreeClimb-4.4.0/test/test_sms.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_sms_all_of.py` & `FreeClimb-4.4.0/test/test_sms_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_start_record_call.py` & `FreeClimb-4.4.0/test/test_start_record_call.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_terminate_conference.py` & `FreeClimb-4.4.0/test/test_terminate_conference.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_terminate_conference_all_of.py` & `FreeClimb-4.4.0/test/test_terminate_conference_all_of.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_unpark.py` & `FreeClimb-4.4.0/test/test_unpark.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_update_call_request.py` & `FreeClimb-4.4.0/test/test_update_call_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_update_call_request_status.py` & `FreeClimb-4.4.0/test/test_update_call_request_status.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_update_conference_participant_request.py` & `FreeClimb-4.4.0/test/test_update_conference_participant_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_update_conference_request.py` & `FreeClimb-4.4.0/test/test_update_conference_request.py`

 * *Files identical despite different names*

### Comparing `FreeClimb-4.3.0/test/test_update_conference_request_status.py` & `FreeClimb-4.4.0/test/test_update_conference_request_status.py`

 * *Files identical despite different names*

