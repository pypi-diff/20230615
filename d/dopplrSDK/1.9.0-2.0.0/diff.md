# Comparing `tmp/dopplrSDK-1.9.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3788 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     4924 b- defN 23-Jun-12 13:28 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-12 13:30 dopplrSDK-1.9.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      457 b- defN 23-Jun-12 13:30 dopplrSDK-1.9.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 13:30 dopplrSDK-1.9.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-12 13:30 dopplrSDK-1.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      477 b- defN 23-Jun-12 13:30 dopplrSDK-1.9.0.dist-info/RECORD
-6 files, 7037 bytes uncompressed, 2922 bytes compressed:  58.5%
+Zip file size: 4392 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     6805 b- defN 23-Jun-15 15:33 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-15 17:00 dopplrSDK-2.0.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      530 b- defN 23-Jun-15 17:00 dopplrSDK-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-15 17:00 dopplrSDK-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-15 17:00 dopplrSDK-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      477 b- defN 23-Jun-15 17:00 dopplrSDK-2.0.0.dist-info/RECORD
+6 files, 8991 bytes uncompressed, 3526 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-1.9.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-2.0.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-1.9.0.dist-info/METADATA
+Filename: dopplrSDK-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-1.9.0.dist-info/WHEEL
+Filename: dopplrSDK-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-1.9.0.dist-info/top_level.txt
+Filename: dopplrSDK-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-1.9.0.dist-info/RECORD
+Filename: dopplrSDK-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -1,63 +1,110 @@
 import pandas as pd
 import psycopg2
 import sys
 import boto3
 import json
 import os
+import base64
+import hashlib
+from Crypto.Cipher import DES3
+from Crypto.Util.Padding import unpad
+from cryptography.fernet import Fernet
+from botocore.client import Config
+
+def decrypt_keys(de_key,s_key):
+    keys={}
+    key = s_key
+    key = hashlib.md5(key.encode("utf-8")).digest()
+    cipher_bytes = base64.b64decode(de_key)
+    cipher = DES3.new(key, DES3.MODE_ECB)
+    decrypted_bytes = cipher.decrypt(cipher_bytes)
+    decrypted_text = unpad(decrypted_bytes, DES3.block_size).decode("utf-8")
+    data=decrypted_text.split('|')
+    
+    for i in data:
+        a=i.split(':')
+        keys[a[0]]=a[1]
+    s3 = boto3.client('s3', aws_access_key_id=keys['Access'], aws_secret_access_key=keys['Secret'])
+    ContainerName = keys['Bucket']
+    file_key = 'Connections/Dopplr_Connection.ini'
+    db = {}
+    response = s3.get_object(Bucket=ContainerName, Key=file_key)
+    file_content = response['Body'].read()
+    key=s_key.encode('utf-8')
+    key=key
+    fernet = Fernet(key)
+    decrypted_data = fernet.decrypt(file_content)
+    decrypted_data = decrypted_data.decode('utf-8')
+    lines = decrypted_data.split('\n')
+    index=lines.index('[postgresql]\r')
+    data=lines[index+1:index+6]
+
+    for i in data:
+        a=i.split('=')
+        db[a[0]]=a[1].replace('\r','')
+    return keys,db,s3
 
-
-
-def putFileTomywrkspace(filePath,file_type,loginName):
+def putFileTomywrkspace(filePath,file_type,loginName,s_key):
     try:
+        keys,db,s3=decrypt_keys("zvkPurRjZz0ptGnEIxMq0tu3062oChYVkuUwkk7RG7pigQttPVQFkoHBQp+hb5dcYuGeb8asmxKv9XkaI9EnTTTT3YT4UvOF9cT46kotQRceh4oRzPwwKSWFUswJmtBBb2NNlUBFBae6qZqoozBn5g==",s_key)
+        
         query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
         #print(query)
-        cnxn = psycopg2.connect(host='adb63cdf19ef14e14b3e7ffd2c4bd4e3-1623479541.ap-south-1.elb.amazonaws.com',database='Dopplr',user='postgres',password='SystechIndia@123',port='5432')
-
+        ContainerName = keys['Bucket']
+        cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
+    
         cur=cnxn.cursor()
         cur.execute(query)
         results = cur.fetchone()
         
 
-        ContainerName=results[2]
-        AwsAccessKey=results[3]
-        AwsSecretKey=results[4]
+        #ContainerName=results[2]
+        #AwsAccessKey=results[3]
+        #AwsSecretKey=results[4]
         UserKey=results[1]
         OrgName=results[0]
         
-        s3 = boto3.client('s3', aws_access_key_id=AwsAccessKey, aws_secret_access_key=AwsSecretKey)
+        
 
         cur=cnxn.cursor()
         file_name = os.path.basename(filePath)
