# Comparing `tmp/pxtextmining-0.5.3.tar.gz` & `tmp/pxtextmining-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxtextmining-0.5.3.tar", max compression
+gzip compressed data, was "pxtextmining-0.5.4.tar", max compression
```

## Comparing `pxtextmining-0.5.3.tar` & `pxtextmining-0.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1068 2022-11-17 15:31:00.811802 pxtextmining-0.5.3/LICENSE
--rw-r--r--   0        0        0      949 2023-04-03 08:21:59.385245 pxtextmining-0.5.3/README.md
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.3/pxtextmining/__init__.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.3/pxtextmining/factories/__init__.py
--rw-r--r--   0        0        0    11885 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/factories/factory_data_load_and_split.py
--rw-r--r--   0        0        0     9562 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/factories/factory_model_performance.py
--rw-r--r--   0        0        0    22115 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/factories/factory_pipeline.py
--rw-r--r--   0        0        0    12046 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/factories/factory_predict_unlabelled_text.py
--rw-r--r--   0        0        0     4509 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/factories/factory_write_results.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.3/pxtextmining/helpers/__init__.py
--rw-r--r--   0        0        0      945 2023-04-03 08:21:49.655245 pxtextmining-0.5.3/pxtextmining/helpers/text_preprocessor.py
--rw-r--r--   0        0        0      625 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/helpers/tokenization.py
--rw-r--r--   0        0        0     6727 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/params.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.3/pxtextmining/pipelines/__init__.py
--rw-r--r--   0        0        0    11682 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/pipelines/multilabel_pipeline.py
--rw-r--r--   0        0        0     5531 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/pipelines/sentiment_pipeline.py
--rw-r--r--   0        0        0     1167 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 pxtextmining-0.5.3/setup.py
--rw-r--r--   0        0        0     2101 1970-01-01 00:00:00.000000 pxtextmining-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-11-17 15:31:00.811802 pxtextmining-0.5.4/LICENSE
+-rw-r--r--   0        0        0      949 2023-04-03 08:21:59.385245 pxtextmining-0.5.4/README.md
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.4/pxtextmining/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.4/pxtextmining/factories/__init__.py
+-rw-r--r--   0        0        0    12270 2023-06-15 12:35:33.524627 pxtextmining-0.5.4/pxtextmining/factories/factory_data_load_and_split.py
+-rw-r--r--   0        0        0     9562 2023-05-31 08:47:52.122923 pxtextmining-0.5.4/pxtextmining/factories/factory_model_performance.py
+-rw-r--r--   0        0        0    22249 2023-06-15 12:35:33.524627 pxtextmining-0.5.4/pxtextmining/factories/factory_pipeline.py
+-rw-r--r--   0        0        0    16813 2023-06-15 12:35:33.524627 pxtextmining-0.5.4/pxtextmining/factories/factory_predict_unlabelled_text.py
+-rw-r--r--   0        0        0     5165 2023-06-15 12:35:33.524627 pxtextmining-0.5.4/pxtextmining/factories/factory_write_results.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.4/pxtextmining/helpers/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-03 08:21:49.655245 pxtextmining-0.5.4/pxtextmining/helpers/text_preprocessor.py
+-rw-r--r--   0        0        0      625 2023-05-31 08:46:58.592917 pxtextmining-0.5.4/pxtextmining/helpers/tokenization.py
+-rw-r--r--   0        0        0     6785 2023-06-15 12:35:33.524627 pxtextmining-0.5.4/pxtextmining/params.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.4/pxtextmining/pipelines/__init__.py
+-rw-r--r--   0        0        0    15841 2023-06-15 12:35:33.524627 pxtextmining-0.5.4/pxtextmining/pipelines/multilabel_pipeline.py
+-rw-r--r--   0        0        0     5545 2023-06-15 12:35:33.524627 pxtextmining-0.5.4/pxtextmining/pipelines/sentiment_pipeline.py
+-rw-r--r--   0        0        0     1167 2023-06-15 12:35:33.524627 pxtextmining-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 pxtextmining-0.5.4/setup.py
+-rw-r--r--   0        0        0     2101 1970-01-01 00:00:00.000000 pxtextmining-0.5.4/PKG-INFO
```

### Comparing `pxtextmining-0.5.3/LICENSE` & `pxtextmining-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.3/README.md` & `pxtextmining-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.3/pxtextmining/factories/factory_data_load_and_split.py` & `pxtextmining-0.5.4/pxtextmining/factories/factory_data_load_and_split.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,33 +62,34 @@
     """
     tokenizer = AutoTokenizer.from_pretrained(model_name)
     try:
         data_encoded = dict(
             tokenizer(
                 list(X["FFT answer"]),
                 truncation=True,
-                padding=True,
+                padding="max_length",
                 max_length=max_length,
                 return_tensors="tf",
             )
         )
     except:
         data_encoded = dict(
             tokenizer(
                 list(X),
                 truncation=True,
-                padding=True,
+                padding="max_length",
                 max_length=max_length,
                 return_tensors="tf",
             )
         )
     data_encoded.pop("attention_mask", None)
     if additional_features == True:
-        onehotted = onehot(X, "FFT_q_standardised")
-        data_encoded["input_cat"] = onehotted.astype(np.float32)
+        data_encoded["input_cat"] = X["FFT_q_standardised"].map(
+            {"what_good": 0, "could_improve": 1, "nonspecific": 2}
+        )
     if Y is not None:
         data_encoded = Dataset.from_tensor_slices((data_encoded, Y))
     return data_encoded
 
 
 def load_multilabel_data(filename, target="major_categories"):
     """Function for loading the multilabel dataset, converting it from csv to pd.DataFrame. Conducts some basic preprocessing,
@@ -116,28 +117,29 @@
         cols = minor_cats
     if target == "test":
         cols = merged_minor_cats
     elif target == "sentiment":
         cols = ["Comment sentiment"]
     # Sort out the features first
     features_df = raw_data.loc[:, features].copy()
-    features_df = clean_empty_features(features_df)
     # Standardize FFT qs
+    features_df["FFT question"] = features_df["FFT question"].fillna("nonspecific")
     features_df.loc[:, "FFT_q_standardised"] = (
         features_df.loc[:, "FFT question"].map(q_map).copy()
     )
     if features_df["FFT_q_standardised"].count() != features_df.shape[0]:
         raise ValueError(
             f'Check q_map is correct. features_df.shape[0] is {features_df.shape[0]}. \n \
                          features_df["FFT_q_standardised"].count()  is {features_df["FFT_q_standardised"].count()}. \n\n\
                          Questions are: {features_df["FFT question"].value_counts()}'
         )
     features_df.loc[:, "text_length"] = features_df.loc[:, "FFT answer"].apply(
         lambda x: len([word for word in str(x).split(" ") if word != ""])
     )
+    features_df = clean_empty_features(features_df)
     # Sort out the targets
     targets_df = raw_data.loc[:, cols].copy()
     targets_df = targets_df.replace("1", 1)
     targets_df = targets_df.fillna(value=0)
     if target == "major_categories":
         for maj, min_list in major_cat_dict.items():
             targets_df = merge_categories(targets_df, maj, min_list)
