# Comparing `tmp/pythttp-0.1.5.tar.gz` & `tmp/pythttp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.1.5.tar", last modified: Fri Jun  9 15:53:29 2023, max compression
+gzip compressed data, was "pythttp-0.1.6.tar", last modified: Thu Jun 15 14:36:10 2023, max compression
```

## Comparing `pythttp-0.1.5.tar` & `pythttp-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:53:29.769920 pythttp-0.1.5/
--rw-rw-rw-   0        0        0     1093 2023-06-09 15:53:29.769920 pythttp-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.5/README.md
--rw-rw-rw-   0        0        0      419 2023-06-09 15:53:10.000000 pythttp-0.1.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-09 15:53:29.757591 pythttp-0.1.5/pythttp/
--rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.5/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     3528 2023-06-06 02:08:51.000000 pythttp-0.1.5/pythttp/Protocol.py
--rw-rw-rw-   0        0        0    12667 2023-06-09 15:52:34.000000 pythttp-0.1.5/pythttp/RequestHandler.py
--rw-rw-rw-   0        0        0     3896 2023-06-06 02:09:28.000000 pythttp-0.1.5/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.5/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.5/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:53:29.767919 pythttp-0.1.5/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-06-09 15:53:29.000000 pythttp-0.1.5/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-06-09 15:53:29.000000 pythttp-0.1.5/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:53:29.000000 pythttp-0.1.5/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-09 15:53:29.000000 pythttp-0.1.5/pythttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 15:53:29.000000 pythttp-0.1.5/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 15:53:29.769920 pythttp-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      634 2023-06-09 15:53:14.000000 pythttp-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:36:10.855509 pythttp-0.1.6/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 14:36:10.854509 pythttp-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.6/README.md
+-rw-rw-rw-   0        0        0      419 2023-06-15 14:33:11.000000 pythttp-0.1.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-15 14:36:10.845324 pythttp-0.1.6/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.6/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     3516 2023-06-14 16:04:13.000000 pythttp-0.1.6/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0    16734 2023-06-15 14:22:39.000000 pythttp-0.1.6/pythttp/RequestHandler.py
+-rw-rw-rw-   0        0        0     3906 2023-06-10 14:25:28.000000 pythttp-0.1.6/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.6/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.6/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:36:10.853509 pythttp-0.1.6/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 14:36:10.000000 pythttp-0.1.6/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-15 14:36:10.000000 pythttp-0.1.6/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 14:36:10.000000 pythttp-0.1.6/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-15 14:36:10.000000 pythttp-0.1.6/pythttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 14:36:10.000000 pythttp-0.1.6/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 14:36:10.855509 pythttp-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      634 2023-06-15 14:33:09.000000 pythttp-0.1.6/setup.py
```

### Comparing `pythttp-0.1.5/PKG-INFO` & `pythttp-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.5
+Version: 0.1.6
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.5/README.md` & `pythttp-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.5/pythttp/Log_Manager.py` & `pythttp-0.1.6/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.5/pythttp/Protocol.py` & `pythttp-0.1.6/pythttp/Protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,17 +23,17 @@
             return self.Receive()
         except ConnectionRefusedError as e:
             print(f'Request to server failed... Reason: {e}')
         finally:
             self.s.close()
 
     def BindAddress(self, address='0.0.0.0', port=80):
-        external_ip = request.urlopen('https://ident.me').read().decode('utf8')  
+        #external_ip = request.urlopen('https://ident.me').read().decode('utf8')  
         self.s.bind((address, port))
-        self.log(f"[ Server started on ] ==> ip/port : \033[94m{external_ip}:{port}\033[0m")
+        self.log(f"[ Server started on ] ==> ip/port : \033[94m:{port}\033[0m")
 
     def listen(self, limit=0):
         self.s.listen(limit)
 
     def AcceptConnection(self):
         self.c, self.addr = self.s.accept()
         self.log(msg=f"[ Connected with ] ==> ip : \033[32m{self.addr}\033[0m")
