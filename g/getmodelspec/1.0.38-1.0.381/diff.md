# Comparing `tmp/getmodelspec-1.0.38.tar.gz` & `tmp/getmodelspec-1.0.381.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.38.tar", last modified: Thu Jun 15 12:23:49 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.381.tar", last modified: Thu Jun 15 12:40:05 2023, max compression
```

## Comparing `getmodelspec-1.0.38.tar` & `getmodelspec-1.0.381.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/
--rw-rw-rw-   0        0        0      350 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/PKG-INFO
--rw-rw-rw-   0        0        0     3785 2023-06-13 15:33:43.000000 getmodelspec-1.0.38/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec/
--rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.38/getmodelspec/__init__.py
--rw-rw-rw-   0        0        0      778 2023-06-13 15:30:10.000000 getmodelspec-1.0.38/getmodelspec/lineup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.38/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-06-15 12:13:47.000000 getmodelspec-1.0.38/getmodelspec/src/panasonic.py
--rw-rw-rw-   0        0        0    23224 2023-06-15 12:23:00.000000 getmodelspec-1.0.38/getmodelspec/src/sony.py
--rw-rw-rw-   0        0        0    28198 2023-06-15 10:52:57.000000 getmodelspec-1.0.38/getmodelspec/src/teast1.py
--rw-rw-rw-   0        0        0     6946 2023-06-14 13:04:06.000000 getmodelspec-1.0.38/getmodelspec/src/test.py
--rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.38/getmodelspec/src/tv_score.py
--rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.38/getmodelspec/src/tv_spepcifications.py
--rw-rw-rw-   0        0        0    10912 2023-06-14 15:15:03.000000 getmodelspec-1.0.38/getmodelspec/test4.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.38/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     2810 2023-06-14 15:20:39.000000 getmodelspec-1.0.38/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.38/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      350 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      605 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/setup.cfg
--rw-rw-rw-   0        0        0      810 2023-06-15 12:23:17.000000 getmodelspec-1.0.38/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/
+-rw-rw-rw-   0        0        0      351 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-06-13 15:33:43.000000 getmodelspec-1.0.381/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/getmodelspec/
+-rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.381/getmodelspec/__init__.py
+-rw-rw-rw-   0        0        0      778 2023-06-13 15:30:10.000000 getmodelspec-1.0.381/getmodelspec/lineup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.381/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-06-15 12:13:47.000000 getmodelspec-1.0.381/getmodelspec/src/panasonic.py
+-rw-rw-rw-   0        0        0    23881 2023-06-15 12:35:00.000000 getmodelspec-1.0.381/getmodelspec/src/sony.py
+-rw-rw-rw-   0        0        0    28198 2023-06-15 10:52:57.000000 getmodelspec-1.0.381/getmodelspec/src/teast1.py
+-rw-rw-rw-   0        0        0      647 2023-06-15 12:38:11.000000 getmodelspec-1.0.381/getmodelspec/src/test.py
+-rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.381/getmodelspec/src/tv_score.py
+-rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.381/getmodelspec/src/tv_spepcifications.py
+-rw-rw-rw-   0        0        0    10912 2023-06-14 15:15:03.000000 getmodelspec-1.0.381/getmodelspec/test4.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.381/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     2810 2023-06-14 15:20:39.000000 getmodelspec-1.0.381/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     5044 2023-06-15 12:25:15.000000 getmodelspec-1.0.381/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      605 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 12:40:05.000000 getmodelspec-1.0.381/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-15 12:40:03.000000 getmodelspec-1.0.381/setup.py
```

### Comparing `getmodelspec-1.0.38/README.md` & `getmodelspec-1.0.381/README.md`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.38/getmodelspec/lineup.py` & `getmodelspec-1.0.381/getmodelspec/lineup.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.38/getmodelspec/src/panasonic.py` & `getmodelspec-1.0.381/getmodelspec/src/panasonic.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.38/getmodelspec/src/sony.py` & `getmodelspec-1.0.381/getmodelspec/src/sony.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import pandas as pd
 from bs4 import BeautifulSoup
 from datetime import date
 import requests
 from tqdm import tqdm
 import traceback
 from collections import OrderedDict
 
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.action_chains import ActionChains
 
+
 from getmodelspec.src.tv_spepcifications import Specifications
 from getmodelspec.src.tv_score import Score
 from getmodelspec.tools.functions import *
 from getmodelspec.tools.webdriver import WebDriver
 
 
 
@@ -280,41 +282,46 @@
             print("parser err", e)
             h4_tag = soup.find('h4').text.strip()
             p_tag =  ""
             pass
         return {h4_tag: p_tag}
 
 class GetSONYjp:
-    def __init__(self, toExcel=True):
+    def __init__(self, toExcel=True , translateToEn=False):
         self.waitTime = 10
         self.toExcel = toExcel
+        self.translateToEn = translateToEn
         pass
 
     def getModels(self, toExcel:bool = True) -> dict:
         self.toExcel=toExcel
         # 메인 페이지에서 시리즈를 추출
         setUrlSeries = self.__getSpecSeries__()
-        print(setUrlSeries)
+        # print(setUrlSeries)
         # ==========================================================================
         # backUp(setUrlSeries, "setUrlSeries")
         # with open(f"setUrlSeries.pickle", "rb") as file:
         #     setUrlSeries = pickle.load(file)
         # ==========================================================================
 
-        ## 웹페이지의 모든 모델 url을 추출
+        # 웹페이지의 모든 모델 url을 추출
         dictModels = {}
         for model, url in tqdm(setUrlSeries.items()):
             print(model,":", url)
             modelspec = self.__getSpec__(url=url)
             dictModels.update(modelspec)
-            # backUp(dictModels, "dictModels_b")
         print("Number of all Series:", len(dictModels))
-        print(dictModels)
+        # print(dictModels)
         backUp(dictModels, "dictModels")
-    # ======export====================================================================
+
+        # with open(f"dictModels.pickle", "rb") as file:
+        #     dictModels = pickle.load(file)
+        if self.translateToEn == True:
+            dictModels = self.__translateDict__(dictModels)
+        # ======export====================================================================
         if self.toExcel == True:
             fileName = f"sonyJp_LineUp_{date.today().strftime('%Y-%m-%d')}"
             dictToexcel(dictModels, fileName=fileName,sheetName="Jp")  # 엑셀 파일로 저장
 
         return dictModels
 
 
@@ -413,15 +420,15 @@
                             #     dictNote[bullet] = " @" + text
                             # 한 step씩 스크롤 내리기
                             wd.execute_script(f"window.scrollBy(0, {step});")
                             time.sleep(1)  # 스크롤이 내려가는 동안 대기
                             scrollDistance += step
                         wd.quit()
                     except Exception as e:
-                        print("An error occurred:", e)
+                        # print("An error occurred:", e)
                         # 웹페이지가 동적이 아닌 경우
                         wd.quit()
 
                 # ## 풋노트 끌어오기
                 # for kNote in dictNote.keys():
                 #     for k, v in dictSpec.items():
                 #         if kNote in k:
@@ -430,16 +437,16 @@
                 #             dictSpec[k] = v.replace(kNote, dictNote.get(kNote))
                 dictSpec['url'] = url
                 dictSpec = self.__splitModels__(dictSpec)
                 for k in dictSpec.keys(): dictSpec[k].update(self.__extractInfo__(k))
 
                 return dictSpec
             except Exception as e:
-                print(f"An error occurred: {str(e)}")
-                print(f"{tryCnt}/{TotalCnt} try to get spec")
+                #print(f"An error occurred: {str(e)}")
+                print(f"{tryCnt+1}/{TotalCnt} try to get spec from {url}")
                 pass
 
     def __splitModels__(self, dictModels):
         dictNewModels = {}
         dictModelsSplited = dictModels.get('型')
         if isinstance(dictModelsSplited, dict):
             for model in dictModelsSplited.keys():
@@ -456,14 +463,26 @@
             model = url.split("/products/")[1].split("/")[0]
             dictNewModels[model] = dictModels
         else:
             # Handle other cases if needed
             pass
         return dictNewModels
 
+    def __translateDict__(self, dictData):
+        dictNewData = {}
+        for k, v in dictData.items():
+            k = translate_text(k, target_lang='en')
+            if isinstance(v, dict):
+                v = self.__translateDict__(v)
+            else:
+                v = translate_text(v, target_lang='en')
+            dictNewData[k] = v
+        return dictNewData
+
+
     # def __splitModels__(self, dictModels):
     #     dictNewModels = {}
     #     dictNewModel = {}
     #
     #     dictModelsSplited = dictModels.get('型')
     #     if isinstance(dictModelsSplited, dict):
     #         for model in dictModelsSplited.keys():
@@ -516,8 +535,8 @@
         }
 
         # 알파벳과 대응하는 연도가 없을 경우 기본값으로 설정할 연도를 지정
         try:
             dictInfo["year"] = year_mapping.get(dictInfo.get("year"))
         except:
             dictInfo["year"] = ""
-        return dictInfo
+        return dictInfo
```

