# Comparing `tmp/getmodelspec-1.0.379.tar.gz` & `tmp/getmodelspec-1.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.379.tar", last modified: Thu Jun 15 11:55:32 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.38.tar", last modified: Thu Jun 15 12:23:49 2023, max compression
```

## Comparing `getmodelspec-1.0.379.tar` & `getmodelspec-1.0.38.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/
--rw-rw-rw-   0        0        0      351 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/PKG-INFO
--rw-rw-rw-   0        0        0     3785 2023-06-13 15:33:43.000000 getmodelspec-1.0.379/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/getmodelspec/
--rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.379/getmodelspec/__init__.py
--rw-rw-rw-   0        0        0      778 2023-06-13 15:30:10.000000 getmodelspec-1.0.379/getmodelspec/lineup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.379/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0    10994 2023-06-15 11:49:30.000000 getmodelspec-1.0.379/getmodelspec/src/panasonic.py
--rw-rw-rw-   0        0        0    23881 2023-06-15 11:54:53.000000 getmodelspec-1.0.379/getmodelspec/src/sony.py
--rw-rw-rw-   0        0        0    28198 2023-06-15 10:52:57.000000 getmodelspec-1.0.379/getmodelspec/src/teast1.py
--rw-rw-rw-   0        0        0     6946 2023-06-14 13:04:06.000000 getmodelspec-1.0.379/getmodelspec/src/test.py
--rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.379/getmodelspec/src/tv_score.py
--rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.379/getmodelspec/src/tv_spepcifications.py
--rw-rw-rw-   0        0        0    10912 2023-06-14 15:15:03.000000 getmodelspec-1.0.379/getmodelspec/test4.py
-drwxrwxrwx   0        0        0        0 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.379/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     2810 2023-06-14 15:20:39.000000 getmodelspec-1.0.379/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.379/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      351 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      605 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 11:55:32.000000 getmodelspec-1.0.379/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-15 11:55:30.000000 getmodelspec-1.0.379/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/
+-rw-rw-rw-   0        0        0      350 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-06-13 15:33:43.000000 getmodelspec-1.0.38/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec/
+-rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.38/getmodelspec/__init__.py
+-rw-rw-rw-   0        0        0      778 2023-06-13 15:30:10.000000 getmodelspec-1.0.38/getmodelspec/lineup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.38/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-06-15 12:13:47.000000 getmodelspec-1.0.38/getmodelspec/src/panasonic.py
+-rw-rw-rw-   0        0        0    23224 2023-06-15 12:23:00.000000 getmodelspec-1.0.38/getmodelspec/src/sony.py
+-rw-rw-rw-   0        0        0    28198 2023-06-15 10:52:57.000000 getmodelspec-1.0.38/getmodelspec/src/teast1.py
+-rw-rw-rw-   0        0        0     6946 2023-06-14 13:04:06.000000 getmodelspec-1.0.38/getmodelspec/src/test.py
+-rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.38/getmodelspec/src/tv_score.py
+-rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.38/getmodelspec/src/tv_spepcifications.py
+-rw-rw-rw-   0        0        0    10912 2023-06-14 15:15:03.000000 getmodelspec-1.0.38/getmodelspec/test4.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.38/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     2810 2023-06-14 15:20:39.000000 getmodelspec-1.0.38/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.38/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      350 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      605 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 12:23:49.000000 getmodelspec-1.0.38/setup.cfg
+-rw-rw-rw-   0        0        0      810 2023-06-15 12:23:17.000000 getmodelspec-1.0.38/setup.py
```

### Comparing `getmodelspec-1.0.379/README.md` & `getmodelspec-1.0.38/README.md`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.379/getmodelspec/lineup.py` & `getmodelspec-1.0.38/getmodelspec/lineup.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.379/getmodelspec/src/panasonic.py` & `getmodelspec-1.0.38/getmodelspec/src/panasonic.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,39 +17,37 @@
         self.maker= "pana"
         self.dir_3rd = f"{self.maker}/log/models"
         pass
 
     def getModels(self, toExcel:bool = True) -> dict:
         self.toExcel=toExcel
         # 메인 페이지에서 시리즈를 추출
-        # setUrlSeries = self.__getSpecSeries__()
-        # print(setUrlSeries)
+        setUrlSeries = self.__getSpecSeries__()
+        print(setUrlSeries)
         # # ==========================================================================
         # # backUp(setUrlSeries, "setUrlSeries")
-        with open(f"setUrlSeries.pickle", "rb") as file:
-            setUrlSeries = pickle.load(file)
+        # with open(f"setUrlSeries.pickle", "rb") as file:
+        #     setUrlSeries = pickle.load(file)
         # ==========================================================================
 
         ## 웹페이지의 모든 모델 url을 추출
         dictModels = OrderedDict()
         for model, url in tqdm(setUrlSeries.items()):
             print(model,":", url)
             modelspec = self.__getSpecGlobal__(url=url)
-            dictModels[model]=modelspec
+            dictModels[model] = modelspec
 
-            print(dictModels.keys())
-            print({model:modelspec})
+            # print({model:modelspec})
             # print(dictModels)
             # backUp(dictModels, "dictModels_b")
         print("Number of all Series:", len(dictModels))
         # print(dictModels)
-        backUp(dictModels, "dictModels")
-
-        with open(f"dictModels.pickle", "rb") as file:
-            dictModels = pickle.load(file)
+        # backUp(dictModels, "dictModels")
+        # with open(f"dictModels.pickle", "rb") as file:
+        #     dictModels = pickle.load(file)
     # ======export====================================================================
         if self.toExcel == True:
             fileName = f"{self.maker}Jp_LineUp_{date.today().strftime('%Y-%m-%d')}"
             dictToexcel(dictModels, fileName=fileName,sheetName="Jp")  # 엑셀 파일로 저장
 
         return dictModels
 
@@ -89,17 +87,16 @@
             title = item.find('div', class_='common-productbox-product__title')
 
             if link and title:
                 link_url = link['href']
                 title_text = title.text.strip()
                 results[title_text] = prefix + link_url
         return results
-
     def __getSpecGlobal__(self, url: str) -> dict:
-        print("get", url)
+        # print("get", url)
         cntTryTotal = 20
         for cntTry in range(cntTryTotal):
             try:
                 dictSpec = {}
                 wd = WebDriver.getChrome()
                 wd.get(url=url)
                 model = getNamefromURL(url)
@@ -173,15 +170,15 @@
                     try:
                         sibling_lv2_element = sibling.find('ul', class_='speclist__item')
                         hierarchy[sibling_key] = self.__extractHierarchy__(sibling_lv2_element, classNames=classNames,
                                                                            cnt=cnt)
                     except:
                         sibling_data_element = sibling.find('div', class_='speclist__item__data')
                         hierarchy[sibling_key] = sibling_data_element.get_text(strip=True)
-        print(hierarchy)
+        # print(hierarchy)
         return hierarchy
 
                 #
                 # except Exception as e:
                 #     hierarchy[key] = sibling.get_text(strip=True)
                 #     print(hierarchy[key])
```

