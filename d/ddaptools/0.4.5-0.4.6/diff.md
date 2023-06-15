# Comparing `tmp/ddaptools-0.4.5.tar.gz` & `tmp/ddaptools-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddaptools-0.4.5.tar", last modified: Wed Jun 14 16:46:58 2023, max compression
+gzip compressed data, was "ddaptools-0.4.6.tar", last modified: Thu Jun 15 18:32:04 2023, max compression
```

## Comparing `ddaptools-0.4.5.tar` & `ddaptools-0.4.6.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 16:46:58.707105 ddaptools-0.4.5/
--rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 ddaptools-0.4.5/LICENSE
--rw-rw-rw-   0        0        0      859 2023-06-14 16:46:58.706115 ddaptools-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 ddaptools-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 16:46:58.508650 ddaptools-0.4.5/ddaptools/
--rw-rw-rw-   0        0        0      391 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:46:58.600925 ddaptools-0.4.5/ddaptools/aws_classes/
--rw-rw-rw-   0        0        0     1242 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/aws_classes/CommonProcesor.py
--rw-rw-rw-   0        0        0     2421 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/aws_classes/JobListener.py
--rw-rw-rw-   0        0        0      190 2023-05-16 18:42:08.000000 ddaptools-0.4.5/ddaptools/aws_classes/__init__.py
--rw-rw-rw-   0        0        0     2177 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/aws_classes/class_adapters.py
--rw-rw-rw-   0        0        0    28115 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/aws_classes/class_enhancement-legacy.py
--rw-rw-rw-   0        0        0    39074 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/aws_classes/class_enhancement.py
--rw-rw-rw-   0        0        0     2302 2023-06-02 21:37:56.000000 ddaptools-0.4.5/ddaptools/aws_classes/class_guardian.py
--rw-rw-rw-   0        0        0    28342 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/aws_classes/class_helpers.py
--rw-rw-rw-   0        0        0     1787 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/aws_classes/class_scheduling.py
--rw-rw-rw-   0        0        0     7173 2023-06-02 21:37:56.000000 ddaptools-0.4.5/ddaptools/aws_classes/config_mapper.py
--rw-rw-rw-   0        0        0    21188 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/aws_classes/config_mapper_df.py
--rw-rw-rw-   0        0        0    19374 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/aws_classes/config_mapper_df_legacy.py
--rw-rw-rw-   0        0        0    20726 2023-06-14 15:57:40.000000 ddaptools-0.4.5/ddaptools/dda_constants.py
--rw-rw-rw-   0        0        0    12357 2023-06-12 14:49:23.000000 ddaptools-0.4.5/ddaptools/dda_models-legacy.py
--rw-rw-rw-   0        0        0    18278 2023-06-13 15:37:26.000000 ddaptools-0.4.5/ddaptools/dda_models.py
--rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 ddaptools-0.4.5/ddaptools/etl_functions.py
--rw-rw-rw-   0        0        0      102 2023-06-02 21:40:09.000000 ddaptools-0.4.5/ddaptools/help.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:46:58.525449 ddaptools-0.4.5/ddaptools.egg-info/
--rw-rw-rw-   0        0        0      859 2023-06-14 16:46:57.000000 ddaptools-0.4.5/ddaptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1177 2023-06-14 16:46:58.000000 ddaptools-0.4.5/ddaptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 16:46:57.000000 ddaptools-0.4.5/ddaptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-14 16:46:58.000000 ddaptools-0.4.5/ddaptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 16:46:58.707105 ddaptools-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      986 2023-06-14 15:57:40.000000 ddaptools-0.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:46:58.702089 ddaptools-0.4.5/test_scenarios/
--rw-rw-rw-   0        0        0     4572 2023-06-14 15:57:40.000000 ddaptools-0.4.5/test_scenarios/JobListener.py
--rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 ddaptools-0.4.5/test_scenarios/__init__.py
--rw-rw-rw-   0        0        0     9407 2023-06-14 15:57:40.000000 ddaptools-0.4.5/test_scenarios/test_adapters.py
--rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 ddaptools-0.4.5/test_scenarios/test_code.py
--rw-rw-rw-   0        0        0     2803 2023-06-14 15:57:40.000000 ddaptools-0.4.5/test_scenarios/test_common_processing.py
--rw-rw-rw-   0        0        0    12469 2023-06-14 15:57:40.000000 ddaptools-0.4.5/test_scenarios/test_enhancement.py
--rw-rw-rw-   0        0        0    20012 2023-06-14 15:57:40.000000 ddaptools-0.4.5/test_scenarios/test_event_normalization.py
--rw-rw-rw-   0        0        0     1781 2023-06-14 15:57:40.000000 ddaptools-0.4.5/test_scenarios/test_guardian.py
--rw-rw-rw-   0        0        0     4599 2023-06-14 15:57:40.000000 ddaptools-0.4.5/test_scenarios/test_helpers.py
--rw-rw-rw-   0        0        0     5415 2023-06-14 15:57:40.000000 ddaptools-0.4.5/test_scenarios/test_scheduling.py
--rw-rw-rw-   0        0        0     4920 2023-06-14 15:57:40.000000 ddaptools-0.4.5/test_scenarios/test_splitting_algorthm.py
+drwxrwxrwx   0        0        0        0 2023-06-15 18:32:04.544957 ddaptools-0.4.6/
+-rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 ddaptools-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0      859 2023-06-15 18:32:04.543380 ddaptools-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 ddaptools-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 18:32:04.120856 ddaptools-0.4.6/ddaptools/
+-rw-rw-rw-   0        0        0      391 2023-06-14 15:57:40.000000 ddaptools-0.4.6/ddaptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 18:32:04.327954 ddaptools-0.4.6/ddaptools/aws_classes/
+-rw-rw-rw-   0        0        0     1242 2023-06-14 15:57:40.000000 ddaptools-0.4.6/ddaptools/aws_classes/CommonProcesor.py
+-rw-rw-rw-   0        0        0     2421 2023-06-14 15:57:40.000000 ddaptools-0.4.6/ddaptools/aws_classes/JobListener.py
+-rw-rw-rw-   0        0        0      190 2023-05-16 18:42:08.000000 ddaptools-0.4.6/ddaptools/aws_classes/__init__.py
+-rw-rw-rw-   0        0        0     2177 2023-06-14 15:57:40.000000 ddaptools-0.4.6/ddaptools/aws_classes/class_adapters.py
+-rw-rw-rw-   0        0        0    28115 2023-06-14 15:57:40.000000 ddaptools-0.4.6/ddaptools/aws_classes/class_enhancement-legacy.py
+-rw-rw-rw-   0        0        0    39316 2023-06-14 20:11:59.000000 ddaptools-0.4.6/ddaptools/aws_classes/class_enhancement.py
+-rw-rw-rw-   0        0        0     2302 2023-06-02 21:37:56.000000 ddaptools-0.4.6/ddaptools/aws_classes/class_guardian.py
+-rw-rw-rw-   0        0        0    29403 2023-06-15 18:27:54.000000 ddaptools-0.4.6/ddaptools/aws_classes/class_helpers.py
+-rw-rw-rw-   0        0        0     1787 2023-06-14 15:57:40.000000 ddaptools-0.4.6/ddaptools/aws_classes/class_scheduling.py
+-rw-rw-rw-   0        0        0     7173 2023-06-02 21:37:56.000000 ddaptools-0.4.6/ddaptools/aws_classes/config_mapper.py
+-rw-rw-rw-   0        0        0    21188 2023-06-14 15:57:40.000000 ddaptools-0.4.6/ddaptools/aws_classes/config_mapper_df.py
+-rw-rw-rw-   0        0        0    19374 2023-06-14 15:57:40.000000 ddaptools-0.4.6/ddaptools/aws_classes/config_mapper_df_legacy.py
+-rw-rw-rw-   0        0        0    20726 2023-06-14 15:57:40.000000 ddaptools-0.4.6/ddaptools/dda_constants.py
+-rw-rw-rw-   0        0        0    12357 2023-06-12 14:49:23.000000 ddaptools-0.4.6/ddaptools/dda_models-legacy.py
+-rw-rw-rw-   0        0        0    14340 2023-06-15 16:18:47.000000 ddaptools-0.4.6/ddaptools/dda_models.py
+-rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 ddaptools-0.4.6/ddaptools/etl_functions.py
+-rw-rw-rw-   0        0        0      102 2023-06-02 21:40:09.000000 ddaptools-0.4.6/ddaptools/help.py
+drwxrwxrwx   0        0        0        0 2023-06-15 18:32:04.162881 ddaptools-0.4.6/ddaptools.egg-info/
+-rw-rw-rw-   0        0        0      859 2023-06-15 18:32:03.000000 ddaptools-0.4.6/ddaptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1246 2023-06-15 18:32:03.000000 ddaptools-0.4.6/ddaptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 18:32:03.000000 ddaptools-0.4.6/ddaptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-15 18:32:03.000000 ddaptools-0.4.6/ddaptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 18:32:04.545912 ddaptools-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      986 2023-06-15 18:31:29.000000 ddaptools-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 18:32:04.539830 ddaptools-0.4.6/test_scenarios/
+-rw-rw-rw-   0        0        0     4572 2023-06-14 15:57:40.000000 ddaptools-0.4.6/test_scenarios/JobListener.py
+-rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 ddaptools-0.4.6/test_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     9407 2023-06-14 15:57:40.000000 ddaptools-0.4.6/test_scenarios/test_adapters.py
+-rw-rw-rw-   0        0        0     1097 2023-06-15 17:38:49.000000 ddaptools-0.4.6/test_scenarios/test_clean_query_demo.py
+-rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 ddaptools-0.4.6/test_scenarios/test_code.py
+-rw-rw-rw-   0        0        0     2989 2023-06-15 17:06:15.000000 ddaptools-0.4.6/test_scenarios/test_common_processing.py
+-rw-rw-rw-   0        0        0    12471 2023-06-15 14:37:46.000000 ddaptools-0.4.6/test_scenarios/test_enhancement.py
+-rw-rw-rw-   0        0        0    19985 2023-06-14 16:54:32.000000 ddaptools-0.4.6/test_scenarios/test_event_normalization.py
+-rw-rw-rw-   0        0        0     1781 2023-06-14 15:57:40.000000 ddaptools-0.4.6/test_scenarios/test_guardian.py
+-rw-rw-rw-   0        0        0     4599 2023-06-14 15:57:40.000000 ddaptools-0.4.6/test_scenarios/test_helpers.py
+-rw-rw-rw-   0        0        0     5415 2023-06-14 15:57:40.000000 ddaptools-0.4.6/test_scenarios/test_scheduling.py
+-rw-rw-rw-   0        0        0     4918 2023-06-14 18:56:19.000000 ddaptools-0.4.6/test_scenarios/test_splitting_algorthm.py
+-rw-rw-rw-   0        0        0     1040 2023-06-15 14:34:41.000000 ddaptools-0.4.6/test_scenarios/test_tenth.py
```

### Comparing `ddaptools-0.4.5/LICENSE` & `ddaptools-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/PKG-INFO` & `ddaptools-0.4.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddaptools
-Version: 0.4.5
+Version: 0.4.6
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/CommonProcesor.py` & `ddaptools-0.4.6/ddaptools/aws_classes/CommonProcesor.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/JobListener.py` & `ddaptools-0.4.6/ddaptools/aws_classes/JobListener.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/class_adapters.py` & `ddaptools-0.4.6/ddaptools/aws_classes/class_adapters.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/class_enhancement-legacy.py` & `ddaptools-0.4.6/ddaptools/aws_classes/class_enhancement-legacy.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/class_enhancement.py` & `ddaptools-0.4.6/ddaptools/aws_classes/class_enhancement.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 user_id=Utils.NoneSafe(user_profile, "user_id"),
                 organization_guid=management_api.organization_guid,
                 application="SALESFORCE",
                 app="SALESFORCE",
                 app_type=None,
                 operation=Utils.NoneSafe(event, "Activity__c"),
                 operation_type=None,
