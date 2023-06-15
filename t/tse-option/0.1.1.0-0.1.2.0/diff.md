# Comparing `tmp/tse_option-0.1.1.0.tar.gz` & `tmp/tse_option-0.1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tse_option-0.1.1.0.tar", last modified: Fri Jan 27 13:15:34 2023, max compression
+gzip compressed data, was "tse_option-0.1.2.0.tar", last modified: Thu Jun 15 08:50:13 2023, max compression
```

## Comparing `tse_option-0.1.1.0.tar` & `tse_option-0.1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 13:15:34.384445 tse_option-0.1.1.0/
--rw-rw-rw-   0        0        0     1097 2022-11-14 08:41:45.000000 tse_option-0.1.1.0/LICENSE
--rw-rw-rw-   0        0        0     4547 2023-01-27 13:15:34.385516 tse_option-0.1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3948 2023-01-27 13:12:22.000000 tse_option-0.1.1.0/README.md
--rw-rw-rw-   0        0        0      892 2023-01-27 13:12:26.000000 tse_option-0.1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-27 13:15:34.386519 tse_option-0.1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-27 13:15:34.276161 tse_option-0.1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-01-27 13:15:34.363060 tse_option-0.1.1.0/src/tse_option/
--rw-rw-rw-   0        0        0    17330 2023-01-27 13:12:51.000000 tse_option-0.1.1.0/src/tse_option/__init__.py
--rw-rw-rw-   0        0        0       72 2023-01-27 13:12:31.000000 tse_option-0.1.1.0/src/tse_option/example.py
-drwxrwxrwx   0        0        0        0 2023-01-27 13:15:34.383484 tse_option-0.1.1.0/src/tse_option.egg-info/
--rw-rw-rw-   0        0        0     4547 2023-01-27 13:15:34.000000 tse_option-0.1.1.0/src/tse_option.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-01-27 13:15:34.000000 tse_option-0.1.1.0/src/tse_option.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 13:15:34.000000 tse_option-0.1.1.0/src/tse_option.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-01-27 13:15:34.000000 tse_option-0.1.1.0/src/tse_option.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-27 13:15:34.000000 tse_option-0.1.1.0/src/tse_option.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 08:50:13.439190 tse_option-0.1.2.0/
+-rw-rw-rw-   0        0        0     1097 2022-11-14 08:41:45.000000 tse_option-0.1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5742 2023-06-15 08:50:13.439190 tse_option-0.1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5143 2023-06-15 08:49:00.000000 tse_option-0.1.2.0/README.md
+-rw-rw-rw-   0        0        0      892 2023-06-15 08:12:07.000000 tse_option-0.1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 08:50:13.440187 tse_option-0.1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 08:50:13.312956 tse_option-0.1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 08:50:13.414357 tse_option-0.1.2.0/src/tse_option/
+-rw-rw-rw-   0        0        0    18168 2023-06-15 08:12:13.000000 tse_option-0.1.2.0/src/tse_option/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-01-27 13:12:31.000000 tse_option-0.1.2.0/src/tse_option/example.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:50:13.438231 tse_option-0.1.2.0/src/tse_option.egg-info/
+-rw-rw-rw-   0        0        0     5742 2023-06-15 08:50:13.000000 tse_option-0.1.2.0/src/tse_option.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-06-15 08:50:13.000000 tse_option-0.1.2.0/src/tse_option.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:50:13.000000 tse_option-0.1.2.0/src/tse_option.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-06-15 08:50:13.000000 tse_option-0.1.2.0/src/tse_option.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 08:50:13.000000 tse_option-0.1.2.0/src/tse_option.egg-info/top_level.txt
```

### Comparing `tse_option-0.1.1.0/LICENSE` & `tse_option-0.1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tse_option-0.1.1.0/PKG-INFO` & `tse_option-0.1.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: tse_option
-Version: 0.1.1.0
-Summary: Option pricing in Tehran Stock Exchange (TSE) and Iran Farabourse (IFB)
-Author-email: Seyed Mohammad Sokout <sm.sokut@gmail.com>
-Project-URL: Homepage, https://github.com/sm-sokout/tse-option
-Keywords: Tehran Stock Exchange,TSE,Iran Farabourse,IFB,Option pricing,BSM
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # tse_option
 
 
 
 این پکیج جهت بررسی و قیمت گذاری اوراق اختیار معامله موجود در بورس اوراق بهادار تهران و فرابورس ایران ایجاد شده است. لازم به یادآوری است که در این ماژول از مدل ارائه شده توسط بلک-شولز-مرتون در سال 1973 برای قیمت گذاری اختیار معامله استفاده شد است. سعی بر آن است که در نسخه های بعدی سایر مدل های قیمت گذاری نیز اضافه شوند.
 
 برخی از توابع این پروژه،از ماژول های [finpy_tse](https://github.com/ARahimiQuant/finpy-tse) و [tsemodule5](https://github.com/python4financeacademy/tsemodule5) اقتباس شده اند.
@@ -32,14 +17,24 @@
 
 
 1- امکان دانلود تاریخچه قیمت سهام و اوراق اختیار معامله
 
 
 2- رفع برخی مشکلات
 
+----------------------------------------------
+
+
+**تغییرات نسخه جدید(0.1.2.0)**: 
+
+
+1- بروزرسانی لینک های tsetmc
+
+
+2- امکان دریافت تاریخچه قیمت چندین نماد(مانند yfinance)
 
 ----------------------------------------------
 
 
 
 
 ### نصب
@@ -93,14 +88,40 @@
 
 
 **leverage:** نمایش مقدار اهرم اختیار معامله
 
 
 **P_BSM:** نمایش نسبت قیمت بازار به قیمت تئوری بلک-شولز-مرتون
 
+-----------------------------------------------------------------
+
+#### دریافت تاریخچه قیمت
+```python
+df = tso.download_history("خودرو", j_date=True, start="1402-01-01", end=None, adjust_price=True, drop_unadjusted=False)
+```
+```python
+df = tso.download_history(symbols=["خودرو","فولاد","وبملت"], j_date=False, start="2023-01-01", end=None, adjust_price=False, drop_unadjusted=False)
+```
+**symbols:** نماد یا نمادهای مورد نظر
+
+
+**j_date:**  نوع تاریخ ورودی
+
+
+**start:** تاریخ شروع (براساس j_date لازم است تعیین شود)
+
+
+**end:** تاریخ پایان (براساس j_date لازم است تعیین شود)
+
+
+**adjust_price:**  نمایش قیمت های تعدیل شده سهام
+
+
+**drop_unadjusted:** حذف ستون های قیمت های تعدیل نشده (حتما باید adjust_price برابر True باشد)
+
 
 -----------------------------------------------------------------
 
 
 برای مشاهده مثال های بیشتر [اینجا](https://github.com/sm-sokout/tse-option/blob/master/Example/Example.ipynb) کلیک کنید.
 
 -----------------------------------------------------------------
```

### Comparing `tse_option-0.1.1.0/pyproject.toml` & `tse_option-0.1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 
 [project]
 name = "tse_option"
-version = "0.1.1.0"
+version = "0.1.2.0"
 authors = [
   { name="Seyed Mohammad Sokout", email="sm.sokut@gmail.com" },
 ]
 description = "Option pricing in Tehran Stock Exchange (TSE) and Iran Farabourse (IFB)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tse_option-0.1.1.0/src/tse_option/__init__.py` & `tse_option-0.1.2.0/src/tse_option/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             
     return np.mean(ytm)
 
 #----------------------------------------
 
 def stock_id(stock_name):
     headers = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'}
-    url = f"http://www.tsetmc.com/tsev2/data/search.aspx?skey={stock_name}"
+    url = f"http://old.tsetmc.com/tsev2/data/search.aspx?skey={stock_name}"
     html = rq.get(url, headers=headers).text
     info = html.split(";")
     for i in info:
         if i.split(",")[0] == stock_name:
             return i.split(",")[2]
         else:
             try:
@@ -90,15 +90,15 @@
 
 #----------------------------------------
 
 def stock_price(stock_name):
     id = stock_id(stock_name)
     if id is None:
         raise NameError("This symbol does not exist. Please enter the symbol correctly!")
-    url = "http://www.tsetmc.com/tsev2/data/instinfofast.aspx?i="+id+"&c=34"
+    url = "http://old.tsetmc.com/tsev2/data/instinfofast.aspx?i="+id+"&c=34"
     tsetmc = rq.get(url)
     return int(tsetmc.text.split(";")[0].split(",")[2])
 
 #----------------------------------------
 
 def tse_options(symbol, stock=True):
     url = "https://tse.ir/json/MarketWatch/MarketWatch_7.xml"
@@ -128,67 +128,84 @@
     "قیمت.1": "حجم بهترین سفارش خرید","قیمت":"قیمت بهترین سفارش فروش",
     "تعداد موقعیت\u200cهای باز":"موقیعت های باز"})
     return data
 
 #----------------------------------------
 
 