```

### Comparing `pythttp-0.1.5/pythttp/RequestHandler.py` & `pythttp-0.1.6/pythttp/RequestHandler.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from datetime import datetime, timedelta
 import secrets
 import pickle
 import base64
 import json
 import uuid
 import re
+import os
 
 
 class Handler:
     def __init__(self) -> None:
         self.http=HyperTextTransferProtocol()
         self.Thread=self.http.Thread
         self.ServerUsersDB=set([])
         self.Sessions = set([])
-        self.ServerDB={}
+        self.ServerPostDB=[]
         self.log=Log().logging
         self.HandleloadDB()
 
     def RunServer(self):
         self.http.BindAddress()
         self.http.listen()
         while True:
@@ -36,204 +37,276 @@
         Request=thread.result
         first_line = thread.result[0]
         if 'GET' in first_line:
             Response=self.HandleGETRequest(Request)
         elif 'POST' in first_line[0]:
             Response=self.HandlePOSTRequest(Request)
         else:
-            raise Exception('This communication is not HTTP protocol')
+            Response=self.ErrorHandler('405 Method Not Allowed',first_line)
         self.http.SendResponse(Response, socket_and_address)
         self.Thread.find_stopped_thread()
         self.Thread.ThreadDestructor(thread_name, client_address)
 
     def HandleGETRequest(self, Request):
         result = parse.unquote(Request[0]).split(' ')[1].replace('\\','/')
         try:
             Response = self.HandleTextFileRequest()
-            if '?print=' in result:
-                Response = self.HandleTextFileRequest(msg=result.split('=')[1])
-            elif '.png' in result:
-                Response= self.HandleFileRequest(f'{result}')
+            if ('.png' in result or '.html' in result or '.css' in result):
+                Response= self.HandleFileRequest(result)
             elif '.ico' in result:
-                Response=self.HandleFileRequest(result)
-            elif '/upload_form' == result:
-                Response= self.HandleTextFileRequest('/upload_form.html')
+                Response= self.HandleFileRequest(f'/icon/{result}')
+            elif '/Feed_Page' == result:
+                Response= self.UpdateFeedPage()
             elif not self.verifySessionCookie(Request)[0]:
-                if '/SignUp_form' == result:
-                    Response= self.HandleTextFileRequest('/SignUp_form.html')
-                elif '/Login_form' == result:
-                    Response= self.HandleTextFileRequest('/Login_form.html')
-            elif (self.verifySessionCookie(Request)[0] and '/Logout_form' == result):
-                Response= self.HandleTextFileRequest('/Logout_form.html')
-            elif '.html' in result:
-                Response=self.HandleTextFileRequest(result)
+                if ('/SignUp_form' == result or '/Login_form' == result):
+                    Response= self.HandleTextFileRequest(f'{result}.html')
+            elif (self.verifySessionCookie(Request)[0]):
+                if '/Logout_form' == result:
+                    Response= self.HandleTextFileRequest(f'{result}.html')
+                elif '/Account_Info' == result:
+                    Response= self.HandleAccountFileRequest(Request)
             return Response
         except FileNotFoundError:
             with open('resource/Error_Form.html','r',encoding='UTF-8') as arg:
                 return self.ErrorHandler('404 Not Found',f'The corresponding resource{result}file could not be found.')
 
     def HandlePOSTRequest(self,Request):
-        JsonData=parse.unquote(Request[1])
+        JsonData=parse.unquote(Request[1].decode())
         DictPostData=json.loads(JsonData)
         Form=DictPostData['Form']
         Response=self.HandleTextFileRequest()
