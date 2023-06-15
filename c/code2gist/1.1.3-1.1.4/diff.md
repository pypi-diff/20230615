# Comparing `tmp/code2gist-1.1.3.tar.gz` & `tmp/code2gist-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code2gist-1.1.3.tar", last modified: Thu Jun 15 18:49:03 2023, max compression
+gzip compressed data, was "code2gist-1.1.4.tar", last modified: Thu Jun 15 21:09:20 2023, max compression
```

## Comparing `code2gist-1.1.3.tar` & `code2gist-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:49:03.116447 code2gist-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 18:48:56.000000 code2gist-1.1.3/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:49:03.116447 code2gist-1.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:49:03.116447 code2gist-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-15 18:48:43.000000 code2gist-1.1.3/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 18:48:43.000000 code2gist-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-15 18:49:03.116447 code2gist-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-15 18:48:43.000000 code2gist-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:49:03.116447 code2gist-1.1.3/code2gist/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 18:48:43.000000 code2gist-1.1.3/code2gist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-15 18:48:43.000000 code2gist-1.1.3/code2gist/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:49:03.116447 code2gist-1.1.3/code2gist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-15 18:49:03.000000 code2gist-1.1.3/code2gist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 18:49:03.000000 code2gist-1.1.3/code2gist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:49:03.000000 code2gist-1.1.3/code2gist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 18:49:03.000000 code2gist-1.1.3/code2gist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 18:49:03.000000 code2gist-1.1.3/code2gist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 18:49:03.000000 code2gist-1.1.3/code2gist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-15 18:48:56.000000 code2gist-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:49:03.116447 code2gist-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:09:20.050333 code2gist-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 21:09:11.000000 code2gist-1.1.4/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:09:20.042333 code2gist-1.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:09:20.046333 code2gist-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-15 21:08:55.000000 code2gist-1.1.4/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 21:08:55.000000 code2gist-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-15 21:09:20.050333 code2gist-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-15 21:08:55.000000 code2gist-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:09:20.046333 code2gist-1.1.4/code2gist/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 21:08:55.000000 code2gist-1.1.4/code2gist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-15 21:08:55.000000 code2gist-1.1.4/code2gist/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:09:20.050333 code2gist-1.1.4/code2gist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-15 21:09:20.000000 code2gist-1.1.4/code2gist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 21:09:20.000000 code2gist-1.1.4/code2gist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:09:20.000000 code2gist-1.1.4/code2gist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 21:09:20.000000 code2gist-1.1.4/code2gist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 21:09:20.000000 code2gist-1.1.4/code2gist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 21:09:20.000000 code2gist-1.1.4/code2gist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-15 21:09:11.000000 code2gist-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:09:20.050333 code2gist-1.1.4/setup.cfg
```

### Comparing `code2gist-1.1.3/LICENSE` & `code2gist-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `code2gist-1.1.3/PKG-INFO` & `code2gist-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,108 +1,112 @@
 Metadata-Version: 2.1
 Name: code2gist
-Version: 1.1.3
+Version: 1.1.4
 Summary: Upload Python files in a directory to a GitHub Gist.
 Author-email: Cameron Spears <flames.garish-0i@icloud.com>
 License: GPL-3.0
 Keywords: python,github,gist,upload
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-#  code2gist
+# code2gist 📦
 
 `code2gist` is a Python package that makes sharing your code projects easier than ever. With a simple command, it lets you upload your code files to GitHub's Gist. `code2gist` is available on [PyPI](https://pypi.org/project/code2gist/).
 
-The package works hand-in-hand with OpenAI's ChatGPT-4's 'Browse with Bing' feature. This compatibility allows you to present substantial code bases to the model in a single instance, eliminating the need to split your code into smaller parts.
+The package works hand-in-hand with OpenAI's ChatGPT-4's 'Browse with Bing' feature. This compatibility allows you to present substantial code bases to the model in a single instance, eliminating the need to split your code into smaller parts. 🤝
 
-Another key feature of `code2gist` is its ability to handle a wide range of text-based file types, not just Python files.
+Another key feature of `code2gist` is its ability to handle a wide range of text-based file types, not just Python files. 📄
 
-In addition, `code2gist` comes with a `prune` feature that provides a clean way to remove all the gists created by this tool from your GitHub account.
+In addition, `code2gist` comes with a `prune` feature that provides a clean way to remove all the gists created by this tool from your GitHub account. 🪓
 
-## Installation
+## Installation ⚙️
 
 You can install the package via pip:
 
 ```
