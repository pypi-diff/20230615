# Comparing `tmp/iosense_connect-4.0.0.tar.gz` & `tmp/iosense_connect-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-4.0.0.tar", last modified: Mon Jun 12 13:46:17 2023, max compression
+gzip compressed data, was "dist\iosense_connect-4.0.1.tar", last modified: Thu Jun 15 13:17:52 2023, max compression
```

## Comparing `iosense_connect-4.0.0.tar` & `iosense_connect-4.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 13:46:17.205919 iosense_connect-4.0.0/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-4.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-06-12 13:46:17.205919 iosense_connect-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 13:46:17.096781 iosense_connect-4.0.0/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-4.0.0/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    25075 2023-06-12 13:46:12.000000 iosense_connect-4.0.0/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-06-12 13:46:17.205919 iosense_connect-4.0.0/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-06-12 13:46:16.000000 iosense_connect-4.0.0/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-12 13:46:16.000000 iosense_connect-4.0.0/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 13:46:16.000000 iosense_connect-4.0.0/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-06-12 13:46:16.000000 iosense_connect-4.0.0/iosense_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-12 13:46:16.000000 iosense_connect-4.0.0/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 13:46:17.205919 iosense_connect-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0      848 2023-06-12 13:45:02.000000 iosense_connect-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:17:52.298842 iosense_connect-4.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-4.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-06-15 13:17:52.297029 iosense_connect-4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-4.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 13:17:52.237850 iosense_connect-4.0.1/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-4.0.1/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    27582 2023-06-15 12:16:28.000000 iosense_connect-4.0.1/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:17:52.294657 iosense_connect-4.0.1/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-06-15 13:17:51.000000 iosense_connect-4.0.1/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-15 13:17:51.000000 iosense_connect-4.0.1/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:17:51.000000 iosense_connect-4.0.1/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-06-15 13:17:51.000000 iosense_connect-4.0.1/iosense_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 13:17:51.000000 iosense_connect-4.0.1/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:17:52.298842 iosense_connect-4.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-06-15 13:17:48.000000 iosense_connect-4.0.1/setup.py
```

### Comparing `iosense_connect-4.0.0/LICENSE.txt` & `iosense_connect-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-4.0.0/PKG-INFO` & `iosense_connect-4.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 4.0.0
+Version: 4.0.1
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-4.0.0/README.md` & `iosense_connect-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-4.0.0/iosense_connect/data_access.py` & `iosense_connect-4.0.1/iosense_connect/data_access.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-import json
+import os
 import sys
+import json
 import fsspec
-import requests
 import urllib3
+import requests
 import numpy as np
 import pandas as pd
 from concurrent.futures import ThreadPoolExecutor
 from cryptography.fernet import Fernet
-from datetime import datetime, timezone
 from datetime import timedelta
+from datetime import datetime, timezone
+from dateutil.relativedelta import relativedelta
 
 pd.options.mode.chained_assignment = None
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
+
 class DataAccess:
     def __init__(self, userid, url, key):
         self.userid = userid
         self.url = url
         self.key = key
 
