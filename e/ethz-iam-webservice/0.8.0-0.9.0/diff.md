# Comparing `tmp/ethz_iam_webservice-0.8.0.tar.gz` & `tmp/ethz_iam_webservice-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethz_iam_webservice-0.8.0.tar", last modified: Mon May 16 12:03:11 2022, max compression
+gzip compressed data, was "ethz_iam_webservice-0.9.0.tar", last modified: Tue Jun 21 15:20:20 2022, max compression
```

## Comparing `ethz_iam_webservice-0.8.0.tar` & `ethz_iam_webservice-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vermeul    (502) staff       (20)        0 2022-05-16 12:03:11.853022 ethz_iam_webservice-0.8.0/
--rw-r--r--   0 vermeul    (502) staff       (20)     8998 2022-05-16 12:03:11.852540 ethz_iam_webservice-0.8.0/PKG-INFO
--rw-r--r--   0 vermeul    (502) staff       (20)     6507 2021-11-15 10:02:13.000000 ethz_iam_webservice-0.8.0/README.md
-drwxr-xr-x   0 vermeul    (502) staff       (20)        0 2022-05-16 12:03:11.849212 ethz_iam_webservice-0.8.0/ethz_iam_webservice/
--rw-r--r--   0 vermeul    (502) staff       (20)      150 2022-05-16 12:01:54.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice/__init__.py
--rw-r--r--   0 vermeul    (502) staff       (20)    19372 2021-11-11 15:44:52.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice/ethz_iam.py
--rw-r--r--   0 vermeul    (502) staff       (20)     2085 2021-07-02 14:17:44.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice/group.py
--rw-r--r--   0 vermeul    (502) staff       (20)     2937 2020-06-25 23:56:47.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice/mailinglist.py
--rw-r--r--   0 vermeul    (502) staff       (20)    17425 2022-05-16 12:01:54.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice/main.py
--rw-r--r--   0 vermeul    (502) staff       (20)     7632 2021-07-02 14:17:44.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice/person.py
--rw-r--r--   0 vermeul    (502) staff       (20)     2499 2021-07-02 14:17:44.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice/service.py
--rw-r--r--   0 vermeul    (502) staff       (20)     6739 2021-11-17 14:58:31.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice/user.py
--rw-r--r--   0 vermeul    (502) staff       (20)     4242 2021-11-17 14:54:41.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice/utils.py
--rw-r--r--   0 vermeul    (502) staff       (20)      175 2020-06-25 23:56:47.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice/verbose.py
-drwxr-xr-x   0 vermeul    (502) staff       (20)        0 2022-05-16 12:03:11.852078 ethz_iam_webservice-0.8.0/ethz_iam_webservice.egg-info/
--rw-r--r--   0 vermeul    (502) staff       (20)     8998 2022-05-16 12:03:11.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice.egg-info/PKG-INFO
--rw-r--r--   0 vermeul    (502) staff       (20)      625 2022-05-16 12:03:11.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice.egg-info/SOURCES.txt
--rw-r--r--   0 vermeul    (502) staff       (20)        1 2022-05-16 12:03:11.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice.egg-info/dependency_links.txt
--rw-r--r--   0 vermeul    (502) staff       (20)       91 2022-05-16 12:03:11.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice.egg-info/entry_points.txt
--rw-r--r--   0 vermeul    (502) staff       (20)        1 2020-05-13 10:05:01.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice.egg-info/not-zip-safe
--rw-r--r--   0 vermeul    (502) staff       (20)       43 2022-05-16 12:03:11.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice.egg-info/requires.txt
--rw-r--r--   0 vermeul    (502) staff       (20)       20 2022-05-16 12:03:11.000000 ethz_iam_webservice-0.8.0/ethz_iam_webservice.egg-info/top_level.txt
--rw-r--r--   0 vermeul    (502) staff       (20)       38 2022-05-16 12:03:11.853138 ethz_iam_webservice-0.8.0/setup.cfg
--rw-r--r--   0 vermeul    (502) staff       (20)     1269 2022-05-16 12:01:54.000000 ethz_iam_webservice-0.8.0/setup.py
+drwxr-xr-x   0 vermeul    (502) staff       (20)        0 2022-06-21 15:20:20.563577 ethz_iam_webservice-0.9.0/
+-rw-r--r--   0 vermeul    (502) staff       (20)     8998 2022-06-21 15:20:20.563254 ethz_iam_webservice-0.9.0/PKG-INFO
+-rw-r--r--   0 vermeul    (502) staff       (20)     6507 2021-11-15 10:02:13.000000 ethz_iam_webservice-0.9.0/README.md
+drwxr-xr-x   0 vermeul    (502) staff       (20)        0 2022-06-21 15:20:20.560386 ethz_iam_webservice-0.9.0/ethz_iam_webservice/
+-rw-r--r--   0 vermeul    (502) staff       (20)      150 2022-06-21 15:20:07.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice/__init__.py
+-rw-r--r--   0 vermeul    (502) staff       (20)    19782 2022-06-21 15:20:07.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice/ethz_iam.py
+-rw-r--r--   0 vermeul    (502) staff       (20)     2085 2021-07-02 14:17:44.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice/group.py
+-rw-r--r--   0 vermeul    (502) staff       (20)     2937 2020-06-25 23:56:47.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice/mailinglist.py
+-rw-r--r--   0 vermeul    (502) staff       (20)    18022 2022-06-21 15:20:07.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice/main.py
+-rw-r--r--   0 vermeul    (502) staff       (20)     7708 2022-06-21 15:20:07.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice/person.py
+-rw-r--r--   0 vermeul    (502) staff       (20)     2499 2021-07-02 14:17:44.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice/service.py
+-rw-r--r--   0 vermeul    (502) staff       (20)     6739 2021-11-17 14:58:31.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice/user.py
+-rw-r--r--   0 vermeul    (502) staff       (20)     4281 2022-06-21 15:20:07.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice/utils.py
+-rw-r--r--   0 vermeul    (502) staff       (20)      175 2020-06-25 23:56:47.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice/verbose.py
+drwxr-xr-x   0 vermeul    (502) staff       (20)        0 2022-06-21 15:20:20.562783 ethz_iam_webservice-0.9.0/ethz_iam_webservice.egg-info/
+-rw-r--r--   0 vermeul    (502) staff       (20)     8998 2022-06-21 15:20:20.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice.egg-info/PKG-INFO
+-rw-r--r--   0 vermeul    (502) staff       (20)      625 2022-06-21 15:20:20.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice.egg-info/SOURCES.txt
+-rw-r--r--   0 vermeul    (502) staff       (20)        1 2022-06-21 15:20:20.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice.egg-info/dependency_links.txt
+-rw-r--r--   0 vermeul    (502) staff       (20)       91 2022-06-21 15:20:20.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice.egg-info/entry_points.txt
+-rw-r--r--   0 vermeul    (502) staff       (20)        1 2020-05-13 10:05:01.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice.egg-info/not-zip-safe
+-rw-r--r--   0 vermeul    (502) staff       (20)       43 2022-06-21 15:20:20.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice.egg-info/requires.txt
+-rw-r--r--   0 vermeul    (502) staff       (20)       20 2022-06-21 15:20:20.000000 ethz_iam_webservice-0.9.0/ethz_iam_webservice.egg-info/top_level.txt
+-rw-r--r--   0 vermeul    (502) staff       (20)       38 2022-06-21 15:20:20.563674 ethz_iam_webservice-0.9.0/setup.cfg
+-rw-r--r--   0 vermeul    (502) staff       (20)     1269 2022-06-21 15:20:07.000000 ethz_iam_webservice-0.9.0/setup.py
```

### Comparing `ethz_iam_webservice-0.8.0/PKG-INFO` & `ethz_iam_webservice-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethz_iam_webservice
-Version: 0.8.0
+Version: 0.9.0
 Summary: Manage users, groups and services of the ETH Identity and Access Management system (IAM)
 Home-page: https://gitlab.ethz.ch/vermeul/ethz-iam-webservice
 Author: Swen Vermeul |  ID SIS | ETH Zürich
 Author-email: swen@ethz.ch
 License: Apache Software License Version 2.0
 Description: # ETHZ IAM Webservice