@@ -174,15 +176,15 @@
     Args:
         df (pd.DataFrame): DataFrame containing data to be one-hot encoded
         col_to_onehot (list): List of column names to be one-hot encoded
 
     Returns:
         (pd.DataFrame): One-hot encoded data
     """
-    encoder = OneHotEncoder(sparse=False)
+    encoder = OneHotEncoder(sparse=False, handle_unknown="ignore")
     col_encoded = encoder.fit_transform(df[[col_to_onehot]])
     return col_encoded
 
 
 def process_data(df, target, preprocess_text=True, additional_features=False):
     """Utilises remove_punc_and_nums and clean_empty_features functions to clean the text data and
     drop any rows that are only whitespace after cleaning. Also fills one-hot encoded columns with
@@ -201,15 +203,19 @@
     """
 
     if preprocess_text == True:
         X = df["FFT answer"].astype(str).apply(remove_punc_and_nums)
         X = clean_empty_features(X)
         print(f"After preprocessing, shape of X is {X.shape}")
     if preprocess_text == False:
-        X = df["FFT answer"].astype(str)
+        X_temp = df["FFT answer"].astype(str).apply(remove_punc_and_nums)
+        X_temp = clean_empty_features(X_temp)
+        print(f"After preprocessing, shape of X is {X_temp.shape}")
+        indices = X_temp.index
+        X = df["FFT answer"].astype(str).filter(indices)
     if additional_features == True:
         X = pd.merge(X, df[["FFT_q_standardised"]], left_index=True, right_index=True)
         X = X.reset_index()
         X = X.drop_duplicates()
         X = X.set_index("Comment ID")
     if target == "sentiment":
         Y = df["Comment sentiment"].astype(int) - 1
```

### Comparing `pxtextmining-0.5.3/pxtextmining/factories/factory_model_performance.py` & `pxtextmining-0.5.4/pxtextmining/factories/factory_model_performance.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.3/pxtextmining/factories/factory_pipeline.py` & `pxtextmining-0.5.4/pxtextmining/factories/factory_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from sklearn.preprocessing import OneHotEncoder, RobustScaler
 from sklearn.svm import SVC
 from sklearn.utils.class_weight import compute_class_weight
 from sklearn.model_selection import cross_validate
 from tensorflow.keras import Sequential, layers
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.initializers import TruncatedNormal
-from tensorflow.keras.layers import Dense, Dropout, Input, concatenate
+from tensorflow.keras.layers import Dense, Dropout, Input, concatenate, CategoryEncoding
 from tensorflow.keras.losses import BinaryCrossentropy, CategoricalCrossentropy
 from tensorflow.keras.models import Model
 from tensorflow.keras.optimizers import Adam
 from transformers import DistilBertConfig, TFDistilBertForSequenceClassification
 import xgboost as xgb
 
 from pxtextmining.helpers.tokenization import spacy_tokenizer
@@ -196,17 +196,19 @@
     bert = transformer_model.layers[0]
     input_ids = Input(shape=(max_length,), name="input_ids", dtype="int32")
     input_text = {"input_ids": input_ids}
     bert_model = bert(input_text)[0][:, 0, :]
     dropout = Dropout(config.dropout, name="pooled_output")
     bert_output = dropout(bert_model, training=False)
     # Get onehotencoded categories in (3 categories)
-    input_cat = Input(shape=(3,), name="input_cat")
+    input_cat = Input(shape=(1,), name="input_cat")
+    onehot_layer = CategoryEncoding(num_tokens=3, output_mode="one_hot")
+    onehot_layer = onehot_layer(input_cat)
     cat_dense = Dense(units=10, activation="relu")
-    cat_dense = cat_dense(input_cat)
+    cat_dense = cat_dense(onehot_layer)
     # concatenate both together
     concat_layer = concatenate([bert_output, cat_dense])
     if multilabel == True:
         output = Dense(
             units=Y_train.shape[1],
             kernel_initializer=TruncatedNormal(stddev=config.initializer_range),
             activation="sigmoid",
@@ -369,79 +371,71 @@
             (cat_transformer, ["FFT_q_standardised"]),
             (vectorizer, "FFT answer"),
             # (num_transformer, ["text_length"]),
         )
         params = {
             "columntransformer__tfidfvectorizer__ngram_range": ((1, 1), (1, 2), (2, 2)),
             "columntransformer__tfidfvectorizer__max_df": [
-                0.85,
-                0.86,
-                0.87,
-                0.88,
-                0.89,
                 0.9,
-                0.91,
-                0.92,
-                0.93,
-                0.94,
                 0.95,
-                0.96,
-                0.97,
-                0.98,
                 0.99,
             ],
-            "columntransformer__tfidfvectorizer__min_df": stats.uniform(0, 0.1),
+            "columntransformer__tfidfvectorizer__min_df": [0, 0.01, 0.02],
         }
     else:
         preproc = create_sklearn_vectorizer(tokenizer=tokenizer)
         params = {
             "tfidfvectorizer__ngram_range": ((1, 1), (1, 2), (2, 2)),
             "tfidfvectorizer__max_df": stats.uniform(0.8, 1),
             "tfidfvectorizer__min_df": stats.uniform(0.01, 0.1),
         }
     if model_type == "mnb":
         pipe = make_pipeline(preproc, MultiOutputClassifier(MultinomialNB()))
         params["multioutputclassifier__estimator__alpha"] = stats.uniform(0.1, 1)
     if model_type == "knn":
         pipe = make_pipeline(preproc, KNeighborsClassifier())
-        params["kneighborsclassifier__n_neighbors"] = stats.randint(1, 50)
-        params["kneighborsclassifier__n_jobs"] = [-1]
+        params["kneighborsclassifier__n_neighbors"] = stats.randint(1, 100)
     if model_type == "svm":
         pipe = make_pipeline(
             preproc,
             MultiOutputClassifier(
                 SVC(
                     probability=True,
                     class_weight="balanced",
                     max_iter=1000,
                     cache_size=1000,
                 ),
                 n_jobs=-1,
             ),
         )
-        params["multioutputclassifier__estimator__C"] = stats.uniform(0.1, 20)
-        params["multioutputclassifier__estimator__kernel"] = [
-            "linear",
-            "rbf",
-            "sigmoid",
-        ]
+        params["multioutputclassifier__estimator__C"] = [10, 15, 20]
+        params["multioutputclassifier__estimator__gamma"] = np.logspace(-9, 3, 13)
+        # params["multioutputclassifier__estimator__kernel"] = [
+        #     "linear",
+        #     "rbf",
+        #     "sigmoid",
+        # ]
     if model_type == "rfc":
         pipe = make_pipeline(preproc, RandomForestClassifier(n_jobs=-1))
         params["randomforestclassifier__max_depth"] = stats.randint(5, 50)
         params["randomforestclassifier__min_samples_split"] = stats.randint(2, 5)
         params["randomforestclassifier__class_weight"] = [
             "balanced",
             "balanced_subsample",
             None,
         ]
         params["randomforestclassifier__min_samples_leaf"] = stats.randint(1, 10)
         params["randomforestclassifier__max_features"] = ["sqrt", "log2", None, 0.3]
     if model_type == "xgb":
-        pipe = make_pipeline(preproc, xgb.XGBClassifier(tree_method="hist"))
-
+        pipe = make_pipeline(
+            preproc, xgb.XGBClassifier(tree_method="hist", n_estimators=200)
+        )
+        params["xgbclassifier__max_depth"] = [4, 5, 6, 7, 8]
+        params["xgbclassifier__min_child_weight"] = [0.5, 1, 2, 5]
+        params["xgbclassifier__gamma"] = [0, 0.1, 0.2, 0.3, 0.4, 0.5]
     return pipe, params
 
 
 def search_sklearn_pipelines(
     X_train, Y_train, models_to_try, target=None, additional_features=True
 ):
     """Iterates through selected estimators, instantiating the relevant sklearn pipelines and searching for the optimum hyperparameters.