-        insert_query = "INSERT INTO doppler.\"DopplerLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplerConnectionDetailsKey\",\"Projectid\",\"Status\") VALUES ("+str(UserKey)+",'"+file_name+"','"+file_type+"',null,'','Uploaded')"
-
-        cur.execute(insert_query)
-
-
-        cnxn.commit()
+        file_name=file_name.replace('.csv','')
+        query="select count(\"TableName\") from doppler.\"DopplerLake\" where \"Source\"='MLStudio' and \"TableName\"="+"'"+file_name+"'"
+        cur.execute(query)
+        results = cur.fetchone()
+        if results[0]<1:
+            insert_query = "INSERT INTO doppler.\"DopplerLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplerConnectionDetailsKey\",\"Projectid\",\"Status\") VALUES ("+str(UserKey)+",'"+file_name+"','"+file_type+"',null,'','Uploaded')"
+            cur.execute(insert_query)
+            cnxn.commit()
+        else:
+            pass
+            
         
         cur1=cnxn.cursor()
         insert_query1 = "SELECT max(\"SourceKey\") as \"SourceKey\" FROM doppler.\"DopplerLake\" where \"UserKey\"="+str(UserKey)+" and \"TableName\"='"+file_name+"'"
         
         cur1.execute(insert_query1)
         results = cur1.fetchone()
         SourceKey=results[0]
         SourceKey=str(SourceKey)
 
 
-        ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/SOURCE/'+file_name)
+        ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/SOURCE/'+file_name+'.csv')
 
         update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+str(OrgName)+"/"+str(loginName).upper()+'/'+(str(SourceKey).lstrip()+'/SOURCE/'+file_name+".csv',\"Source\"= 'MLStudio' ,\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey))
         cur2=cnxn.cursor()
         #print("update_query ",update_query)
         cur2.execute(update_query)
         cnxn.commit()
-
+        if '.csv' in filePath:
+            filePath=filePath
+        else:
+            filePath=filePath+'.csv'
         s3.upload_file(filePath, ContainerName, ConnectionString)
-
          # Generate a pre-signed URL
         
         s3.put_object_acl(ACL='public-read',
                           Bucket=ContainerName,
                           Key=ConnectionString)
         #url = f"https://{ContainerName}.s3.ap-south-1.amazonaws.com/{ConnectionString}"
         url = f"s3://{ContainerName}/{ConnectionString}"
@@ -69,37 +116,39 @@
             dopplrsource= 'File does not exists'
             print("Error : ", dopplrsource)
             sys.exit()
         else:
             print("Error : ",error)
 
 
-def getWorkspaceFile(fileName,destination,loginName):
+def getWorkspaceFile(fileName,destination,loginName,s_key):
     #type = 1 then get file (Actual file) 
     #type = 2 then get file* (file pattern)
 
 
-    #destination = "/data"
-    folder_prefix = 'Systech/'+loginName.upper()+'/'
-    query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
+    keys,db,s3=decrypt_keys("zvkPurRjZz0ptGnEIxMq0tu3062oChYVkuUwkk7RG7pigQttPVQFkoHBQp+hb5dcYuGeb8asmxKv9XkaI9EnTTTT3YT4UvOF9cT46kotQRceh4oRzPwwKSWFUswJmtBBb2NNlUBFBae6qZqoozBn5g==",s_key)
 
-    cnxn = psycopg2.connect(host='adb63cdf19ef14e14b3e7ffd2c4bd4e3-1623479541.ap-south-1.elb.amazonaws.com',database='Dopplr',user='postgres',password='SystechIndia@123',port='5432')
+    
+    query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
+    ContainerName = keys['Bucket']
+    cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
 
     cur=cnxn.cursor()
     cur.execute(query)
     results = cur.fetchone()
         
 
-    ContainerName=results[2]
-    AwsAccessKey=results[3]
-    AwsSecretKey=results[4]
+    #ContainerName=results[2]
+    #AwsAccessKey=results[3]
+    #AwsSecretKey=results[4]
     UserKey=results[1]
     OrgName=results[0]
+    folder_prefix = OrgName+'/'+loginName.upper()+'/'
         
-    s3 = boto3.client('s3', aws_access_key_id=AwsAccessKey, aws_secret_access_key=AwsSecretKey)
+    #s3 = boto3.client('s3', aws_access_key_id=AwsAccessKey, aws_secret_access_key=AwsSecretKey)
 
     # Check if the file exists
     if os.path.exists(destination):
         print('folder exists')
     else:
         os.mkdir(destination)
 
@@ -110,17 +159,16 @@
         key = obj['Key']
         #print(key,fileName)
             
         is_same = is_file_name_same(key, fileName)
 
         if(is_same):                
             s3.download_file(ContainerName, key, destination)
+            print("download")
 
 def is_file_name_same(file_path, expected_file_name):
         file_name = os.path.basename(file_path)
         return file_name == expected_file_name
 
 
-#putFileTomywrkspace("C:\\Users\\JakeerAhamedShaik\\Downloads\\Forecasting.csv",'csv',"Anand")
 
-#getWorkspaceFile("Transaction","C:\\Users\\AnandThirurangaruban\\Documents\\dopplrSDK","Anand")
```

## Comparing `dopplrSDK-1.9.0.dist-info/LICENSE.txt` & `dopplrSDK-2.0.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

