# Comparing `tmp/pytrendseries-0.1.8.tar.gz` & `tmp/pytrendseries-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytrendseries-0.1.8.tar", last modified: Wed Jul 13 12:52:11 2022, max compression
+gzip compressed data, was "pytrendseries-0.1.9.tar", max compression
```

## Comparing `pytrendseries-0.1.8.tar` & `pytrendseries-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,8 @@
-drwxr-xr-x   0 Rafael     (501) staff       (20)        0 2022-07-13 12:52:11.576356 pytrendseries-0.1.8/
--rw-r--r--   0 Rafael     (501) staff       (20)     7926 2022-07-13 12:52:11.575222 pytrendseries-0.1.8/PKG-INFO
-drwxr-xr-x   0 Rafael     (501) staff       (20)        0 2022-07-13 12:52:11.567407 pytrendseries-0.1.8/pytrendseries/
--rwxrwxrwx   0 Rafael     (501) staff       (20)     8959 2022-07-13 11:26:52.000000 pytrendseries-0.1.8/pytrendseries/README.md
--rwxrwxrwx   0 Rafael     (501) staff       (20)     7816 2022-07-13 11:27:42.000000 pytrendseries-0.1.8/pytrendseries/README_pypi.md
--rwxrwxrwx   0 Rafael     (501) staff       (20)      190 2022-07-12 20:25:28.000000 pytrendseries-0.1.8/pytrendseries/__init__.py
--rwxrwxrwx   0 Rafael     (501) staff       (20)    13578 2022-07-12 17:47:16.000000 pytrendseries-0.1.8/pytrendseries/coverage.xml
--rwxrwxrwx   0 Rafael     (501) staff       (20)     7289 2022-07-12 17:41:58.000000 pytrendseries-0.1.8/pytrendseries/detecttrend.py
--rwxrwxrwx   0 Rafael     (501) staff       (20)     3757 2022-07-12 19:26:34.000000 pytrendseries-0.1.8/pytrendseries/example.py
--rwxrwxrwx   0 Rafael     (501) staff       (20)     4486 2022-07-12 17:33:28.000000 pytrendseries-0.1.8/pytrendseries/maxtrend.py
--rw-r--r--   0 Rafael     (501) staff       (20)     6843 2022-07-13 11:54:01.000000 pytrendseries-0.1.8/pytrendseries/poetry.lock
--rw-r--r--   0 Rafael     (501) staff       (20)      429 2022-07-13 11:48:31.000000 pytrendseries-0.1.8/pytrendseries/pyproject.toml
--rwxrwxrwx   0 Rafael     (501) staff       (20)     1304 2022-07-12 13:23:46.000000 pytrendseries-0.1.8/pytrendseries/setup.py
--rwxrwxrwx   0 Rafael     (501) staff       (20)     1842 2022-07-13 11:28:17.000000 pytrendseries-0.1.8/pytrendseries/time_under_water.py
--rwxrwxrwx   0 Rafael     (501) staff       (20)      108 2022-07-13 11:30:48.000000 pytrendseries-0.1.8/pytrendseries/version.py
--rwxrwxrwx   0 Rafael     (501) staff       (20)     4641 2022-07-12 16:09:32.000000 pytrendseries-0.1.8/pytrendseries/vizplot.py
-drwxr-xr-x   0 Rafael     (501) staff       (20)        0 2022-07-13 12:52:11.573743 pytrendseries-0.1.8/pytrendseries.egg-info/
--rw-r--r--   0 Rafael     (501) staff       (20)     7926 2022-07-13 12:52:11.000000 pytrendseries-0.1.8/pytrendseries.egg-info/PKG-INFO
--rw-r--r--   0 Rafael     (501) staff       (20)      540 2022-07-13 12:52:11.000000 pytrendseries-0.1.8/pytrendseries.egg-info/SOURCES.txt
--rw-r--r--   0 Rafael     (501) staff       (20)        1 2022-07-13 12:52:11.000000 pytrendseries-0.1.8/pytrendseries.egg-info/dependency_links.txt
--rw-r--r--   0 Rafael     (501) staff       (20)      109 2022-07-13 12:52:11.000000 pytrendseries-0.1.8/pytrendseries.egg-info/requires.txt
--rw-r--r--   0 Rafael     (501) staff       (20)       14 2022-07-13 12:52:11.000000 pytrendseries-0.1.8/pytrendseries.egg-info/top_level.txt
--rw-r--r--   0 Rafael     (501) staff       (20)       38 2022-07-13 12:52:11.576759 pytrendseries-0.1.8/setup.cfg
--rwxrwxrwx   0 Rafael     (501) staff       (20)     1304 2022-07-12 13:23:46.000000 pytrendseries-0.1.8/setup.py
+-rwxr-xr-x   0        0        0     8975 2023-06-14 23:11:25.290520 pytrendseries-0.1.9/README_pypi.md
+-rwxr-xr-x   0        0        0      460 2023-06-14 23:33:03.815920 pytrendseries-0.1.9/pyproject.toml
+-rwxr-xr-x   0        0        0      195 2023-06-14 23:44:42.348926 pytrendseries-0.1.9/src/pytrendseries/__init__.py
+-rwxr-xr-x   0        0        0     9534 2023-06-14 23:31:38.589092 pytrendseries-0.1.9/src/pytrendseries/detecttrend.py
+-rwxr-xr-x   0        0        0     1947 2023-06-14 23:31:26.839918 pytrendseries-0.1.9/src/pytrendseries/time_under_water.py
+-rwxr-xr-x   0        0        0      108 2023-06-14 23:08:16.830134 pytrendseries-0.1.9/src/pytrendseries/version.py
+-rwxr-xr-x   0        0        0     3284 2023-06-14 23:31:08.022954 pytrendseries-0.1.9/src/pytrendseries/vizplot.py
+-rw-r--r--   0        0        0     9449 1970-01-01 00:00:00.000000 pytrendseries-0.1.9/PKG-INFO
```

### Comparing `pytrendseries-0.1.8/PKG-INFO` & `pytrendseries-0.1.9/README_pypi.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,188 +1,228 @@
-Metadata-Version: 2.1
-Name: pytrendseries
-Version: 0.1.8
-Summary: Detect trend in time series.
-Home-page: UNKNOWN
-Author: Rafael Rodrigues
-Author-email: rafael.rafarod@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.8,<4.0
-Description-Content-Type: text/markdown
-
-<!-- buttons -->
-<p align="center">
-    <a href="https://www.python.org/">
-        <img src="https://img.shields.io/badge/python-v3-brightgreen.svg"
-            alt="python"></a> &nbsp;
-    <a href="https://opensource.org/licenses/MIT">
-        <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"
-            alt="MIT license"></a> &nbsp;
-      <a href="https://codecov.io/gh/rafa-rod/detecttrend">
-        <img src="https://codecov.io/gh/rafa-rod/detecttrend/branch/main/graph/badge.svg?token=98EMCTZTOY"/>
-      </a>
-</p>
-
-<!-- content -->
-
-**pytrendseries** is a Python library for detection of trends in time series like: stock prices, monthly sales, daily temperature of a city and so on.
-The input data must be a `pandas.DataFrame` format containing one column as observed data (in float or int format). Follow example below:
-
-```python
-import pandas as pd
-data = pd.read_csv("tests/resource/stock_prices.csv")
-filtered_data = data[['period','close']].set_index("period")
-filtered_data.columns = ['close_price']
-filtered_data.index = pd.to_datetime(filtered_data.index)
-filtered_data.index = filtered_data.sort_index()
-```
-
-Once some trend is identified, **pytrendseries** provides period on trend, drawdown, maximum drawdown (or buildup in case of uptrend) and a plot with all trends found.
-
-## Installation
-
-### Using pip
-
-You can install using the pip package manager by running:
-
-```sh
-pip install pytrendseries
-```
-
-Alternatively, you could install the latest version directly from Github:
-
-```sh
-pip install https://github.com/rafa-rod/pytrendseries/archive/refs/heads/main.zip
-```
-
-## Why pytrendseries is important?
-
-Detection of trends could be used in machine learning algorithms such as classification problems like binary (1 = uptrend, 0 = otherwise) or non-binary classifications (1 = uptrend, -1 = downtrend, 0 = otherwise). Besides that, could be used in prediction problems.
-
-## Example
-
-Inform:
- - type of trend you desire to investigate => downtrend or uptrend;
- - window or maximum period of a trend (example: 60 days considering 1 day as 1 period) **optional**;
- - the minimum value that represents the number of consecutive days (or anohter period of time) to be considered a trend (default 5 periods) **optional**;
- - instead of minimum period, you may inform the quantile of time span (consecutive days in trend) such as 0.8 (80%).
-
-```python
-import pytrendseries
-
-trend = "downtrend"
-window = 126 #6 months
-
-trends_detected, statistcs = pytrendseries.detecttrend(filtered_data, trend=trend, window=window)
-```
-
-The variable `trends_detected` is a dataframe that contains the initial and end date of each trend, the prices of each date, time span of each trend and the drawdown of each trend. Let's see the first five rows of this dataframe:
-
-```
-| from                | to                  |   price0 |   price1 |   indice_from |   indice_to |   time_span |   drawdown |
-|:--------------------|:--------------------|---------:|---------:|--------------:|------------:|------------:|-----------:|
-| 2000-01-03 00:00:00 | 2000-01-31 00:00:00 |  5.90057 |  5.12252 |             0 |          19 |          19 |  0.131859  |
-| 2000-03-09 00:00:00 | 2000-04-24 00:00:00 |  6.42701 |  5.02208 |            45 |          76 |          31 |  0.218597  |
-| 2000-05-02 00:00:00 | 2000-05-11 00:00:00 |  5.53684 |  5.29352 |            81 |          88 |           7 |  0.0439456 |
-| 2000-05-16 00:00:00 | 2000-05-24 00:00:00 |  5.59962 |  5.24807 |            91 |          97 |           6 |  0.0627803 |
-| 2000-06-08 00:00:00 | 2000-06-15 00:00:00 |  6.30359 |  6.1646  |           108 |         113 |           5 |  0.0220487 |
-```
-
-The output `statistcs` shows the basic statistics such as: minimum, maximum (must be equal to window variable) and other percentiles of all periods of trends.
-This is important if you want to filter all small and unnecessary trends detected such as: trend with only 2 consecutive days. By default, the limit variable cut off all trends with 5 periods found. 
-The statistcs exhibit all trend with no cut off at all.
-
-Let's see the `statistcs`:
-
-```
-|       |   time_span |
-|:------|------------:|
-| count |   2444      |
-| mean  |     12.5569 |
-| std   |     26.0989 |
-| min   |      1      |
-| 25%   |      1      |
-| 50%   |      2      |
-| 75%   |      8      |
-| 80%   |     12      |
-| 85%   |     18.55   |
-| 90%   |     33      |
-| 92.5% |     57.775  |
-| 95%   |     88      |
-| 97.5% |    110      |
-| 99%   |    122      |
-| max   |    126      |
-```
-
-As we just saw, the median (50% percentile) shows that 50% of trends is just 2 periods (2 days in this case), therefore the default limit of 5 it is a good cut number.
-Next, we will redefine the limit value with 21 periods.
-
-The easiest way to vizualize the trends detected, just call `plot_trend` function.
-All trends detected, with maximum window informed and the minimum informed by the limit value, will be displayed.
-
-```python
-import pytrendseries
-pytrendseries.vizplot.plot_trend(filtered_data, trends_detected, trend)
-```
-
-It is also possible to filter data by informing year variable. In this example, the series contains data after year 2005.
-
-```python
-year = 2005
-
-trends_detected, _ = pytrendseries.detecttrend(filtered_data, trend=trend, limit=21,
-                                      window=janela, year=year)
-
-#same:
-trends_detected, _ = pytrendseries.detecttrend(filtered_data, trend=trend, quantile=0.85,
-                                      window=janela, year=year)
-```
-
-The maximum drawdown or maximum run up is calculate calling the function `max_trend` which return: peak and valley values, data in which they occurred and the maxdrawdown/maxrunup value.
-
-```python
-import pytrendseries
-maxdd = pytrendseries.getmaxtrend(filtered_data, trend, year) 
-```
-
-```
-|   peak_price |   valley_price | peak_date_maxdrawdown   | valley_date_maxdrawdown   |   maxdrawdown | time_span          |
-|-------------:|---------------:|:------------------------|:--------------------------|--------------:|:-------------------|
-|        52.51 |            4.2 | 2008-05-21 00:00:00     | 2016-01-26 00:00:00       |      0.920015 | 2806 days 00:00:00 |
-```
-
-Instead, you may want to known the maximum drawdown (maximum run up) according to informed window. To do that, just code:
-
-```python
-maxdd_in_window = trends_detected.sort_values("drawdown",ascending=False).iloc[0:1]
-```
-
-To exhibit the maximium drawdown of the time series just call `plot_maxdrawdown` function and select the style of the plot: shadow, area or plotly.
-
-```python
-import pytrendseries
-pytrendseries.plot_maxdrawdown(filtered_data, maxdd, trend, year, style="shadow")
-pytrendseries.plot_maxdrawdown(filtered_data, maxdd, trend, year, style="area")
-pytrendseries.plot_maxdrawdown(filtered_data, maxdd, trend, year, style="plotly")
-```
-
-To get time under water (tuw), just type:
-
-```python
-import pytrendseries
-pytrendseries.tuw(filtered_data)
-```
-
-The output would be (showing the tail of the dataframe):
-
-```
-| inital_date|   peak    |   valley  |   drawdown  |   time underwater |   final_date |
-|:-----------|----------:|----------:|------------:|------------------:|-------------:|
-| 2007-12-28 |  44.66140 |  33.58194 |     0.24808 |                85 |   2008-05-06 |
-| 2008-05-06 |  45.00000 |  44.85000 |     0.00333 |                4  |   2008-05-09 |
-| 2008-05-13 |  46.95000 |  46.30000 |     0.01384 |                3  |   2008-05-15 |
-| 2008-05-21 |  52.51000 |  4.20000  |     0.92002 |               NaN |          NaN |
-```
-
-The table show time underwater as NaN, it means that the timeseries still on downtrend.
-
+<!-- buttons -->
+<p align="center">
+    <a href="https://www.python.org/">
+        <img src="https://img.shields.io/badge/python-v3-brightgreen.svg"
+            alt="python"></a> &nbsp;
+    <a href="https://opensource.org/licenses/MIT">
+        <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"
+            alt="MIT license"></a> &nbsp;
+      <a href="https://codecov.io/gh/rafa-rod/detecttrend">
+        <img src="https://codecov.io/gh/rafa-rod/detecttrend/branch/main/graph/badge.svg?token=98EMCTZTOY"/>
+      </a>
+</p>
+
+<!-- content -->
+
+**pytrendseries** is a Python library for detection of trends in time series like: stock prices, monthly sales, daily temperature of a city and so on.
+The input data must be a `pandas.DataFrame` format containing one column as observed data (in float or int format). Follow example below:
+
+```python
+import pandas as pd
+data = pd.read_csv("tests/resource/stock_prices.csv")
+filtered_data = data[['period','close']].set_index("period")
+filtered_data.columns = ['close_price']
+filtered_data.index = pd.to_datetime(filtered_data.index)
+filtered_data = filtered_data.sort_index()
+```
+
+Once some trend is identified, **pytrendseries** provides period on trend, drawdown, maximum drawdown (or drawup in case of uptrend) and a plot with all trends found.
+
+## Installation
+
+### Using pip
+
+You can install using the pip package manager by running:
+
+```sh
+pip install pytrendseries
+```
+
+Alternatively, you could install the latest version directly from Github:
+
+```sh
+pip install https://github.com/rafa-rod/pytrendseries/archive/refs/heads/main.zip
+```
+
+## Why pytrendseries is important?
+
+Detection of trends could be used in machine learning algorithms such as classification problems like binary (1 = uptrend, 0 = otherwise) or non-binary classifications (1 = uptrend, -1 = downtrend, 0 = otherwise). Besides that, could be used in prediction problems.
+
+## Example
+
+Inform:
+ - type of trend you desire to investigate => downtrend or uptrend;
+ - window or maximum period of a trend (example: 60 days considering 1 day as 1 period);
+ - the minimum value that represents the number of consecutive days (or another period of time) to be considered a trend (default 5 periods).
+
+```python
+import pytrendseries
+
+trend = "downtrend"
+window = 126 #6 months
+
+trends_detected = pytrendseries.detecttrend(filtered_data, trend=trend, window=window)
+```
+
+The variable `trends_detected` is a dataframe that contains the initial and end date of each trend, the prices of each date, time span of each trend and the drawdown of each trend. Let's see the first five rows of this dataframe:
+
+```
+| from                | to                  |   price0 |   price1 |   indice_from |   indice_to |   time_span |   drawdown |
+|:--------------------|:--------------------|---------:|---------:|--------------:|------------:|------------:|-----------:|
+| 2000-01-03 00:00:00 | 2000-01-31 00:00:00 |  5.90057 |  5.12252 |             0 |          19 |          19 |  0.131859  |
+| 2000-03-09 00:00:00 | 2000-04-24 00:00:00 |  6.42701 |  5.02208 |            45 |          76 |          31 |  0.218597  |
+| 2000-05-02 00:00:00 | 2000-05-11 00:00:00 |  5.53684 |  5.29352 |            81 |          88 |           7 |  0.0439456 |
+| 2000-05-16 00:00:00 | 2000-05-24 00:00:00 |  5.59962 |  5.24807 |            91 |          97 |           6 |  0.0627803 |
+| 2000-06-08 00:00:00 | 2000-06-15 00:00:00 |  6.30359 |  6.1646  |           108 |         113 |           5 |  0.0220487 |
+```
+
+The easiest way to vizualize the trends detected, just call `plot_trend` function.
+All trends detected, with maximum window informed and the minimum informed by the limit value, will be displayed.
+
+```python
+import pytrendseries
+trend = "downtrend"
+window = 30
+year = 2020
+
+trends_detected = pytrendseries.detecttrend(filtered_data, trend=trend, window=window)
+pytrendseries.vizplot.plot_trend(filtered_data, trends_detected, trend, year)
+```
+
+To visualize all uptrends found, inform `trend='uptrend'`:
+
+```python
+import pytrendseries
+window = 30
+year = 2020
+
+trends_detected = pytrendseries.detecttrend(filtered_data, trend='uptrend', window=window)
+pytrendseries.vizplot.plot_trend(filtered_data, trends_detected, 'uptrend', year)
+```
+
+The maximum drawdown or maximum drawup can be obtained by sorting the dataframe by column drawdown. To do that, just code:
+
+```python
+maxdd_in_window = trends_detected.sort_values("drawdown", ascending=False).iloc[0:1]
+```
+
+Another way is to call the function `maxdrawdown`. Note that this result will be differente once the maximum drawdown of the intire timeseries.
+
+```python
+maxdd = pytrendseries.maxdrawdown(filtered_data)
+```
+
+You can code to vizualize as follows:
+
+```python
+import matplotlib.pyplot as plt
+
+plt.figure(figsize=(14,5))
+plt.plot(filtered_data, alpha=0.6)
+location_x = maxdd.values[:,0]
+location_y = maxdd.values[:,1]
+for i in range(location_x.shape[0]):
+    plt.axvspan(location_x[i], location_y[i], alpha=0.3, color="red")
+plt.grid(axis='x')
+plt.show()
+```
+
+You may pass the parameter window to obtain the same result:
+
+```python
+maxdd_in_window = pytrendseries.maxdrawdown(filtered_data, window=252)
+```
+
+To vizualize all drawdowns of timeseries, call the following function:
+
+```python
+import pytrendseries
+pytrendseries.plot_drawdowns(filtered_data, figsize = (10,4), color="gray", alpha=0.6, title="Drawdowns", axis="y")
+```
+
+Another option is:
+
+```python
+import pytrendseries
+pytrendseries.plot_evolution(filtered_data, figsize = (10,4), colors=["gray", "red"], alphas=[1,0.6])
+```
+
+To get time underwater (tuw), just type:
+
+```python
+import pytrendseries
+pytrendseries.tuw(filtered_data)
+```
+
+The output would be (showing the tail of the dataframe):
+
+```
+| inital_date|   peak    |   valley  |   drawdown  |   time underwater |   final_date |
+|:-----------|----------:|----------:|------------:|------------------:|-------------:|
+| 2007-12-28 |  44.66140 |  33.58194 |     0.24808 |                85 |   2008-05-06 |
+| 2008-05-06 |  45.00000 |  44.85000 |     0.00333 |                4  |   2008-05-09 |
+| 2008-05-13 |  46.95000 |  46.30000 |     0.01384 |                3  |   2008-05-15 |
+| 2008-05-21 |  52.51000 |  4.20000  |     0.92002 |               NaN |          NaN |
+```
+
+The table shows time underwater as NaN, it means that the timeseries still on downtrend.
+
+Another important usage of `pytrendseries` is to obtain the series of drawdowns or series of maximum drawdowns in order to calculate the drawdown at risk or maximum drawdown at risk.
+
+```python
+import pytrendseries
+import matplotlib.pyplot as plt
+import seaborn as sns; sns.set_style("white")
+
+trend = "downtrend"
+window = 126 #6 months
+
+trends_detected = pytrendseries.detecttrend(filtered_data, trend=trend, window=window)
+
+plt.figure(figsize=(15,5))
+sns.histplot(trends_detected["drawdown"]*100, kde=True, bins=30)
+plt.ylabel("")
+plt.box(False)
+plt.annotate('Maximum Drawdown', xy=((trends_detected["drawdown"].max()-0.005)*100, 1),
+             xycoords='data',
+            xytext=(-105, 30), textcoords='offset points',color="red",
+            weight='bold',
+            arrowprops=dict(arrowstyle="->", color="r",
+                            connectionstyle='arc3,rad=-0.1'))
+plt.annotate('Quantile 97,5%', xy=((trends_detected["drawdown"].quantile(0.975)-0.005)*100, 0.2),
+             xycoords='data',
+            xytext=(-135, 30), textcoords='offset points',color="red",
+            weight='bold',
+            arrowprops=dict(arrowstyle="->", color="r",
+                            connectionstyle='arc3,rad=-0.1'))
+plt.xlabel("Drawdown (%)")
+plt.ylabel("Density", rotation=0, labelpad=-30, loc="top")
+plt.show()
+```
+
+```python
+import pytrendseries
+import matplotlib.pyplot as plt
+import seaborn as sns; sns.set_style("white")
+
+maxdd_in_window = maxdrawdown(filtered_data, window=126)
+
+plt.figure(figsize=(15,5))
+sns.histplot(maxdd_in_window["MaxDD"]*100, kde=True, bins=30)
+plt.ylabel("")
+plt.box(False)
+plt.annotate('Maximum Drawdown', xy=((maxdd_in_window["MaxDD"].max()-0.005)*100, 1),
+             xycoords='data',
+            xytext=(-105, 30), textcoords='offset points',color="red",
+            weight='bold',
+            arrowprops=dict(arrowstyle="->", color="r",
+                            connectionstyle='arc3,rad=-0.1'))
+plt.annotate('Quantile 95%', xy=((maxdd_in_window["MaxDD"].quantile(0.95)-0.005)*100, 0.2),
+             xycoords='data',
+            xytext=(-135, 50), textcoords='offset points',color="red",
+            weight='bold',
+            arrowprops=dict(arrowstyle="->", color="r",
+                            connectionstyle='arc3,rad=-0.1'))
+plt.xlabel("Maximum Drawdowns (%)")
+plt.ylabel("Density", rotation=0, labelpad=-30, loc="top")
+plt.show()
+```
```

#### html2text {}

```diff
@@ -1,92 +1,101 @@
-Metadata-Version: 2.1 Name: pytrendseries Version: 0.1.8 Summary: Detect trend
-in time series. Home-page: UNKNOWN Author: Rafael Rodrigues Author-email:
-rafael.rafarod@gmail.com License: UNKNOWN Platform: UNKNOWN Requires-Python:
->=3.8,<4.0 Description-Content-Type: text/markdown
 [python]   [MIT_license]   [https://codecov.io/gh/rafa-rod/detecttrend/branch/
                     main/graph/badge.svg?token=98EMCTZTOY]
  **pytrendseries** is a Python library for detection of trends in time series
 like: stock prices, monthly sales, daily temperature of a city and so on. The
 input data must be a `pandas.DataFrame` format containing one column as
 observed data (in float or int format). Follow example below: ```python import
 pandas as pd data = pd.read_csv("tests/resource/stock_prices.csv")
 filtered_data = data[['period','close']].set_index("period")
 filtered_data.columns = ['close_price'] filtered_data.index = pd.to_datetime
-(filtered_data.index) filtered_data.index = filtered_data.sort_index() ``` Once
-some trend is identified, **pytrendseries** provides period on trend, drawdown,
-maximum drawdown (or buildup in case of uptrend) and a plot with all trends
+(filtered_data.index) filtered_data = filtered_data.sort_index() ``` Once some
+trend is identified, **pytrendseries** provides period on trend, drawdown,
+maximum drawdown (or drawup in case of uptrend) and a plot with all trends
 found. ## Installation ### Using pip You can install using the pip package
 manager by running: ```sh pip install pytrendseries ``` Alternatively, you
 could install the latest version directly from Github: ```sh pip install https:
 //github.com/rafa-rod/pytrendseries/archive/refs/heads/main.zip ``` ## Why
 pytrendseries is important? Detection of trends could be used in machine
 learning algorithms such as classification problems like binary (1 = uptrend, 0
 = otherwise) or non-binary classifications (1 = uptrend, -1 = downtrend, 0 =
 otherwise). Besides that, could be used in prediction problems. ## Example
 Inform: - type of trend you desire to investigate => downtrend or uptrend; -
 window or maximum period of a trend (example: 60 days considering 1 day as 1
-period) **optional**; - the minimum value that represents the number of
-consecutive days (or anohter period of time) to be considered a trend (default
-5 periods) **optional**; - instead of minimum period, you may inform the
-quantile of time span (consecutive days in trend) such as 0.8 (80%). ```python
-import pytrendseries trend = "downtrend" window = 126 #6 months
-trends_detected, statistcs = pytrendseries.detecttrend(filtered_data,
-trend=trend, window=window) ``` The variable `trends_detected` is a dataframe
-that contains the initial and end date of each trend, the prices of each date,
-time span of each trend and the drawdown of each trend. Let's see the first
-five rows of this dataframe: ``` | from | to | price0 | price1 | indice_from |
-indice_to | time_span | drawdown | |:--------------------|:--------------------
-|---------:|---------:|--------------:|------------:|------------:|-----------:
-| | 2000-01-03 00:00:00 | 2000-01-31 00:00:00 | 5.90057 | 5.12252 | 0 | 19 | 19
-| 0.131859 | | 2000-03-09 00:00:00 | 2000-04-24 00:00:00 | 6.42701 | 5.02208 |
-45 | 76 | 31 | 0.218597 | | 2000-05-02 00:00:00 | 2000-05-11 00:00:00 | 5.53684
-| 5.29352 | 81 | 88 | 7 | 0.0439456 | | 2000-05-16 00:00:00 | 2000-05-24 00:00:
-00 | 5.59962 | 5.24807 | 91 | 97 | 6 | 0.0627803 | | 2000-06-08 00:00:00 |
-2000-06-15 00:00:00 | 6.30359 | 6.1646 | 108 | 113 | 5 | 0.0220487 | ``` The
-output `statistcs` shows the basic statistics such as: minimum, maximum (must
-be equal to window variable) and other percentiles of all periods of trends.
-This is important if you want to filter all small and unnecessary trends
-detected such as: trend with only 2 consecutive days. By default, the limit
-variable cut off all trends with 5 periods found. The statistcs exhibit all
-trend with no cut off at all. Let's see the `statistcs`: ``` | | time_span | |:
-------|------------:| | count | 2444 | | mean | 12.5569 | | std | 26.0989 | |
-min | 1 | | 25% | 1 | | 50% | 2 | | 75% | 8 | | 80% | 12 | | 85% | 18.55 | |
-90% | 33 | | 92.5% | 57.775 | | 95% | 88 | | 97.5% | 110 | | 99% | 122 | | max
-| 126 | ``` As we just saw, the median (50% percentile) shows that 50% of
-trends is just 2 periods (2 days in this case), therefore the default limit of
-5 it is a good cut number. Next, we will redefine the limit value with 21
-periods. The easiest way to vizualize the trends detected, just call
-`plot_trend` function. All trends detected, with maximum window informed and
-the minimum informed by the limit value, will be displayed. ```python import
-pytrendseries pytrendseries.vizplot.plot_trend(filtered_data, trends_detected,
-trend) ``` It is also possible to filter data by informing year variable. In
-this example, the series contains data after year 2005. ```python year = 2005
-trends_detected, _ = pytrendseries.detecttrend(filtered_data, trend=trend,
-limit=21, window=janela, year=year) #same: trends_detected, _ =
-pytrendseries.detecttrend(filtered_data, trend=trend, quantile=0.85,
-window=janela, year=year) ``` The maximum drawdown or maximum run up is
-calculate calling the function `max_trend` which return: peak and valley
-values, data in which they occurred and the maxdrawdown/maxrunup value.
-```python import pytrendseries maxdd = pytrendseries.getmaxtrend(filtered_data,
-trend, year) ``` ``` | peak_price | valley_price | peak_date_maxdrawdown |
-valley_date_maxdrawdown | maxdrawdown | time_span | |-------------:|-----------
-----:|:------------------------|:--------------------------|--------------:|:--
------------------| | 52.51 | 4.2 | 2008-05-21 00:00:00 | 2016-01-26 00:00:00 |
-0.920015 | 2806 days 00:00:00 | ``` Instead, you may want to known the maximum
-drawdown (maximum run up) according to informed window. To do that, just code:
-```python maxdd_in_window = trends_detected.sort_values
-("drawdown",ascending=False).iloc[0:1] ``` To exhibit the maximium drawdown of
-the time series just call `plot_maxdrawdown` function and select the style of
-the plot: shadow, area or plotly. ```python import pytrendseries
-pytrendseries.plot_maxdrawdown(filtered_data, maxdd, trend, year,
-style="shadow") pytrendseries.plot_maxdrawdown(filtered_data, maxdd, trend,
-year, style="area") pytrendseries.plot_maxdrawdown(filtered_data, maxdd, trend,
-year, style="plotly") ``` To get time under water (tuw), just type: ```python
+period); - the minimum value that represents the number of consecutive days (or
+another period of time) to be considered a trend (default 5 periods). ```python
+import pytrendseries trend = "downtrend" window = 126 #6 months trends_detected
+= pytrendseries.detecttrend(filtered_data, trend=trend, window=window) ``` The
+variable `trends_detected` is a dataframe that contains the initial and end
+date of each trend, the prices of each date, time span of each trend and the
+drawdown of each trend. Let's see the first five rows of this dataframe: ``` |
+from | to | price0 | price1 | indice_from | indice_to | time_span | drawdown |
+|:--------------------|:--------------------|---------:|---------:|------------
+--:|------------:|------------:|-----------:| | 2000-01-03 00:00:00 | 2000-01-
+31 00:00:00 | 5.90057 | 5.12252 | 0 | 19 | 19 | 0.131859 | | 2000-03-09 00:00:
+00 | 2000-04-24 00:00:00 | 6.42701 | 5.02208 | 45 | 76 | 31 | 0.218597 | |
+2000-05-02 00:00:00 | 2000-05-11 00:00:00 | 5.53684 | 5.29352 | 81 | 88 | 7 |
+0.0439456 | | 2000-05-16 00:00:00 | 2000-05-24 00:00:00 | 5.59962 | 5.24807 |
+91 | 97 | 6 | 0.0627803 | | 2000-06-08 00:00:00 | 2000-06-15 00:00:00 | 6.30359
+| 6.1646 | 108 | 113 | 5 | 0.0220487 | ``` The easiest way to vizualize the
+trends detected, just call `plot_trend` function. All trends detected, with
+maximum window informed and the minimum informed by the limit value, will be
+displayed. ```python import pytrendseries trend = "downtrend" window = 30 year
+= 2020 trends_detected = pytrendseries.detecttrend(filtered_data, trend=trend,
+window=window) pytrendseries.vizplot.plot_trend(filtered_data, trends_detected,
+trend, year) ``` To visualize all uptrends found, inform `trend='uptrend'`:
+```python import pytrendseries window = 30 year = 2020 trends_detected =
+pytrendseries.detecttrend(filtered_data, trend='uptrend', window=window)
+pytrendseries.vizplot.plot_trend(filtered_data, trends_detected, 'uptrend',
+year) ``` The maximum drawdown or maximum drawup can be obtained by sorting the
+dataframe by column drawdown. To do that, just code: ```python maxdd_in_window
+= trends_detected.sort_values("drawdown", ascending=False).iloc[0:1] ```
+Another way is to call the function `maxdrawdown`. Note that this result will
+be differente once the maximum drawdown of the intire timeseries. ```python
+maxdd = pytrendseries.maxdrawdown(filtered_data) ``` You can code to vizualize
+as follows: ```python import matplotlib.pyplot as plt plt.figure(figsize=
+(14,5)) plt.plot(filtered_data, alpha=0.6) location_x = maxdd.values[:,0]
+location_y = maxdd.values[:,1] for i in range(location_x.shape[0]): plt.axvspan
+(location_x[i], location_y[i], alpha=0.3, color="red") plt.grid(axis='x')
+plt.show() ``` You may pass the parameter window to obtain the same result:
+```python maxdd_in_window = pytrendseries.maxdrawdown(filtered_data,
+window=252) ``` To vizualize all drawdowns of timeseries, call the following
+function: ```python import pytrendseries pytrendseries.plot_drawdowns
+(filtered_data, figsize = (10,4), color="gray", alpha=0.6, title="Drawdowns",
+axis="y") ``` Another option is: ```python import pytrendseries
+pytrendseries.plot_evolution(filtered_data, figsize = (10,4), colors=["gray",
+"red"], alphas=[1,0.6]) ``` To get time underwater (tuw), just type: ```python
 import pytrendseries pytrendseries.tuw(filtered_data) ``` The output would be
 (showing the tail of the dataframe): ``` | inital_date| peak | valley |
 drawdown | time underwater | final_date | |:-----------|----------:|----------:
 |------------:|------------------:|-------------:| | 2007-12-28 | 44.66140 |
 33.58194 | 0.24808 | 85 | 2008-05-06 | | 2008-05-06 | 45.00000 | 44.85000 |
 0.00333 | 4 | 2008-05-09 | | 2008-05-13 | 46.95000 | 46.30000 | 0.01384 | 3 |
 2008-05-15 | | 2008-05-21 | 52.51000 | 4.20000 | 0.92002 | NaN | NaN | ``` The
-table show time underwater as NaN, it means that the timeseries still on
-downtrend.
+table shows time underwater as NaN, it means that the timeseries still on
+downtrend. Another important usage of `pytrendseries` is to obtain the series
+of drawdowns or series of maximum drawdowns in order to calculate the drawdown
+at risk or maximum drawdown at risk. ```python import pytrendseries import
+matplotlib.pyplot as plt import seaborn as sns; sns.set_style("white") trend =
+"downtrend" window = 126 #6 months trends_detected = pytrendseries.detecttrend
+(filtered_data, trend=trend, window=window) plt.figure(figsize=(15,5))
+sns.histplot(trends_detected["drawdown"]*100, kde=True, bins=30) plt.ylabel("")
+plt.box(False) plt.annotate('Maximum Drawdown', xy=((trends_detected
+["drawdown"].max()-0.005)*100, 1), xycoords='data', xytext=(-105, 30),
+textcoords='offset points',color="red", weight='bold', arrowprops=dict
+(arrowstyle="->", color="r", connectionstyle='arc3,rad=-0.1')) plt.annotate
+('Quantile 97,5%', xy=((trends_detected["drawdown"].quantile(0.975)-0.005)*100,
+0.2), xycoords='data', xytext=(-135, 30), textcoords='offset
+points',color="red", weight='bold', arrowprops=dict(arrowstyle="->", color="r",
+connectionstyle='arc3,rad=-0.1')) plt.xlabel("Drawdown (%)") plt.ylabel
+("Density", rotation=0, labelpad=-30, loc="top") plt.show() ``` ```python
+import pytrendseries import matplotlib.pyplot as plt import seaborn as sns;
+sns.set_style("white") maxdd_in_window = maxdrawdown(filtered_data, window=126)
+plt.figure(figsize=(15,5)) sns.histplot(maxdd_in_window["MaxDD"]*100, kde=True,
+bins=30) plt.ylabel("") plt.box(False) plt.annotate('Maximum Drawdown', xy=(
+(maxdd_in_window["MaxDD"].max()-0.005)*100, 1), xycoords='data', xytext=(-105,
+30), textcoords='offset points',color="red", weight='bold', arrowprops=dict
+(arrowstyle="->", color="r", connectionstyle='arc3,rad=-0.1')) plt.annotate
+('Quantile 95%', xy=((maxdd_in_window["MaxDD"].quantile(0.95)-0.005)*100, 0.2),
+xycoords='data', xytext=(-135, 50), textcoords='offset points',color="red",
+weight='bold', arrowprops=dict(arrowstyle="->", color="r",
+connectionstyle='arc3,rad=-0.1')) plt.xlabel("Maximum Drawdowns (%)")
+plt.ylabel("Density", rotation=0, labelpad=-30, loc="top") plt.show() ```
```