-                staging_details_guid=Utils.NoneSafe(event, "Id"),
+                staging_detail_guid=Utils.NoneSafe(event, "Id"),
                 staging_guid=management_api.guid,
                 platform_id=self.platform_id,
                 organization_id=None,
                 local_timezone=None,
                 timestamp=timestamp,
                 end_time=None,
                 timestamp_local=None,
@@ -190,15 +190,15 @@
                 user_id=Utils.NoneSafe(user_profile, "user_id"),
                 organization_guid=management_api.organization_guid,
                 application="CHROME",
                 app=Utils.NoneSafe(event, "domain"),
                 app_type=None,
                 operation=Utils.NoneSafe(event, "type"),
                 operation_type=None,
-                staging_details_guid=Utils.NoneSafe(event, "guid"),
+                staging_detail_guid=Utils.NoneSafe(event, "guid"),
                 staging_guid=management_api.guid,
                 platform_id=self.platform_id,
                 organization_id=Utils.NoneSafe(user_profile, "user_organization_id"),
                 local_timezone=Utils.NoneSafe(user_profile, "user_timezone"),
                 timestamp=timestamp,
                 end_time=Utils.NoneSafe(event, "endTime"),
                 timestamp_local=None,
@@ -224,15 +224,18 @@
                 email_cc=None,
                 email_imid=None,
                 phone_result=None,
                 record_url=None,
                 recording_url=None,
                 record_id=None,
                 keystrokes=getSumFeats(event, "keyboard"),