```

### Comparing `pxtextmining-0.5.3/pxtextmining/factories/factory_predict_unlabelled_text.py` & `pxtextmining-0.5.4/pxtextmining/factories/factory_predict_unlabelled_text.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 import numpy as np
 import pandas as pd
 
+from tensorflow.keras.saving import load_model
+
 from pxtextmining.factories.factory_data_load_and_split import (
     bert_data_to_dataset,
     remove_punc_and_nums,
+    clean_empty_features,
 )
 from pxtextmining.params import minor_cats
 
+
 def process_text(text):
-    """ Enacts same text preprocessing as is found in factory_data_load_and_split when creating training data. Converts to string, removes trailing whitespaces, null values, punctuation and numbers. Converts to lowercase.
+    """Enacts same text preprocessing as is found in factory_data_load_and_split when creating training data. Converts to string, removes trailing whitespaces, null values, punctuation and numbers. Converts to lowercase.
 
     Args:
         text (pd.Series): Series containing data to be cleaned.
 
     Returns:
         (pd.Series): Processed text data
     """
     text_as_str = text.astype(str)
     text_stripped = text_as_str.str.strip()
-    text_no_whitespace = text_stripped.replace([r"^\s*$", r"(?i)^nan$", r"(?i)^null$", r"(?i)^n\/a$"],
-                                             np.nan, regex=True)
+    text_no_whitespace = text_stripped.replace(
+        [r"^\s*$", r"(?i)^nan$", r"(?i)^null$", r"(?i)^n\/a$"], np.nan, regex=True
+    )
     text_no_nans = text_no_whitespace.dropna()
     text_cleaned = text_no_nans.astype(str).apply(remove_punc_and_nums)
     processed_text = text_cleaned.replace(r"^\s*$", np.nan, regex=True).dropna()
     return processed_text
 
 
 def predict_multilabel_sklearn(
     data,
     model,
-    labels = minor_cats,
-    additional_features = False,
-    label_fix = True,
-    enhance_with_probs = True
+    labels=minor_cats,
+    additional_features=False,
+    label_fix=True,
+    enhance_with_probs=True,
 ):
     """Conducts basic preprocessing to remove punctuation and numbers.
     Utilises a pretrained sklearn machine learning model to make multilabel predictions on the cleaned text.
     Also takes the class with the highest predicted probability as the predicted class in cases where no class has
     been predicted, if fix_no_labels = True.
 
     Args:
@@ -49,55 +54,154 @@
 
     Returns:
         (pd.DataFrame): DataFrame containing one hot encoded predictions, and a column with a list of the predicted labels.
     """
     if additional_features == False:
         text = pd.Series(data)
     else:
-        text = data['FFT answer']
+        text = data["FFT answer"]
     processed_text = process_text(text)
     if additional_features == False:
         final_data = processed_text
     else:
-        final_data = pd.merge(processed_text, data['FFT_q_standardised'], how='left', on='Comment ID')
+        final_data = pd.merge(
+            processed_text, data["FFT_q_standardised"], how="left", on="Comment ID"
+        )
     binary_preds = model.predict(final_data)
     pred_probs = np.array(model.predict_proba(final_data))
     if label_fix == True:
         predictions = fix_no_labels(binary_preds, pred_probs, model_type="sklearn")
     else:
         predictions = binary_preds
     if enhance_with_probs == True:
         for row in range(predictions.shape[0]):
             for label_index in range(predictions.shape[1]):
-                prob_of_label = pred_probs[label_index, row, 1]
+                if pred_probs.ndim == 3:
+                    prob_of_label = pred_probs[label_index, row, 1]
+                if pred_probs.ndim == 2:
+                    prob_of_label = pred_probs[row, label_index]
                 if prob_of_label > 0.5:
                     predictions[row][label_index] = 1
     preds_df = pd.DataFrame(predictions, index=processed_text.index, columns=labels)
     preds_df["labels"] = preds_df.apply(get_labels, args=(labels,), axis=1)
     return preds_df
 
+
+def predict_multilabel_bert(
+    data, model, labels=minor_cats, additional_features=False, label_fix=True
+):
+    """Conducts basic preprocessing to remove blank text.
+    Utilises a pretrained transformer-based machine learning model to make multilabel predictions on the cleaned text.
+    Also takes the class with the highest predicted probability as the predicted class in cases where no class has
+    been predicted, if fix_no_labels = True.
+
+    Args:
+        text (pd.Series OR pd.DataFrame): DataFrame or Series containing data to be processed and utilised for predictions. Must be DataFrame with columns 'FFT answer' and 'FFT_q_standardised' if additional_features = True
+        model (tf.Model): Trained tensorflow estimator able to perform multilabel classification.
+        labels (list, optional): List containing target labels. Defaults to major_cats.
+        additional_features (bool, optional): Whether or not FFT_q_standardised is included in data. Defaults to False.
+        label_fix (bool, optional): Whether or not the class with the highest probability is taken as the predicted class in cases where no classes are predicted. Defaults to True.
+
+    Returns:
+        (pd.DataFrame): DataFrame containing one hot encoded predictions, and a column with a list of the predicted labels.
+    """
+    if additional_features == False:
+        text = pd.Series(data)
+    else:
+        text = data["FFT answer"]
+    processed_text = clean_empty_features(text)
+    if additional_features == False:
+        final_data = processed_text
+    else:
+        final_data = pd.merge(
+            processed_text, data["FFT_q_standardised"], how="left", on="Comment ID"
+        )
+    y_probs = predict_with_bert(
+        final_data,
+        model,
+        additional_features=additional_features,
+        already_encoded=False,
+    )
+    y_binary = turn_probs_into_binary(y_probs)
+    if label_fix == True:
+        predictions = fix_no_labels(y_binary, y_probs, model_type="bert")
+    else:
+        predictions = y_binary
+    preds_df = pd.DataFrame(predictions, index=processed_text.index, columns=labels)
+    preds_df["labels"] = preds_df.apply(get_labels, args=(labels,), axis=1)
+    return preds_df
+
+
+def predict_sentiment_bert(
+    data, model, additional_features=False, preprocess_text=False
+):
+    """Conducts basic preprocessing to remove blank text.
+    Utilises a pretrained transformer-based machine learning model to make multilabel predictions on the cleaned text.
+    Also takes the class with the highest predicted probability as the predicted class in cases where no class has
+    been predicted, if fix_no_labels = True.
+
+    Args:
+        text (pd.Series OR pd.DataFrame): DataFrame or Series containing data to be processed and utilised for predictions. Must be DataFrame with columns 'FFT answer' and 'FFT_q_standardised' if additional_features = True
+        model (tf.Model): Trained tensorflow estimator able to perform multilabel classification.
+        additional_features (bool, optional): Whether or not FFT_q_standardised is included in data. Defaults to False.
+        preprocess_text (bool, optional): Whether or not text is to be preprocessed (punctuation and numbers removed).
+
+    Returns:
+        (pd.DataFrame): DataFrame containing input data and predicted sentiment
+    """
+    if additional_features == False:
+        text = pd.Series(data)
+    else:
+        text = data["FFT answer"]
+    if preprocess_text == True:
+        processed_text = text.astype(str).apply(remove_punc_and_nums)
+        processed_text = clean_empty_features(processed_text).dropna()
+    else:
+        processed_text = clean_empty_features(text).dropna()
+    if additional_features == False:
+        final_data = processed_text
+        final_data = clean_empty_features(final_data)
+    else:
+        final_data = pd.merge(
+            processed_text, data["FFT_q_standardised"], how="left", on="Comment ID"
+        )
+    final_index = final_data.index
+    predictions = predict_multiclass_bert(
+        final_data, model, additional_features, already_encoded=False
+    )
+    preds_df = data.filter(items=final_index, axis=0)
+    preds_df["sentiment"] = predictions
+    preds_df["sentiment"] = preds_df["sentiment"] + 1
+    return preds_df
+
+
 def predict_multiclass_bert(x, model, additional_features, already_encoded):
     """Makes multiclass predictions using a transformer-based model. Can encode the data if not already encoded.
 
     Args:
         x (pd.DataFrame): DataFrame containing features to be passed through model.
         model (tf.keras.models.Model): Pretrained transformer based model in tensorflow keras.
         additional_features (bool, optional): Whether or not additional features (e.g. question type) are included. Defaults to False.
         already_encoded (bool, optional): Whether or not the input data needs to be encoded. Defaults to False.
 
     Returns:
         (np.array): Predicted labels in one-hot encoded format.
     """
-    y_probs = predict_with_bert(x, model, additional_features = additional_features,
-                           already_encoded = already_encoded)
+    y_probs = predict_with_bert(
+        x,
+        model,
+        additional_features=additional_features,
+        already_encoded=already_encoded,
+    )
     y_binary = turn_probs_into_binary(y_probs)
-    y_binary_fixed = fix_no_labels(y_binary, y_probs, model_type = 'bert')
+    y_binary_fixed = fix_no_labels(y_binary, y_probs, model_type="bert")
     y_preds = np.argmax(y_binary_fixed, axis=1)
     return y_preds
 
+
 def predict_with_probs(x, model, labels):
     """Given a trained model and some features, makes predictions based on the model's outputted probabilities using the model.predict_proba function.
     Any label with a predicted probability over 0.5 is taken as the predicted label. If no labels are over 0.5 probability then the
     label with the highest probability is taken.
     Converts into one-hot encoded format (similar to what model.predict would output).
     Currently only works with sklearn models.
 
