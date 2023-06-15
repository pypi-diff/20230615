# Comparing `tmp/ProTstab2-1.0.2.tar.gz` & `tmp/ProTstab2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProTstab2-1.0.2.tar", last modified: Tue May 16 08:07:10 2023, max compression
+gzip compressed data, was "ProTstab2-2.0.0.tar", last modified: Thu Jun 15 15:15:55 2023, max compression
```

## Comparing `ProTstab2-1.0.2.tar` & `ProTstab2-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:07:10.982064 ProTstab2-1.0.2/
--rw-rw-rw-   0        0        0    35823 2023-05-15 09:13:01.000000 ProTstab2-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2679 2023-05-16 08:07:10.981063 ProTstab2-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 08:07:10.974059 ProTstab2-1.0.2/ProTstab2/
--rw-rw-rw-   0        0        0     6089 2023-05-16 08:04:29.000000 ProTstab2-1.0.2/ProTstab2/__init__.py
--rw-rw-rw-   0        0        0     6192 2023-05-16 06:02:46.000000 ProTstab2-1.0.2/ProTstab2/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:07:10.980063 ProTstab2-1.0.2/ProTstab2.egg-info/
--rw-rw-rw-   0        0        0     2679 2023-05-16 08:07:10.000000 ProTstab2-1.0.2/ProTstab2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-16 08:07:10.000000 ProTstab2-1.0.2/ProTstab2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:07:10.000000 ProTstab2-1.0.2/ProTstab2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-16 08:07:10.000000 ProTstab2-1.0.2/ProTstab2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 08:07:10.000000 ProTstab2-1.0.2/ProTstab2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2161 2023-05-16 06:21:35.000000 ProTstab2-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 08:07:10.982064 ProTstab2-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-05-16 08:06:55.000000 ProTstab2-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:15:55.947924 ProTstab2-2.0.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-15 09:13:01.000000 ProTstab2-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2341 2023-06-15 15:15:55.946923 ProTstab2-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 15:15:55.940925 ProTstab2-2.0.0/ProTstab2/
+-rw-rw-rw-   0        0        0     5524 2023-06-15 15:06:45.000000 ProTstab2-2.0.0/ProTstab2/__init__.py
+-rw-rw-rw-   0        0        0    18423 2023-06-15 14:46:47.000000 ProTstab2-2.0.0/ProTstab2/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:15:55.945924 ProTstab2-2.0.0/ProTstab2.egg-info/
+-rw-rw-rw-   0        0        0     2341 2023-06-15 15:15:55.000000 ProTstab2-2.0.0/ProTstab2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-15 15:15:55.000000 ProTstab2-2.0.0/ProTstab2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 15:15:55.000000 ProTstab2-2.0.0/ProTstab2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-15 15:15:55.000000 ProTstab2-2.0.0/ProTstab2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-15 15:15:55.000000 ProTstab2-2.0.0/ProTstab2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1823 2023-06-15 15:13:31.000000 ProTstab2-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 15:15:55.947924 ProTstab2-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2023-06-15 15:15:33.000000 ProTstab2-2.0.0/setup.py
```

### Comparing `ProTstab2-1.0.2/LICENSE` & `ProTstab2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ProTstab2-1.0.2/ProTstab2/__init__.py` & `ProTstab2-2.0.0/ProTstab2/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,97 @@
 import os.path
 import pickle
+import re
 import zipfile
 
 import numpy as np
-import pandas as pd
 import requests
-import tensorflow as tf
-from sklearn.preprocessing import RobustScaler
-from tensorflow.python.keras.preprocessing import sequence
+from sklearn.externals import joblib
 
-from ProTstab2.utils import Attention, get_feature_from_profeat_replace, trans, trans_6, zero_or_one
+from ProTstab2.utils import A_LIST, get_all_features_from_protstab
 
 
 class ProTstab2:
-    def __init__(self, base_model_path):
-        self.base_model_path = base_model_path
-        self.deep_tp_model_name = 'model_DeepTP.h5'
-        self.deep_tp_model_name_zip = 'model_DeepTP.zip'
-        self.features_model_name = 'selector_RFECV_205_0711_797features.pickle'
-        self.features_model_name_zip = 'selector_RFECV_205_0711_797features.zip'
-        self.csv_name = 'train_features.csv'
-        self.csv_name_zip = 'train_features.zip'
-        self.download_msg = f"""
-You can download the model in either of the following two ways:
-1. https://drive.google.com/drive/folders/1OEKabeJmdGiGG1PJsPu0bgcE5_GVGXc9?usp=share_link
-2. https://luke9012.lanzoub.com/b00r1vhre | password:ddpt
-"""
+    def __init__(self):
+        self.base_model_path = os.path.join(os.path.dirname(__file__), "models")
+        self.features_model_name = 'selector_1028_200_with6935.pickle'
+        self.my_model_name = 'LightGBM_200_with6935.pkl'
+
         self._check()
 
         # 乏了，就这么写吧，懒得改了
         self.get_model = None