-                mouse_clicks=getSumFeats(event, " auxclick", "click", ", dbclick")
+                mouse_clicks=getSumFeats(event, " auxclick", "click", ", dbclick"),
+                span_sequence=Utils.NoneSafe(event, "span_squence", 0),
+                span_guid=Utils.NoneSafe(event, "span_guid", Utils.NoneSafe(event, "guid")),
+                span_start = Utils.NoneSafe(event, "span_start", timestamp)
 
             )
             new_details.append(fileEvent)
         management_api.details = new_details
         return management_api.to_dict()
 
 class WindowsAdapter(SourceAdapter):
@@ -316,15 +319,15 @@
                     user_id=Utils.NoneSafe(user_profile, "user_id"),
                     organization_guid=management_api.organization_guid,
                     application=Utils.NoneSafe(event, "process"),
                     app=Utils.NoneSafe(event, "process"),
                     app_type=None,
                     operation=Utils.NoneSafe(event, "event_type"),
                     operation_type=None,
-                    staging_details_guid=Utils.NoneSafe(event, "guid"),
+                    staging_detail_guid=Utils.NoneSafe(event, "guid"),
                     staging_guid=management_api.guid,
                     platform_id=self.platform_id,
                     organization_id=Utils.NoneSafe(user_profile, "organization_id"),
                     local_timezone=Utils.NoneSafe(user_profile, "user_timezone"),
                     timestamp=timestamp,
                     end_time=Utils.NoneSafe(event, "event_end_date"),
                     timestamp_local=None,
```

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/class_guardian.py` & `ddaptools-0.4.6/ddaptools/aws_classes/class_guardian.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/class_helpers.py` & `ddaptools-0.4.6/ddaptools/aws_classes/class_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     def __init__(self, credentials, settings):
         self.credentials = credentials
         self.settings = settings
         
 
     @abstractmethod
     def publish(self, events: List[dict]):
-        print("publishing to database:", events)
+        # print("publishing to database:", events)
+        pass
 
     @abstractmethod
     def getOne(self, key_value, key_column: str = "guid", table_name: str = "events"):
         print("Getting source with: ", key_value, "in", key_column, "column")
 
 class MockDatabaseProvider(DatabaseProvider):
     """Prints publishing and getters, using for debugging, also returns static examples
@@ -244,24 +245,26 @@
         Args:
             events (List[dict]): List of events to publish.
         """
 
 
         # Pushes the changes into SQL
         insert_sql = f"INSERT INTO {tablename} ({', '.join(column_names)}) VALUES ({', '.join(['%s'] * len(column_names))})"
-        
         def cleanQueryArgument(queryArgument):
             # If the queryArg is a list or dict, format it into a way that is query insertable
             if isinstance(queryArgument, (dict)):
                 # If the is List and the first element is a dict, then it is a list of objects
                 return json.dumps(queryArgument)
             if isinstance(queryArgument, List) and len(queryArgument) >0 and isinstance(queryArgument[0], dict):
                 # return an array of strings of the json
+                # seq = 0
+                dict_result = {}
                 for(i, item) in enumerate(queryArgument):
-                    queryArgument[i] = cleanQueryArgument(item)
+                    dict_result[i] = item
+                return json.dumps(dict_result)
             
             return queryArgument
 
         for row in events:
             values = []
             for col in column_names:
                 value = row.get(col, None)
@@ -406,27 +409,31 @@
     
     
 
     def eventDataIntoTimeSlots(eventData: dict, limit_minutes_per_slot=10) -> List[Timeslot]:
         """
         Split the events into time slots based on the next 10th multiple of minutes.
 
-        Notes: 
-        - 2023-06-14 10:07:29 If the duration is None then, 
+        Notes + Decision: 
+        - 2023-06-14 10:07:29 If the duration is None then, it should still create an empty Timeslot 
+        - 2023-06-14 15:42:32 It should have an increasing if the span_sequence is None span_sequence when 
+        splicing. + Should contain also have the span_guid if it is None => event_guid
 
         Args:
             eventData (dict): Event data dictionary.
             limit_minutes_per_slot (int, optional): The maximum time in minutes to split the events into. Defaults to 10.
 
         Returns:
             List[Timeslot]: A list of Timeslot events.
         """
         timeslots_res = []
         timeslots_event_data = []
         duration = eventData["duration"]
+        span_sequence = eventData["span_sequence"] #should be 0 if not provided
+        span_guid = eventData["span_guid"]
 
         def createEventDataCopy(eventData, start_time, current_endtime):
             """Creates a copy of evetData but overwriting the startTIme and current_endtime
 
             Args:
                 eventData (EventData): original eventData to copy with
                 start_time (datetime): start datetime for the current event to overwrite the eventData copy with
@@ -434,44 +441,63 @@
 
             Returns:
                 EventData: Copy of the Event data with the overwriten start and endtimes
             """
             eventDataCopy = eventData.copy()
             eventDataCopy["timestamp"] = start_time
             eventDataCopy["end_time"] = current_endtime
+            eventDataCopy["span_sequence"] = span_sequence
+            eventDataCopy["span_guid"] = span_guid
+            
             return eventDataCopy
 
+
         if duration is not None and duration > 0:
             start_time = parser.parse(eventData["timestamp"]).astimezone(tz.UTC)
             end_time = parser.parse(eventData["end_time"]).astimezone(tz.UTC)
 
             while start_time < end_time:
-                next_multiple_of_limit = datetime.datetime(
+
+                next_minutes = start_time.minute + limit_minutes_per_slot - (start_time.minute % limit_minutes_per_slot)
+                # Floor math of next_mintutes / 60
+                
+                next_minutes_carries_int = math.floor(next_minutes / 60)
+                next_minutes %= 60
+
+        
+                next_tenth_minutes = datetime.datetime(
                     start_time.year, start_time.month, start_time.day,
-                    start_time.hour, start_time.minute + limit_minutes_per_slot - (start_time.minute % limit_minutes_per_slot),
+                    start_time.hour, next_minutes,
                     tzinfo=tz.UTC
                 )
 
-                current_endtime = min(next_multiple_of_limit, end_time)
+                # Add the minute in datetime as delta if the minute carries 
+
+                if(next_minutes_carries_int > 0):
+                    minutes_to_add =  datetime.timedelta(hours=next_minutes_carries_int)
+                    next_tenth_minutes += minutes_to_add
+
+
+
+                current_endtime = min(next_tenth_minutes, end_time)
                 eventDataCopy = createEventDataCopy(eventData, start_time.isoformat(), current_endtime.isoformat())
                 timeslots_event_data.append(eventDataCopy)
 
-
+                span_sequence += 1
                 start_time = current_endtime
 
         else: 
             # Create a simple timeslot here
 
             start_time = eventData["timestamp"]
             # NOTE: Make sure that end_time can be None on the postgresql model.
             # 2023-06-14 10:12:17 It is Nullable in both local and utc, as well as in duration
             end_time = eventData["end_time"] # It will probably be None, so you have to create something on the date_related_population to support those cases
 
             eventDataCopy = createEventDataCopy(eventData=eventData, start_time=start_time, current_endtime=end_time)
-            print("non duration detected, creating the event Copy", eventDataCopy)
             timeslots_event_data.append(eventDataCopy)
 
             
 
             
 
         if len(timeslots_event_data) > 0:
```

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/class_scheduling.py` & `ddaptools-0.4.6/ddaptools/aws_classes/class_scheduling.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/config_mapper.py` & `ddaptools-0.4.6/ddaptools/aws_classes/config_mapper.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/config_mapper_df.py` & `ddaptools-0.4.6/ddaptools/aws_classes/config_mapper_df.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/aws_classes/config_mapper_df_legacy.py` & `ddaptools-0.4.6/ddaptools/aws_classes/config_mapper_df_legacy.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/dda_constants.py` & `ddaptools-0.4.6/ddaptools/dda_constants.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/dda_models-legacy.py` & `ddaptools-0.4.6/ddaptools/dda_models-legacy.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/ddaptools/dda_models.py` & `ddaptools-0.4.6/ddaptools/dda_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                  user_id: str,
                  organization_guid: str,
                  application: str,
                  app: str,
                  app_type: str,
                  operation: str,
                  operation_type: str,