### Comparing `getmodelspec-1.0.38/getmodelspec/src/teast1.py` & `getmodelspec-1.0.381/getmodelspec/src/teast1.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.38/getmodelspec/src/tv_score.py` & `getmodelspec-1.0.381/getmodelspec/src/tv_score.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.38/getmodelspec/src/tv_spepcifications.py` & `getmodelspec-1.0.381/getmodelspec/src/tv_spepcifications.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.38/getmodelspec/test4.py` & `getmodelspec-1.0.381/getmodelspec/test4.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.38/getmodelspec/tools/functions.py` & `getmodelspec-1.0.381/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.38/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.381/getmodelspec/tools/webdriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         설명:
             헤드리스 모드로 실행되는 Chrome 웹 드라이버 객체를 반환합니다.
         반환값:
             - driver (WebDriver): Chrome 웹 드라이버 객체
         """
         user_agent = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.50 Safari/537.36'
         chrome_options = webdriver.ChromeOptions()
-        chrome_options.add_argument('--headless')  # 헤드리스 모드로 실행
-        chrome_options.add_argument('--no-sandbox')  # 헤드리스 크롬 브라우저를 "사용자 네임스페이스" 옵션 없이 실행하도록 설정
-        chrome_options.add_argument('--disable-dev-shm-usage')  # 헤드리스
+        # chrome_options.add_argument('--headless')  # 헤드리스 모드로 실행
+        # chrome_options.add_argument('--no-sandbox')  # 헤드리스 크롬 브라우저를 "사용자 네임스페이스" 옵션 없이 실행하도록 설정
+        # chrome_options.add_argument('--disable-dev-shm-usage')  # 헤드리스
         chrome_options.add_argument('user-agent={0}'.format(user_agent))  # 에이전트 우회
         # chrome_options.add_argument('lang=ko_kr')  # 브라우저 언어
         service = ChromeService(executable_path='chromedriver')
         driver = webdriver.Chrome(service=service , options=chrome_options)
         return driver
 
     @staticmethod
```

### Comparing `getmodelspec-1.0.38/getmodelspec.egg-info/SOURCES.txt` & `getmodelspec-1.0.381/getmodelspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.38/setup.py` & `getmodelspec-1.0.381/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='getmodelspec',
-    version='1.0.38',
+    version='1.0.381',
     author='xikest',
     description='get model spec,',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy',
         'pandas',
```