+Copy code
 pip install code2gist
 ```
 
-### Adding code2gist Directory to the PATH Environment Variable
+### Adding code2gist Directory to the PATH Environment Variable 👣
 
 Here are step-by-step instructions to add the code2gist directory to your PATH environment variable on Windows:
 
 1. Open the **Control Panel**.
 2. Navigate to **System and Security > System**.
 3. Click on the **Advanced system settings** link on the left panel.
 4. Click **Environment Variables**.
 5. Under the **System Variables** section, find and double-click the variable **PATH**.
 6. Click **New**.
 7. Add the directory where code2gist is installed. For example, if you have Python 3.11 installed, the directory might look like this: `C:\...\Python311\Scripts`
 8. Click **OK** to close all windows and save the changes.
 
-After following these steps, your system should recognize code2gist commands from any directory in the command line.
+After following these steps, your system should recognize code2gist commands from any directory in the command line. 👍
 
-### GitHub Token
+### GitHub Token 🔑
 
 `code2gist` requires a GitHub token to function. You need to create a new token with the `gist` scope (which allows it to create gists). Follow [this guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a new token.
 
 Once you have your token, you should store it in the "GITHUB_TOKEN" environment variable. Here are the steps to set this variable in Windows:
 
 1. Open the Control Panel.
 2. Search for "Environment Variables".
 3. Click on "Edit the system environment variables".
 4. In the System Properties window that appears, click the "Environment Variables..." button.
 5. In the Environment Variables window, click the "New..." button under the "User variables" section.
 6. Enter "GITHUB_TOKEN" as the variable name and your token as the variable value.
 7. Click "OK" on all open windows to apply the changes.
 
-Please ensure that you have this variable set before using the package.
+Please ensure that you have this variable set before using the package. ✅
 
-## Usage
+## Usage 🚀
 
-### Uploading Files
+### Uploading Files 📤
 
 To use `code2gist`, simply use the following command:
 
 ```
+Copy code
 code2gist .
 ```
 
 This command will upload all Python files in the current directory to a private Gist on your GitHub account. The Gist will be titled with the name of the current directory, followed by "[code2gist]".
 
 If you want to include files with different extensions, you can specify them using the `--ext` option:
 
 ```
+cssCopy code
 code2gist . --ext .txt .md .py
 ```
 
 This command will include all text, Markdown, and Python files in the upload.
 
-### Deleting Gists
+### Deleting Gists 🗑️
 
 The `prune` feature allows you to delete all gists created by `code2gist`:
 
 ```
+cssCopy code
 code2gist --prune
 ```
 
 Running this command will delete all your gists with "[code2gist]" in the description.
 
-## .gitignore Support
+## .gitignore Support ✅
 
 `code2gist` respects `.gitignore` rules. Files that match a rule in the `.gitignore` file of the directory being uploaded will be skipped. In addition, by default, `code2gist` skips files and directories that start with a dot (`.`), although this behavior may change in future versions to strictly adhere to `.gitignore`.
 
-## Note
+## Note 📝
 
 The gists created by `code2gist` are private by default, providing a safe way for you to share your code without making it publicly available.
 
 Please remember that `code2gist` is a tool for sharing code and should not be used to share sensitive information. Always ensure that your files do not contain any confidential data before uploading them.
 
-## License
+## License ⚖️
 
-`code2gist` is licensed underthe [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
+`code2gist` is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
 
 ------
 
-We hope `code2gist` serves as a valuable tool in your development toolkit. Happy coding!
+We hope `code2gist` serves as a valuable tool in your development toolkit. Happy coding! 💻👨‍💻
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `code2gist-1.1.3/README.md` & `code2gist-1.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,96 +1,100 @@
-#  code2gist
+# code2gist 📦
 
 `code2gist` is a Python package that makes sharing your code projects easier than ever. With a simple command, it lets you upload your code files to GitHub's Gist. `code2gist` is available on [PyPI](https://pypi.org/project/code2gist/).
 
