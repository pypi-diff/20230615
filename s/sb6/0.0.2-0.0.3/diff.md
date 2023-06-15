# Comparing `tmp/sb6-0.0.2.tar.gz` & `tmp/sb6-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sb6-0.0.2.tar", last modified: Thu May 18 12:59:45 2023, max compression
+gzip compressed data, was "sb6-0.0.3.tar", last modified: Thu Jun 15 14:25:38 2023, max compression
```

## Comparing `sb6-0.0.2.tar` & `sb6-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 12:59:45.221224 sb6-0.0.2/
--rw-rw-rw-   0        0        0     1067 2023-04-11 12:54:43.000000 sb6-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      462 2023-05-18 12:59:45.221224 sb6-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-05-12 01:06:50.000000 sb6-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 12:59:45.221224 sb6-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-05-18 12:56:54.000000 sb6-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 12:59:45.201588 sb6-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 12:59:45.221224 sb6-0.0.2/src/sb6.egg-info/
--rw-rw-rw-   0        0        0      462 2023-05-18 12:59:45.000000 sb6-0.0.2/src/sb6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-05-18 12:59:45.000000 sb6-0.0.2/src/sb6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 12:59:45.000000 sb6-0.0.2/src/sb6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-18 12:59:45.000000 sb6-0.0.2/src/sb6.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-18 12:59:45.000000 sb6-0.0.2/src/sb6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   123303 2023-05-17 19:50:11.000000 sb6-0.0.2/src/sb6.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:25:38.998940 sb6-0.0.3/
+-rw-rw-rw-   0        0        0     1067 2023-04-11 12:54:43.000000 sb6-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      462 2023-06-15 14:25:38.998940 sb6-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-05-12 01:06:50.000000 sb6-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 14:25:38.998940 sb6-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-06-15 14:24:22.000000 sb6-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:25:38.983314 sb6-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 14:25:38.998940 sb6-0.0.3/src/sb6.egg-info/
+-rw-rw-rw-   0        0        0      462 2023-06-15 14:25:38.000000 sb6-0.0.3/src/sb6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-06-15 14:25:38.000000 sb6-0.0.3/src/sb6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 14:25:38.000000 sb6-0.0.3/src/sb6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-15 14:25:38.000000 sb6-0.0.3/src/sb6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-15 14:25:38.000000 sb6-0.0.3/src/sb6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   138791 2023-06-15 14:20:16.000000 sb6-0.0.3/src/sb6.py
```

### Comparing `sb6-0.0.2/LICENSE` & `sb6-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sb6-0.0.2/setup.py` & `sb6-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sb6",
-    version="0.0.2",
+    version="0.0.3",
     description='chatbot',
     license='MIT',
     author="aiml department",
     author_email="aiml@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

### Comparing `sb6-0.0.2/src/sb6.py` & `sb6-0.0.3/src/sb6.py`

 * *Files 2% similar despite different names*