```

### Comparing `ethz_iam_webservice-0.8.0/README.md` & `ethz_iam_webservice-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ethz_iam_webservice-0.8.0/ethz_iam_webservice/ethz_iam.py` & `ethz_iam_webservice-0.9.0/ethz_iam_webservice/ethz_iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,14 +297,16 @@
         respAdminRole=None,
         description=None,
         guestTechnicalContact=None,
         notification=None,
         hostOrg=None,
         startDate=None,
         endDate=None,
+        deactivationStartDate=None,
+        deactivationEndDate=None,
     ):
         body = {"username": username}
         if host:
             body["host"] = host
         if respAdminRole:
             body["respAdminRole"] = respAdminRole
         if description:
@@ -316,14 +318,22 @@
             body["notification"] = notification
         if hostOrg:
             body["hostOrg"] = hostOrg
         if startDate:
             body["startDate"] = startDate
         if endDate:
             body["endDate"] = endDate
+        if startDate:
+            body["startDate"] = startDate
+        if deactivationEndDate is not None:
+            body["deactivationEndDate"] = deactivationEndDate
+        if endDate:
+            body["endDate"] = endDate
+        if deactivationStartDate is not None:
+            body["deactivationStartDate"] = deactivationStartDate
 
         guest = Guest(conn=self, data=body, is_new=False)
         guest.save()
         return guest
 
     def new_guest(
         self,
```

### Comparing `ethz_iam_webservice-0.8.0/ethz_iam_webservice/group.py` & `ethz_iam_webservice-0.9.0/ethz_iam_webservice/group.py`

 * *Files identical despite different names*

### Comparing `ethz_iam_webservice-0.8.0/ethz_iam_webservice/mailinglist.py` & `ethz_iam_webservice-0.9.0/ethz_iam_webservice/mailinglist.py`

 * *Files identical despite different names*

### Comparing `ethz_iam_webservice-0.8.0/ethz_iam_webservice/main.py` & `ethz_iam_webservice-0.9.0/ethz_iam_webservice/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -332,47 +332,62 @@
 )
 @click.option(
     "-s", "--startDate", help="Start date of guest (YYYY-DD-MM). Default: today"
 )
 @click.option(
     "-e", "--endDate", help="End date of guest (YYYY-MM-DD). Default: today+1 year"
 )