-def download_history(symbol, j_date=False, start=None, end=None, adjust_price=False, drop_unadjusted=False):
+def download_history(symbols, j_date=False, start=None, end=None, adjust_price=False, drop_unadjusted=False):
     headers = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'}
-    if "ی" in symbol:
-        symbol = symbol.replace("ی","ي")
-    id = stock_id(symbol)
-    url = 'http://www.tsetmc.com/tsev2/data/Export-txt.aspx?t=i&a=1&b=0&i=' + id
-    html=rq.get(url,headers=headers).content
-    df=pd.read_csv(io.StringIO(html.decode("utf-8")),index_col="<DTYYYYMMDD>",parse_dates=True)[::-1]
-    df=df.rename(columns={"<OPEN>": "Yesterday", "<CLOSE>": "Close","<FIRST>":"Open","<HIGH>":"High","<LOW>":"Low","<VOL>":"Volume"})
-    df.index.rename('Date',inplace=True)
-    df = df[["Open","High","Low","Close","Volume","Yesterday"]]
-    df["Date"] = df.index
-    df["JDate"] = df["Date"].jalali.to_jalali()
+    if type(symbols) == str:
+        symbols = [symbols]
+    for symbol in symbols:
+        symbol = symbol.replace("ی","ي").replace('ک','ك')
+        id = stock_id(symbol)
+        url = 'http://old.tsetmc.com/tsev2/data/Export-txt.aspx?t=i&a=1&b=0&i=' + id
+        html=rq.get(url,headers=headers).content
+        df=pd.read_csv(io.StringIO(html.decode("utf-8")),index_col="<DTYYYYMMDD>",parse_dates=True)[::-1]
+        df=df.rename(columns={"<OPEN>": "Yesterday", "<CLOSE>": "Close","<FIRST>":"Open","<HIGH>":"High","<LOW>":"Low","<VOL>":"Volume"})
+        df.index.rename('Date',inplace=True)
+        df = df[["Open","High","Low","Close","Volume","Yesterday"]]
+        
+        def adjusting(df:pd.DataFrame)->pd.DataFrame:
+            df["temp"] = (df["Close"].shift(1) / df["Yesterday"]).fillna(1)
+            df["temp"] = (df["temp"].iloc[::-1].cumprod().iloc[::-1].shift(-1)).fillna(1)
+            df["Adj Open"] = (df["Open"] / df["temp"]).astype(int)
+            df["Adj High"] = (df["High"] / df["temp"]).astype(int)
+            df["Adj Low"] = (df["Low"] / df["temp"]).astype(int)
+            df["Adj Close"] = (df["Close"] / df["temp"]).astype(int)
+            df = df.drop(columns=["temp"])
+            return df
+        if adjust_price:
+            df = adjusting(df)
+            if drop_unadjusted:
+                df["Open"] = df["Adj Open"]
+                df["High"] = df["Adj High"]
+                df["Low"] = df["Adj Low"]
+                df["Close"] = df["Adj Close"]
+                df.drop(["Adj Open","Adj High","Adj Low","Adj Close"], axis=1, inplace=True)
+        df.drop(["Yesterday"], axis=1, inplace=True) 
+        if len(symbols) > 1:
+            for j in df.columns:
+                df = df.rename(columns={f'{j}': f'{symbol},{j}'})
+            try:
+                data = pd.concat([data, df],axis=1)
+            except:
+                data = df.copy()
+    if len(symbols) > 1:
+        data.columns = pd.MultiIndex.from_tuples([(x.split(",")[1], x.split(",")[0]) for x in data.columns])
+        data["Date","Date"] = data.index
+        data["JDate"] = data["Date","Date"].jalali.to_jalali()
+        data = data.reindex(data.columns.levels[0], level=0, axis=1)
+    else:
+        data = df.copy()
+        data["Date"] = data.index
+        data["JDate"] = data["Date"].jalali.to_jalali()
     if j_date:
         if start != None:
             start = jdatetime.date(int(start[:4]),int(start[5:7]),int(start[8:])).togregorian()
             start = str(start.year)+"-"+str(start.month) + "-" + str(start.day)
         if end != None:
             end = jdatetime.date(int(end[:4]),int(end[5:7]),int(end[8:])).togregorian()
             end = str(end.year)+"-"+str(end.month)+"-"+str(end.day)
     if start != None:
-        df = df[start:]
+        data = data[start:]
     if end != None:
-        df = df[:end]
-    def adjusting(df:pd.DataFrame)->pd.DataFrame:
-        df["temp"] = (df["Close"].shift(1) / df["Yesterday"]).fillna(1)
-        df["temp"] = (df["temp"].iloc[::-1].cumprod().iloc[::-1].shift(-1)).fillna(1)
-        df["Adj Open"] = (df["Open"] / df["temp"]).astype(int)
-        df["Adj High"] = (df["High"] / df["temp"]).astype(int)
-        df["Adj Low"] = (df["Low"] / df["temp"]).astype(int)
-        df["Adj Close"] = (df["Close"] / df["temp"]).astype(int)
-        df = df.drop(columns=["temp"])
-        return df
-    if adjust_price:
-        df = adjusting(df)
-        if drop_unadjusted:
-            df["Open"] = df["Adj Open"]
-            df["High"] = df["Adj High"]
-            df["Low"] = df["Adj Low"]
-            df["Close"] = df["Adj Close"]
-            df.drop(["Adj Open","Adj High","Adj Low","Adj Close"], axis=1, inplace=True)
-    df.drop(["Yesterday", "Date"], axis=1, inplace=True)
-    return df
+        data = data[:end]
+    data.drop(["Date"], axis=1, inplace=True)
+    return data
 
 #----------------------------------------
 
 
 def pricing_based_on_stock(stock_name:str, trading_days:int=100, IV=False, leverage=True, P_BSM=False, sort="Maturity"):
     """
     Valuation of all options on a particular stock
     """
