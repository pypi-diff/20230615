# Comparing `tmp/rotspectools-0.1.4.tar.gz` & `tmp/rotspectools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotspectools-0.1.4.tar", max compression
+gzip compressed data, was "rotspectools-0.1.5.tar", max compression
```

## Comparing `rotspectools-0.1.4.tar` & `rotspectools-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.4/LICENSE
--rw-r--r--   0        0        0      974 2023-06-09 22:48:57.252972 rotspectools-0.1.4/README.rst
--rw-r--r--   0        0        0      459 2023-06-10 01:51:52.249953 rotspectools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.4/rotspectools/.DS_Store
--rw-r--r--   0        0        0      146 2023-06-09 22:48:57.256906 rotspectools-0.1.4/rotspectools/__init__.py
--rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.4/rotspectools/cli.py
--rw-r--r--   0        0        0    19459 2023-06-10 01:50:31.482562 rotspectools-0.1.4/rotspectools/rotspectools.py
--rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 rotspectools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1754 2023-06-11 01:21:50.352482 rotspectools-0.1.5/README.rst
+-rw-r--r--   0        0        0      459 2023-06-15 18:13:07.255869 rotspectools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.5/rotspectools/.DS_Store
+-rw-r--r--   0        0        0      146 2023-06-15 18:12:39.518028 rotspectools-0.1.5/rotspectools/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.5/rotspectools/cli.py
+-rw-r--r--   0        0        0    29906 2023-06-15 18:05:26.747016 rotspectools-0.1.5/rotspectools/rotspectools.py
+-rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 rotspectools-0.1.5/PKG-INFO
```

### Comparing `rotspectools-0.1.4/LICENSE` & `rotspectools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.4/rotspectools/.DS_Store` & `rotspectools-0.1.5/rotspectools/.DS_Store`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.4/rotspectools/rotspectools.py` & `rotspectools-0.1.5/rotspectools/rotspectools.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scienceplots
 from matplotlib.legend_handler import HandlerPatch
 from pandas import DataFrame
-from inspect import currentframe, getframeinfo
 
 mpl.rc("text", usetex=True)
 plt.style.use(["science", "ieee"])
 
 
 class Experiment:
     def __init__(
@@ -175,27 +174,30 @@
                 branches.append("R-Branch")
             elif value == -1:
                 branches.append("P-Branch")
             else:
                 branches.append("Q-Branch")
         self.res_dataframe["Branch"] = branches
 
-    def delta_values(self) -> DataFrame:
+    def delta_values(self):
         self.res_dataframe = self.res_dataframe.apply(pd.to_numeric, errors="ignore")
         self.res_dataframe["Delta J"] = (
             self.res_dataframe["J"] - self.res_dataframe["J'"]
         )
         self.res_dataframe["Delta Ka"] = (
             self.res_dataframe["Ka"] - self.res_dataframe["Ka'"]
         )
         self.res_dataframe["Delta Kc"] = (
             self.res_dataframe["Kc"] - self.res_dataframe["Kc'"]
         )
+        self.res_dataframe["Delta_v"] = (
+            self.res_dataframe["v"] - self.res_dataframe["v'"]
+        )
 
-    def categorize_error(self) -> DataFrame:
+    def categorize_error(self):
         self.res_dataframe["blend O-C"].fillna(
             value=self.res_dataframe["O-C"], inplace=True
         )
         self.res_dataframe["blend O-C"] = self.res_dataframe["blend O-C"].abs()
         self.res_dataframe["blend O-C/error"] = (
             self.res_dataframe["blend O-C"].abs() / self.res_dataframe["Error"]
         )
@@ -252,14 +254,22 @@
         df_cq = self.res_dataframe.loc[
             (self.res_dataframe["Transition Type"] == "c-type")
             & (self.res_dataframe["Branch"] == "Q-Branch")
         ]
 
         return (df_ar, df_br, df_cr, df_ap, df_bp, df_cp, df_aq, df_bq, df_cq)
 
+    def get_IR(df: DataFrame) -> DataFrame:
+        df_IR = df.loc[df["Delta_v"] != 0]
+        return df_IR
+
+    def get_rot(df: DataFrame) -> DataFrame:
+        df_rot = df.loc[df["Delta_v"] == 0]
+        return df_rot
+
     def plot_data_dist(self, max_Ka: int, max_J: int):
         mpl.rc("text", usetex=True)
         plt.style.use(["science", "ieee"])
         self.categorize_error()
         self.res_dataframe = self.res_dataframe.sort_values(
             by=["Transition Type"], ascending=True
         )
@@ -267,14 +277,300 @@
         fig, ax = plt.subplots(1, 2, figsize=(8, 4))
         for i in range(0, 2):
             condition = dataframes[i]["blend O-C/error"] >= 4
             df_high_error = dataframes[i][condition]
             df_normal = dataframes[i][~condition]
             ax[0].scatter(
                 df_normal["Ka'"],
+                df_normal["J'"],
+                s=4 * df_normal["blend O-C/error"],
+                facecolors=df_normal["Transition Type"].map(
+                    {
+                        "a-type": "#0000FF65",
+                        "b-type": "#00800045",
+                        "c-type": "#FFFFFF00",
+                    }
+                ),
+                edgecolors=df_normal["Transition Type"].map(
+                    {"a-type": "blue", "b-type": "green", "c-type": "orange"}
+                ),
+                linewidth=0.8,
+            )
+            ax[0].scatter(
+                df_high_error["Ka'"],
+                df_high_error["J'"],
+                s=4 * df_high_error["blend O-C/error"],
+                facecolors="#FF000065",
+                edgecolors="red",
+                linewidth=0.8,
+            )
+        condition_q = dataframes[2]["blend O-C/error"] >= 4
+        df_high_error_q = dataframes[2][condition_q]
+        df_normal_q = dataframes[2][~condition_q]
+        ax[1].scatter(
+            df_high_error_q["Ka'"],
+            df_high_error_q["J'"],
+            s=4 * df_high_error_q["blend O-C/error"],
+            facecolors="#FF000065",
+            edgecolors="red",
+            linewidth=0.8,
+        )
+        ax[1].scatter(
+            df_normal_q["Ka'"],
+            df_normal_q["J'"],
+            s=4 * df_normal_q["blend O-C/error"],
+            facecolors=df_normal_q["Transition Type"].map(
+                {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "#FFFFFF00"}
+            ),
+            edgecolors=df_normal_q["Transition Type"].map(
+                {"a-type": "blue", "b-type": "green", "c-type": "orange"}
+            ),
+            linewidth=0.8,
+        )
+
+        ax[0].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
+        ax[0].set_xlabel("$K_a''$", fontsize=14)
+        ax[0].set_ylabel("$J''$", fontsize=14)
+        ax[0].set_ylim(0, max_J)
+        ax[0].set_xlim(-0.5, max_Ka)
+        ax[0].set_xticks((0, 10, 20, 30, 40, 50, 60))
+        ax[0].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
+        ax[0].text(38, 110, "R-Branch", fontsize=18)
+
+        ax[1].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
+        ax[1].set_xlabel("$K_a''$", fontsize=14)
+        ax[1].set_ylabel("$J''$", fontsize=14)
+        ax[1].set_ylim(0, max_J)
+        ax[1].set_xlim(-0.5, max_Ka)
+        ax[1].set_xticks((0, 10, 20, 30, 40, 50, 60))
+        ax[1].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
+        ax[1].text(38, 110, "Q-Branch", fontsize=18)
+
+        c = [
+            mpatches.Circle(
+                (0.5, 0.5),
+                radius=0.25,
+                facecolor="#0000FF65",
+                edgecolor="blue",
+                label="a-type",
+            ),
+            mpatches.Circle(
+                (0.5, 0.5),
+                radius=0.25,
+                facecolor="#00800045",
+                edgecolor="green",
+                label="b-type",
+            ),
+            mpatches.Circle(
+                (0.5, 0.5),
+                radius=0.25,
+                facecolor="#FFA50065",
+                edgecolor="orange",
+                label="c-type",
+            ),
+            mpatches.Circle(
+                (0.5, 0.5),
+                radius=0.25,
+                facecolor="#FF000065",
+                edgecolor="red",
+                label=r"$>$ $3\sigma$",
+            ),
+        ]
+        texts = ["a-type", "b-type", "c-type", r"$>$ $3\sigma$"]
+        legend = ax[0].legend(
+            c,
+            texts,
+            loc="lower right",
+            fontsize=8,
+            frameon=True,
+            edgecolor="black",
+            framealpha=1,
+            borderaxespad=0,
+            fancybox=False,
+            handler_map={mpatches.Circle: HandlerEllipse()},
+        )
+        frame = legend.get_frame()
+        frame.set_linewidth(0.5)
+
+        legend1 = ax[1].legend(
+            c,
+            texts,
+            loc="lower right",
+            fontsize=8,
+            frameon=True,
+            edgecolor="black",
+            framealpha=1,
+            borderaxespad=0,
+            fancybox=False,
+            handler_map={mpatches.Circle: HandlerEllipse()},
+        )
+        frame1 = legend1.get_frame()
+        frame1.set_linewidth(0.5)
+        file_path = self.file_name + ".jpg"
+        fig.savefig(file_path, dpi=800)
+
+    def plot_data_dist_rot(self, max_Ka: int, max_J: int):
+        mpl.rc("text", usetex=True)
+        plt.style.use(["science", "ieee"])
+        self.categorize_error()
+        self.res_dataframe = self.res_dataframe.sort_values(
+            by=["Transition Type"], ascending=True
+        )
+        dataframes = self.split_branches()
+        dataframes = tuple(map(self.get_rot, dataframes))
+        fig, ax = plt.subplots(1, 2, figsize=(8, 4))
+        for i in range(0, 2):
+            condition = dataframes[i]["blend O-C/error"] >= 4
+            df_high_error = dataframes[i][condition]
+            df_normal = dataframes[i][~condition]
+            ax[0].scatter(
+                df_normal["Ka'"],
+                df_normal["J'"],
+                s=4 * df_normal["blend O-C/error"],
+                facecolors=df_normal["Transition Type"].map(
+                    {
+                        "a-type": "#0000FF65",
+                        "b-type": "#00800045",
+                        "c-type": "#FFFFFF00",
+                    }
+                ),
+                edgecolors=df_normal["Transition Type"].map(
+                    {"a-type": "blue", "b-type": "green", "c-type": "orange"}
+                ),
+                linewidth=0.8,
+            )
+            ax[0].scatter(
+                df_high_error["Ka'"],
+                df_high_error["J'"],
+                s=4 * df_high_error["blend O-C/error"],
+                facecolors="#FF000065",
+                edgecolors="red",
+                linewidth=0.8,
+            )
+        condition_q = dataframes[2]["blend O-C/error"] >= 4
+        df_high_error_q = dataframes[2][condition_q]
+        df_normal_q = dataframes[2][~condition_q]
+        ax[1].scatter(
+            df_high_error_q["Ka'"],
+            df_high_error_q["J'"],
+            s=4 * df_high_error_q["blend O-C/error"],
+            facecolors="#FF000065",
+            edgecolors="red",
+            linewidth=0.8,
+        )
+        ax[1].scatter(
+            df_normal_q["Ka'"],
+            df_normal_q["J'"],
+            s=4 * df_normal_q["blend O-C/error"],
+            facecolors=df_normal_q["Transition Type"].map(
+                {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "#FFFFFF00"}
+            ),
+            edgecolors=df_normal_q["Transition Type"].map(
+                {"a-type": "blue", "b-type": "green", "c-type": "orange"}
+            ),
+            linewidth=0.8,
+        )
+
+        ax[0].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
+        ax[0].set_xlabel("$K_a''$", fontsize=14)
+        ax[0].set_ylabel("$J''$", fontsize=14)
+        ax[0].set_ylim(0, max_J)
+        ax[0].set_xlim(-0.5, max_Ka)
+        ax[0].set_xticks((0, 10, 20, 30, 40, 50, 60))
+        ax[0].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
+        ax[0].text(38, 110, "R-Branch", fontsize=18)
+
+        ax[1].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
+        ax[1].set_xlabel("$K_a''$", fontsize=14)
+        ax[1].set_ylabel("$J''$", fontsize=14)
+        ax[1].set_ylim(0, max_J)
+        ax[1].set_xlim(-0.5, max_Ka)
+        ax[1].set_xticks((0, 10, 20, 30, 40, 50, 60))
+        ax[1].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
+        ax[1].text(38, 110, "Q-Branch", fontsize=18)
+
+        c = [
+            mpatches.Circle(
+                (0.5, 0.5),
+                radius=0.25,
+                facecolor="#0000FF65",
+                edgecolor="blue",
+                label="a-type",
+            ),
+            mpatches.Circle(
+                (0.5, 0.5),
+                radius=0.25,
+                facecolor="#00800045",
+                edgecolor="green",
+                label="b-type",
+            ),
+            mpatches.Circle(
+                (0.5, 0.5),
+                radius=0.25,
+                facecolor="#FFA50065",
+                edgecolor="orange",
+                label="c-type",
+            ),
+            mpatches.Circle(
+                (0.5, 0.5),
+                radius=0.25,
+                facecolor="#FF000065",
+                edgecolor="red",
+                label=r"$>$ $3\sigma$",
+            ),
+        ]
+        texts = ["a-type", "b-type", "c-type", r"$>$ $3\sigma$"]
+        legend = ax[0].legend(
+            c,
+            texts,
+            loc="lower right",
+            fontsize=8,
+            frameon=True,
+            edgecolor="black",
+            framealpha=1,
+            borderaxespad=0,
+            fancybox=False,
+            handler_map={mpatches.Circle: HandlerEllipse()},
+        )
+        frame = legend.get_frame()
+        frame.set_linewidth(0.5)
+
+        legend1 = ax[1].legend(
+            c,
+            texts,
+            loc="lower right",
+            fontsize=8,
+            frameon=True,
+            edgecolor="black",
+            framealpha=1,
+            borderaxespad=0,
+            fancybox=False,
+            handler_map={mpatches.Circle: HandlerEllipse()},
+        )
+        frame1 = legend1.get_frame()
+        frame1.set_linewidth(0.5)
+        file_path = self.file_name + ".jpg"
+        fig.savefig(file_path, dpi=800)
+
+    def plot_data_dist_IR(self, max_Ka: int, max_J: int):
+        mpl.rc("text", usetex=True)
+        plt.style.use(["science", "ieee"])
+        self.categorize_error()
+        self.res_dataframe = self.res_dataframe.sort_values(
+            by=["Transition Type"], ascending=True
+        )
+        dataframes = self.split_branches()
+        dataframes = tuple(map(self.get_IR, dataframes))
+        fig, ax = plt.subplots(1, 2, figsize=(8, 4))
+        for i in range(0, 2):
+            condition = dataframes[i]["blend O-C/error"] >= 4
+            df_high_error = dataframes[i][condition]
+            df_normal = dataframes[i][~condition]
+            ax[0].scatter(
+                df_normal["Ka'"],
                 df_normal["J'"],
                 s=4 * df_normal["blend O-C/error"],
                 facecolors=df_normal["Transition Type"].map(
                     {
                         "a-type": "#0000FF65",
                         "b-type": "#00800045",
                         "c-type": "#FFFFFF00",
```