-                 staging_details_guid: str,
+                 staging_detail_guid: str,
                  staging_guid: str,
                  platform_id: int,
                  organization_id: int,
                  local_timezone: str,
                  timestamp: datetime,
                  end_time: datetime,
                  timestamp_local: datetime,
@@ -90,25 +90,28 @@
                  phone_result: str,
                  record_url: str,
                  recording_url: str,
                  record_id: int,
                 #  These are the only ones that are not in the original model
                  mouse_clicks: int = 0,
                  keystrokes: int = 0,
+                 span_sequence: int = 0,
+                 span_guid:str = "",
+                 span_start:datetime = None
                  ):
         
         self.guid = str(uuid.uuid4())
         self.user_id = user_id
         self.organization_guid = organization_guid
         self.application = application
         self.app = app
         self.app_type = app_type
         self.operation = operation
         self.operation_type = operation_type
-        self.staging_details_guid = staging_details_guid
+        self.staging_detail_guid = staging_detail_guid
         self.staging_guid = staging_guid
         self.platform_id = platform_id
         self.organization_id = organization_id
         self.local_timezone = local_timezone
         self.timestamp = timestamp
         self.end_time = end_time
         self.timestamp_local = timestamp_local
@@ -135,49 +138,51 @@
         self.email_imid = email_imid
         self.phone_result = phone_result
         self.record_url = record_url
         self.recording_url = recording_url
         self.record_id = record_id
         self.mouse_clicks = mouse_clicks
         self.keystrokes = keystrokes
+        self.span_guid = span_guid
+        self.span_sequence = span_sequence
+        self.span_start = span_start
 
 
 class Event(StructureModel):
     """
     This is the time based event. Which will be used on modeling the database.
     """
     def __init__(self, guid: str, user_id: str, application: str, app: str,
-                 app_type: str, operation: str, operation_type: str, platform_id: str, organization_id: str, local_timezone: str,
+                 app_type: str, operation: str, operation_type: str, platform_id: str, organization_guid: str, local_timezone: str,
                  timestamp: datetime, end_time: datetime, timestamp_local: datetime,
                  end_time_local: datetime, duration: float, description: str, title: str,
-                 url: str, site: str, url_domain: str, files: List[dict], file_count: int,
+                 url: str, site: str, files: List[dict], file_count: int,
                  action_type: str, geolocation: dict, ipv4: str, local_ipv4: str,
                  size: int, sha2: str, email_subject: str, from_address: str, to_address: str,
                  email_cc: str, email_bcc: str, email_imid: str, phone_result: str,
                  record_url: str, recording_url: str, record_id: int):
         # Generate random guid
         self.guid = guid
         self.user_id = user_id
         self.application = application
         self.app = app
         self.app_type = app_type
         self.operation = operation
         self.operation_type = operation_type
         self.platform_id = platform_id
-        self.organization_id = organization_id
+        self.organization_guid = organization_guid
         self.local_timezone = local_timezone
         self.timestamp = timestamp
         self.end_time = end_time
         self.timestamp_local = timestamp_local
         self.end_time_local = end_time_local
         self.description = description
         self.title = title
         self.url = url
         self.site = site
-        self.url_domain = url_domain
         self.files = files
         self.file_count = file_count
         self.action_type = action_type
         self.geolocation = geolocation
         self.ipv4 = ipv4
         self.local_ipv4 = local_ipv4
         self.size = size