@@ -121,29 +225,30 @@
         probabilities.append(label_probs)
     probability_s = pd.Series(probabilities)
     probability_s.index = x.index
     # Parse dict of probabilities into one hot encoded format
     prob_preds = []
     for d in range(len(probability_s)):
         row_preds = [0] * len(labels)
-        for k,v in probability_s.iloc[d].items():
+        for k, v in probability_s.iloc[d].items():
             max_val = 0
             if v > max_val:
                 max_k = k
             if v > 0.5:
                 index_over_5 = labels.index(k)
                 row_preds[index_over_5] = 1
         if sum(row_preds) == 0:
             index_max = labels.index(max_k)
             row_preds[index_max] = 1
         prob_preds.append(row_preds)
     np.array(prob_preds).shape
     y_pred = np.array(prob_preds)
     return y_pred
 
+
 def get_probabilities(label_series, labels, predicted_probabilities, model_type):
     """Given a pd.Series containing labels, the list of labels, and a model's outputted predicted_probabilities for each label,
     create a dictionary containing the label and the predicted probability of that label.
 
     Args:
         label_series (pd.Series): Series containing labels in the format `['label_one', 'label_two']`
         labels (list): List of the label names
@@ -155,25 +260,29 @@
     """
     probabilities = []
     for i in range(label_series.shape[0]):
         label_probs = {}
         predicted_labels = label_series.iloc[i]
         for each in predicted_labels:
             index_label = labels.index(each)
-            if model_type == 'sklearn':
-                prob_of_label = predicted_probabilities[index_label, i, 1]
-            elif model_type in ('tf', 'bert'):
+            if model_type == "sklearn":
+                if predicted_probabilities.ndim == 3:
+                    prob_of_label = predicted_probabilities[index_label, i, 1]
+                else:
+                    prob_of_label = predicted_probabilities[i][index_label]
+            elif model_type in ("tf", "bert"):
                 prob_of_label = predicted_probabilities[i][index_label]
             label_probs[each] = round(prob_of_label, 5)
         probabilities.append(label_probs)
     probability_s = pd.Series(probabilities)
     probability_s.index = label_series.index
-    probability_s.name = f'{label_series.name}_probabilities'
+    probability_s.name = f"{label_series.name}_probabilities"
     return probability_s
 
+
 def get_labels(row, labels):
     """Given a one-hot encoded row of predictions from a dataframe,
     returns a list containing the actual predicted labels as a `str`.
 
     Args:
         row (pd.DataFrame): Row in a DataFrame containing one-hot encoded predicted labels.
         labels (list): List containing all the target labels, which should also be columns in the dataframe.
@@ -222,21 +331,25 @@
         binary_preds (np.array): Predicted labels, in a one-hot encoded binary format. Some rows may not have any predicted labels.
         predicted_probs (np.array): Predicted probability of each label.
         model_type (str, optional): Whether the model is a sklearn or tensorflow keras model; options are 'tf', 'bert', or 'sklearn. Defaults to "sklearn".
 
     Returns:
         (np.array): Predicted labels in one-hot encoded format, with all rows containing at least one predicted label.
     """
+
     for i in range(len(binary_preds)):
         if binary_preds[i].sum() == 0:
             if model_type in ("tf", "bert"):
                 # index_max = list(predicted_probs[i]).index(max(predicted_probs[i])
                 index_max = np.argmax(predicted_probs[i])
             if model_type == "sklearn":
-                index_max = np.argmax(predicted_probs[:, i, 1])
+                if predicted_probs.ndim == 3:
+                    index_max = np.argmax(predicted_probs[:, i, 1])
+                else:
+                    index_max = np.argmax(predicted_probs[i])
             binary_preds[i][index_max] = 1
     return binary_preds
 
 
 def turn_probs_into_binary(predicted_probs):
     """Takes predicted probabilities (floats between 0 and 1) and converts these to binary outcomes.
     Scope to finetune this in later iterations of the project depending on the label and whether recall/precision
```

### Comparing `pxtextmining-0.5.3/pxtextmining/factories/factory_write_results.py` & `pxtextmining-0.5.4/pxtextmining/factories/factory_write_results.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import pickle
 import os
 import numpy as np
 import pandas as pd
 
-from pxtextmining.factories.factory_predict_unlabelled_text import get_labels, predict_multilabel_sklearn, predict_with_probs, get_probabilities
 from tensorflow.keras import Model, Sequential
+from pxtextmining.factories.factory_predict_unlabelled_text import (
+    get_labels,
+    predict_multilabel_sklearn,
+    predict_multilabel_bert,
+    get_probabilities,
+    predict_with_bert
+)
 from pxtextmining.factories.factory_model_performance import parse_metrics_file
 
 
 def write_multilabel_models_and_metrics(models, model_metrics, path):
     """Saves models and their associated performance metrics into a specified folder
 
     Args:
@@ -20,56 +26,91 @@
         model_name = f"model_{i}"
         if not os.path.exists(path):
             os.makedirs(path)
         fullpath = os.path.join(path, model_name)
         if isinstance(models[i], (Sequential, Model)):
             models[i].save(fullpath)
         else:
-            modelpath = os.path.join(path, model_name + '.sav')
+            modelpath = os.path.join(path, model_name + ".sav")
             pickle.dump(models[i], open(modelpath, "wb"))
         # Write performance metrics file