-    def get_caliberation(self, device_id, metadata, df,onpremise=False):
+    def get_caliberation(self, device_id, metadata, df, onpremise=False):
         """
+        :param onpremise:
         :param metadata:
         :param df: Dataframe
         :param device_id: string
         :return: Calibrated dataframe
 
         Perform cal on original data
              y = mx + c
@@ -36,42 +40,43 @@
         sensor_name_list.remove('time')
         if "(" not in sensor_name_list[0]:
             sensor_id_list = sensor_name_list
         else:
             sensor_id_list = [s[s.rfind("(") + 1:s.rfind(")")] for s in sensor_name_list]
 
         if len(metadata) == 0:
-            metadata = DataAccess.get_device_metadata(self, device_id,onpremise=onpremise)
+            metadata = DataAccess.get_device_metadata(self, device_id, onpremise=onpremise)
         data = metadata['params']
 
         for (value1, value2) in zip(sensor_id_list, sensor_name_list):
             df_meta = pd.DataFrame(data[str(value1)])
             df_meta = df_meta.set_index('paramName').transpose()
 
             if 'm' in df_meta.columns and 'c' in df_meta.columns:
                 m = float(df_meta.iloc[0]['m'])
-                c = int(str(df_meta.iloc[0]['c']).replace(',',''))
+                c = int(str(df_meta.iloc[0]['c']).replace(',', ''))
 
                 df[str(value2)] = df[str(value2)].replace('BAD 255', '-99999').replace('-', '99999').replace(
-                    'BAD undefined', '-99999').replace('BAD 0', '-99999').replace('true',True).replace('false',False)
+                    'BAD undefined', '-99999').replace('BAD 0', '-99999').replace('true', True).replace('false', False)
 
                 df[str(value2)] = df[str(value2)].astype('float')
                 df[str(value2)] = (df[str(value2)] * m) + c
                 if 'min' in df_meta.columns:
-                    min = int(df_meta.iloc[0]['min'])
-                    df[str(value2)] = np.where(df[str(value2)] <= min, min, df[str(value2)])
+                    min_value = int(df_meta.iloc[0]['min'])
+                    df[str(value2)] = np.where(df[str(value2)] <= min_value, min_value, df[str(value2)])
                 if 'max' in df_meta.columns:
-                    max = int(str(df_meta.iloc[0]['max']).replace('-', '99999').replace(
+                    max_value = int(str(df_meta.iloc[0]['max']).replace('-', '99999').replace(
                         '1000000000000000000000000000', '99999').replace('100000000000', '99999'))
-                    df[str(value2)] = np.where(df[str(value2)] >= max, max, df[str(value2)])
+                    df[str(value2)] = np.where(df[str(value2)] >= max_value, max_value, df[str(value2)])
         return df
 
-    def get_device_metadata(self, device_id,onpremise=False):
+    def get_device_metadata(self, device_id, onpremise=False):
         """
 
+        :param onpremise:
         :param device_id: string
         :return: Json
 
          Every detail related to a particular device like device added date, calibration values, sensor details etc
 
         """
         try:
@@ -89,43 +94,45 @@
                 raw_data = json.loads(response.text)['data']
                 return raw_data
 
         except Exception as e:
             print('Failed to fetch device Metadata')
             print(e)
 
-    def get_sensor_alias(self, device_id, df, raw_metadata,onpremise=False):
+    def get_sensor_alias(self, device_id, df, raw_metadata, onpremise=False):
         """
 
+        :param onpremise:
         :param raw_metadata: json of device metadata
         :param device_id: string
         :param df: Dataframe
         :return: dataframe with columns having sensor alias
 
         Maps sensor_alias/ sensor name with corresponding sensor ID
         replaces column names with sensor_alias_sensor_id
 
         """
         sensors = list(df.columns)
         sensors.remove('time')
         if len(raw_metadata) == 0:
-            raw_metadata = DataAccess.get_device_metadata(self, device_id,onpremise=onpremise)
+            raw_metadata = DataAccess.get_device_metadata(self, device_id, onpremise=onpremise)
         sensor_spec = 'sensors'
         sensor_param_df = pd.DataFrame(raw_metadata[sensor_spec])
         for sensor in sensors:
             sensor_param_df1 = sensor_param_df[sensor_param_df['sensorId'] == sensor]
             if len(sensor_param_df1) != 0:
                 sensor_name = sensor_param_df1.iloc[0]['sensorName']
                 sensor_name = sensor_name + " (" + sensor + ")"
-                df.rename(columns={sensor:sensor_name},inplace=True)
+                df.rename(columns={sensor: sensor_name}, inplace=True)
         return df, raw_metadata
 
-    def time_grouping(self, df, bands,compute=None):
+    def time_grouping(self, df, bands, compute=None):
         """
 