### Comparing `getmodelspec-1.0.379/getmodelspec/src/sony.py` & `getmodelspec-1.0.38/getmodelspec/src/sony.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import pandas as pd
 from bs4 import BeautifulSoup
 from datetime import date
 import requests
 from tqdm import tqdm
 import traceback
 from collections import OrderedDict
 
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.action_chains import ActionChains
 
-
 from getmodelspec.src.tv_spepcifications import Specifications
 from getmodelspec.src.tv_score import Score
 from getmodelspec.tools.functions import *
 from getmodelspec.tools.webdriver import WebDriver
 
 
 
@@ -282,46 +280,41 @@
             print("parser err", e)
             h4_tag = soup.find('h4').text.strip()
             p_tag =  ""
             pass
         return {h4_tag: p_tag}
 
 class GetSONYjp:
-    def __init__(self, toExcel=True , translateToEn=False):
+    def __init__(self, toExcel=True):
         self.waitTime = 10
         self.toExcel = toExcel
-        self.translateToEn = translateToEn
         pass
 
     def getModels(self, toExcel:bool = True) -> dict:
         self.toExcel=toExcel
         # 메인 페이지에서 시리즈를 추출
         setUrlSeries = self.__getSpecSeries__()
-        # print(setUrlSeries)
+        print(setUrlSeries)
         # ==========================================================================
         # backUp(setUrlSeries, "setUrlSeries")
         # with open(f"setUrlSeries.pickle", "rb") as file:
         #     setUrlSeries = pickle.load(file)
         # ==========================================================================
 
-        # 웹페이지의 모든 모델 url을 추출
+        ## 웹페이지의 모든 모델 url을 추출
         dictModels = {}
         for model, url in tqdm(setUrlSeries.items()):
             print(model,":", url)
             modelspec = self.__getSpec__(url=url)
             dictModels.update(modelspec)