-        txtpath = os.path.join(path, model_name + '.txt')
+        txtpath = os.path.join(path, model_name + ".txt")
         with open(txtpath, "w") as file:
             file.write(model_metrics[i])
     print(f"{len(models)} models have been written to {path}")
 
-def write_model_preds(x, y, model, labels, additional_features = True, path = 'labels.xlsx'):
+
+def write_model_preds(
+    x, y, model, labels, additional_features=True, path="labels.xlsx"
+):
     """Writes an Excel file to enable easier analysis of model outputs using the test set. Columns of the Excel file are: comment_id, actual_labels, predicted_labels, actual_label_probs, and predicted_label_probs.
 
     Currently only works with sklearn models.
 
     Args:
         x (pd.DataFrame): Features to be used to make the prediction.
         y (np.array): Numpy array containing the targets, in one-hot encoded format
         model (sklearn.base): Trained sklearn multilabel classifier.
         labels (list): List of labels for the categories to be predicted.
         additional_features (bool, optional): Whether or not FFT_q_standardised is included in data. Defaults to True.
         path (str, optional): Filename for the outputted file. Defaults to 'labels.xlsx'.
     """
-    actual_labels = pd.DataFrame(y, columns = labels).apply(get_labels, args=(labels,), axis=1)
-    actual_labels.name = 'actual_labels'
-    predicted_labels = predict_multilabel_sklearn(x,
-                                                  model,
-                                                  labels=labels,
-                                                  additional_features = additional_features,
-                                                  label_fix = True,
-                                                  enhance_with_probs=True
-                                                ).reset_index()['labels']
-    predicted_labels.name = 'predicted_labels'
+    actual_labels = pd.DataFrame(y, columns=labels).apply(
+        get_labels, args=(labels,), axis=1
+    )
+    actual_labels.name = "actual_labels"
+    if isinstance(model, Model) == True:
+        predicted_labels = predict_multilabel_bert(
+            x,
+            model,
+            labels=labels,
+            additional_features=additional_features,
+            label_fix=True,
+        ).reset_index()["labels"]
+    else:
+        predicted_labels = predict_multilabel_sklearn(
+            x,
+            model,
+            labels=labels,
+            additional_features=additional_features,
+            label_fix=True,
+            enhance_with_probs=True,
+        ).reset_index()["labels"]
+    predicted_labels.name = "predicted_labels"
     df = x.reset_index()
+    if isinstance(model, Model) == True:
+        probabilities = predict_with_bert(
+            x,
+            model,
+            max_length=150,
+            additional_features=additional_features,
+            already_encoded=False,
+        )
+    else:
+        probabilities = np.array(model.predict_proba(x))
+    if isinstance(model, Model) == True:
+        model_type = 'bert'
+    else:
+        model_type = 'sklearn'
+    probs_actual = get_probabilities(
+        actual_labels, labels, probabilities, model_type=model_type
+    )
+    probs_predicted = get_probabilities(
+        predicted_labels, labels, probabilities, model_type=model_type
+    )
+    df = df.merge(actual_labels, left_index=True, right_index=True)
+    df = df.merge(predicted_labels, left_index=True, right_index=True)
+    df = df.merge(probs_actual, left_index=True, right_index=True)
+    df = df.merge(probs_predicted, left_index=True, right_index=True)
+    # Deal with any rogue characters
+    df.applymap(lambda x: x.encode('unicode_escape').
+                 decode('utf-8') if isinstance(x, str) else x)
+    df.to_excel(path, index=False)
+    print(f"Successfully completed, written to {path}")
 
