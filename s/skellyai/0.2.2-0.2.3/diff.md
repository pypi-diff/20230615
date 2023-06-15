# Comparing `tmp/skellyai-0.2.2.tar.gz` & `tmp/skellyai-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skellyai-0.2.2.tar", last modified: Tue Jun 13 04:09:34 2023, max compression
+gzip compressed data, was "dist/skellyai-0.2.3.tar", last modified: Thu Jun 15 17:53:37 2023, max compression
```

## Comparing `skellyai-0.2.2.tar` & `skellyai-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 04:09:34.165656 skellyai-0.2.2/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-13 04:09:34.165063 skellyai-0.2.2/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-06-13 04:09:34.165833 skellyai-0.2.2/setup.cfg
--rw-r--r--   0 bennicholl   (501) staff       (20)      713 2023-06-13 04:07:51.000000 skellyai-0.2.2/setup.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 04:09:34.158360 skellyai-0.2.2/skellyai/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.2/skellyai/__init__.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 04:09:34.161947 skellyai-0.2.2/skellyai/get_multi_labels/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.2/skellyai/get_multi_labels/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     1686 2023-05-19 20:23:21.000000 skellyai-0.2.2/skellyai/get_multi_labels/get_multi_labels.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 04:09:34.164361 skellyai-0.2.2/skellyai/perform_inference/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.2/skellyai/perform_inference/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)      838 2023-06-09 19:43:52.000000 skellyai-0.2.2/skellyai/perform_inference/get_probs.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     2821 2023-06-13 04:07:29.000000 skellyai-0.2.2/skellyai/perform_inference/get_probs_mult_keywords.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.2.2/skellyai/train_transformer.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 04:09:34.160920 skellyai-0.2.2/skellyai.egg-info/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-13 04:09:33.000000 skellyai-0.2.2/skellyai.egg-info/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)      435 2023-06-13 04:09:34.000000 skellyai-0.2.2/skellyai.egg-info/SOURCES.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-06-13 04:09:33.000000 skellyai-0.2.2/skellyai.egg-info/dependency_links.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-06-13 04:09:33.000000 skellyai-0.2.2/skellyai.egg-info/requires.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       62 2023-06-13 04:09:33.000000 skellyai-0.2.2/skellyai.egg-info/top_level.txt
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-15 17:53:37.908238 skellyai-0.2.3/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-15 17:53:37.907896 skellyai-0.2.3/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-06-15 17:53:37.908354 skellyai-0.2.3/setup.cfg
+-rw-r--r--   0 bennicholl   (501) staff       (20)      713 2023-06-15 17:51:18.000000 skellyai-0.2.3/setup.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-15 17:53:37.901695 skellyai-0.2.3/skellyai/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.3/skellyai/__init__.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-15 17:53:37.905362 skellyai-0.2.3/skellyai/get_multi_labels/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.3/skellyai/get_multi_labels/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     1686 2023-05-19 20:23:21.000000 skellyai-0.2.3/skellyai/get_multi_labels/get_multi_labels.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-15 17:53:37.907368 skellyai-0.2.3/skellyai/perform_inference/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.3/skellyai/perform_inference/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)      838 2023-06-09 19:43:52.000000 skellyai-0.2.3/skellyai/perform_inference/get_probs.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     2983 2023-06-15 17:49:38.000000 skellyai-0.2.3/skellyai/perform_inference/get_probs_mult_keywords.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.2.3/skellyai/train_transformer.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-15 17:53:37.904429 skellyai-0.2.3/skellyai.egg-info/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-15 17:53:37.000000 skellyai-0.2.3/skellyai.egg-info/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)      435 2023-06-15 17:53:37.000000 skellyai-0.2.3/skellyai.egg-info/SOURCES.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-06-15 17:53:37.000000 skellyai-0.2.3/skellyai.egg-info/dependency_links.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-06-15 17:53:37.000000 skellyai-0.2.3/skellyai.egg-info/requires.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       62 2023-06-15 17:53:37.000000 skellyai-0.2.3/skellyai.egg-info/top_level.txt
```

### Comparing `skellyai-0.2.2/setup.py` & `skellyai-0.2.3/setup.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-from setuptools import setupsetup(    name='skellyai',    version='0.2.2',        description='generated labeled data',    author='Ben Nicholl',    author_email='ben.nicholl66@gmail.com',    license='BSD 2-clause',    packages=['skellyai', 'skellyai/perform_inference', 'skellyai/get_multi_labels'],    install_requires=[                      'pandas==1.4.4',                      'sagemaker==2.155.0'                      ],    classifiers=[        'Development Status :: 1 - Planning',        'Intended Audience :: Science/Research',        'License :: OSI Approved :: BSD License',          'Operating System :: POSIX :: Linux',                "Programming Language :: Python :: 3"    ],)
+from setuptools import setupsetup(    name='skellyai',    version='0.2.3',        description='generated labeled data',    author='Ben Nicholl',    author_email='ben.nicholl66@gmail.com',    license='BSD 2-clause',    packages=['skellyai', 'skellyai/perform_inference', 'skellyai/get_multi_labels'],    install_requires=[                      'pandas==1.4.4',                      'sagemaker==2.155.0'                      ],    classifiers=[        'Development Status :: 1 - Planning',        'Intended Audience :: Science/Research',        'License :: OSI Approved :: BSD License',          'Operating System :: POSIX :: Linux',                "Programming Language :: Python :: 3"    ],)
```

### Comparing `skellyai-0.2.2/skellyai/get_multi_labels/get_multi_labels.py` & `skellyai-0.2.3/skellyai/get_multi_labels/get_multi_labels.py`

 * *Files identical despite different names*

### Comparing `skellyai-0.2.2/skellyai/perform_inference/get_probs.py` & `skellyai-0.2.3/skellyai/perform_inference/get_probs.py`

 * *Files identical despite different names*

### Comparing `skellyai-0.2.2/skellyai/perform_inference/get_probs_mult_keywords.py` & `skellyai-0.2.3/skellyai/perform_inference/get_probs_mult_keywords.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-import pandas as pdimport timefrom sagemaker.pytorch.model import PyTorchPredictorfrom sagemaker.deserializers import JSONDeserializerfrom sagemaker.serializers import JSONSerializerfrom sagemaker.predictor_async import AsyncPredictorfrom sagemaker.predictor import Predictordef get_probs(endpoint_key, sentences, questions, append_data_back = None, threshold = 0.6):        if type(questions) != list:        raise TypeError("questions parameter must be of type list, with string values inside of that list!")        list_of_probs_for_all_cats = []    for question in questions:            data = {"sentences" : sentences,                     "questions": [question]}                predictor = Predictor(endpoint_name=endpoint_key, serializer=JSONSerializer(), deserializer=JSONDeserializer())        async_predictor = AsyncPredictor(predictor)                        result = async_predictor.predict_async(data, "s3://ask-t5-stage/async_inference/ip")                list_of_probs_for_specific_cat = []                while True:            try:                results = result.get_result()                for result in results:                    list_of_probs_for_specific_cat.append(result[1])                                list_of_probs_for_all_cats.append(list_of_probs_for_specific_cat)                break            except:                time.sleep(5)        transpose_list_of_probs_for_all_cats = [list(i) for i in zip(*list_of_probs_for_all_cats)]    probs_df = pd.DataFrame( transpose_list_of_probs_for_all_cats)    probs_df.columns = questions        """nelow code up until the if isinstance line is responsible for creating a thrid column that has the     respective categories assigned to the respective sentences """    label_results = []    for row in transpose_list_of_probs_for_all_cats:        row_result = []        for i, element in enumerate(row):            if element > threshold:                row_result.append(questions[i])        label_results.append(row_result)    probs_df['labels'] = label_results                if isinstance(append_data_back, pd.DataFrame):            append_data_back.reset_index(drop=True, inplace=True)        probs_df.reset_index(drop=True, inplace=True)        original_df_with_probs = pd.concat([append_data_back, probs_df], axis=1)                return original_df_with_probs        elif isinstance(append_data_back, list):        df_with_sentences = pd.DataFrame(append_data_back, columns = ['sentences'])        df_with_sentences = pd.concat([df_with_sentences, probs_df], axis=1)        return df_with_sentences        elif append_data_back == None:                return probs_df            else:        raise TypeError("df parameter must be of type pandas dataframe!")        
+import pandas as pdimport timefrom sagemaker.pytorch.model import PyTorchPredictorfrom sagemaker.deserializers import JSONDeserializerfrom sagemaker.serializers import JSONSerializerfrom sagemaker.predictor_async import AsyncPredictorfrom sagemaker.predictor import Predictordef get_probs(endpoint_key, sentences, questions, append_data_back = None, threshold = 0.6):        if type(questions) != list:        raise TypeError("questions parameter must be of type list, with string values inside of that list!")        list_of_probs_for_all_cats = []    for question in questions:            data = {"sentences" : sentences,                     "questions": [question]}                predictor = Predictor(endpoint_name=endpoint_key, serializer=JSONSerializer(), deserializer=JSONDeserializer())        async_predictor = AsyncPredictor(predictor)                        result = async_predictor.predict_async(data, "s3://ask-t5-stage/async_inference/ip")                list_of_probs_for_specific_cat = []                while True:            try:                results = result.get_result()                for result in results:                    list_of_probs_for_specific_cat.append(result[1])                                list_of_probs_for_all_cats.append(list_of_probs_for_specific_cat)                break            except Exception as e:                if 'Inference could still be running' in str(e):                    time.sleep(5)                else:                    raise(str(e))        transpose_list_of_probs_for_all_cats = [list(i) for i in zip(*list_of_probs_for_all_cats)]    probs_df = pd.DataFrame( transpose_list_of_probs_for_all_cats)    probs_df.columns = questions        """nelow code up until the if isinstance line is responsible for creating a thrid column that has the     respective categories assigned to the respective sentences """    label_results = []    for row in transpose_list_of_probs_for_all_cats:        row_result = []        for i, element in enumerate(row):            if element > threshold:                row_result.append(questions[i])        label_results.append(row_result)    probs_df['labels'] = label_results                if isinstance(append_data_back, pd.DataFrame):            append_data_back.reset_index(drop=True, inplace=True)        probs_df.reset_index(drop=True, inplace=True)        original_df_with_probs = pd.concat([append_data_back, probs_df], axis=1)                return original_df_with_probs        elif isinstance(append_data_back, list):        df_with_sentences = pd.DataFrame(append_data_back, columns = ['sentences'])        df_with_sentences = pd.concat([df_with_sentences, probs_df], axis=1)        return df_with_sentences        elif append_data_back == None:                return probs_df            else:        raise TypeError("append_data_back parameter must be of type pandas dataframe or list!")
```

### Comparing `skellyai-0.2.2/skellyai/train_transformer.py` & `skellyai-0.2.3/skellyai/train_transformer.py`

 * *Files identical despite different names*

