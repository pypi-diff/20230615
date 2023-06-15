# Comparing `tmp/Java Dependency Manager-1.0.0.tar.gz` & `tmp/Java Dependency Manager-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Java Dependency Manager-1.0.0.tar", last modified: Thu Jun 15 09:40:26 2023, max compression
+gzip compressed data, was "Java Dependency Manager-1.1.0.tar", last modified: Thu Jun 15 13:45:05 2023, max compression
```

## Comparing `Java Dependency Manager-1.0.0.tar` & `Java Dependency Manager-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 09:40:26.629861 Java Dependency Manager-1.0.0/
-drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 09:40:26.629171 Java Dependency Manager-1.0.0/Java_Dependency_Manager.egg-info/
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     1405 2023-06-15 09:40:26.000000 Java Dependency Manager-1.0.0/Java_Dependency_Manager.egg-info/PKG-INFO
--rw-r--r--   0 nagarajurepala   (501) staff       (20)      352 2023-06-15 09:40:26.000000 Java Dependency Manager-1.0.0/Java_Dependency_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)        1 2023-06-15 09:40:26.000000 Java Dependency Manager-1.0.0/Java_Dependency_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       58 2023-06-15 09:40:26.000000 Java Dependency Manager-1.0.0/Java_Dependency_Manager.egg-info/entry_points.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       17 2023-06-15 09:40:26.000000 Java Dependency Manager-1.0.0/Java_Dependency_Manager.egg-info/requires.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       16 2023-06-15 09:40:26.000000 Java Dependency Manager-1.0.0/Java_Dependency_Manager.egg-info/top_level.txt
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     1405 2023-06-15 09:40:26.629726 Java Dependency Manager-1.0.0/PKG-INFO
-drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 09:40:26.629401 Java Dependency Manager-1.0.0/javadepsmanager/
--rw-r--r--   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 07:45:23.000000 Java Dependency Manager-1.0.0/javadepsmanager/__init__.py
--rw-r--r--   0 nagarajurepala   (501) staff       (20)     9069 2023-06-15 08:50:06.000000 Java Dependency Manager-1.0.0/javadepsmanager/command_line.py
--rw-r--r--   0 nagarajurepala   (501) staff       (20)       38 2023-06-15 09:40:26.629901 Java Dependency Manager-1.0.0/setup.cfg
--rw-r--r--   0 nagarajurepala   (501) staff       (20)      819 2023-06-15 09:40:04.000000 Java Dependency Manager-1.0.0/setup.py
+drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 13:45:05.308557 Java Dependency Manager-1.1.0/
+drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 13:45:05.307716 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1616 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)      360 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)        1 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       58 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       17 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/requires.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       16 2023-06-15 13:45:05.000000 Java Dependency Manager-1.1.0/Java_Dependency_Manager.egg-info/top_level.txt
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1035 2023-06-15 12:49:38.000000 Java Dependency Manager-1.1.0/LICENSE
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1616 2023-06-15 13:45:05.308407 Java Dependency Manager-1.1.0/PKG-INFO
+drwxr-xr-x   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 13:45:05.307970 Java Dependency Manager-1.1.0/javadepsmanager/
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)        0 2023-06-15 07:45:23.000000 Java Dependency Manager-1.1.0/javadepsmanager/__init__.py
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     9755 2023-06-15 13:16:10.000000 Java Dependency Manager-1.1.0/javadepsmanager/command_line.py
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)       38 2023-06-15 13:45:05.308599 Java Dependency Manager-1.1.0/setup.cfg
+-rw-r--r--   0 nagarajurepala   (501) staff       (20)     1015 2023-06-15 13:44:01.000000 Java Dependency Manager-1.1.0/setup.py
```

### Comparing `Java Dependency Manager-1.0.0/Java_Dependency_Manager.egg-info/PKG-INFO` & `Java Dependency Manager-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
-Name: Java-Dependency-Manager
-Version: 1.0.0
+Name: Java Dependency Manager
+Version: 1.1.0
 Summary: Generates Dependency tree for any java project also compares dependencies between two versions, use jdm in commandline to use this tool
 Home-page: https://github.com/Nagaraju6242/javadepsmanager
 Author: Repala Nagaraju
 Author-email: nagarajrepala@gmail.com