-    probabilities = np.array(model.predict_proba(x))
-    probs_actual = get_probabilities(actual_labels, labels, probabilities, model_type = 'sklearn')
-    probs_predicted = get_probabilities(predicted_labels, labels, probabilities, model_type = 'sklearn')
-    df = df.merge(actual_labels, left_index = True, right_index = True)
-    df = df.merge(predicted_labels, left_index = True, right_index = True)
-    df = df.merge(probs_actual, left_index = True, right_index = True)
-    df = df.merge(probs_predicted, left_index = True, right_index = True)
-    df.to_excel(path, index = False)
-    print(f'Successfully completed, written to {path}')
 
 def write_model_analysis(model_name, labels, dataset, path):
     """Writes an Excel file with the performance metrics of each label, as well as the counts of samples for each label.
 
     Args:
         model_name (str): Model name used in the performance metrics file
         labels (list): List of labels for the categories to be predicted.
```

### Comparing `pxtextmining-0.5.3/pxtextmining/helpers/text_preprocessor.py` & `pxtextmining-0.5.4/pxtextmining/helpers/text_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.3/pxtextmining/helpers/tokenization.py` & `pxtextmining-0.5.4/pxtextmining/helpers/tokenization.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.3/pxtextmining/params.py` & `pxtextmining-0.5.4/pxtextmining/params.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,196 +1,201 @@
-dataset = "datasets/hidden/multilabel_230522.csv"
+dataset = "datasets/hidden/v6merged_230612.csv"
+
+random_state = 42
 
 model_name = "distilbert-base-uncased"
 
 q_map = {
-        "Please tell us why": "nonspecific",
-        "Please tells us why you gave this answer?": "nonspecific",
-        "FFT Why?": "nonspecific",
-        "What was good?": "what_good",
-        "Is there anything we could have done better?": "could_improve",
-        "How could we improve?": "could_improve",
-        "What could we do better?": "could_improve",
-        "Please can you tell us why you gave your answer and what we could have done better?": "nonspecific",
-        "Please describe any things about the 111 service that\r\nyou were particularly satisfied and/or dissatisfied with": "nonspecific",
-        "Please describe any things about the 111 service that \nyou were particularly satisfied and/or dissatisfied with": "nonspecific",
-        "Please describe any things about the 111 service that\nyou were particularly satisfied and/or dissatisfied with": 'nonspecific',
-        "Nonspecific": 'nonspecific',
-        "nonspecific": 'nonspecific'
-    }
+    "Please tell us why": "nonspecific",
+    "Please tells us why you gave this answer?": "nonspecific",
+    "FFT Why?": "nonspecific",
+    "What was good?": "what_good",
+    "Is there anything we could have done better?": "could_improve",
+    "How could we improve?": "could_improve",
+    "What could we do better?": "could_improve",
+    "Please can you tell us why you gave your answer and what we could have done better?": "nonspecific",
+    "Please describe any things about the 111 service that\r\nyou were particularly satisfied and/or dissatisfied with": "nonspecific",
+    "Please describe any things about the 111 service that \nyou were particularly satisfied and/or dissatisfied with": "nonspecific",
+    "Please describe any things about the 111 service that\nyou were particularly satisfied and/or dissatisfied with": "nonspecific",
+    "Nonspecific": "nonspecific",
+    "nonspecific": "nonspecific",
+}
 
+# v6
 major_cat_dict = {
     "General": [
-        "Gratitude/ good experience",
-        "Negative experience",
+        "Labelling not possible",
+        "Positive experience & gratitude",
+        "Negative experience & dissatisfaction",
         "Not assigned",
         "Organisation & efficiency",
         "Funding & use of financial resources",
-        "Collecting patients feedback",
     ],
     "Staff": [
-        "Non-specific praise for staff",
-        "Non-specific dissatisfaction with staff",
         "Staff manner & personal attributes",
         "Number & deployment of staff",
         "Staff responsiveness",
         "Staff continuity",
         "Competence & training",
     ],
     "Communication & involvement": [
         "Unspecified communication",
         "Staff listening, understanding & involving patients",
         "Information directly from staff during care",
         "Information provision & guidance",
         "Being kept informed, clarity & consistency of information",
-        "Service involvement with family/ carers",
-        "Patient contact with family/ carers",
+        "Interaction with family/ carers",
     ],
     "Access to medical care & support": [
         "Contacting services",
         "Appointment arrangements",
         "Appointment method",
         "Timeliness of care",
     ],
     "Medication": ["Supplying & understanding medication", "Pain management"],
     "Patient journey & service coordination": [
         "Diagnosis & triage",
         "Referals & continuity of care",
         "Admission",
-        "Length of stay/ duration of care",
         "Discharge",
         "Care plans",
         "Patient records",
         "Impact of treatment/ care",
-        "Links with non-NHS organisations",
     ],
     "Food & diet": ["Food & drink provision & facilities"],
     "Category TBC": [
         "Feeling safe",
         "Patient appearance & grooming",
         "Equality, Diversity & Inclusion",
     ],
     "Activities": ["Activities & access to fresh air", "Electronic entertainment"],
     "Environment & equipment": [
         "Cleanliness, tidiness & infection control",
         "Sensory experience",
         "Environment & Facilities",
-        "Safety & security",
         "Provision of medical equipment",
     ],
     "Mental Health specifics": ["Mental Health Act"],
     "Service location, travel & transport": [
         "Service location",
         "Transport to/ from services",
         "Parking",
     ],
 }
 
 major_cats = list(major_cat_dict.keys())
 
-# v5 20230420
+# v6 20230602
 merged_minor_cats = [
     "Gratitude/ good experience",
+    #     "Negative experience",
     "Not assigned",
     "Organisation & efficiency",
-    "Funding & use of financial resources",
+    #     "Funding & use of financial resources",
     "Non-specific praise for staff",
+    #     "Non-specific dissatisfaction with staff",
     "Staff manner & personal attributes",
     "Number & deployment of staff",
     "Staff responsiveness",
     "Staff continuity",
     "Competence & training",
     "Unspecified communication",
     "Staff listening, understanding & involving patients",
     "Information directly from staff during care",
     "Information provision & guidance",
     "Being kept informed, clarity & consistency of information",
+    #     "Service involvement with family/ carers",
+    #     "Patient contact with family/ carers",
     "Contacting services",
     "Appointment arrangements",
     "Appointment method",
     "Timeliness of care",
     "Pain management",
     "Diagnosis & triage",
+    "Referals & continuity of care",
+    #     "Length of stay/ duration of care",
+    "Discharge",
     "Care plans",
+    #     "Patient records",
+    #     "Links with non-NHS organisations",
     "Cleanliness, tidiness & infection control",
-    "Provision of medical equipment",
+    "Safety & security",
+    #     "Provision of medical equipment",
     "Service location",
     "Transport to/ from services",
     "Parking",
     "Electronic entertainment",
+    "Feeling safe",
     "Patient appearance & grooming",
     "Mental Health Act",
     "Equality, Diversity & Inclusion",
-    "Collecting patients feedback",
+    "Admission",
+    #     "Collecting patients feedback",
     "Labelling not possible",
     "Environment & Facilities",
     "Supplying & understanding medication",
     "Activities & access to fresh air",
     "Food & drink provision & facilities",
     "Sensory experience",
     "Impact of treatment/ care",
-    "Safety",
-    "Family/ carers",
     "Negative experience/ dissatisfaction",
-    "Patient journey",
+    "Family/ carers",
 ]
 
-# v5 20230419
+# v6 20230806
 minor_cats = [
-    "Gratitude/ good experience",
-    "Negative experience",
     "Not assigned",
     "Organisation & efficiency",
     "Funding & use of financial resources",
-    "Non-specific praise for staff",
-    "Non-specific dissatisfaction with staff",
     "Staff manner & personal attributes",
     "Number & deployment of staff",
     "Staff responsiveness",
     "Staff continuity",
     "Competence & training",
     "Unspecified communication",
     "Staff listening, understanding & involving patients",
     "Information directly from staff during care",
     "Information provision & guidance",
     "Being kept informed, clarity & consistency of information",
-    "Service involvement with family/ carers",
-    "Patient contact with family/ carers",
     "Contacting services",
     "Appointment arrangements",
     "Appointment method",
     "Timeliness of care",
     "Pain management",
     "Diagnosis & triage",
     "Referals & continuity of care",
-    "Length of stay/ duration of care",
     "Discharge",
     "Care plans",
     "Patient records",
-    "Links with non-NHS organisations",
     "Cleanliness, tidiness & infection control",
-    "Safety & security",
     "Provision of medical equipment",
     "Service location",
     "Transport to/ from services",
     "Parking",
     "Electronic entertainment",
     "Feeling safe",
     "Patient appearance & grooming",
     "Mental Health Act",
     "Equality, Diversity & Inclusion",
     "Admission",
-    "Collecting patients feedback",
     "Labelling not possible",
     "Environment & Facilities",
     "Supplying & understanding medication",
     "Activities & access to fresh air",
     "Food & drink provision & facilities",
     "Sensory experience",
     "Impact of treatment/ care",
+    # "Psychological therapy arrangements",
+    # "Existence of services",
+    # "Choice of services",
+    # "Out of hours support (community services)",
+    # "Learning organisation",
+    "Interaction with family/ carers",
+    "Negative experience & dissatisfaction",
+    "Positive experience & gratitude",
 ]
 
 sentiment_dict = {
     1: "very positive",
     2: "positive",
     3: "neutral",
     4: "negative",
```

### Comparing `pxtextmining-0.5.3/pxtextmining/pipelines/multilabel_pipeline.py` & `pxtextmining-0.5.4/pxtextmining/pipelines/multilabel_pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 import random
 import pandas as pd
+import os
+
+# import warnings filter
+from warnings import simplefilter
+
+# ignore all future warnings
+simplefilter(action="ignore", category=FutureWarning)
+
 
 from sklearn.model_selection import train_test_split
 
 from pxtextmining.factories.factory_data_load_and_split import (
     bert_data_to_dataset,
     load_multilabel_data,
     process_and_split_data,
@@ -21,80 +29,95 @@
     search_sklearn_pipelines,
     train_bert_model,
     train_tf_model,
 )
 from pxtextmining.factories.factory_write_results import (
     write_multilabel_models_and_metrics,
     write_model_preds,
-    write_model_analysis
+    write_model_analysis,
 )
 from pxtextmining.helpers.text_preprocessor import tf_preprocessing
-from pxtextmining.params import major_cats, minor_cats, dataset, merged_minor_cats
+from pxtextmining.params import (
+    major_cats,
+    minor_cats,
+    dataset,
+    merged_minor_cats,
+    major_cat_dict,
+    random_state,
+)
 
 
 def run_sklearn_pipeline(
     additional_features=False,
     target=major_cats,
     models_to_try=["mnb", "knn", "svm", "rfc"],
     path="test_multilabel",
-    include_analysis = False
+    include_analysis=False,
 ):
     """Runs all the functions required to load multilabel data, preprocess it, and split it into training and test sets.
     Creates sklearn pipelines and hyperparameters to search, using specified estimators.
     For each estimator type selected, performs a randomized search across the hyperparameters to identify the parameters providing the best
     results on the holdout data within the randomized search.
     Evaluates the performance of the refitted estimator with the best hyperparameters on the test set, and saves the model
     and the performance metrics to a specified folder.
 
     Args:
         additional_features (bool, optional): Whether or not additional features (question type and text length) are used. Defaults to False.
         target (list, optional): The target labels, which should be columns in the dataset DataFrame. Defaults to major_cats.
         models_to_try (list, optional): List of the estimators to try. Defaults to ["mnb", "knn", "svm", "rfc"]. Permitted values are "mnb" (Multinomial Naive Bayes), "knn" (K Nearest Neighbours), "svm" (Support Vector Classifier), or "rfc" (Random Forest Classifier).
         path (str, optional): Path where the models are to be saved. If path does not exist, it will be created. Defaults to 'test_multilabel'.
     """
-    random_state = random.randint(1, 999)
+    # random_state = random.randint(1, 999)
     if target == major_cats:
         target_name = "major_categories"
     if target == minor_cats:
         target_name = "minor_categories"
+    if target == merged_minor_cats:
+        target_name = "test"
     df = load_multilabel_data(filename=dataset, target=target_name)
     X_train, X_test, Y_train, Y_test = process_and_split_data(
         df,
         target=target,
         additional_features=additional_features,
         random_state=random_state,
     )
     models, training_times = search_sklearn_pipelines(
         X_train,
         Y_train,
         models_to_try=models_to_try,
-        additional_features=additional_features
+        additional_features=additional_features,
     )
     model_metrics = []
     for i in range(len(models)):
         m = models[i]
         t = training_times[i]
         model_metrics.append(
             get_multilabel_metrics(
                 X_test,
                 Y_test,
                 random_state=random_state,
                 labels=target,
                 model_type="sklearn",
                 model=m,
                 training_time=t,
-                additional_features=additional_features
+                additional_features=additional_features,
             )
         )
     write_multilabel_models_and_metrics(models, model_metrics, path=path)
     if include_analysis == True:
         for i in range(len(models)):
-            model_name = f'model_{i}'
-            write_model_preds(X_test, Y_test, models[i], labels=target,
-                              additional_features=additional_features, path=f"{path}/{model_name}_labels.xlsx")
+            model_name = f"model_{i}"
+            write_model_preds(
+                X_test,
+                Y_test,
+                models[i],
+                labels=target,
+                additional_features=additional_features,
+                path=f"{path}/{model_name}_labels.xlsx",
+            )
             write_model_analysis(model_name, labels=target, dataset=df, path=path)
     print("Pipeline complete")
 
 
 def run_svc_pipeline(
     additional_features=False,
     target=major_cats,
@@ -109,15 +132,15 @@
     Args:
         additional_features (bool, optional): Whether or not additional features (question type and text length) are used. Defaults to False.
         target (list, optional): The target labels, which should be columns in the dataset DataFrame. Defaults to major_cats.
         path (str, optional): Path where the models are to be saved. If path does not exist, it will be created. Defaults to 'test_multilabel'.
         include_analysis (bool, optional): Whether or not to create Excel files including further analysis of the model's performance. Defaults to False. If True, writes two Excel files to the specified folder, one containing the labels and the performance metrics for each label, and one containing the predicted labels and the actual labels for the test set, with the model's probabilities for both.
 
     """