### Comparing `pytrendseries-0.1.8/pytrendseries/time_under_water.py` & `pytrendseries-0.1.9/src/pytrendseries/time_under_water.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,40 +5,52 @@
 
 @author: Rafael
 """
 import pandas as pd
 import numpy as np
 
 import warnings
-warnings.filterwarnings('ignore')
+
+warnings.filterwarnings("ignore")
+
 
 def _treat_parameters(prices):
-    '''Checking all parameters'''
-    if isinstance(prices, pd.core.frame.DataFrame)==False or prices.empty or prices.shape[1]>1:
-        raise ValueError("Input must be a dataframe containing one column and its index must be in datetime format.")
+    """Checking all parameters"""
+    if (
+        isinstance(prices, pd.core.frame.DataFrame) == False
+        or prices.empty
+        or prices.shape[1] > 1
+    ):
+        raise ValueError(
+            "Input must be a dataframe containing one column and its index must be in datetime format."
+        )
+
 
 def tuw(df: pd.DataFrame, **kwargs) -> pd.DataFrame:
-    '''The maximum distance in time, from a previous peak to a new peak. it calculates how long it takes an investor to recover its money at the start of the maximum drawdown period.
+    """The maximum distance in time, from a previous peak to a new peak. it calculates how long it takes an investor to recover its money at the start of the maximum drawdown period.
     Parameters:
         df (dataframe): timeseries.
     Returns:
         df1 (dataframe): dataframe containing inital date (where peak occurs), final date, peak and valley values, drawdown and time underwater.