@@ -193,42 +198,45 @@
         self.recording_url = recording_url
         self.record_id = record_id
 
 
     @staticmethod
     def get_attribute_keys():
         """Returns all the attributes of the class.
-
+        - 2023-06-14 14:33:16 Removed "files", until solution is found
         Returns:
             List[str]: List of attributes.
         """
         return [
             "guid", "user_id",  "application", "app", "app_type",
             "operation", "operation_type", "platform_id",
-            "organization_id", "local_timezone", "timestamp", "end_time", "timestamp_local",
+            "organization_guid", "local_timezone", "timestamp", "end_time", "timestamp_local",
             "end_time_local", "duration", "description", "title", "url", "site",
-            "url_domain", "files", "file_count", "action_type", "geolocation", "ipv4",
+             "file_count", "action_type", "geolocation", "ipv4",
             "local_ipv4", "size", "sha2", "email_subject", "from_address", "to_address",
             "email_cc", "email_bcc", "email_imid", "phone_result", "record_url",
-            "recording_url", "record_id"
+            "recording_url", "record_id", "files"
         ]
 
 
 
 class Timeslot(StructureModel):
     """Timeslot
     This is the timeslot based event in which an hour is divided into 6 slots of 10 minutes.
     """
     def __init__(self, event_guid: str, timeslot: int, timeslot_local: int, hour: int, minute: int,
                  day: int, month: int, year: int, week: int, weekday: int,
                  hour_local: int, minute_local: int, day_local: int, month_local: int,
                  year_local: int, week_local: int, weekday_local: int, mouse_clicks: int,
                  keystrokes: int,
                  staging_guid: str,
-                 staging_details_guid: str):
+                 organization_guid: str,
+                 staging_detail_guid: str, 
+                 span_sequence: int,
+                 span_guid: str):
         self.event_guid = event_guid
         self.timeslot = timeslot
         self.timeslot_local = timeslot_local
         self.hour = hour
         self.minute = minute
         self.day = day
         self.month = month
@@ -240,16 +248,19 @@
         self.day_local = day_local
         self.month_local = month_local
         self.year_local = year_local
         self.week_local = week_local
         self.weekday_local = weekday_local
         self.mouse_clicks = mouse_clicks
         self.keystrokes = keystrokes
+        self.organization_guid = organization_guid
         self.staging_guid = staging_guid
-        self.staging_details_guid = staging_details_guid
+        self.staging_detail_guid = staging_detail_guid
+        self.span_guid = span_guid
+        self.span_sequence = span_sequence
 
 
     @staticmethod
     def get_attribute_keys():
         """Returns all the attributes of the class.
 
         Args:
@@ -258,128 +269,20 @@
         Returns:
             List[str]: List of attributes.
         """
         return [
             "event_guid", "timeslot", "timeslot_local", "hour", "minute", "day", "month",
             "year", "week", "weekday", "hour_local", "minute_local", "day_local",
             "month_local", "year_local", "week_local", "weekday_local", "mouse_clicks",
-            "staging_guid",
-            "keystrokes", "staging_details_guid"
+            "staging_guid", "organization_guid",
+            "keystrokes", "staging_detail_guid",
+            "span_sequence", "span_guid"
         ]
 
     
-# TODO => Delete the following classes (legacy)
-
-class GenericEvent(StructureModel):
-    """Generic event inside the staging area
-    """
-    def __init__(self, event_guid: str, user_guid: str, timestamp_utc: datetime, loadbatch_id: int, raw_details: str, application: str):
-        self.event_guid = event_guid
-        self.user_guid = user_guid
-        self.timestamp_utc = timestamp_utc
-        self.loadbatch_id = loadbatch_id
-        self.raw_details = raw_details
-        self.application = application
-
-
-class FileEvent(GenericEvent):
-    def __init__(self, event_guid: str, user_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, version_source_uri: Attachment, source_uri: Attachment, application: str):
-        super().__init__(event_guid, user_guid,  timestamp_utc, loadbatch_id, raw_details, application=application)
-        self.operation = operation
-        self.version_source_uri = version_source_uri
-        self.source_uri = source_uri
-
-    def to_dict(self):
-        event_dict = super().to_dict()
-        event_dict.update({
-            "operation": self.operation,
-            "version_source_uri": self.version_source_uri.to_dict(),
-            "source_uri": self.source_uri.to_dict(),
-        })
-        return event_dict
-
-class SalesEvent(GenericEvent):
-    """Version 2.0 Introduction with support for sales events
-    2023-05-12 17:53:20: Where are the 
-    """
-    def __init__(self, event_guid: str, user_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str):
-        super().__init__(event_guid, user_guid,  timestamp_utc, loadbatch_id, raw_details, application=application)
-        self.operation = operation #activity__c
-        self.category = category # Object being dealed: Opportunity, Lead, Account, Contact, etc.
-        self.description = description # Description of the activity
-
-    def to_dict(self):
-        event_dict = super().to_dict()
-        event_dict.update({
-            "operation": self.operation,
-            "category": self.category,
-            "description": self.description
-        })
-        return event_dict
-
-class ChromeEvent(SalesEvent):
-    """Verion 3.0 Introduction with support for Chrome events This would be the mapped end interface.
-
-        start_time	str
-        end_time	str
-        duration	double
-        title	str
-        description	str
-        url	
-        attachments	<ST-Attachment>List({id, url, file_type, file_extension_size})
-        action_origin	str
-        span_guid	String
-        root_reference	STRING
-        root_start	Datetime
-        root_end	Datetime
-        root_duration	Number
-
-
-    """
-
-    def __init__(self, event_guid: str, user_guid: str, timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str, 
-                 start_time: str, end_time: str, duration: float, 
-                 title: str, url: str, attachments: Dict[str, Attachment], 
-                 action_origin: str, span_guid: str, root_reference: str, root_start: datetime, root_end: datetime, root_duration: float):
-        super().__init__(event_guid, user_guid, timestamp_utc, loadbatch_id, raw_details, operation, category, application, description)
-        self.start_time = start_time
-        self.end_time = end_time
-        self.duration = duration
-        self.title = title
-        self.url = url
-        self.attachments = attachments
-        self.action_origin = action_origin
-        self.span_guid = span_guid
-        self.root_reference = root_reference
-        self.root_start = root_start
-        self.root_end = root_end
-        self.root_duration = root_duration
-
-
-
-
-    def to_dict(self):
-        event_dict = super().to_dict()
-        event_dict.update({
-            "start_time": self.start_time,
-            "end_time": self.end_time,
-            "duration": self.duration,
-            "title": self.title,
-            "url": self.url,
-            "attachments": self.attachments,
-            "action_origin": self.action_origin,
-            "span_guid": self.span_guid,
-            "root_reference": self.root_reference,
-            "root_start": self.root_start,
-            "root_end": self.root_end,
-            "root_duration": self.root_duration
-        })
-        return event_dict
-        
-
 class StagingModel():
     """
     Model for Staging Events. 
     """
     def __init__(self, version = "", connector_guid="", type = "", organization_guid = "", item_count = 2, details = [], hash_1 = "", hash_2 = "", processed_time = datetime.now(), status = "", last_error_message = "", last_error_time = None, created_time = datetime.now(), updated_time = datetime.now()):
         self.guid = str(uuid.uuid4()) #Random GUID
         self.version = version