-The package works hand-in-hand with OpenAI's ChatGPT-4's 'Browse with Bing' feature. This compatibility allows you to present substantial code bases to the model in a single instance, eliminating the need to split your code into smaller parts.
+The package works hand-in-hand with OpenAI's ChatGPT-4's 'Browse with Bing' feature. This compatibility allows you to present substantial code bases to the model in a single instance, eliminating the need to split your code into smaller parts. 🤝
 
-Another key feature of `code2gist` is its ability to handle a wide range of text-based file types, not just Python files.
+Another key feature of `code2gist` is its ability to handle a wide range of text-based file types, not just Python files. 📄
 
-In addition, `code2gist` comes with a `prune` feature that provides a clean way to remove all the gists created by this tool from your GitHub account.
+In addition, `code2gist` comes with a `prune` feature that provides a clean way to remove all the gists created by this tool from your GitHub account. 🪓
 
-## Installation
+## Installation ⚙️
 
 You can install the package via pip:
 
 ```
+Copy code
 pip install code2gist
 ```
 
-### Adding code2gist Directory to the PATH Environment Variable
+### Adding code2gist Directory to the PATH Environment Variable 👣
 
 Here are step-by-step instructions to add the code2gist directory to your PATH environment variable on Windows:
 
 1. Open the **Control Panel**.
 2. Navigate to **System and Security > System**.
 3. Click on the **Advanced system settings** link on the left panel.
 4. Click **Environment Variables**.
 5. Under the **System Variables** section, find and double-click the variable **PATH**.
 6. Click **New**.
 7. Add the directory where code2gist is installed. For example, if you have Python 3.11 installed, the directory might look like this: `C:\...\Python311\Scripts`
 8. Click **OK** to close all windows and save the changes.
 
-After following these steps, your system should recognize code2gist commands from any directory in the command line.
+After following these steps, your system should recognize code2gist commands from any directory in the command line. 👍
 