-        self.new_model = None
-        self.test_data_x = None
+        self.my_model = None
         self.load_models()
 
-    def _unzip(self, p):
-        f = zipfile.ZipFile(p, 'r')  # 压缩文件位置
-        for file in f.namelist():
-            f.extract(file, self.base_model_path)  # 解压位置
-        f.close()
-
-    def _exists(self, p, pz):
-        tmp = os.path.join(self.base_model_path, p)
-        if not os.path.exists(tmp):
-            tmpz = os.path.join(self.base_model_path, pz)
-            if os.path.exists(tmpz):
-                self._unzip(tmpz)
-            else:
-                raise OSError(f'{pz} file not found, please download it from {self.download_msg}')
-        if not os.path.exists(tmp):
-            raise OSError(f'{p} file not found, please download it from {self.download_msg}')
-
     def _check(self):
         assert os.path.exists(self.base_model_path), 'path does not exist'
-        self._exists(self.deep_tp_model_name, self.deep_tp_model_name_zip)
-        self._exists(self.features_model_name, self.features_model_name_zip)
-        self._exists(self.csv_name, self.csv_name_zip)
 
     def load_models(self):
         with open(os.path.join(self.base_model_path, self.features_model_name), 'rb') as f:
             self.get_model = pickle.load(f)
-        new_model = tf.keras.models.load_model(os.path.join(self.base_model_path, self.deep_tp_model_name),
-                                               custom_objects={'Attention': Attention})
-        # new_model.summary()
-        self.new_model = new_model
-
-        test_data = pd.read_csv(os.path.join(self.base_model_path, self.csv_name), index_col=0)
-        test_data = test_data[test_data['Sequence'].str.len() <= 1500]
-        test_data_x = test_data.drop(['uniprot_id', 'Sequence', 'temp'], axis=1).select_dtypes(exclude=['object'])
-        self.test_data_x = test_data_x
+        my_model = joblib.load(os.path.join(self.base_model_path, self.my_model_name))
+        self.my_model = my_model
 
-    def predict(self, name, seq=None):
-        if seq is None:
+    def check_seq_input2(self, name, seq):
+        names = re.findall(">([^>]*)", name.replace("\n", "").replace("\r", ""))
+        if "|" in seq and names == []:
+            seqs = []
+            temp = re.findall(r">[^>]*?\|([\w]+)\|.*\n((?:\w|\n|\r)*)", seq, re.MULTILINE)
+            if seq.count(">") != len(temp):
+                raise TypeError("Data length is not same")
+            for t in temp:
+                if len(t) == 2:
+                    if "x" in t[1].lower():
+                        names.append(t[0])
+                        # msg = "序列中不能包含X"
+                        raise TypeError("sequence contains X. The tool used to calculate the features cannot handle sequence containing X.")
+                    else:
+                        t_seqs = t[1].replace("\r", "").replace("\n", "")
+                        re_result = re.findall("([" + "".join(A_LIST) + r"]+)(.*)", t_seqs)
+
+                        if re_result and len(re_result) == 1 and re_result[0][0] == t_seqs:
+                            names.append(t[0])
+                            seqs.append(t_seqs)
+                        else:
+                            names.append(t[0])
+                            # seqs.append(WarningMsg(t[1], f"只能包含这{len(A_LIST)}个字符:{''.join(A_LIST)}, "
+                            #                              f"但是发现奇异字符: {re_result[0][1][:1]}"))
+                            raise TypeError("error input.")
+                else:
+                    raise TypeError("The length of regular matching is not 2")
+        else:
+            seqs = re.findall(">([^>]*)", seq.replace("\n", "").replace("\r", ""))
+
+        print(seqs)
+        if seqs:
+            return names[0], seqs[0]
+        else:
+            return names[0], ''
+
+    def predict(self, input_name, input_seq=None):
+        name, seq = self.check_seq_input2(input_name, input_seq)
+        if not seq:
             seq = self.get_seq_info(name)
+        if not seq:
+            raise TypeError("sequence is empty")
+        print("name", name)
+        print("seq", seq)
         support = self.get_model.get_support(True)