+License: MIT
+Project-URL: Source Code, https://github.com/Nagaraju6242/javadepsmanager
+Project-URL: Tracker, https://github.com/Nagaraju6242/javadepsmanager/issues
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Java Dependency Manager
 
-The Java Dependency Manager (JDM) is a powerful tool for managing dependencies in Java projects. It allows you to generate a dependency tree for any Java project and compare dependencies between two different versions.
+The Java Dependency Manager (JDM) is a powerful tool for generating dependencies in Java projects. It allows you to generate a dependency tree for any Java project and compare dependencies between two different versions.
 
 ## Features
 
 - Generate a visual dependency tree for a Java project.
 - Compare dependencies between two different versions of a project.
 - Includes Search functionality 
 
 ## Installation
 
 You can install JDM using pip:
 
 ```
-pip install Java-Dependency-Manager
+python3 -m pip install Java-Dependency-Manager
 ```
 
 ## Usage
 Once installed, you can use JDM through the command-line interface (CLI). Simply run the following command:
 
 ```
 jdm
@@ -35,11 +39,11 @@
 
 
 ## Requirements
 
 Make sure you have the following before running jdm
 
 1. Java JDK Installed and `JAVA_HOME` added to path
-2. Apache Maven  
+2. Apache Maven added to path
 
 ## Contact
 For any inquiries or feedback, feel free to reach out to the author, `Repala Nagaraju`, via email at nagarajrepala@gmail.com.
```

### Comparing `Java Dependency Manager-1.0.0/javadepsmanager/command_line.py` & `Java Dependency Manager-1.1.0/javadepsmanager/command_line.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 import requests
 import subprocess
 import os
 import sys
 
 MAXIMUM_SEARCH_RESULTS = 15
 OUTPUT_DIR = os.path.join(os.path.expanduser('~'), '.jdm')
+DEPENDENCIES_DIR = os.path.join(OUTPUT_DIR, 'dependencies')
+if sys.platform == 'win32':
+    SHELL = True  # Use shell=True for PowerShell on Windows
+else:
+    SHELL = False  # Use shell=False for macOS (and other Unix-like systems)
+
 
 session = requests.Session()
 base_url = 'https://repo1.maven.org/maven2'
 
 def print_in_color(text, color):
     if color == "red":
         print("\033[91m {}\033[00m" .format(text))
@@ -56,20 +62,22 @@
     return group_id, artifact_id, version
 
 def save_dependencies_list(group_id, artifact_id, version, nopom=False):
     if not nopom:
         print("Downloading POM.xml for version", version)
         save_pom(group_id, artifact_id, version)
     print("Generating dependencies list for version", version)
-    cmd = ["mvn", "dependency:list", "-Dstyle.color=never", "-Dsort=true","-DincludeScope=runtime", f"-DoutputFile={OUTPUT_DIR}/dependencies/{artifact_id}-{version}-list.txt"]
-    subprocess.run(cmd, capture_output=True, text=True, cwd=OUTPUT_DIR)
+    file_path = os.path.join(DEPENDENCIES_DIR, f"{artifact_id}-{version}-list.txt")
+    cmd = ["mvn", "dependency:list", "-Dstyle.color=never", "-Dsort=true","-DincludeScope=runtime", f"-DoutputFile={file_path}"]
+    subprocess.run(cmd, capture_output=True, text=True, cwd=OUTPUT_DIR,shell=SHELL)
 
 
 def parse_dependencies_list(file_name):
-    with open(f"{OUTPUT_DIR}/dependencies/{file_name}") as f:
+    file_path = os.path.join(DEPENDENCIES_DIR, file_name)
+    with open(file_path) as f:
         lines = f.readlines()
     dependencies = []
     for line in lines:
         line = line.strip()
         if line == "":
             continue
         if line == "The following files have been resolved:":
@@ -91,36 +99,36 @@
         dependencies2.append(dep)
     return dependencies1, dependencies2
 
 def save_dependency_tree(group_id, artifact_id, version):
     print(f"Downloading POM file for {artifact_id} v{version}...")
     save_pom(group_id, artifact_id, version)
     print(f"Generating dependency tree for {artifact_id} v{version}...")