+        :param compute:
         :param df: DataFrame
         :param bands: 05,1W,1D
         :return: Dataframe
 
         Group time series DataFrame
         Example: The values in Dataframe are at 30s interval we can group and change the 30s interval to 5 mins, 10 mins, 1 day or 1 week.
         The resultant dataframe contains values at given interval.
@@ -156,15 +163,15 @@
 
         df = df.sort_values('time')
         df.reset_index(drop=True, inplace=True)
         results = df.pivot(index='time', columns='sensor', values='value')
         results.reset_index(drop=False, inplace=True)
         return results
 
-    def get_device_details(self,onpremise=False):
+    def get_device_details(self, onpremise=False):
         """
 
         :return: Details Device id and Device Name of a particular account
 
         Dataframe with columne device ids and device names.
 
         """
@@ -185,41 +192,72 @@
                 df_raw = pd.DataFrame(raw_data)
                 return df_raw
 
         except Exception as e:
             print('Failed to fetch device Details')
             print(e)
 
-    def get_load_entities(self,mongoid=None,onpremise=False):
+    def get_load_entities(self, onpremise=False, clusters=None):
         try:
-            if mongoid == None or len(mongoid) < 25 or type(mongoid) == "list" or type(mongoid) == "int":
-                raise Exception("Message: Please Enter Valid mongoid")
-            if str(onpremise).lower() == 'true':
-                url = "http://"+self.url+"/api/metaData/fetchLoadEntity/"+mongoid
+            if type(clusters) == list:
+                len_clusters = len(clusters)
+                if len_clusters == 0:
+                    raise Exception('Message: No clusters provided')
+            elif clusters is None:
+                pass
             else:
-                url = "https://"+self.url+"/api/metaData/fetchLoadEntity/"+mongoid
-            header = {'userID': self.userid}
-            payload = {}
-            response = requests.request('GET', url, headers=header, data=payload, verify=False)
+                raise Exception('Message: Incorrect type of clusters')
 
-            if response.status_code != 200:
-                raw = json.loads(response.text)
-                raise ValueError(raw['error'])
-            else:
-                raw_data = json.loads(response.text)['data']
-                return raw_data
+            page_count = 1
+            cluster_count = 1
+            while True:
+                if str(onpremise).lower() == 'true':
+                    url = "http://" + self.url + "/api/metaData/getAllClusterData/" + self.userid + "/" + str(
+                        page_count) + "/" + str(cluster_count)
+                else:
+                    url = "https://" + self.url + "/api/metaData/getAllClusterData/" + self.userid + "/" + str(
+                        page_count) + "/" + str(cluster_count)
+                header = {'userID': self.userid}
+                payload = {}
+                result = []
+                response = requests.request('GET', url, headers=header, data=payload, verify=False)
+                if response.status_code == 200 and "error" not in json.loads(response.text):
+                    raw_data = json.loads(response.text)
+                    result = result + raw_data["data"]
+                    total_count = json.loads(response.text)['totalCount']
+                    cluster_names = [item['name'] for item in raw_data['data']]
+                    page_count = page_count + 1
+                    cluster_count = total_count
+                    if len(cluster_names) == total_count:
+                        break
+                    if response.status_code != 200:
+                        raw = json.loads(response.text)["error"]
+                        if raw == "The requested page does not exist as the number of elements requested exceeds the total count.":
+                            page_count = page_count - 1
+                        else:
+                            raise ValueError(raw['error'])
+                else:
+                    page_count = page_count - 1
+            if clusters is None:
+                return result
+            else:
+                cluster_dict = []
+                for cluster_name in clusters:
+                    desired_dict = next((item for item in result if item['name'] == cluster_name), None)
+                    cluster_dict.append(desired_dict)
+                return cluster_dict
         except Exception as e:
-            print('Failed to Fetch Load Entities \t',e)
+            print('Failed to Fetch Load Entities \t', e)
 
-    def get_database_credentials(self,db):
+    def get_cloud_credentials(self, db):
         try:
-            header = {"userID":self.userid}
+            header = {"userID": self.userid}
             payload = {}
-            url = "https://"+self.url+"/api/metaData/getCredentials/"+str(db)
-            response = requests.request('GET',url,headers=header,json=payload,verify=False)
+            url = "https://" + self.url + "/api/metaData/getCredentials/" + str(db)
+            response = requests.request('GET', url, headers=header, json=payload, verify=False)
             if response.status_code != 200:
                 raw = json.loads(response.text)
                 raise ValueError(raw)
             else:
                 credentials = json.loads(response.text)['data']
                 cipher = Fernet(self.key)
                 if type(credentials) == list:
@@ -228,44 +266,47 @@
                     credentials[1] = cipher.decrypt(credentials[1].encode('utf-8')).decode()
                 else:
                     credentials = cipher.decrypt(credentials.encode('utf-8')).decode()
                 return credentials
         except Exception as e:
             print(e)
 
-    def get_dp(self, device_id, sensors=None, n=1, cal=True, end_time=datetime.now(),alias=True, IST=True,onpremise=False):
+    def get_dp(self, device_id, sensors=None, n=1, cal=True, end_time=datetime.now(), alias=True, IST=True,
+               onpremise=False):
         """
 
+        :param onpremise:
+        :param alias:
         :param device_id: string
         :param sensors: IST of sensors
         :param n: number of data points (default: 1)
         :param cal: bool (default: True)
         :param end_time: 'YYYY:MM:DD HH:MM:SS'
         :param IST: bool (default: True) Indian Standard Timezone
         :return: Dataframe with values
 
         Get Data Point fetches data containing values of last n data points of given sensor at given time.
 
         """
         try:
 
             metadata = {}
-            if sensors == None:
-                metadata = DataAccess.get_device_metadata(self, device_id,onpremise=onpremise)
+            if sensors is None:
+                metadata = DataAccess.get_device_metadata(self, device_id, onpremise=onpremise)
                 data_sensor = metadata['sensors']
                 df_sensor = pd.DataFrame(data_sensor)
                 sensor_id_list = list(df_sensor['sensorId'])
                 sensors = sensor_id_list
 
             end_time = pd.to_datetime(end_time)
             if IST:
                 end_time = end_time - timedelta(hours=5, minutes=30)
             else:
                 if end_time == datetime.now:
-                    end_time=datetime.now(timezone.utc)
+                    end_time = datetime.now(timezone.utc)
             end_time = int(round(end_time.timestamp()))
             if type(sensors) == list:
                 len_sensors = len(sensors)
                 if len_sensors == 0:
                     raise Exception('Message: No sensors provided')
                 if n < 1:
                     raise ValueError('Incorrect number of data points')
@@ -285,15 +326,15 @@
                     sys.stdout.write("Approx Records Fetched %d" % (10000 * record))
                     sys.stdout.flush()
                 if str(onpremise).lower() == "true":
                     url = "http://" + self.url + "/api/apiLayer/getLimitedDataMultipleSensors/?device=" + device_id + "&sensor=" + sensor_values + "&eTime=" + str(
                         cursor['end']) + "&lim=" + str(cursor['limit']) + "&cursor=true"
                 else:
                     url = "https://" + self.url + "/api/apiLayer/getLimitedDataMultipleSensors/?device=" + device_id + "&sensor=" + sensor_values + "&eTime=" + str(
-                    cursor['end']) + "&lim=" + str(cursor['limit']) + "&cursor=true"
+                        cursor['end']) + "&lim=" + str(cursor['limit']) + "&cursor=true"
                 response = requests.request("GET", url, headers=header, data=payload)
                 raw = json.loads(response.text)
                 if response.status_code != 200:
                     raise ValueError(response.status_code)
                 if 'success' in raw:
                     raise ValueError(raw)
                 else:
@@ -305,42 +346,41 @@
                 if cursor['end'] is None:
                     break
             if len(df) != 0:
                 if IST:
                     df['time'] = pd.to_datetime(df['time'], utc=False)
                     df['time'] = df['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
                 if str(alias).lower() == "true":
-                    df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata,onpremise=onpremise)
+                    df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata, onpremise=onpremise)
                 df = DataAccess.get_cleaned_table(self, df)
                 if str(cal).lower() == 'true':
-                    df = DataAccess.get_caliberation(self, device_id, metadata, df,onpremise=onpremise)
+                    df = DataAccess.get_caliberation(self, device_id, metadata, df, onpremise=onpremise)
             return df
         except Exception as e:
             print(e)
 
-    def fetch_data(self, device_id,start_time, end_time=datetime.now(), alias=True,sensors=None, echo=True,onpremise=False,IST=True):
+    def fetch_data(self, device_id, start_time, end_time=datetime.now(), alias=True, sensors=None, echo=True,
+                   onpremise=False, IST=True):
         """
         Fetch data from influxdb using apis in given timeslot
         """
         metadata = {}
         if sensors is None:
-            metadata = DataAccess.get_device_metadata(self, device_id,onpremise=onpremise)
+            metadata = DataAccess.get_device_metadata(self, device_id, onpremise=onpremise)
             data_sensor = metadata['sensors']
             df_sensor = pd.DataFrame(data_sensor)
             sensor_id_list = list(df_sensor['sensorId'])
             sensors = sensor_id_list
 
         rawdata_res = []
         temp = ''
         try:
-            end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S')
-        except Exception:
-            if type(end_time) == str:
-                end_time = str(end_time) + " 23:59:59"
-            pass
+            end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S').strftime('%Y-%m-%d %H:%M:%S')
+        except:
+            end_time = str(end_time) + " 23:59:59" if isinstance(end_time, str) else end_time
         s_time = pd.to_datetime(start_time)
         e_time = pd.to_datetime(end_time)
         if IST:
             s_time = s_time - timedelta(hours=5, minutes=30)
             e_time = e_time - timedelta(hours=5, minutes=30)
         st_time = int(round(s_time.timestamp())) * 10000
         en_time = int(round(e_time.timestamp())) * 10000
@@ -391,136 +431,137 @@
         if len(df) != 0:
             if IST:
                 df['time'] = pd.to_datetime(df['time'], utc=False)
                 df['time'] = df['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
             if len(df.columns) == 2:
                 df['sensor'] = sensors[0]
             if str(alias).lower() == "true":
-                df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata,onpremise=onpremise)
+                df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata, onpremise=onpremise)
             df = DataAccess.get_cleaned_table(self, df)
         return df
 
-    def data_query(self, device_id, sensors,start_time, end_time=datetime.now(), db=None,alias=True,cal=True, bands=None,onpremise=False,compute=None,api=False,IST=True):
+    def data_query(self, device_id, sensors, start_time, end_time=datetime.now(), db=None, alias=True, cal=True,
+                   bands=None, onpremise=False, compute=None, api=False, IST=True):
         """
 
+        :param api:
+        :param compute:
+        :param onpremise:
+        :param alias:
+        :param db:
+        :param sensors:
         :param device_id: string
         :param start_time: yyyy-MM-dd HH:MM:SS
         :param end_time: yyyy-MM-dd HH:MM:SS
         :param cal: bool
         :param bands: None
         :param IST: bool Indian Time Zone
         :return: df
 
         If requested data exists in feature store fetch data from the container.
         IF data is not available the data is fetched from influxdb
 
         """
         try:
-            if db == None:
-                raise Exception("Invalid DB")
             def get_month_year(filename):
-                parts = filename.split('.')[0].split('-')
-                month = int(parts[0])
-                year = int(parts[1])
+                month, year = map(int, filename.split('.')[0].split('-'))
                 return datetime(year, month, 1)
 
             def generate_month_year_dates(start_date, end_date):