-        res = get_feature_from_profeat_replace(name, seq)
-        rbs = RobustScaler()
-        rbs.fit_transform(self.test_data_x)
-        res_1 = rbs.transform(res)
-        x_bio_data = np.array([res_1[1]])[:, support]
-
-        test_t_x = trans(seq)
-        test_t_x = [test_t_x]
-        max_length = 1500
-        test_t_x = sequence.pad_sequences(test_t_x, maxlen=max_length)
-        x_test_t_1 = np.reshape(test_t_x, (test_t_x.shape[0], 1500, 1))
-        test_t_x_6 = trans_6(seq)
-        test_t_x_6 = [test_t_x_6]
-        max_length = 1500
-        test_t_x_6 = sequence.pad_sequences(test_t_x_6, maxlen=max_length)
-        x_test1_t_6 = np.reshape(test_t_x_6, (test_t_x_6.shape[0], 1500, 1))
-        result = self.new_model.predict([x_test_t_1, x_test1_t_6, x_bio_data])
-        # print(result.flatten())
-        result1 = list(map(zero_or_one, result))
-        # print(result1)
-        return result.flatten()[0], 'Thermophilic protein' if result1[0] == 1 else 'Mesophilic protein'
+        res = get_all_features_from_protstab(name, seq)
+        train_data = np.array([res[1]])[:, support]
+        r = self.my_model.predict(train_data)
+        return r[0]
 
     @staticmethod
     def get_seq_info(pr_id):
+        if pr_id.startswith('>'):
+            pr_id = pr_id[1:]
+        if '\n' in pr_id:
+            raise TypeError("The input name cannot contain line breaks")
         headers = {
             'authority': 'www.uniprot.org',
             'sec-ch-ua': '"Google Chrome";v="95", "Chromium";v="95", ";Not A Brand";v="99"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'upgrade-insecure-requests': '1',
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.69 Safari/537.36',
@@ -122,12 +112,20 @@
         if '<html' in out_simple or 'http:' in out_simple:
             # out_simple = ErrorMsg("爬虫网站挂了，别试了")
             raise Exception("There are some errors with input. Please have a check.(Maybe the website is down)")
         return out_simple
 
 
 if __name__ == '__main__':
-    name = "Q4JB77"
-    seq = "MRAAVLEEYKKPLRISEVDSPSINESSEVLLQVTATGLCHGDIHIAMGEWDSQIQVNLPIILGHEVVGRVLQSNHDKIKKNDLVLVYNAFGCKNCKYCKFKEYQFCEKVKVIGVNLNGGFAEYVKIPDGDNLVRVNTSDPIKLAPLADAGLTAYNSVKDLEENSKVLIIGTGAVALIALQLLKLKNVDVTVIGENQLKLDSAEKLGADEVISIKREEDSYLSLLPGKKFDYILDYVGSTRTLAESPWLLNKKGELRIIGEFGGVLRAEEQLLVLRGLRIRGILYGSLQDLKHILDIYLKGKIDTLTTVYKLEDINEAITDVTEGKVVGRAVIVP"
-    p = ProTstab2(r'D:\_code\_github\ProTstab2\drop')
-    r, r2 = p.predict(name, seq)
-    print(r, r2)
+    # _name = ">P30177"
+    _name = ""
+    # _seq = ""
+    _seq = """>sp|P30177|YBIB_ECOLI Uncharacterized protein YbiB OS=Escherichia coli (strain K12) OX=83333 GN=ybiB PE=1 SV=1
+MDYRKIIKEIGRGKNHARDLDRDTARGLYAHMLNGEVPDLELGGVLIALRIKGEGEAEML
+GFYEAMQNHTIKLTPPAGKPMPIVIPSYNGARKQANLTPLLAILLHKLGFPVVVHGVSED
+PTRVLTETIFELMGITPTLHGGQAQAKLDEHQPVFMPVGAFCPPLEKQLAMRWRMGVRNS
+AHTLAKLATPFAEGEALRLSSVSHPEYIGRVAKFFSDIGGRALLMHGTEGEVYANPQRCP
+QINLIDREGMRVLYEKQDTAGSELLPQAKDPETTAQWIERCLAGSEPIPESLKIQMACCL
+VATGEAATISDGLARVNQAF"""
+    p = ProTstab2()
+    r = p.predict(_name, _seq)
+    print(r)
```

### Comparing `ProTstab2-1.0.2/setup.py` & `ProTstab2-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ProTstab2',  # 包名
-    version='1.0.2',  # 版本号
+    version='2.0.0',  # 版本号
     description='Protein prediction package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Jianjun Zhao',
     author_email='20204227057@stu.suda.edu.cn',
     url='http://8.133.174.28:8989/DeepTP/',
     install_requires=[
         'rpy2==3.4.5',
         'scikit-learn==0.22.2',
         'tensorflow==2.4.0',
         'pandas==1.1.5',
         'lightgbm==2.3.1',
         'requests==2.24.0',
+        'bs4',
     ],
     license='MIT',
     packages=find_packages(),
     platforms=["all"],
     python_requires='>=3.6',
     classifiers=[
         'Intended Audience :: Developers',
```