```

### Comparing `ddaptools-0.4.5/ddaptools.egg-info/PKG-INFO` & `ddaptools-0.4.6/ddaptools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddaptools
-Version: 0.4.5
+Version: 0.4.6
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ddaptools-0.4.5/ddaptools.egg-info/SOURCES.txt` & `ddaptools-0.4.6/ddaptools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 ddaptools/aws_classes/class_scheduling.py
 ddaptools/aws_classes/config_mapper.py
 ddaptools/aws_classes/config_mapper_df.py
 ddaptools/aws_classes/config_mapper_df_legacy.py
 test_scenarios/JobListener.py
 test_scenarios/__init__.py
 test_scenarios/test_adapters.py
+test_scenarios/test_clean_query_demo.py
 test_scenarios/test_code.py
 test_scenarios/test_common_processing.py
 test_scenarios/test_enhancement.py
 test_scenarios/test_event_normalization.py
 test_scenarios/test_guardian.py
 test_scenarios/test_helpers.py
 test_scenarios/test_scheduling.py
-test_scenarios/test_splitting_algorthm.py
+test_scenarios/test_splitting_algorthm.py
+test_scenarios/test_tenth.py
```

### Comparing `ddaptools-0.4.5/setup.py` & `ddaptools-0.4.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.4.5'
+VERSION = '0.4.6'
 DESCRIPTION = 'DDAPP Modules'
 LONG_DESCRIPTION = 'Common Constants, classes and methods for ETL and other python projects'
 
 # Setting up
 #nenewang08
 setup(
     name="ddaptools",
```

### Comparing `ddaptools-0.4.5/test_scenarios/JobListener.py` & `ddaptools-0.4.6/test_scenarios/JobListener.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/test_scenarios/test_adapters.py` & `ddaptools-0.4.6/test_scenarios/test_adapters.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/test_scenarios/test_common_processing.py` & `ddaptools-0.4.6/test_scenarios/test_common_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,19 @@
         "COLUMN_NAMES_EVENTS": Event.get_attribute_keys(),
         "TABLENAME_TIMESLOTS": "timeslot",
         "COLUMN_NAMES_TIMESLOTS": Timeslot.get_attribute_keys()
     }
     publishingDBProvider = PostgreSQLProviderTimeSlotPlusEventsPublishing(credentials=credentials, settings=settings)
     mockingDBProvide = MockDatabaseProvider(credentials=credentials, settings=settings)
 
+    # Raw Sample: e297909e-dcc4-ebf6-04e7-4e37946f50e5
+    # Demo Sample: 387a26ff-ceed-5015-a6c9-afa
+    
     processor = ConnecToGUIDHarcodedDictBasedCommonProcessor(
         job_parameters={"guid": "387a26ff-ceed-5015-a6c9-afa"},
+        # job_parameters={"guid": "e297909e-dcc4-ebf6-04e7-4e37946f50e5"},
         organization_provider=organizationDBProvider,
         publishingDBProvider=publishingDBProvider
         # publishingDBProvider=mockingDBProvide
     ) 
     
     processor.runJobs() # Should also post at the Mock Database
```

### Comparing `ddaptools-0.4.5/test_scenarios/test_enhancement.py` & `ddaptools-0.4.6/test_scenarios/test_enhancement.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
       "type": "tab-focus",
       "url": "https://www.google.com/search?q=queriable+site%3F&rlz=1C1GCEA_enUS1016US1016&oq=queriable+site%3F&aqs=chrome..69i57j33i10i160.2846j1j7&sourceid=chrome&ie=UTF-8"
     },
     # An extra large event.
     {
     "domain": "pnp.github.io",
     "timestamp": "2023-06-12T14:23:36.135Z",
-    "endTime": "2023-06-12T14:43:40.477Z",
+    "endTime": "2023-06-12T15:43:40.477Z",
     "duration": 1204.34,
     "guid": "fee6724b-2abe-f829-d6a3-46eb5bd6c477",
     "incognito": False,
     "interactions": {
         "scroll": 1
     },
     "isEventComplete": True,
@@ -252,14 +252,15 @@
   },
   
 ],
     "hash_1": "d8298e88a929de23ab1bcb06f7a05d0e694f871fb15ef31800d8027d0f76a2ff",
     "hash_2": "3baea71e7edcb8b8aa4417fb640c0fa0d7f9791c8a2b17ca3f499d10f7a43dcd"
 }
 
+
 # Grab local json file named sample_windows
 sample_widows_raw_input = {}
 
 
 
 DEBUG = False
```

#### html2text {}

```diff
@@ -74,15 +74,15 @@
 5ade-6bd6-8bb51735d054", "incognito": False, "interactions": {},
 "isEventComplete": True, "params": {}, "spanGUID": "460a111f-8bbf-870c-0428-
 cd927ba2b7c4", "spanSequence": 1, "spanStartTime": "2023-06-12T14:23:40.480Z",
 "title": "queriable site? - Google Search (Part 2)", "type": "tab-focus",
 "url": "https://www.google.com/
 search?q=queriable+site%3F&rlz=1C1GCEA_enUS1016US1016&oq=queriable+site%3F&aqs=chrome..69i57j33i10i160.2846j1j7&sourceid=chrome&ie=UTF-
 8" }, # An extra large event. { "domain": "pnp.github.io", "timestamp": "2023-