```diff
@@ -1057,14 +1057,280 @@
 27,58000,0
 27,84000,0
 32,150000,1
 25,33000,0
 35,65000,0
 '''
         """)
+    def id3():
+        """
+    building decision trees
+
+    - load_csv(filename): reads in a CSV file and returns the dataset and headers as a tuple.
+    - subtables(data, col, delete): creates subtables for a given column in the dataset.
+    - entropy(S): calculates the entropy of a set of data.
+    - compute_gain(data, col): calculates the information gain for a given column in the dataset.
+    - build_tree(data, features): builds a decision tree using the ID3 algorithm.
+    - print_tree(node, level): prints the decision tree to the console.
+    - classify(node, x_test, features): classifies a test instance using the decision tree.
+        """
+        print("""
+import math 
+import csv
+
+def load_csv(filename):
+	lines=csv.reader(open(filename,"r"))
+	dataset=list(lines)
+	headers=dataset.pop(0)
+	return dataset,headers
+
+class Node:
+	def __init__(self,attribute):
+		self.attribute=attribute
+		self.children=[]
+		self.answer=""
+
+def subtables(data,col,delete):
+	dic={}
+	coldata=[row[col] for row in data]
+	attr=list(set(coldata))
+	counts=[0]*len(attr)
+	r=len(data)
+	c=len(data[0])
+	for x in range(len(attr)):
+		for y in range(r):
+			if data[y][col]==attr[x]:
+				counts[x]+=1
+	for x in range(len(attr)):
+		dic[attr[x]]=[[0 for i in range(c)]for j in range(counts[x])]
+		pos=0
+		for y in range(r):
+			if data[y][col]==attr[x]:
+				if delete:
+					del data[y][col]
+				dic[attr[x]][pos]=data[y]
+				pos+=1
+	return attr,dic
+	
+def entropy(S):
+	attr=list(set(S))
+	if len(attr)==1:
+		return 0
+	counts=[0,0]
+	for i in range(2):
+		counts[i]=sum([1 for x in S if attr[i]==x])/(len(S)*1.0)
+	sums=0
+	for cnt in counts:
+		sums+=-1*cnt*math.log(cnt,2)
+	return sums
+
+def compute_gain(data,col):
+	attr,dic=subtables(data,col,delete=False)
+	total_size=len(data)
+	entropies=[0]*len(attr)
+	ratio=[0]*len(attr)
+	total_entropy=entropy([row[-1] for row in data])
+	for x in range(len(attr)):
+		ratio[x]=len(dic[attr[x]])/(total_size*1.0)
+		entropies[x]=entropy([row[-1] for row in dic[attr[x]]])
+		total_entropy-=ratio[x]*entropies[x]
+	return total_entropy
+
+def build_tree(data,features):
+	lastcol=[row[-1] for row in data]
+	if(len(set(lastcol)))==1:
+		node=Node("")
+		node.answer=lastcol[0]
+		return node
+	n=len(data[0])-1
+	gains=[0]*n
+	for col in range(n):
+		gains[col]=compute_gain(data,col)
+	split=gains.index(max(gains))
+	node=Node(features[split])
+	fea=features[:split]+features[split+1:]
+	attr,dic=subtables(data,split,delete=True)
+	for x in range(len(attr)):
+		child=build_tree(dic[attr[x]],fea)
+		node.children.append((attr[x],child))
+	return node
+	
+def print_tree(node,level):
+	if node.answer!="":
+		print(" "*level,node.answer)
+		return
+	print(" "*level,node.attribute)
+	for value,n in node.children:
+		print(" "*(level+1),value)
+		print_tree(n,level+2)
+		
+def classify(node,x_test,features):
+	if node.answer!="":
+		print(node.answer)
+		return
+	pos=features.index(node.attribute)
+	for value,n in node.children:
+		if x_test[pos]==value:
+			classify(n,x_test,features)
+			
+'''Main program'''
+dataset,features=load_csv("id3.csv")
+node1=build_tree(dataset,features)
+print("The decision tree for the dataset using ID3 algorithm is ")
+print_tree(node1,0)
+testdata,features=load_csv("id3_test_1.csv")
+for xtest in testdata:
+	print("The test instance: ",xtest)
+	print("The label for test instance: ",end=" ")
+	classify(node1,xtest,features)
+        """)
+        
+    def rf():
+        """
+      Demonstrate the working of the Random forest algorithm. Use an appropriate data set for building and apply this knowledge to classify a new sample.
+      Random Forest is a popular machine learning algorithm that belongs to the category of ensemble learning methods. 
+      It is widely used for both classification and regression tasks.
+
+    In Random Forest, multiple decision trees are trained on different subsets of the training data, using a technique called "bootstrap aggregating" or "bagging." 
+    Each tree is trained independently, and the final prediction is obtained by aggregating the predictions of all the individual trees.
+        """
+        print("""
+from sklearn.datasets import load_iris
+iris = load_iris()
+X = iris.data
+y = iris.target
+
+from sklearn.model_selection import train_test_split
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)
+
+from sklearn.ensemble import RandomForestClassifier
+model = RandomForestClassifier(n_estimators=100,max_leaf_nodes=16,n_jobs=-1)
+model.fit(X_train, y_train)
+y_pred = model.predict(X_test)
+
+from sklearn.metrics import accuracy_score
+accuracy = accuracy_score(y_test, y_pred)
+print(f"Accuracy: {accuracy}")
+
+from sklearn.tree import export_graphviz
+export_graphviz(model.estimators_[99], out_file="iris_tree.dot", feature_names=iris.feature_names, class_names=iris.target_names, filled=True, rounded=True)
+
+import numpy as np
+new_sample = np.array([[5.1, 3.5, 1.4, 0.2]])
+new_sample_class = model.predict(new_sample)
+print(f"Predicted class for the new sample: {iris.target_names[new_sample_class[0]]}")
+
+''' manual 
+import pandas as pd
+import numpy as np
+data = pd.read_csv('Iris.csv',index_col=0)
+data.reset_index(drop=True,inplace=True)
+X = np.array(data.iloc[:,:-1])
+y = np.array(data.iloc[:,-1])
+from sklearn.model_selection import train_test_split
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)
+from sklearn.ensemble import RandomForestClassifier
+clf = RandomForestClassifier(n_estimators=100)
+clf.fit(X_train, y_train)
+y_pred = clf.predict(X_test)
+from sklearn.metrics import accuracy_score
+accuracy = accuracy_score(y_test, y_pred)
+print(f"Accuracy: {accuracy}")
+# Create a new sample for classification
+new_sample = np.array([[3, 3, 2, 2]])
+y_pred = clf.predict(new_sample)
+print(y_pred)
+
+from sklearn.tree import export_graphviz
+for i, tree_in_forest in enumerate(clf.estimators_):
+    if i<1:         # to print only 1st tree
+        export_graphviz(tree_in_forest, out_file=f"tree_{i+1}.dot", feature_names=['SepalLength', 'SepalWidth', 'PetalLength', 'PetalWidth'])
+        print(f"dot -Tpng tree_{i+1}.dot -o tree_{i+1}.png")
+'''
+        """)
+        
+    def knn():
+        """
+      k-Nearest Neighbors (k-NN) is a supervised machine learning algorithm used for both classification and regression tasks. 
+      It is a non-parametric algorithm that makes predictions based on the similarity between a new data point and its k nearest neighbors in the feature space.
+      When a new data point is given, the algorithm calculates the distance between that point and all the data points in the training set. 
+      The distance metric used is typically Euclidean distance, although other metrics can also be used.
+      For classification, the predicted class label for the new data point is determined by majority voting among its k nearest neighbors
+        """
+        print("""
+import pandas as pd
+data = pd.read_csv('Iris.csv')
+X = data.iloc[:, :-1].values
+y = data.iloc[:, -1].values
+
+from sklearn.model_selection import train_test_split
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)
+
+from sklearn.neighbors import KNeighborsClassifier
+knn_classifier = KNeighborsClassifier(n_neighbors=3)
+knn_classifier.fit(X_train, y_train)
+y_pred = knn_classifier.predict(X_test)
+
+from sklearn.metrics import accuracy_score,confusion_matrix
+accuracy = accuracy_score(y_test, y_pred)
+print(f"Accuracy: {accuracy}")
+print(f"Accuracy: \n",confusion_matrix(y_test, y_pred))
+
+'''
+from sklearn.datasets import load_iris
+iris = load_iris()
+X = iris.data
+y = iris.target
+'''
+        """)
+        
+    def em():
+        """
+     A DataFrame is a two-dimensional labeled data structure in pandas, which is a popular library for data manipulation and analysis in Python. 
+    It organizes data into rows and columns, similar to a table or spreadsheet, and provides various methods and operations for data manipulation.
+    GaussianMixture is a class in scikit-learn, a popular machine learning library in Python. It is used to model data using a Gaussian Mixture Model (GMM). 
+    GMM is a probabilistic model that assumes the data points are generated from a mixture of Gaussian distributions. 
+    It is commonly used for clustering tasks where the goal is to assign data points to different clusters based on their statistical properties.
+    EM algorithm, short for Expectation-Maximization algorithm, is an iterative algorithm used to estimate the parameters of statistical models when there are hidden or unobserved variables involved. 
+    It is commonly used in unsupervised learning tasks such as clustering, where the goal is to find latent patterns or groupings in the data.
+        """
+        print("""
+from sklearn.datasets import load_iris
+import pandas as pd
+dataset = load_iris()
+x = pd.DataFrame(dataset.data, columns=['sepal_length', 'sepal_width', 'petal_length', 'petal_width'])
+y = pd.DataFrame(dataset.target, columns=['Targets'])
+
+import numpy as np
+colormap = np.array(['red', 'lime', 'black'])    # Create a colormap for visualization
+
+import matplotlib.pyplot as plt
+fig = plt.figure(figsize=(14, 7))           # Plot the original data
+plt.subplot(1, 3, 1)
+plt.scatter(x['petal_length'], x['petal_width'], c=colormap[y['Targets']], s=40)
+plt.title('Real')
+
+from sklearn import preprocessing
+scaler = preprocessing.StandardScaler()
+x_scaled = scaler.fit_transform(x)
+x_scaled = pd.DataFrame(x_scaled, columns=x.columns)
+
+from sklearn.mixture import GaussianMixture
+gmm = GaussianMixture(n_components=3)
+gmm.fit(x_scaled)
+y_cluster_gmm = gmm.predict(x_scaled)
+
+import sklearn.metrics as sm
+print("The accuracy score of EM:", sm.accuracy_score(y['Targets'], y_cluster_gmm))
+
+plt.subplot(1, 3, 3)        # Plot the clusters predicted by GMM
+plt.scatter(x['petal_length'], x['petal_width'], c=colormap[y_cluster_gmm], s=40)
+plt.title('GMM Clusters')
+plt.show()
+        """)
 
 class mlfull():
     """
 pg1() : FIND-S : Finding a Maximally Specific (0) Hypothesis  
     Implement and demonstrate the FIND-S algorithm for finding the most specific hypothesis based on a given set of training data samples. 
     Read the training data from a .CSV file and show the output for test cases. 
     Develop an interactive program by Compareing the result by implementing LIST THEN ELIMINATE algorithm. 
@@ -2536,15 +2802,14 @@
 else display a toast message saying “Login Failed”.The user is given only two attempts and after
 thatdisplay a toast message saying “Failed Login Attempts” and disable the SIGN IN button. Use
 Bundle to transfer information from one activity to another.
         """
         print(r"""
  // MainActivity.java
 package com.example.project4;
-
 import androidx.appcompat.app.AppCompatActivity;
 import android.content.Intent;
 import android.os.Bundle;
 import android.view.View;
 import android.widget.Button;
 import android.widget.EditText;
 import android.widget.Toast;
@@ -3069,97 +3334,228 @@
         """)
     
     def texttospeech():
         """
     Develop a simple application “convert text to speech” that converts the user input text into voice.
         """
         print(r"""
-package com.example.texttospeech;
+ // MainActivity.java
+package com.example.project5;
+
+import androidx.appcompat.app.AppCompatActivity;
 import android.os.Bundle;
 import android.speech.tts.TextToSpeech;
 import android.view.View;
 import android.widget.Button;
 import android.widget.EditText;
-import androidx.appcompat.app.AppCompatActivity;
 import java.util.Locale;
 public class MainActivity extends AppCompatActivity {
     Button b1;
     EditText et1;
     TextToSpeech t1;
     @Override
     protected void onCreate(Bundle savedInstanceState) {
-    super.onCreate(savedInstanceState);
-    setContentView(R.layout.activity_main);
-    b1 = findViewById(R.id.button);
-    et1 = findViewById(R.id.text);
-    t1 = new TextToSpeech(getApplicationContext(), status -> {
-    if(status!=TextToSpeech.ERROR){
-    t1.setLanguage(Locale.ENGLISH);
-    }
-    });
+        super.onCreate(savedInstanceState);
+        setContentView(R.layout.activity_main);
+        et1 = findViewById(R.id.ed1);
+        b1 = findViewById(R.id.bt1);
+        t1 = new TextToSpeech(getApplicationContext(),status -> {
+            if(status!=TextToSpeech.ERROR){
+                t1.setLanguage(Locale.ENGLISH);
+            }
+        });
     }
-    public void convert(View view)
-    {
-    String tospeak = et1.getText().toString();
-    t1.speak(tospeak,TextToSpeech.QUEUE_FLUSH,null);
+    public void convert(View view){
+        String tospeak = et1.getText().toString();
+        t1.speak(tospeak,TextToSpeech.QUEUE_FLUSH,null);
     }
 }
+
+//activity_main.xml
+<?xml version="1.0" encoding="utf-8"?>
+<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
+    xmlns:app="http://schemas.android.com/apk/res-auto"
+    xmlns:tools="http://schemas.android.com/tools"
+    android:layout_width="match_parent"
+    android:layout_height="match_parent"
+    android:onClick="convert"
+    tools:context=".MainActivity">
+
+    <TextView
+        android:id="@+id/textView"
+        android:layout_width="368dp"
+        android:layout_height="59dp"
+        android:gravity="center"
+        android:text="TTS Application"
+        android:textColor="@color/design_default_color_error"
+        android:textSize="38sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.4"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.037" />
+
+    <EditText
+        android:id="@+id/ed1"
+        android:layout_width="370dp"
+        android:layout_height="165dp"
+        android:ems="10"
+        android:gravity="center"
+        android:hint="Enter your text here"
+        android:inputType="textPersonName"
+        android:textSize="24sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.487"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.353" />
+
+    <Button
+        android:id="@+id/bt1"
+        android:layout_width="297dp"
+        android:layout_height="70dp"
+        android:text="CONVERT TTS"
+        android:textSize="34sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.662" />
+</androidx.constraintlayout.widget.ConstraintLayout>
         """)
         
     def phone():
         """
         Create an activity like a phone dialer with CALL and SAVE options
         """
         print(r"""
 // MainActivity.java
-package com.example.call;
+package com.example.project6;
+
 import androidx.appcompat.app.AppCompatActivity;
-import android.annotation.SuppressLint;
 import android.content.Intent;
 import android.net.Uri;
 import android.os.Bundle;
-import android.provider.Contacts;
 import android.provider.ContactsContract;
 import android.view.View;
 import android.widget.Button;
 import android.widget.EditText;
 public class MainActivity extends AppCompatActivity {
     Button call,save,clear;
     EditText et1;
     @Override
     protected void onCreate(Bundle savedInstanceState) {
         super.onCreate(savedInstanceState);
         setContentView(R.layout.activity_main);
-        et1 = findViewById(R.id.et);
-        clear = findViewById(R.id.clear);
-        call = findViewById(R.id.call);
-        save = findViewById(R.id.save);
+        et1 = findViewById(R.id.ed1);
+        clear = findViewById(R.id.clrbtn);
+        call = findViewById(R.id.clbtn);
+        save = findViewById(R.id.svbtn);
         clear.setOnClickListener(view -> et1.setText(""));
         call.setOnClickListener(view -> {
-        String number = et1.getText().toString();
-        Intent intent = new Intent(Intent.ACTION_DIAL);
-        intent.setData(Uri.parse("tel:"+number));
-        startActivity(intent);
+            String number = et1.getText().toString();
+            Intent intent = new Intent(Intent.ACTION_DIAL);
+            intent.setData(Uri.parse("tel:"+number));
+            startActivity(intent);
         });
         save.setOnClickListener(view -> {
-        String number = et1.getText().toString();
-        Intent intent = new Intent(Intent.ACTION_INSERT,
-        ContactsContract.Contacts.CONTENT_URI);
-        intent.putExtra(ContactsContract.Intents.Insert.PHONE,number);
-        startActivity(intent);
+            String number = et1.getText().toString();
+            Intent intent = new Intent(Intent.ACTION_INSERT, ContactsContract.Contacts.CONTENT_URI);
+            intent.putExtra(ContactsContract.Intents.Insert.PHONE,number);
+            startActivity(intent);
         });
     }
-    @SuppressLint("SetTextI18n")
     public void inputnumber(View view){
-        Button btn=(Button)view;
+        Button btn=(Button) view;
         String digit = btn.getText().toString();
         String phonenumber = et1.getText().toString();
         et1.setText(phonenumber+digit);
     }
 }
+
+//activity_main.xml
+<?xml version="1.0" encoding="utf-8"?>
+<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
+    xmlns:app="http://schemas.android.com/apk/res-auto"
+    xmlns:tools="http://schemas.android.com/tools"
+    android:layout_width="match_parent"
+    android:layout_height="match_parent"
+    tools:context=".MainActivity">
+
+    <Button
+        android:id="@+id/clrbtn"
+        android:layout_width="157dp"
+        android:layout_height="71dp"
+        android:text="CLEAR"
+        android:textSize="34sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.498"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.808" />
+
+    <Button
+        android:id="@+id/svbtn"
+        android:layout_width="177dp"
+        android:layout_height="65dp"
+        android:text="SAVE"
+        android:textSize="34sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.651" />
+
+    <TextView
+        android:id="@+id/textView"
+        android:layout_width="311dp"
+        android:layout_height="86dp"
+        android:gravity="center"
+        android:text="CALLER"
+        android:textColor="@color/design_default_color_error"
+        android:textSize="48sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.496"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.07" />
+
+    <EditText
+        android:id="@+id/ed1"
+        android:layout_width="405dp"
+        android:layout_height="74dp"
+        android:ems="10"
+        android:gravity="center"
+        android:hint="Enter Phone Number"
+        android:inputType="textPersonName"
+        android:textSize="34sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.432"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.275" />
+
+    <Button
+        android:id="@+id/clbtn"
+        android:layout_width="146dp"
+        android:layout_height="66dp"
+        android:text="CALL"
+        android:textSize="34sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.498"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.491" />
+</androidx.constraintlayout.widget.ConstraintLayout>
         """)
         
         
 class general:
     """
 sb6.general.read_csv_file()  :-  read csv files and getting the data
 sb6.general.load_iris_dataset() :- Load the iris dataset
```