-    cmd = ["mvn", "dependency:tree", "-Dscope=runtime", f"-DoutputFile={OUTPUT_DIR}/dependencies/{artifact_id}-{version}-tree.txt"]
-    subprocess.run(cmd, capture_output=True, text=True, cwd=OUTPUT_DIR)
-    filename = f"{artifact_id}-{version}-tree.txt"
-    with open(f"{OUTPUT_DIR}/dependencies/{filename}") as f:
+    file_path = os.path.join(DEPENDENCIES_DIR, f"{artifact_id}-{version}-tree.txt")
+    cmd = ["mvn", "dependency:tree", "-Dscope=runtime", f"-DoutputFile={file_path}"]
+    subprocess.run(cmd, capture_output=True, text=True, cwd=OUTPUT_DIR,shell=SHELL)
+    with open(file_path) as f:
         content = f.read()
     lines = content.split("\n")
     newlines = []
     for line in lines:
         if line.endswith("compile") or line.endswith("runtime"):
             newlines.append(line[:-7])
         elif "compile (optional)" in line:
             newlines.append(line.replace("compile (optional)", " (optional)"))
         elif "runtime (optional)" in line:
             newlines.append(line.replace("runtime (optional)", " (optional)"))
         else:
             newlines.append(line)
     newcontent = "\n".join(newlines)
-    with open(f"{OUTPUT_DIR}/dependencies/{filename}", "w") as f:
+    with open(file_path, "w") as f:
         f.write(newcontent)
     # get the full path of the file
-    filename = os.path.abspath(f"{OUTPUT_DIR}/dependencies/{filename}")
-    print_in_color(f"\nDependency tree for {artifact_id} v{version} saved to {filename}", "green")
+    abs_file_path = os.path.abspath(file_path)
+    print_in_color(f"\nDependency tree for {artifact_id} v{version} saved to {abs_file_path}", "green")
     print("----------------------------------------")
     print(f"Dependency tree for {artifact_id} v{version}:\n")
     print_in_color(newcontent, "cyan")
     print("----------------------------------------\n")
     return newcontent
 
 def save_pom(group_id, artifact_id, version):
@@ -128,69 +136,77 @@
     url = f"{base_url}/{group_url}/{artifact_id}/{version}/{artifact_id}-{version}.pom"
     response = session.get(url)
     if response.status_code == 404:
         print_in_color(f"POM not found for version {version} of {artifact_id}. Possible reasons might be version is incorrect or artifact might be moved.", "red")
         sys.exit()
     response.raise_for_status()
     xml = response.content.decode("utf-8")
-    with open(f"{OUTPUT_DIR}/pom.xml","w") as f:
+    pom_path = os.path.join(OUTPUT_DIR, "pom.xml")
+    with open(pom_path,"w") as f:
         f.write(xml)
 
 def main():
     keeppom = False
     compare_versions = False
     version = None
     if(len(sys.argv) > 1 and sys.argv[1] == "keeppom"):
         keeppom = True
     
-    print_in_color("Welcome to Maven Dependency Downloader", "green")
-    if not os.path.exists(OUTPUT_DIR):
-        os.makedirs(OUTPUT_DIR)
+    print_in_color("Welcome to Java Dependency Manager", "green")
+    if not os.path.exists(DEPENDENCIES_DIR):
+        os.makedirs(DEPENDENCIES_DIR)
 
     query = input("Enter the maven artifact name to search (or pom.xml url): ")
     if(query.startswith("https://repo1.maven.org/maven2/")):
         group_id, artifact_id, version = parse_pom_link(query)
         print(f"Selected {group_id} >> {artifact_id} >> {version}")
     else:
         results = advanced_search(query)
+        if(len(results) == 0):
+            print_in_color("No results found for the given query", "red")
+            sys.exit()
         for i,result in enumerate(results, start=1):
             print(f"{i}. {result['namespace']} >> {result['name']} -- {result['latestVersionInfo']['version']}(latest)")