-06-12T14:23:36.135Z", "endTime": "2023-06-12T14:43:40.477Z", "duration":
+06-12T14:23:36.135Z", "endTime": "2023-06-12T15:43:40.477Z", "duration":
 1204.34, "guid": "fee6724b-2abe-f829-d6a3-46eb5bd6c477", "incognito": False,
 "interactions": { "scroll": 1 }, "isEventComplete": True, "params": {},
 "spanGUID": "58e82818-800d-249e-dbac-42617821dbdb", "spanSequence": 0,
 "spanStartTime": "2023-06-12T14:23:36.135Z", "title": "queryable - PnP/PnPjs",
 "type": "tab-focus", "url": "https://pnp.github.io/pnpjs/queryable/queryable/
 " }, { "id": 16, "url": "https://mazzzystar.github.io/images/2023-05-10/
 superCLUE.jpg", "guid": "0adeb6d2-c889-4592-0b46-e43e887e4d71", "mime": "image/
```

### Comparing `ddaptools-0.4.5/test_scenarios/test_event_normalization.py` & `ddaptools-0.4.6/test_scenarios/test_event_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         ],
           "hash_1": "d8298e88a929de23ab1bcb06f7a05d0e694f871fb15ef31800d8027d0f76a2ff",
           "hash_2": "3baea71e7edcb8b8aa4417fb640c0fa0d7f9791c8a2b17ca3f499d10f7a43dcd",
           "created_time": "2023-02-21T12:34:56Z"
         }
       
     normalized_events = ConfigMapper.event_normalization(sample_stagging_event)
-    if DEBUG: # print(normalized_events)
+    # if DEBUG: # print(normalized_events)
     assert(len(normalized_events) == 2)
 
 
 
 def test_join_organizations_fields():
 
     sample_normalized_events = [{'start_time': '2022-08-15T03:21:45.000Z', 'end_time': '2022-08-15T03:22:30.000Z ', 'log_duration': 58000, 'cick_count': 1200, 'keystroke_count': 22000, 'application': 'Word', 'event_guid': 'qwab-erty-9876-zxcv', 'user_guid': '#jenkins', 'source_system': 'interactor', 'timestamp_utc': '2022-08-15T03 :22:50.000Z', 'loadbatc_id': 45, 'raw_details': '{source.....}', 'staging_guid': '123e4567-e89b-12d3-a456-asdss ', 'version': '1.0', 'source_type': 'CHROME_HISTORY', 'actor': 'nwang@abc.com', 'connector_guid': '123e4567-e89b -12d3-a456-client'}, {'start_time': '2022-08-15T03:23:10.000Z', 'end_time': '2022-08-15T03:24:00.000Z', 'log_ duration': 62000, 'cick_count': 900, 'keystroke_count': 15000, 'application': 'PowerPoint', 'event_guid': 'kl op-asd8-mjui-bvcx', 'user_guid': '#jenkins', 'source_system': 'interactor', 'timestamp_utc': '2022-08-15T03:2 5:10.000Z', 'loadbatc_id': 78, 'raw_details': '{source.....}', 'staging_guid': '123e4567-e89b-12d3-a456-asdss',  'version': '1.0', 'source_type': 'CHROME_HISTORY', 'actor': 'nwang@abc.com', 'connector_guid': '123e4567-e89b-1 2d3-a456-client'}]
@@ -82,26 +82,26 @@
 
     joint_events = ConfigMapper.join_organization_fields(
         normalized_events=sample_normalized_events, 
         user_information_table=organization_params
         )
     
     # expected_events = [{'start_time': '2022-08-15T03:21:45.000Z', 'end_time': '2022-08-15T03:22:30.000 Z ', 'log_duration': 58000, 'cick_count': 1200, 'keystroke_count': 22000, 'application': 'Word', 'event_guid' : 'qwab-erty-9876-zxcv', 'user_guid': '#jenkins', 'source_system': 'interactor', 'timestamp_utc': '2022-08-15 T03 :22:50.000Z', 'loadbatc_id': 45, 'raw_details': '{source.....}', 'staging_guid': '123e4567-e89b-12d3-a456-a sdss ', 'version': '1.0', 'source_type': 'CHROME_HISTORY', 'actor': 'nwang@abc.com', 'connector_guid': '123e4567 -e89b -12d3-a456-client', 'organization_id': 123456, 'user_id': 789012, 'user_team_id': [1, 2, 3], 'p rofile_id': [4, 5, 6], 'user_timezone': 'America/Los_Angeles', 'user_work_hours_start': [9, 10, 11, 9, 9, 0, 0], 'user_work_hours_end': [17, 18, 19, 17, 17, 0, 0], 'user_escape_dates': ['2022-04-15', '2022-06-10'], 'profile_mapp ing_instruction': {'instruction1': 'value1', 'instruction2': 'value2'}}, {'start_time': '2022-08-15T03:23:10. 000Z', 'end_time': '2022-08-15T03:24:00.000Z', 'log_ duration': 62000, 'cick_count': 900, 'keystroke_count': 15000, 'application': 'PowerPoint', 'event_guid': 'kl op-asd8-mjui-bvcx', 'user_guid': '#jenkins', 'sourc e_system': 'interactor', 'timestamp_utc': '2022-08-15T03:2 5:10.000Z', 'loadbatc_id': 78, 'raw_details': '{source... ..}', 'staging_guid': '123e4567-e89b-12d3-a456-asdss', 'version': '1.0', 'source_type': 'CHROME_HISTORY', 'a ctor': 'nwang@abc.com', 'connector_guid': '123e4567-e89b-1 2d3-a456-client', 'organization_id': 123456, 'employe e_id': 789012, 'user_team_id': [1, 2, 3], 'profile_id': [4, 5, 6], 'user_timezone': 'America/Los_Ange les', 'user_work_hours_start': [9, 10, 11, 9, 9, 0, 0], 'user_work_hours_end': [17, 18, 19, 17, 17, 0, 0], 'user_escape_dat es': ['2022-04-15', '2022-06-10'], 'profile_mapping_instruction': {'instruction1': 'value1', 'instruction2': 'value2'}}]