-    random_state = random.randint(1, 999)
+    # random_state = random.randint(1, 999)
     if target == major_cats:
         target_name = "major_categories"
     if target == minor_cats:
         target_name = "minor_categories"
     if target == merged_minor_cats:
         target_name = "test"
     df = load_multilabel_data(filename=dataset, target=target_name)
@@ -142,19 +165,20 @@
     if include_analysis == True:
         write_model_preds(
             X_test,
             Y_test,
             model,
             labels=target,
             additional_features=additional_features,
-            path=f"{path}/labels.xlsx"
+            path=f"{path}/labels.xlsx",
         )
-        write_model_analysis(model_name='model_0', labels=target, dataset = df, path = path)
+        write_model_analysis(model_name="model_0", labels=target, dataset=df, path=path)
     print("Pipeline complete!")
 
+
 def run_tf_pipeline(target=major_cats, path="test_multilabel/tf"):
     """Runs all the functions required to load multilabel data, preprocess it, and split it into training and test sets.
     Creates tf.keras LSTM model and trains it on the train set.
     Evaluates the performance of trained model with the best hyperparameters on the test set, and saves the model
     and the performance metrics to a specified folder.
     Cannot currently take additional features, is only designed for text data alone.
     This model architecture performs very poorly and may be taken out of the model.
@@ -186,31 +210,36 @@
         model=model_trained,
         training_time=training_time,
     )
     write_multilabel_models_and_metrics([model_trained], [model_metrics], path=path)
 
 
 def run_bert_pipeline(
-    additional_features=False, path="test_multilabel/bert", target=major_cats
+    additional_features=False,
+    path="test_multilabel/bert",
+    target=major_cats,
+    include_analysis=False,
 ):
     """Runs all the functions required to load multilabel data, preprocess it, and split it into training, test and validation sets.
     Creates tf.keras Transformer model with additional layers specific to the classification task, and trains it on the train set.
     Evaluates the performance of trained model with the best hyperparameters on the test set, and saves the model
     and the performance metrics to a specified folder.
 
     Args:
         additional_features (bool, optional): Whether or not additional features (question type and text length) are used. Defaults to False.
         path (str, optional): Path where the models are to be saved. If path does not exist, it will be created. Defaults to 'test_multilabel'.
     """
-    random_state = random.randint(1, 999)
+    # random_state = random.randint(1, 999)
     print(f"random_state is: {random_state}")
     if target == major_cats:
         target_name = "major_categories"
     if target == minor_cats:
         target_name = "minor_categories"
+    if target == merged_minor_cats:
+        target_name = "test"
     df = load_multilabel_data(filename=dataset, target=target_name)
     X_train_val, X_test, Y_train_val, Y_test = process_and_split_data(
         df,
         target=target,
         preprocess_text=False,
         additional_features=additional_features,
         random_state=random_state,
@@ -247,18 +276,121 @@
         model_type="bert",
         model=model_trained,
         training_time=training_time,
         additional_features=additional_features,
         already_encoded=True,
     )
     write_multilabel_models_and_metrics([model_trained], [model_metrics], path=path)
+    if include_analysis == True:
+        write_model_preds(
+            X_test,
+            Y_test,
+            model,
+            labels=target,
+            additional_features=additional_features,
+            path=f"{path}/labels.xlsx",
+        )
+        write_model_analysis(model_name="model_0", labels=target, dataset=df, path=path)
+    print("Pipeline complete!")
+
+
+def run_two_layer_sklearn_pipeline(
+    additional_features=True,
+    models_to_try=["mnb", "knn", "xgb"],
+    path="test_multilabel/230605",
+):
+    random_state = random.randint(1, 999)
+    df_major = load_multilabel_data(filename=dataset, target="major_categories")
+    df_minor = load_multilabel_data(filename=dataset, target="minor_categories")
+    # major cats first
+    X_train, X_test, Y_train, Y_test = process_and_split_data(
+        df_major,
+        target=major_cats,
+        additional_features=additional_features,
+        random_state=random_state,
+    )
+    target = major_cats
+    models, training_times = search_sklearn_pipelines(
+        X_train,
+        Y_train,
+        models_to_try=models_to_try,
+        additional_features=additional_features,
+    )
+    svc, svc_time = create_and_train_svc_model(X_train, Y_train)
+    models.append(svc)
+    training_times.append(svc_time)
+    model_metrics = []
+    for i in range(len(models)):
+        m = models[i]
+        t = training_times[i]
+        model_metrics.append(
+            get_multilabel_metrics(
+                X_test,
+                Y_test,
+                random_state=random_state,
+                labels=target,
+                model_type="sklearn",
+                model=m,
+                training_time=t,
+                additional_features=additional_features,
+            )
+        )
+    write_multilabel_models_and_metrics(models, model_metrics, path=path)
+    # minor cats
+    for k, v in major_cat_dict.items():
+        if len(v) > 1:
+            print(k)
+            target = v
+            model_name = k
+            minipath = os.path.join(path, model_name)
+            X_train, X_test, Y_train, Y_test = process_and_split_data(
+                df_minor,
+                target=target,
+                additional_features=additional_features,
+                random_state=random_state,
+            )
+            models, training_times = search_sklearn_pipelines(
+                X_train,
+                Y_train,
+                models_to_try=["mnb", "knn", "xgb"],
+                additional_features=additional_features,
+            )
+            svc, svc_time = create_and_train_svc_model(X_train, Y_train)
+            models.append(svc)
+            training_times.append(svc_time)
+            model_metrics = []
+            for i in range(len(models)):
+                m = models[i]
+                t = training_times[i]
+                model_metrics.append(
+                    get_multilabel_metrics(
+                        X_test,
+                        Y_test,
+                        random_state=random_state,
+                        labels=target,
+                        model_type="sklearn",
+                        model=m,
+                        training_time=t,
+                        additional_features=additional_features,
+                    )
+                )
+            write_multilabel_models_and_metrics(models, model_metrics, path=minipath)
 
 
 if __name__ == "__main__":
-    # run_bert_pipeline(additional_features = True, path = 'test_multilabel/bert_minorcats', target = minor_cats)
-    # run_sklearn_pipeline(additional_features = True, target= minor_cats, models_to_try = ["svm"], path = 'test_multilabel/230522-b')
-    run_svc_pipeline(
+    # run_sklearn_pipeline(additional_features = True, target= minor_cats, models_to_try = ["xgb"], path = 'test_multilabel/v6_230806/xgb',
+    #                      include_analysis=True)
+    # run_svc_pipeline(
+    #     additional_features=True,
+    #     target=minor_cats,
+    #     path="test_multilabel/v6_230806/svc",
+    #     include_analysis=True
+    # )
+    run_bert_pipeline(
         additional_features=True,
+        path="test_multilabel/v6_230806",
         target=minor_cats,
-        path="test_multilabel/230522",
-        include_analysis=True
+        include_analysis=True,
     )
+    # run_sklearn_pipeline(additional_features = True, target= minor_cats, models_to_try = ["svm"], path = 'test_multilabel/v6_230806/svc_2',
+    #                      include_analysis=True)
+    # run_two_layer_sklearn_pipeline()
```

### Comparing `pxtextmining-0.5.3/pxtextmining/pipelines/sentiment_pipeline.py` & `pxtextmining-0.5.4/pxtextmining/pipelines/sentiment_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,23 @@
     process_and_split_data,
 )
 from pxtextmining.factories.factory_model_performance import get_multiclass_metrics
 from pxtextmining.factories.factory_pipeline import (
     search_sklearn_pipelines,
     create_bert_model_additional_features,
     train_bert_model,
-    create_bert_model
+    create_bert_model,
 )
 from pxtextmining.factories.factory_write_results import (
     write_multilabel_models_and_metrics,
 )
 from pxtextmining.params import dataset
 
-random_state = random.randint(1,999)
+random_state = random.randint(1, 999)
+
 
 def run_sentiment_pipeline(
     additional_features=False,
     models_to_try=["svm", "xgb"],
     path="test_multilabel/sentiment",
 ):
     """Runs all the functions required to load multiclass data, preprocess it, and split it into training, test and validation sets.