+                end_date = end_date.strftime("%Y-%m-%d %H:%M:%S") if isinstance(end_date, datetime) else str(end_date)
+                start_date = str(start_date) + " 00:00:00" if len(str(start_date).split()) == 1 else str(start_date)
+                end_date = str(end_date) + " 00:00:00" if len(str(end_date).split()) == 1 else str(end_date)
+
                 try:
-                    end_date = end_date.strftime("%Y-%m-%d %H:%M:%S")
+                    current_date = datetime.strptime(start_date, "%Y-%m-%d %H:%M:%S")
+                    end_date = datetime.strptime(end_date, "%Y-%m-%d %H:%M:%S")
                 except:
-                    pass
-                end_date = str(end_date)
-                if len(start_date.split()) == 1:
-                    start_date += " 00:00:00"
-                if len(str(end_date).split()) == 1:
-                    end_date += " 00:00:00"
+                    current_date = datetime.strptime(start_date, "%Y-%m-%d %H:%M:%S.%f")
 
-                current_date = datetime.strptime(start_date, "%Y-%m-%d %H:%M:%S")
-                end_date = datetime.strptime(end_date, "%Y-%m-%d %H:%M:%S")
                 dates = []
-                while current_date <= end_date:
-                    month_year = current_date.strftime("%#m-%Y") + ".parquet"
+                while str(current_date) <= str(end_date):
+                    month = str(current_date.month)
+                    month_year = month + "-" + str(current_date.year) + ".parquet"
                     dates.append(month_year)
-                    current_date += timedelta(days=32)
+                    current_date += relativedelta(months=1)
                     current_date = current_date.replace(day=1)
 
                 return dates
 
-            def read_one(filenames):
-                with connector.open(container_name + str(device_id) + "/" + str(filenames),
-                                 "rb") as src_file:
+            def read_one(filename):
+                with connector.open(container_name + str(device_id) + "/" + str(filename),
+                                    "rb") as src_file:
                     df = pd.read_parquet(src_file)
                 return df
 
-            def thread_read(filenames):
-                results = []
-                if len(filenames) != 0:
+            def thread_read(filenames_list):
+                if len(filenames_list) != 0:
                     with ThreadPoolExecutor(max_workers=40) as executor:  # function to thread
-                        for record in range(len(filenames)):
+                        for record in range(len(filenames_list)):
                             sys.stdout.write('\r')
                             sys.stdout.write("Please Wait .. ")
                             sys.stdout.flush()
-                        results = executor.map(read_one, filenames)
+                        results = executor.map(read_one, filenames_list)
                     fetched_df = pd.concat(results, axis=0)
                 else:
                     fetched_df = pd.DataFrame()
                 return fetched_df
+            start_time = pd.to_datetime(start_time)
+            end_time = pd.to_datetime(end_time)
             if type(end_time) == str:
                 try:
-                    end_time = str(datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S'))
+                    end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S').strftime('%Y-%m-%d %H:%M:%S')
                 except Exception:
-
-                    if type(end_time) == str:
-                        end_time = str(end_time) + " 23:59:59"
-                    pass
+                    end_time = str(end_time) + " 23:59:59" if isinstance(end_time, str) else end_time
             df = pd.DataFrame()
             metadata = {}
             connector = None
             container_name = None
-            credentials = DataAccess.get_database_credentials(self,db)
-            if db == "gcs":
-                credentials = eval(credentials)
-                connector = fsspec.filesystem("gs", project=credentials['project_id'],
-                                              token=credentials)
-                container_name = "faclon-ds-feature-store/"
-
-            elif db == "az":
-                connector = fsspec.filesystem("az", account_name=credentials[0],
-                                              account_key=credentials[1])
-                container_name = "feature-store/"
-
-            elif db == "s3":
-                connector = fsspec.filesystem("s3", key=credentials[0],
-                                              secret=credentials[1])
-                container_name = "faclon-ai-public-bucket/"
-
-            else:
-                raise Exception('Enter correct Database name')
-
-            blobs = connector.ls(container_name)
-            device_list = [blob.split("/")[1] for blob in blobs]
-            if device_id in device_list:
-                blobs = [blob_name.split("/")[2] for blob_name in connector.ls(container_name + str(device_id) + "/")]
-                dates = generate_month_year_dates(start_time, end_time)
-
-                filenames = list(set(dates).intersection(blobs))
-                filenames = sorted(filenames, key=get_month_year)
-                df = thread_read(filenames)
+            if db is not None:
+                credentials = DataAccess.get_cloud_credentials(self, db)
+                if len(credentials) !=0:
+                    if db == "gcs":
+                        credentials = eval(credentials)
+                        connector = fsspec.filesystem("gs", project=credentials['project_id'],
+                                                      token=credentials)
+                        container_name = "faclon-ds-feature-store/"
+
+                    elif db == "az":
+                        connector = fsspec.filesystem("az", account_name=credentials[0],
+                                                      account_key=credentials[1])
+                        container_name = "feature-store/"
+
+                    elif db == "s3":
+                        connector = fsspec.filesystem("s3", key=credentials[0],
+                                                      secret=credentials[1])
+                        container_name = "faclon-ai-public-bucket/"
+
+                    else:
+                        raise Exception('Enter correct Database name')
+
+                    blobs = connector.ls(container_name)
+                    device_list = [blob.split("/")[1] for blob in blobs]
+                    if device_id in device_list:
+                        blobs = [blob_name.split("/")[2] for blob_name in connector.ls(container_name + str(device_id) + "/")]
+                        dates = generate_month_year_dates(start_time, end_time)
+                        filenames = list(set(dates).intersection(blobs))
+                        filenames = sorted(filenames, key=get_month_year)
+                        df = thread_read(filenames)
             else:
                 df_devices = DataAccess.get_device_details(self)
                 device_list = df_devices['devID'].tolist()
                 if device_id in device_list:
                     df = DataAccess.fetch_data(self, device_id, start_time, end_time, alias, sensors=sensors, echo=True,
                                                onpremise=onpremise, IST=IST)
                 else:
                     raise Exception('Message: Device not added in account')
             if len(df) != 0:
 
                 try:
-                    start_time = datetime.strptime(start_time, '%Y-%m-%d %H:%M:%S')
+                    start_time = datetime.strptime(str(start_time), '%Y-%m-%d %H:%M:%S')
                     end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S')
                 except ValueError:
                     pass
                 except Exception as e:
                     print('Message:', e)
 
                 df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
@@ -542,30 +583,26 @@
                     if str(last_date) < str(end_time):
                         df1 = DataAccess.fetch_data(self, device_id, start_time=last_date, alias=False,
                                                     end_time=end_time, sensors=sensors, echo=True,
                                                     onpremise=onpremise, IST=True)
                         df = pd.concat([df, df1])
                         df.reset_index(drop=True, inplace=True)
 
-
-
             if len(df) != 0:
                 if str(alias).lower() == "true":
                     df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata, onpremise=onpremise)
 
-
                 if str(cal).lower() == 'true':
                     df = DataAccess.get_caliberation(self, device_id, metadata, df, onpremise=onpremise)
 
                 if bands is not None:
                     df = DataAccess.time_grouping(self, df, bands, compute)
                 df = df.set_index(['time'])
                 df = df.fillna(value=np.nan)
                 df.dropna(axis=0, how='all', inplace=True)
                 df.reset_index(drop=False, inplace=True)
                 df.drop_duplicates(inplace=True)
-                if IST == False:
+                if IST is False:
                     df['time'] = pd.to_datetime(df['time']) - timedelta(hours=5, minutes=30)
             return df
         except Exception as e:
             print(e)
-
```

### Comparing `iosense_connect-4.0.0/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-4.0.1/iosense_connect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 4.0.0
+Version: 4.0.1
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