-### GitHub Token
+### GitHub Token 🔑
 
 `code2gist` requires a GitHub token to function. You need to create a new token with the `gist` scope (which allows it to create gists). Follow [this guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a new token.
 
 Once you have your token, you should store it in the "GITHUB_TOKEN" environment variable. Here are the steps to set this variable in Windows:
 
 1. Open the Control Panel.
 2. Search for "Environment Variables".
 3. Click on "Edit the system environment variables".
 4. In the System Properties window that appears, click the "Environment Variables..." button.
 5. In the Environment Variables window, click the "New..." button under the "User variables" section.
 6. Enter "GITHUB_TOKEN" as the variable name and your token as the variable value.
 7. Click "OK" on all open windows to apply the changes.
 
-Please ensure that you have this variable set before using the package.
+Please ensure that you have this variable set before using the package. ✅
 
-## Usage
+## Usage 🚀
 
-### Uploading Files
+### Uploading Files 📤
 
 To use `code2gist`, simply use the following command:
 
 ```
+Copy code
 code2gist .
 ```
 
 This command will upload all Python files in the current directory to a private Gist on your GitHub account. The Gist will be titled with the name of the current directory, followed by "[code2gist]".
 
 If you want to include files with different extensions, you can specify them using the `--ext` option:
 
 ```
+cssCopy code
 code2gist . --ext .txt .md .py
 ```
 
 This command will include all text, Markdown, and Python files in the upload.
 
-### Deleting Gists
+### Deleting Gists 🗑️
 
 The `prune` feature allows you to delete all gists created by `code2gist`:
 
 ```
+cssCopy code
 code2gist --prune
 ```
 
 Running this command will delete all your gists with "[code2gist]" in the description.
 
-## .gitignore Support
+## .gitignore Support ✅
 
 `code2gist` respects `.gitignore` rules. Files that match a rule in the `.gitignore` file of the directory being uploaded will be skipped. In addition, by default, `code2gist` skips files and directories that start with a dot (`.`), although this behavior may change in future versions to strictly adhere to `.gitignore`.
 
-## Note
+## Note 📝
 
 The gists created by `code2gist` are private by default, providing a safe way for you to share your code without making it publicly available.
 
 Please remember that `code2gist` is a tool for sharing code and should not be used to share sensitive information. Always ensure that your files do not contain any confidential data before uploading them.
 
-## License
+## License ⚖️
 
-`code2gist` is licensed underthe [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
+`code2gist` is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
 
 ------
 
-We hope `code2gist` serves as a valuable tool in your development toolkit. Happy coding!
+We hope `code2gist` serves as a valuable tool in your development toolkit. Happy coding! 💻👨‍💻
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `code2gist-1.1.3/code2gist/main.py` & `code2gist-1.1.4/code2gist/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import argparse
 import json
 import os
+import textwrap
 
 import pathspec
 import requests
 
 
 def create_gist(description, files):
     token = os.getenv("GITHUB_TOKEN")
     if not token:
-        raise ValueError("GITHUB_TOKEN environment variable not found")
+        raise ValueError("❌ GITHUB_TOKEN environment variable not found")
     url = "https://api.github.com/gists"
     headers = {
         "Authorization": f"token {token}",
         "Accept": "application/vnd.github.v3+json",
     }
     data = {
         "public": False,
         "description": description,
         "files": files
     }
     response = requests.post(url, headers=headers, data=json.dumps(data))
     if response.status_code != 201:
-        print(f"Failed to create a gist: {response.text}")
+        print(f"❌ Failed to create a gist: {response.text}")
         return None
     return response.json()
 
+
 def get_files_in_directory(directory, extensions):
     # Load the .gitignore file, if it exists.
     gitignore_path = os.path.join(directory, '.gitignore')
     gitignore = None
     if os.path.exists(gitignore_path):
         with open(gitignore_path, 'r') as f:
             gitignore = pathspec.PathSpec.from_lines('gitwildmatch', f)
@@ -47,56 +49,72 @@
             if gitignore and gitignore.match_file(rel_path):
                 continue
 
             try:
                 with open(path, 'rt') as file:
                     files[rel_path] = {"content": file.read()}
             except (UnicodeDecodeError, IOError) as e:
-                print(f"Error reading file: {path}. Error: {str(e)}")
+                print(f"❌ Error reading file: {path}. Error: {str(e)}")
                 continue
     return files
 
+
 def delete_old_gists():
     token = os.getenv("GITHUB_TOKEN")
     if not token:
-        raise ValueError("GITHUB_TOKEN environment variable not found")
+        raise ValueError("❌ GITHUB_TOKEN environment variable not found")
     url = "https://api.github.com/gists"
     headers = {
         "Authorization": f"token {token}",
         "Accept": "application/vnd.github.v3+json",
     }
     response = requests.get(url, headers=headers)
     if response.status_code != 200:
-        print(f"Failed to fetch gists: {response.text}")
+        print(f"❌ Failed to fetch gists: {response.text}")
         return
     gists = response.json()
     for gist in gists:
         if '[code2gist]' in gist['description']:
             delete_url = f"https://api.github.com/gists/{gist['id']}"
             delete_response = requests.delete(delete_url, headers=headers)
             if delete_response.status_code != 204:
-                print(f"Failed to delete Gist: {gist['id']}, response: {delete_response.text}")
+                print(f"❌ Failed to delete Gist: {gist['id']}, response: {delete_response.text}")
                 continue
-            print(f"Deleted Gist: {gist['id']}")
+            print(f"🔥 Deleted Gist: {gist['id']}")
+
 
 def main():
     parser = argparse.ArgumentParser(description='Upload Python files in a directory to Gist.')
     parser.add_argument('directory', type=str, nargs='?', help='the directory to upload')
     parser.add_argument('--ext', nargs='+', default=['.py'], help='file extensions to include')
     parser.add_argument('--prune', action='store_true', help='delete all gists created by this application')
     args = parser.parse_args()
 
     if args.directory:
         directory = args.directory
         description = os.path.basename(os.getcwd()) + " [code2gist]"
         files = get_files_in_directory(directory, args.ext)
         response = create_gist(description, files)
-        if response:
-            for filename, file_info in response['files'].items():
-                print(f"\n- File: {filename}")
-                print(f" URL: {file_info['raw_url']}")
-                print()
+
+    if response:
+        wrapper = textwrap.TextWrapper(width=99, subsequent_indent=' '*12)
+
+        print("\n" + "="*100)
+        print("📂 Gist URL 📂".center(100))
+        print()
+        print("\n".join(wrapper.wrap(f"{'🌐 URL:'.ljust(10)} {response['html_url']}")))
+        print()
+        print("-"*100)
+        print("📄 File URLs 📄".center(100))
+        for filename, file_info in response['files'].items():
+            print(f"\n{'📁 File:'.ljust(10)} {filename}")
+            url_parts = file_info['raw_url'].split('/raw', 1)
+            print(f"{'🌐 URL:'.ljust(10)} {url_parts[0]}")
+            print(" "*12 + "/raw" + url_parts[1])
+        print("="*100 + "\n")
+
     if args.prune:
         delete_old_gists()
 
+
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `code2gist-1.1.3/code2gist.egg-info/PKG-INFO` & `code2gist-1.1.4/code2gist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,108 +1,112 @@
 Metadata-Version: 2.1
 Name: code2gist
-Version: 1.1.3
+Version: 1.1.4
 Summary: Upload Python files in a directory to a GitHub Gist.
 Author-email: Cameron Spears <flames.garish-0i@icloud.com>
 License: GPL-3.0
 Keywords: python,github,gist,upload
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-#  code2gist
+# code2gist 📦
 
 `code2gist` is a Python package that makes sharing your code projects easier than ever. With a simple command, it lets you upload your code files to GitHub's Gist. `code2gist` is available on [PyPI](https://pypi.org/project/code2gist/).
 
-The package works hand-in-hand with OpenAI's ChatGPT-4's 'Browse with Bing' feature. This compatibility allows you to present substantial code bases to the model in a single instance, eliminating the need to split your code into smaller parts.
+The package works hand-in-hand with OpenAI's ChatGPT-4's 'Browse with Bing' feature. This compatibility allows you to present substantial code bases to the model in a single instance, eliminating the need to split your code into smaller parts. 🤝
 
-Another key feature of `code2gist` is its ability to handle a wide range of text-based file types, not just Python files.
+Another key feature of `code2gist` is its ability to handle a wide range of text-based file types, not just Python files. 📄
 
-In addition, `code2gist` comes with a `prune` feature that provides a clean way to remove all the gists created by this tool from your GitHub account.
+In addition, `code2gist` comes with a `prune` feature that provides a clean way to remove all the gists created by this tool from your GitHub account. 🪓
 
-## Installation
+## Installation ⚙️
 
 You can install the package via pip:
 
 ```
+Copy code
 pip install code2gist
 ```
 
-### Adding code2gist Directory to the PATH Environment Variable
+### Adding code2gist Directory to the PATH Environment Variable 👣
 
 Here are step-by-step instructions to add the code2gist directory to your PATH environment variable on Windows:
 
 1. Open the **Control Panel**.
 2. Navigate to **System and Security > System**.
 3. Click on the **Advanced system settings** link on the left panel.
 4. Click **Environment Variables**.
 5. Under the **System Variables** section, find and double-click the variable **PATH**.
 6. Click **New**.
 7. Add the directory where code2gist is installed. For example, if you have Python 3.11 installed, the directory might look like this: `C:\...\Python311\Scripts`
 8. Click **OK** to close all windows and save the changes.
 
-After following these steps, your system should recognize code2gist commands from any directory in the command line.
+After following these steps, your system should recognize code2gist commands from any directory in the command line. 👍
 
-### GitHub Token
+### GitHub Token 🔑
 
 `code2gist` requires a GitHub token to function. You need to create a new token with the `gist` scope (which allows it to create gists). Follow [this guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a new token.
 
 Once you have your token, you should store it in the "GITHUB_TOKEN" environment variable. Here are the steps to set this variable in Windows:
 
 1. Open the Control Panel.
 2. Search for "Environment Variables".
 3. Click on "Edit the system environment variables".
 4. In the System Properties window that appears, click the "Environment Variables..." button.
 5. In the Environment Variables window, click the "New..." button under the "User variables" section.
 6. Enter "GITHUB_TOKEN" as the variable name and your token as the variable value.
 7. Click "OK" on all open windows to apply the changes.
 
-Please ensure that you have this variable set before using the package.
+Please ensure that you have this variable set before using the package. ✅
 
-## Usage
+## Usage 🚀
 
-### Uploading Files
+### Uploading Files 📤
 
 To use `code2gist`, simply use the following command:
 
 ```
+Copy code
 code2gist .
 ```
 
 This command will upload all Python files in the current directory to a private Gist on your GitHub account. The Gist will be titled with the name of the current directory, followed by "[code2gist]".
 
 If you want to include files with different extensions, you can specify them using the `--ext` option:
 
 ```
+cssCopy code
 code2gist . --ext .txt .md .py
 ```
 
 This command will include all text, Markdown, and Python files in the upload.
 
-### Deleting Gists
+### Deleting Gists 🗑️
 
 The `prune` feature allows you to delete all gists created by `code2gist`:
 
 ```
+cssCopy code
 code2gist --prune
 ```
 
 Running this command will delete all your gists with "[code2gist]" in the description.
 
-## .gitignore Support
+## .gitignore Support ✅
 
 `code2gist` respects `.gitignore` rules. Files that match a rule in the `.gitignore` file of the directory being uploaded will be skipped. In addition, by default, `code2gist` skips files and directories that start with a dot (`.`), although this behavior may change in future versions to strictly adhere to `.gitignore`.
 
-## Note
+## Note 📝
 
 The gists created by `code2gist` are private by default, providing a safe way for you to share your code without making it publicly available.
 
 Please remember that `code2gist` is a tool for sharing code and should not be used to share sensitive information. Always ensure that your files do not contain any confidential data before uploading them.
 
-## License
+## License ⚖️
 
-`code2gist` is licensed underthe [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
+`code2gist` is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
 
 ------
 
-We hope `code2gist` serves as a valuable tool in your development toolkit. Happy coding!
+We hope `code2gist` serves as a valuable tool in your development toolkit. Happy coding! 💻👨‍💻
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `code2gist-1.1.3/pyproject.toml` & `code2gist-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "code2gist"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
     {name = "Cameron Spears", email = "flames.garish-0i@icloud.com"},
 ]
 description = "Upload Python files in a directory to a GitHub Gist."
 readme = "README.md"
 requires-python = ">=3.11.4"
 keywords = ["python", "github", "gist", "upload"]
```