-        print_in_color("If you cannot find the required artifact, try using the pom.xml url option", "magenta")
+        print_in_color("\nIf you cannot find the required artifact, try using the pom.xml url option\n", "magenta")
         choice = input("Select an option to proceed (or pom.xml url): ")
         if(choice.startswith("https://repo1.maven.org/maven2/")):
             group_id, artifact_id, version = parse_pom_link(choice)
             print(f"Selected {group_id} >> {artifact_id} >> {version}")
         else:
             if(choice == ""):
                 choice = 0
             else:
-                choice = int(choice) - 1
+                try:
+                    choice = int(choice) - 1
+                except:
+                    print_in_color("Invalid choice", "red")
+                    sys.exit()
             if(choice < len(results) and choice >= 0):
                 group_id = results[choice]["namespace"]
                 artifact_id = results[choice]["name"]
             else:
                 print("Invalid choice")
-                exit()
+                sys.exit()
 
             print(f"Selected {group_id} >> {artifact_id}")
 
-    compare = input("Do you want to Compare versions? (y/n)[N]: ")
+    compare = input("Do you want to Compare versions?(y/n) [N]: ")
     if(compare.lower() == "y" or compare.lower() == "yes"):
         compare_versions = True
 
     if not version:
-        version = input("Enter the required version or leave empty to use latest version: ")
+        version = input(f"Enter the required version or leave empty to use latest version: ").strip()
         if(version == ""):
             version = results[choice]['latestVersionInfo']['version']
     
     if(compare_versions):
-        version2 = input("Enter the second version to compare with or leave empty to use latest version: ")
+        version2 = input(f"Enter the second version to compare with or leave empty to use latest version: ").strip()
         if(version2 == ""):
             version2 = results[choice]['latestVersionInfo']['version']
-        print(f"Comparing {version} and {version2}")
+        print_in_color(f"Comparing {version} and {version2}", "magenta")
 
     save_dependency_tree(group_id, artifact_id, version)
     if(compare_versions):
         save_dependencies_list(group_id, artifact_id, version, nopom=True)
         dependencies1 = parse_dependencies_list(f"{artifact_id}-{version}-list.txt")
         save_dependency_tree(group_id, artifact_id, version2)
         save_dependencies_list(group_id, artifact_id, version2, nopom=True)
@@ -207,16 +223,17 @@
         print("\n----------------------------------------\n")
         print_in_color(f"Dependencies in version {version2} but not in version {version}:\n", "yellow")
         if(len(deps_in_version2) == 0):
             print_in_color("None", "red")
         else:
             print_in_color("\n".join(deps_in_version2), "red")
         print()
-        os.remove(f"{OUTPUT_DIR}/dependencies/{artifact_id}-{version}-list.txt")
-        os.remove(f"{OUTPUT_DIR}/dependencies/{artifact_id}-{version2}-list.txt")
+        list1_path = os.path.join(DEPENDENCIES_DIR, f"{artifact_id}-{version}-list.txt")
+        list2_path = os.path.join(DEPENDENCIES_DIR, f"{artifact_id}-{version2}-list.txt")
+        os.remove(list1_path)
+        os.remove(list2_path)
 
     if(not keeppom):
-        os.remove("pom.xml")
-
+        os.remove(os.path.join(OUTPUT_DIR, "pom.xml"))
 
 if __name__ == "__main__":
     main()
```

### Comparing `Java Dependency Manager-1.0.0/setup.py` & `Java Dependency Manager-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Java Dependency Manager',
-    version='1.0.0',
+    version='1.1.0',
     packages=['javadepsmanager'],
     entry_points={
         'console_scripts': [
             'jdm=javadepsmanager.command_line:main'
         ]
     },
     install_requires=[
@@ -18,8 +18,13 @@
     ],
     author='Repala Nagaraju',
     author_email='nagarajrepala@gmail.com',
     description='Generates Dependency tree for any java project also compares dependencies between two versions, use jdm in commandline to use this tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Nagaraju6242/javadepsmanager',
+    license='MIT',
+    project_urls={
+        'Source Code': 'https://github.com/Nagaraju6242/javadepsmanager',
+        'Tracker': 'https://github.com/Nagaraju6242/javadepsmanager/issues',
+    },
 )
```