-        is_valid_cookie,cookie_value=self.verifySessionCookie(Request[0])
-        try:
-            if Form == 'SignUp':
-                Response=self.SignUp_Handler(DictPostData['UserID'],DictPostData['UserName'],DictPostData['UserPw'],is_valid_cookie)
-            elif Form == 'Login':
-                Response=self.Login_Handler(DictPostData['UserID'],DictPostData['UserPw'],is_valid_cookie)
-            elif Form == 'Logout':
-                Response=self.Logout_Handler(cookie_value)
-        except Exception as e:
-            Response=self.ErrorHandler('400 Bad Request',e)
+        is_valid_cookie,cookie_value,session=self.verifySessionCookie(Request[0])
+        # try:
+        if Form == 'SignUp':
+            Response=self.SignUp_Handler(DictPostData['UserID'],DictPostData['UserEmail'],DictPostData['UserName'],DictPostData['UserPw'],is_valid_cookie)
+        elif Form == 'Login':
+            Response=self.Login_Handler(DictPostData['UserID'],DictPostData['UserPw'],is_valid_cookie)
+        elif Form == 'Logout':
+            Response=self.Logout_Handler(cookie_value)
+        elif Form == 'Account':
+            Response=self.UpdateAccount_Handler(DictPostData,session)
+        elif Form == 'Upload_Post':
+            Response=self.UploadPost_Handler(DictPostData,session)
+        # except Exception as e:
+        #     Response=self.ErrorHandler('500 Internal Server Error',e)
         return Response
 
     def verifySessionCookie(self,RequestData:list):
         for data in RequestData:
             if ('Cookie' in data and 'SessionID=' in data):
                 Values = data.split('SessionID=')[1]
                 for Session in self.Sessions:
                     if Values==Session.SessionToken:
-                        return True, Values
-        return False, None
+                        return True, Values ,Session
+        return False, None, None
 
-    def HandleFileRequest(self,img_file='/a.png'):
-        with open(f'resource{img_file}', 'rb') as ImgFile:
+    def HandleFileRequest(self,file='/a.png'):
+        with open(f'resource{file}', 'rb') as ImgFile:
             Response_file=ImgFile.read()
             return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
         
     def HandleTextFileRequest(self,flie='/Index.html',Cookie=None):
         with open(f'resource{flie}','r',encoding='UTF-8') as TextFile:
             Response_file=TextFile.read().encode('UTF-8')
         return PrepareHeader()._response_headers('200 OK',Response_file,Cookie) + Response_file
     
     def ErrorHandler(self,Error_code,Error_msg):
         with open(f'resource/Error_Form.html','r',encoding='UTF-8') as TextFile:
             Response_file=TextFile.read()
-            Response_file=Response_file.replace('{0}',Error_code).replace('{1}',Error_msg).encode('utf-8')
-        self.log(f"[ Handle Error ] ==> Code : \033[91m{Error_code}\033[0m")
-        return PrepareHeader()._response_headers('200',Response_file) + Response_file
+            Response_file=Response_file.format(Error_code,Error_msg).encode('utf-8')
+        self.log(f"[ Handle Error ] ==> Code : \033[35m{Error_code}\033[0m")
+        return PrepareHeader()._response_headers(Error_code,Response_file) + Response_file
     
     def addFormatToHTML(self,HtmlText : str, FormatData : dict, style : str):
         Format=''
         for key,val in FormatData.items():
             Format+=f'{style.format(val=val,key=key)}'
         HtmlText=HtmlText.format(Format=Format)
         return HtmlText
     
     def ImgFileUpload(self,img_file,file_name):
         with open(f'resource/ImgFileUpload/{file_name}', 'wb') as ImgFile:
             ImgFile.write(img_file)
             self.ServerDB['Img']={file_name:f'/ImgFileUpload/{file_name}'}
             return file_name
 