+            # backUp(dictModels, "dictModels_b")
         print("Number of all Series:", len(dictModels))
-        # print(dictModels)
+        print(dictModels)
         backUp(dictModels, "dictModels")
-
-        # with open(f"dictModels.pickle", "rb") as file:
-        #     dictModels = pickle.load(file)
-        if self.translateToEn == True:
-            dictModels = self.__translateDict__(dictModels)
-        # ======export====================================================================
+    # ======export====================================================================
         if self.toExcel == True:
             fileName = f"sonyJp_LineUp_{date.today().strftime('%Y-%m-%d')}"
             dictToexcel(dictModels, fileName=fileName,sheetName="Jp")  # 엑셀 파일로 저장
 
         return dictModels
 
 
@@ -420,15 +413,15 @@
                             #     dictNote[bullet] = " @" + text
                             # 한 step씩 스크롤 내리기
                             wd.execute_script(f"window.scrollBy(0, {step});")
                             time.sleep(1)  # 스크롤이 내려가는 동안 대기
                             scrollDistance += step
                         wd.quit()
                     except Exception as e:
-                        # print("An error occurred:", e)
+                        print("An error occurred:", e)
                         # 웹페이지가 동적이 아닌 경우
                         wd.quit()
 
                 # ## 풋노트 끌어오기
                 # for kNote in dictNote.keys():
                 #     for k, v in dictSpec.items():
                 #         if kNote in k:
@@ -437,16 +430,16 @@
                 #             dictSpec[k] = v.replace(kNote, dictNote.get(kNote))
                 dictSpec['url'] = url
                 dictSpec = self.__splitModels__(dictSpec)
                 for k in dictSpec.keys(): dictSpec[k].update(self.__extractInfo__(k))
 
                 return dictSpec
             except Exception as e:
-                #print(f"An error occurred: {str(e)}")
-                print(f"{tryCnt+1}/{TotalCnt} try to get spec from {url}")
+                print(f"An error occurred: {str(e)}")
+                print(f"{tryCnt}/{TotalCnt} try to get spec")
                 pass
 
     def __splitModels__(self, dictModels):
         dictNewModels = {}
         dictModelsSplited = dictModels.get('型')
         if isinstance(dictModelsSplited, dict):
             for model in dictModelsSplited.keys():
@@ -463,26 +456,14 @@
             model = url.split("/products/")[1].split("/")[0]
             dictNewModels[model] = dictModels
         else:
             # Handle other cases if needed
             pass
         return dictNewModels
 
-    def __translateDict__(self, dictData):
-        dictNewData = {}
-        for k, v in dictData.items():
-            k = translate_text(k, target_lang='en')
-            if isinstance(v, dict):
-                v = self.__translateDict__(v)
-            else:
-                v = translate_text(v, target_lang='en')
-            dictNewData[k] = v
-        return dictNewData
-
-
     # def __splitModels__(self, dictModels):
     #     dictNewModels = {}
     #     dictNewModel = {}
     #
     #     dictModelsSplited = dictModels.get('型')
     #     if isinstance(dictModelsSplited, dict):
     #         for model in dictModelsSplited.keys():
@@ -535,8 +516,8 @@
         }
 
         # 알파벳과 대응하는 연도가 없을 경우 기본값으로 설정할 연도를 지정
         try:
             dictInfo["year"] = year_mapping.get(dictInfo.get("year"))
         except:
             dictInfo["year"] = ""
-        return dictInfo
+        return dictInfo
```

### Comparing `getmodelspec-1.0.379/getmodelspec/src/teast1.py` & `getmodelspec-1.0.38/getmodelspec/src/teast1.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.379/getmodelspec/src/test.py` & `getmodelspec-1.0.38/getmodelspec/src/test.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.379/getmodelspec/src/tv_score.py` & `getmodelspec-1.0.38/getmodelspec/src/tv_score.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.379/getmodelspec/src/tv_spepcifications.py` & `getmodelspec-1.0.38/getmodelspec/src/tv_spepcifications.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.379/getmodelspec/test4.py` & `getmodelspec-1.0.38/getmodelspec/test4.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.379/getmodelspec/tools/functions.py` & `getmodelspec-1.0.38/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.379/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.38/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.379/getmodelspec.egg-info/SOURCES.txt` & `getmodelspec-1.0.38/getmodelspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.379/setup.py` & `getmodelspec-1.0.38/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='getmodelspec',
-    version='1.0.379',
+    version='1.0.38',
     author='xikest',
     description='get model spec,',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy',
         'pandas',
```