+@click.option(
+    "--deactivationStartDate",
+    help='Deactivation start date of guest (YYYY-DD-MM). Set it to "" to remove',
+)
+@click.option(
+    "--deactivationEndDate",
+    help='Deactivation end date of guest (YYYY-MM-DD). Set it to "" to remove',
+)
 @guest.command("update", help="update an existing guest")
 @click.argument("username")
 @click.pass_context
 def update_guest(
     ctx,
     description,
     hostorg,
     host,
     technicalcontact,
     admingroup,
     notification,
     startdate,
     enddate,
     username,
+    deactivationstartdate,
+    deactivationenddate,
 ):
-
     if startdate:
         startdate = to_date(startdate)
     if enddate:
         enddate = to_date(enddate)
+    if deactivationstartdate:
+        deactivationstartdate = to_date(deactivationstartdate)
+    if deactivationenddate:
+        deactivationenddate = to_date(deactivationenddate)
 
     iam = ctx.obj["iam"]
     try:
         guest = iam.update_guest(
             username=username,
             host=host,
             respAdminRole=admingroup,
             description=description,
             guestTechnicalContact=technicalcontact,
             notification=notification,
             hostOrg=hostorg,
             startDate=startdate,
             endDate=enddate,
+            deactivationStartDate=deactivationstartdate,
+            deactivationEndDate=deactivationenddate,
         )
         print(json.dumps(guest._data_formatted(), indent=4, sort_keys=True))
     except Exception as exc:
         raise click.ClickException(exc)
 
 
 @guest.command("new", help="create a new guest")