-    def SignUp_Handler(self,UserID,UserName,UserPw,is_valid_cookie):
+    def SignUp_Handler(self,UserID,UserEmail,UserName,UserPw,is_valid_cookie):
         UserUID=uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), UserID)
         if self.Sessions and is_valid_cookie:
             return self.ErrorHandler('403 Forbidden','Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
         for DB in self.ServerUsersDB:
             if (UserUID == DB.UserUID):
                 return self.ErrorHandler('406 Not Acceptable',f'User information error! Duplicate ID! : {UserID}')  
         try:
             AuthenticatedName,AuthenticatedPassword=Verify().VerifyCredentials(UserName, UserPw)
         except Exception as e:
             return self.ErrorHandler('403 Forbidden',f'{e} : {UserName,UserPw}')
-        DB=StructDB(UserUID,AuthenticatedName,AuthenticatedPassword)
+        DB=StructDB(UserUID,AuthenticatedName,AuthenticatedPassword,UserEmail)
         self.ServerUsersDB.add(DB)
-        self.log(f"[ New DataBase Constructed ] ==> DBID : \033[95m{DB.DataBaseID}\033[0m")
+        self.log(f"[ New DataBase Constructed ] ==> DBID : \033[36m{DB.DataBaseID}\033[0m")
         self.log(f"[ SignUp User ] ==> UUID : \033[96m{UserUID}\033[0m")
         self.HandleSaveDB()
         return self.HandleTextFileRequest('/SignUp_Action.html')
 
-    def Login_Handler(self, user_id, user_pw ,is_valid_cookie):
-        user_uid = uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), user_id)
+    def Login_Handler(self, UserID, UserPw, is_valid_cookie):
+        UserUID = uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), UserID)
         # Check if user is already logged in
         if self.Sessions and is_valid_cookie:
             return self.ErrorHandler('403 Forbidden','Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
         # Check user credentials and create new session
         for db in self.ServerUsersDB:
-            if user_uid == db.UserUID and user_pw == db.UserPw:
-                session_id = self.RegisterUserSession(7, {'UserUID': user_uid})
+            if (UserUID == db.UserUID and UserPw == db.UserPw):
+                session_id = self.RegisterUserSession(7, {'UserUID': UserUID, 'DataBaseID':db.DataBaseID, 'UserName':db.UserName})
                 self.log(f"[ New Session Constructed ] ==> SessionID: \033[96m{session_id}\033[0m")
                 return self.HandleTextFileRequest('/Login_Action.html',Cookie=f'SessionID = {session_id}')       
-        return self.ErrorHandler('422 Unprocessable Entity',f'User ID or password does not exist: {user_id, user_pw}')
-
+        return self.ErrorHandler('422 Unprocessable Entity',f'User ID or password does not exist: {UserID, UserPw}')
     
     def Logout_Handler(self,SessionID):
         for Session in self.Sessions:
             if Session.SessionToken == SessionID:
                 self.Sessions.remove(Session)
                 self.log(f"[ Session Destructed ] ==> SessionID : \033[96m{SessionID}\033[0m")
                 return self.HandleTextFileRequest('/Logout_Action.html')
         return self.ErrorHandler('403 Forbidden',f'To log out, you must first log in. Please verify your account information and log in before attempting to log out')
+    
+    def HandleAccountFileRequest(self,Request):
+        DataBaseID=self.verifySessionCookie(Request)[2].UserInfo['DataBaseID']
+        for db in self.ServerUsersDB:
+            if DataBaseID == db.DataBaseID:
+                Username=db.UserName
+                UserUID=db.UserUID
+                Useremail=db.UserEmail
+        with open(f'resource/Account_Info.html','r',encoding='UTF-8') as TextFile:
+            Response_file=TextFile.read()
+            Response_file=Response_file.format(UserName=Username,UserUID=UserUID,UserEmail=Useremail,UserBirthDate='None').encode('utf-8')
+        return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
+    
+    def UpdateAccount_Handler(self,newUserInfo,session):
+        DataBaseID=session.UserInfo['DataBaseID']
+        for DataBase in self.ServerUsersDB:
+            if DataBaseID == DataBase.DataBaseID:
+                DataBase.UserName=newUserInfo['UserName']
+                DataBase.UserEmail=newUserInfo['UserEmail']
+                if DataBase.UserPw!=newUserInfo['UserPw']:
+                    DataBase.UserPw=newUserInfo['UserPw']
+                    self.Logout_Handler(session.SessionToken)   
+            self.HandleSaveDB()
+            return self.HandleTextFileRequest('/Account_Action.html')
+        
+    def UploadPost_Handler(self,PostData,Session):
+        if Session == None:
+            return self.ErrorHandler('403 Forbidden','Warning! You are attempting to post without logging in. If you wish to make a post, please proceed with the login.')
+        PostImageName=''
+        User=Session.UserInfo['UserUID']
+        UploadTime=datetime.now().strftime('%Y-%m-%d_%H%M')
+        try:
+            os.mkdir(f'resource/PostFileUpload/{User}')
+        except:
+            pass
+        PostFileName=f'resource/PostFileUpload/{User}/_{UploadTime}.html'.replace(':','-')
+        title=PostData['title']
+        content=PostData['content']
+        name=Session.UserInfo['UserName']
+        if 'image' in PostData.keys():
+            OriginalData=base64.b64decode(PostData['image'].split(',')[1])
+            PostImageName=f'_{UploadTime}.png'
+            with open(f'resource/PostFileUpload/{User}/{PostImageName}','wb') as ImageFile:
+                ImageFile.write(OriginalData)
+        with open(f'resource/Post_Form.html','r',encoding='UTF-8') as PostFormFile:
+            with open(PostFileName,'w',encoding='UTF-8') as PostTempFile:
+                PostTempFile.write(PostFormFile.read().format(PostTitle=title,PostContent=content,UserName=name,PostImage=PostImageName))
+                self.ServerPostDB.append({str(User):{'Path':f'/_{UploadTime}.html','title':title,'content':content,'name':name}})
+        return self.UpdateFeedPage()
+
+    def UpdateFeedPage(self):
+        FeedPost=''
+        FeedPostForm="""
+        <a href="{Path}">
+        <li>
+          <div class="user-profile">
+            <img src="" alt="{name}">
+          </div>
+          <div class="post-content">
+              <h2>{title}</h2>
+              <p>{content}</p>
+          </div>
+        </li>
+        </a>\n"""
+        with open(f'resource/Feed_Page.html','r+',encoding='UTF-8') as FeedFormFile:
+            FeedForm = FeedFormFile.read()
+        if self.ServerPostDB:
+            for i in self.ServerPostDB:
+                for ID,Post in i.items():
+                    PostFilePath=f'/PostFileUpload/{ID}'+Post['Path'].replace(':','-')
+                    FeedPost+=FeedPostForm.format(Path=PostFilePath,name=Post['name'],title=Post['title'],content=Post['content'])
+        FeedForm = FeedForm.replace('{FeedPost}',FeedPost).encode('UTF-8')
+        with open(f'resource/PostStorage.html','a',encoding='UTF-8') as PostStorage:
+            PostStorage.write(FeedPost)
+        return PrepareHeader()._response_headers('200 OK',FeedForm) + FeedForm
+        
 
     def RegisterUserSession(self,  SessionValidityDays: str, UserInfo: dict):
         SessionInfo = Session(SessionValidityDays, UserInfo)
         self.Sessions.add(SessionInfo)
         return SessionInfo.SessionToken
 
     def HandleSaveDB(self):
         with open(f'resource/ServerUserDB.DB','wb') as DBfile:
             pickle.dump(self.ServerUsersDB,DBfile)
-            self.log(f"[ Database Save Successful ] ==> path : \033[95mresource/ServerUserDB.DB\033[0m")
+            self.log(f"[ Database Save Successful ] ==> path : \033[34mresource/ServerUserDB.DB\033[0m")
 
     def HandleloadDB(self):
         try:
             with open(f'resource/ServerUserDB.DB','rb') as DBfile:
                 self.ServerUsersDB=pickle.load(DBfile)
-                self.log(f"[ Database Load Successful ] ==> path : \033[95mresource/ServerUserDB.DB\033[0m")
+                self.log(f"[ Database Load Successful ] ==> path : \033[34mresource/ServerUserDB.DB\033[0m")
         except FileNotFoundError:
             pass
 
 @dataclass
 class Session:
     """
     Session class represents a data model for storing session information.
-
     Attributes:
         SessionToken (str): The token of the session. It is initialized as a 16-character random value.
         SessionValidity (float): The validity timestamp of the session.
         SessionValidityDays (int): The number of days the session is valid for.
         UserInfo (dict): Additional information about the session's user.
         SessionDict (dict): The dictionary representation of the session information.
-
     Methods:
         __post_init__(): Initializes the SessionToken, SessionValidity, and SessionDict attributes after object creation.
     """
     SessionToken: str = field(init=False, default=None)
     SessionValidity: float = field(init=False, default=None)
     SessionValidityDays: int
     UserInfo: dict = field(default_factory=dict)
-    SessionDict: dict = field(init=False, default_factory=dict)
+    #SessionDict: dict = field(init=False, default_factory=dict)
 
     def __post_init__(self):
         """
         Initializes the SessionToken, SessionValidity, and SessionDict attributes after object creation.
         """
         self.SessionToken = SessionID(16).Token
         self.SessionValidity = (datetime.now() + timedelta(days=self.SessionValidityDays)).timestamp()
-        self.SessionDict['SessionID'] = self.SessionToken
-        self.SessionDict['SessionValidity'] = self.SessionValidity
-        self.SessionDict['UserInfo'] = self.UserInfo
+        # self.SessionDict['SessionID'] = self.SessionToken
+        # self.SessionDict['SessionValidity'] = self.SessionValidity
+        # self.SessionDict['UserInfo'] = self.UserInfo
 
     def __hash__(self):
         return hash(self.SessionToken)
 
 @dataclass
 class SessionID:
     """
     Data class representing a session identifier.
-
     python
     Copy code
     Attributes:
     length (int): The length of the session identifier.
     Token (str): The session token (automatically generated).
-
     """
     length: int
     Token: str = field(init=False, default=None)
 
     def __post_init__(self):
         """
         Method executed after initialization.
@@ -265,9 +338,8 @@
             return True
         return False
 
     def _NameDuplicateCheck(self):
         if len(self.ServerDB) != 0:
             for item in self.ServerDB.items():
                 return item['user_ID']==self.verified_UserID
-        else: return False
-
+        else: return False
```

### Comparing `pythttp-0.1.5/pythttp/Structure.py` & `pythttp-0.1.6/pythttp/Structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     UserName: str
     UserPw: str
     UserEmail: str = None
     UserUploadFiles: dict =field(default_factory=dict)
     StructDBdict: dict =field(init=False,default_factory=dict)
     def __post_init__(self):
         self.DataBaseID = DataBaseID(16).Token
-        self.StructDBdict['UserUID'] = self.UserUID
-        self.StructDBdict['UserName'] = self.UserName
-        self.StructDBdict['UserPw'] = self.UserPw
-        self.StructDBdict['UserEmail'] = self.UserEmail
-        self.StructDBdict['UserUploadFiles'] = self.UserUploadFiles
+        # self.StructDBdict['UserUID'] = self.UserUID
+        # self.StructDBdict['UserName'] = self.UserName
+        # self.StructDBdict['UserPw'] = self.UserPw
+        # self.StructDBdict['UserEmail'] = self.UserEmail
+        # self.StructDBdict['UserUploadFiles'] = self.UserUploadFiles
 
     def __hash__(self):
         return hash(self.DataBaseID)
 
 @dataclass
 class DataBaseID:
     """
```

### Comparing `pythttp-0.1.5/pythttp/Thread_Manager.py` & `pythttp-0.1.6/pythttp/Thread_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.5/pythttp.egg-info/PKG-INFO` & `pythttp-0.1.6/pythttp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.5
+Version: 0.1.6
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.5/setup.py` & `pythttp-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.1.5",
+    version="0.1.6",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=['dataclasses','datetime','uuid'],
```