-    '''
+    """
 
     if pd.api.types.is_datetime64_ns_dtype(df.index.dtype) == False:
-        df.index = pd.to_datetime(df.index, format=kwargs.get('format'))
-        
+        df.index = pd.to_datetime(df.index, format=kwargs.get("format"))
+
     _treat_parameters(df)
 
     df0 = df.copy()
     df0["peak"] = df0.expanding().max()
     df1 = df0["peak"].drop_duplicates(keep="first").to_frame().reset_index()
-    df1.columns = ['initial_date',"peak"]
+    df1.columns = ["initial_date", "peak"]
     df1 = df1.set_index("initial_date")
     df1["peak"] = pd.to_numeric(df1["peak"])
     df1["valley"] = df0.groupby("peak").min().reset_index()[df0.columns[0]].values
-    df1["drawdown"]= 1-df1["valley"]/df1["peak"]
-    tuw = [df0[(df0.index>=df1.index[x]) & (df0.index<=df1.index[x+1])].shape[0] for x in range(df1.index.shape[0]-1)]
+    df1["drawdown"] = 1 - df1["valley"] / df1["peak"]
+    tuw = [
+        df0[(df0.index >= df1.index[x]) & (df0.index <= df1.index[x + 1])].shape[0]
+        for x in range(df1.index.shape[0] - 1)
+    ]
     df1["time underwater"] = tuw + [np.nan]
     df1["final_date"] = df1.index[1:].tolist() + [np.nan]
-    df1 = df1[df1["peak"]!=df1["valley"]]
-    return df1.reset_index()
+    df1 = df1[df1["peak"] != df1["valley"]]
+    return df1.reset_index()
```