@@ -61,15 +62,15 @@
         metrics = get_multiclass_metrics(
             X_test,
             Y_test,
             labels=target_names,
             random_state=random_state,
             model=m,
             training_time=t,
-            additional_features = additional_features
+            additional_features=additional_features,
         )
         model_metrics.append(metrics)
     write_multilabel_models_and_metrics(models, model_metrics, path)
 
 
 def run_sentiment_bert_pipeline(
     additional_features=True, path="test_multilabel/sentiment_bert"
@@ -121,15 +122,17 @@
     model_metrics = get_multiclass_metrics(
         X_test,
         Y_test,
         random_state=random_state,
         labels=target_names,
         model=model_trained,
         training_time=training_time,
-        additional_features = additional_features
+        additional_features=additional_features,
     )
     write_multilabel_models_and_metrics([model_trained], [model_metrics], path=path)
 
 
 if __name__ == "__main__":
-    run_sentiment_pipeline(additional_features=False)
-    run_sentiment_bert_pipeline(additional_features = False, path="test_multilabel/sentiment_bert")
+    # run_sentiment_pipeline(additional_features=False)
+    run_sentiment_bert_pipeline(
+        additional_features=True, path="test_multilabel/sentiment_bert"
+    )
```

### Comparing `pxtextmining-0.5.3/pyproject.toml` & `pxtextmining-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pxtextmining"
-version = "0.5.3"
+version = "0.5.4"
 description = "Multilabel text classification of patient experience feedback."
 authors = ['CDU Data Science <cdudatascience@nottshc.nhs.uk>',
 'YiWen Hon <yiwen.hon@nottshc.nhs.uk>']
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/CDU-data-science-team/pxtextmining"
 documentation = "https://cdu-data-science-team.github.io/pxtextmining"
```

### Comparing `pxtextmining-0.5.3/setup.py` & `pxtextmining-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'spacy>=3.4.4,<4.0.0',
  'tensorflow>=2.11.0,<3.0.0',
  'transformers>=4.26.1,<5.0.0',
  'xgboost>=1.7.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'pxtextmining',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'Multilabel text classification of patient experience feedback.',
     'long_description': '# pxtextmining: Text Classification of Patient Experience feedback\n\n## Project description\n**pxtextmining** is a Python package for classifying patient feedback comments collected via the [NHS England Friends and Family Test](https://www.england.nhs.uk/fft/) (FFT). It is part of the [Patient Experience Qualitative Data Categorisation project](https://cdu-data-science-team.github.io/PatientExperience-QDC/), funded by NHS England and hosted by Nottinghamshire Healthcare NHS Foundation Trust.\n\n__We are working openly by [open-sourcing](https://github.com/CDU-data-science-team/pxtextmining/blob/main/LICENSE) the analysis code and data where possible to promote replication, reproducibility and further developments. Pull requests are more than welcome.__\n\n## Documentation and installation\n\nFull documentation, including installation instructions, is available on our [documentation page](https://cdu-data-science-team.github.io/pxtextmining/).\n',
     'author': 'CDU Data Science',
     'author_email': 'cdudatascience@nottshc.nhs.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CDU-data-science-team/pxtextmining',
```

### Comparing `pxtextmining-0.5.3/PKG-INFO` & `pxtextmining-0.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxtextmining
-Version: 0.5.3
+Version: 0.5.4
 Summary: Multilabel text classification of patient experience feedback.
 Home-page: https://github.com/CDU-data-science-team/pxtextmining
 License: MIT
 Author: CDU Data Science
 Author-email: cdudatascience@nottshc.nhs.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