```

### Comparing `ethz_iam_webservice-0.8.0/ethz_iam_webservice/person.py` & `ethz_iam_webservice-0.9.0/ethz_iam_webservice/person.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,14 +178,15 @@
 
 class Guest:
     def __init__(self, conn, data=None, is_new=False):
         self.date_fields = [
             "startDate",
             "endDate",
             "deactivationStartDate",
+            "deactivationEndDate",
             "dateOfBirth",
         ]
         self.conn = conn
         self.is_new = is_new
         if data:
             self._set_data(data)
 
@@ -197,15 +198,16 @@
         self.data = data
 
     def _server_body(self):
         """Transform data to be send to the server"""
         body = copy.deepcopy(self.data)
         for date_field in self.date_fields:
             if date_field in body:
-                body[date_field] = body[date_field].strftime("%d.%m.%Y")
+                if body[date_field]:
+                    body[date_field] = body[date_field].strftime("%d.%m.%Y")
         return body
 
     def _data_formatted(self):
         body = copy.deepcopy(self.data)
         for date_field in self.date_fields:
             if date_field in body:
                 body[date_field] = body[date_field].strftime("%Y-%m-%d")
```

### Comparing `ethz_iam_webservice-0.8.0/ethz_iam_webservice/service.py` & `ethz_iam_webservice-0.9.0/ethz_iam_webservice/service.py`

 * *Files identical despite different names*

### Comparing `ethz_iam_webservice-0.8.0/ethz_iam_webservice/user.py` & `ethz_iam_webservice-0.9.0/ethz_iam_webservice/user.py`

 * *Files identical despite different names*

### Comparing `ethz_iam_webservice-0.8.0/ethz_iam_webservice/utils.py` & `ethz_iam_webservice-0.9.0/ethz_iam_webservice/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,16 @@
 
 
 def to_date(date, astz="CET"):
     """Converts a given date format into a datetime object
     and adjusts the timezone to local timezone.
     Assumes 1.5.2021 is actually May 1st 2021.
     """
+    if date == "":
+        return ""
     local_tz = tz.tzlocal()
     date_formats = [
         r"^(?P<dd>\d{1,2})\.(?P<mm>\d{1,2})\.(?P<yyyy>\d{4})",
         r"^(?P<yyyy>\d{4})\-(?P<mm>\d{1,2})\-(?P<dd>\d{1,2})",
     ]
     date = str(date)
     for i, date_format in enumerate(date_formats):
```

### Comparing `ethz_iam_webservice-0.8.0/ethz_iam_webservice.egg-info/PKG-INFO` & `ethz_iam_webservice-0.9.0/ethz_iam_webservice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethz-iam-webservice
-Version: 0.8.0
+Version: 0.9.0
 Summary: Manage users, groups and services of the ETH Identity and Access Management system (IAM)
 Home-page: https://gitlab.ethz.ch/vermeul/ethz-iam-webservice
 Author: Swen Vermeul |  ID SIS | ETH Zürich
 Author-email: swen@ethz.ch
 License: Apache Software License Version 2.0
 Description: # ETHZ IAM Webservice
```

### Comparing `ethz_iam_webservice-0.8.0/ethz_iam_webservice.egg-info/SOURCES.txt` & `ethz_iam_webservice-0.9.0/ethz_iam_webservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethz_iam_webservice-0.8.0/setup.py` & `ethz_iam_webservice-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="ethz_iam_webservice",
-    version="0.8.0",
+    version="0.9.0",
     author="Swen Vermeul |  ID SIS | ETH Zürich",
     author_email="swen@ethz.ch",
     description="Manage users, groups and services of the ETH Identity and Access Management system (IAM)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.ethz.ch/vermeul/ethz-iam-webservice",
     packages=find_packages(),
```