-    if DEBUG: # print(joint_events)
+    # if DEBUG: # print(joint_events)
     
     check_has_columns(check_columns_exists, joint_events)
 
 def test_date_related_population():
     sample_joint_events = [{"start_time":"2023-02-27T17:22:50.000Z","end_time":"2023-02-27T17:25:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-27T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,10,11],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,18,19],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}},{"start_time":"2023-02-22T01:22:50.000Z","end_time":"2023-02-22T01:23:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-22T01:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,10,11],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,18,19],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}},{"start_time":"2023-02-26T03:21:45.000Z","end_time":"2023-02-26T03:23:45.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-26T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,10,11],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,18,19],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}},{"start_time":"2022-08-15T03:23:10.000Z","end_time":"2022-08-15T03:24:00.000Z","log_duration":62000,"cick_count":900,"keystroke_count":15000,"application":"PowerPoint","event_guid":"klop-asd8-mjui-bvcx","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2022-08-16T03:25:10.000Z","loadbatc_id":78,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,10,11],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,18,19],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}}]
     
     check_has_columns_exists = [MONTH_ROW, MONTHNAME_ROW, WEEKDAY_ROW, WEEKDAYNAME_ROW, DAYS_ROW, HOUR_ROW, MINUTES_ROW, DATE_ROW, timestamp_client_local_ROW, TIMESLOT_ROW]
     date_mapped_events = ConfigMapper.date_related_population(sample_joint_events)
     # # print(joint_events)
     
-    if DEBUG: # print(date_mapped_events)
+    # if DEBUG: # print(date_mapped_events)
 
     # Refactoring Resistant test
     check_has_columns(check_columns_exists=check_has_columns_exists,
                       events=date_mapped_events)
 
 def test_bucket_classification():
     # Tests if operations or activity or any others are correctly classified.
@@ -152,28 +152,28 @@
 
     
     date_mapped_events_df = pd.DataFrame(sample_date_events)
 
     classified_events: pd.core.frame.DataFrame = ConfigMapper.mapping_application(date_mapped_events_df=date_mapped_events_df, bucket_instructions=bucket_instructions)
     
     classified_dicts = classified_events.to_dict(orient="records")
-    if DEBUG: # print(classified_dicts)
+    
     
     assert( classified_dicts[0].get(APPLICATIONTYPE_ROW) == "Editor" )
 
 def test_event_classification():
     # Different than the test above, this tests classfications such as 'AFTERHOUR'
     sample_date_events =[{"start_time":"2023-02-27T17:22:50.000Z","end_time":"2023-02-27T17:25:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-27T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,9,9,9,9],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,17,17,17,17],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":2,"month_name":"February","weekday_number":0,"weekday_name":"Mon","day":27,"hour":9,"minute":22,"date":"2023-02-27","timestamp_client_local":"2023-02-27T09:22:50","time_slot":56},{"start_time":"2023-02-22T03:22:50.000Z","end_time":"2023-02-22T03:23:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-22T03:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,9,9,9,9],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,17,17,17,17],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":2,"month_name":"February","weekday_number":1,"weekday_name":"Tue","day":21,"hour":17,"minute":22,"date":"2023-02-21","timestamp_client_local":"2023-02-21T17:22:50","time_slot":104},{"start_time":"2023-02-26T03:21:45.000Z","end_time":"2023-02-26T03:23:45.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-26T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,9,9,9,9],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,17,17,17,17],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":2,"month_name":"February","weekday_number":6,"weekday_name":"Sun","day":26,"hour":9,"minute":22,"date":"2023-02-26","timestamp_client_local":"2023-02-26T09:22:50","time_slot":56},{"start_time":"2022-08-15T03:23:10.000Z","end_time":"2022-08-15T03:24:00.000Z","log_duration":62000,"cick_count":900,"keystroke_count":15000,"application":"PowerPoint","event_guid":"klop-asd8-mjui-bvcx","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2022-08-16T03:25:10.000Z","loadbatc_id":78,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,9,9,9,9],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,17,17,17,17],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":8,"month_name":"August","weekday_number":0,"weekday_name":"Mon","day":15,"hour":20,"minute":25,"date":"2022-08-15","timestamp_client_local":"2022-08-15T20:25:10","time_slot":122}]
 
     date_mapped_events_df = pd.DataFrame(sample_date_events)
     classified_events: pd.core.frame.DataFrame = ConfigMapper.classify_events(date_mapped_events_df=date_mapped_events_df)
     
     classified_dicts = classified_events.to_dict(orient="records")
     
-    if True: # print(classified_dicts)
+    # if True: # print(classified_dicts)
     assert( classified_dicts[0].get(EVENTYPE_ROW) == EDetermination.WORKHOURS.value )
     assert( classified_dicts[2].get(EVENTYPE_ROW) ==  EDetermination.WEEKENDS.value )
     assert( classified_dicts[3].get(EVENTYPE_ROW) ==  EDetermination.AFTERHOURS.value )
```

### Comparing `ddaptools-0.4.5/test_scenarios/test_guardian.py` & `ddaptools-0.4.6/test_scenarios/test_guardian.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/test_scenarios/test_helpers.py` & `ddaptools-0.4.6/test_scenarios/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/test_scenarios/test_scheduling.py` & `ddaptools-0.4.6/test_scenarios/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `ddaptools-0.4.5/test_scenarios/test_splitting_algorthm.py` & `ddaptools-0.4.6/test_scenarios/test_splitting_algorthm.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             "title": "The Leverage of LLMs for Individuals | TL;DR",
             "url": "https://mazzzystar.github.io/images/2023-05-10/superCLUE.jpg",
             "site": "mazzzystar.github.io",
             "url_domain": "mazzzystar.github.io",
             "file_count": 0,
             "action_type": "PASSIVE",
             "staging_guid": "0adeb6d2-c889-4592-0b46-e43e887e4d71",
-            "staging_details_guid": "0adeb6d2-c889-4592-0b46-staging-details-guid",
+            "staging_detail_guid": "0adeb6d2-c889-4592-0b46-staging-details-guid",
             "mouse_clicks": 13,
             "keystrokes": 10,
             "size": 0
         }
 
 
 
@@ -57,15 +57,15 @@
             "title": "The Leverage of LLMs for Individuals | TL;DR",
             "url": "https://mazzzystar.github.io/images/2023-05-10/superCLUE.jpg",
             "site": "mazzzystar.github.io",
             "url_domain": "mazzzystar.github.io",
             "file_count": 0,
             "action_type": "PASSIVE",
             "staging_guid": "0adeb6d2-c889-4592-0b46-e43e887e4d71",
-            "staging_details_guid": "0adeb6d2-c889-4592-0b46-staging-details-guid",
+            "staging_detail_guid": "0adeb6d2-c889-4592-0b46-staging-details-guid",
             "mouse_clicks": 13,
             "keystrokes": 10,
             "size": 0
         }
         eventData = nondurationeventData
         
         expected_timeslots = [
```