-    if "ی" in stock_name:
-        stock_name = stock_name.replace("ی","ي")
+    stock_name = stock_name.replace("ی","ي").replace('ک','ك')
     last_price = stock_price(stock_name)
     df_stock = download_history(stock_name, start=None, end=None, adjust_price=True)[-trading_days:]
     df = df_stock[["Adj Close"]].copy()
     df["return"] = np.log(df["Adj Close"]/df["Adj Close"].shift())
     sigma = df["return"].std() * np.sqrt(240)
     rf = risk_free_interest_rate()
     data = tse_options(stock_name)
@@ -272,18 +289,17 @@
 
 #----------------------------------------
 
 def pricing_based_on_option(option_name:str, trading_days:int=100, IV=False, leverage=True, P_BSM=False):
     """
     Valuation of a particular option
     """
-    if "ی" in option_name:
-        option_name = option_name.replace("ی","ي")
+    option_name = option_name.replace("ی","ي").replace('ک','ك')
     headers = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'}
-    url = f"http://www.tsetmc.com/tsev2/data/search.aspx?skey={option_name}"
+    url = f"http://old.tsetmc.com/tsev2/data/search.aspx?skey={option_name}"
     html = rq.get(url, headers=headers).text
     if len(html.split(";")) == 2:
         stock_name = html.split(",")[1].split("-")[0].split(" ")[1]
         last_price = stock_price(stock_name)
         df_stock = download_history(stock_name, start=None, end=None, adjust_price=True)[-trading_days:]
         df = df_stock[["Adj Close"]].copy()
         df["return"] = np.log(df["Adj Close"]/df["Adj Close"].shift())
```

