# Comparing `tmp/stellanow_cli-0.0.2.tar.gz` & `tmp/stellanow_cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellanow_cli-0.0.2.tar", last modified: Thu Jun 15 21:08:47 2023, max compression
+gzip compressed data, was "stellanow_cli-0.0.3.tar", last modified: Thu Jun 15 21:23:45 2023, max compression
```

## Comparing `stellanow_cli-0.0.2.tar` & `stellanow_cli-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.175656 stellanow_cli-0.0.2/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7787 2023-06-15 21:08:47.174300 stellanow_cli-0.0.2/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1761 2023-06-15 20:48:36.000000 stellanow_cli-0.0.2/README.md
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-15 21:08:47.175822 stellanow_cli-0.0.2/setup.cfg
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      935 2023-06-15 21:02:18.000000 stellanow_cli-0.0.2/setup.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:46.927672 stellanow_cli-0.0.2/stellanow_cli/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      322 2023-06-15 20:52:42.000000 stellanow_cli-0.0.2/stellanow_cli/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       22 2023-06-15 21:00:57.000000 stellanow_cli-0.0.2/stellanow_cli/_version.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.036609 stellanow_cli-0.0.2/stellanow_cli/api/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      422 2023-06-15 20:54:39.000000 stellanow_cli-0.0.2/stellanow_cli/api/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6483 2023-06-15 20:54:33.000000 stellanow_cli-0.0.2/stellanow_cli/api/stellanow_api.py
--rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1354 2023-06-15 21:06:20.000000 stellanow_cli-0.0.2/stellanow_cli/cli.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.109286 stellanow_cli-0.0.2/stellanow_cli/code_generators/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      403 2023-06-15 20:54:24.000000 stellanow_cli-0.0.2/stellanow_cli/code_generators/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.2/stellanow_cli/code_generators/code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3185 2023-06-15 20:54:11.000000 stellanow_cli-0.0.2/stellanow_cli/code_generators/csharp_code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3856 2023-06-15 20:52:20.000000 stellanow_cli-0.0.2/stellanow_cli/command_config.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.161181 stellanow_cli-0.0.2/stellanow_cli/config/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.2/stellanow_cli/config/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.2/stellanow_cli/config/config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.2/stellanow_cli/config/dev.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.2/stellanow_cli/config/int.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      879 2023-06-15 20:52:13.000000 stellanow_cli-0.0.2/stellanow_cli/logger.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-15 20:51:44.000000 stellanow_cli-0.0.2/stellanow_cli/utils.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      797 2023-06-15 20:51:30.000000 stellanow_cli-0.0.2/stellanow_cli/validate.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.007513 stellanow_cli-0.0.2/stellanow_cli.egg-info/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7787 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      782 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/entry_points.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/requires.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/top_level.txt
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.170423 stellanow_cli-0.0.2/tests/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.2/tests/test_command_configure.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:23:45.757886 stellanow_cli-0.0.3/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7811 2023-06-15 21:23:45.757337 stellanow_cli-0.0.3/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     9418 2023-06-15 21:15:01.000000 stellanow_cli-0.0.3/README.md
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-15 21:23:45.757974 stellanow_cli-0.0.3/setup.cfg
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      935 2023-06-15 21:02:18.000000 stellanow_cli-0.0.3/setup.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:23:45.633817 stellanow_cli-0.0.3/stellanow_cli/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      322 2023-06-15 20:52:42.000000 stellanow_cli-0.0.3/stellanow_cli/__init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       22 2023-06-15 21:23:09.000000 stellanow_cli-0.0.3/stellanow_cli/_version.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:23:45.715865 stellanow_cli-0.0.3/stellanow_cli/api/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      422 2023-06-15 20:54:39.000000 stellanow_cli-0.0.3/stellanow_cli/api/__init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6483 2023-06-15 20:54:33.000000 stellanow_cli-0.0.3/stellanow_cli/api/stellanow_api.py
+-rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1354 2023-06-15 21:06:20.000000 stellanow_cli-0.0.3/stellanow_cli/cli.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:23:45.751266 stellanow_cli-0.0.3/stellanow_cli/code_generators/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      403 2023-06-15 20:54:24.000000 stellanow_cli-0.0.3/stellanow_cli/code_generators/__init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.3/stellanow_cli/code_generators/code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3185 2023-06-15 20:54:11.000000 stellanow_cli-0.0.3/stellanow_cli/code_generators/csharp_code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3856 2023-06-15 20:52:20.000000 stellanow_cli-0.0.3/stellanow_cli/command_config.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:23:45.755369 stellanow_cli-0.0.3/stellanow_cli/config/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.3/stellanow_cli/config/__init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.3/stellanow_cli/config/config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.3/stellanow_cli/config/dev.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.3/stellanow_cli/config/int.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      879 2023-06-15 20:52:13.000000 stellanow_cli-0.0.3/stellanow_cli/logger.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-15 20:51:44.000000 stellanow_cli-0.0.3/stellanow_cli/utils.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      797 2023-06-15 20:51:30.000000 stellanow_cli-0.0.3/stellanow_cli/validate.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:23:45.702633 stellanow_cli-0.0.3/stellanow_cli.egg-info/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7811 2023-06-15 21:23:45.000000 stellanow_cli-0.0.3/stellanow_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      782 2023-06-15 21:23:45.000000 stellanow_cli-0.0.3/stellanow_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-15 21:23:45.000000 stellanow_cli-0.0.3/stellanow_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-15 21:23:45.000000 stellanow_cli-0.0.3/stellanow_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-15 21:23:45.000000 stellanow_cli-0.0.3/stellanow_cli.egg-info/requires.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-15 21:23:45.000000 stellanow_cli-0.0.3/stellanow_cli.egg-info/top_level.txt
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:23:45.756379 stellanow_cli-0.0.3/tests/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.3/tests/test_command_configure.py
```

### Comparing `stellanow_cli-0.0.2/PKG-INFO` & `stellanow_cli-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,140 @@
 Metadata-Version: 2.1
 Name: stellanow_cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: A comprehensive Python package for data analysis and visualization.
 Requires-Python: ==3.10.*
 
-# StellaNow CLI Tool
+StellaNow CLI Tool
+==================
+
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
 
-## Installation
+Installation
+------------
+
 To install the StellaNow CLI tool, run the following command:
 
     pip install stellanow
 
 The tool is hosted on PYPI and can be installed via pip.
 
-## Usage
+Usage
+-----
+
 After installation, you can use the 'stellanow' command in your terminal to interact with StellaNow services. Here is how to use some of the available commands:
 
-### Configure
+**Configure**
+
 You can use the 'configure' command to setup the necessary credentials and configurations for a specific profile. The profile will store a particular set of configurations.
 
 Here is how to use the command:
 
     stellanow configure --profile YOUR_PROFILE_NAME
 
 If no profile is specified, the configurations will be stored under the 'DEFAULT' profile. Profile names are case-sensitive.
 
-### Environment Variables
+**Environment Variables**
+
 The stellanow CLI can also read the following environment variables:
 
     STELLANOW_ACCESS_KEY: Your access key.
     STELLANOW_ACCESS_TOKEN: Your access token.
 
-### Credentials Precedence Order
+**Credentials Precedence Order**
+
 In StellaNow CLI, there is a specific order of precedence for the way credentials and other settings are obtained. This means if a setting is provided in more than one place, the setting from the source with the highest precedence will be used. The order of precedence is:
 
     Environment Variables -> Command Line Options -> Configuration File
 
 * **Environment Variables**: These have the highest precedence. If a setting is provided as an environment variable, it will override any value provided as a command line option or in the configuration file.
 * **Command Line Options**: These have the second-highest precedence. If a setting is provided as a command line option, it will override any value provided in the configuration file.
 * **Configuration File**: This has the lowest precedence. Settings in the configuration file will be used if no value for the same setting is provided as an environment variable or as a command line option.
 
 * This order of precedence provides flexibility, allowing you to set default values in the configuration file but override them for specific operations with command line options or environment variables.
 
-## Commands
+Commands
+--------
+
+**'configure'**
 
-### 'configure'
 The **'configure'** command sets up the necessary credentials and configurations for a specific profile or for the DEFAULT profile if none is specified.
 
-#### Command usage:
+Command usage:
 
     stellanow configure --profile myProfile
 
-#### Command options:
+Command options:
 
 * **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 
 This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is 'myProfile'. If you do not specify a profile, the command will default to the 'DEFAULT' profile.
 
 The command validates the provided values to ensure they meet the expected formats: the access key should be a valid email address or a string containing only alphanumeric characters, dashes, and underscores; the access token should be a string with no whitespace and a length of 8-64 characters; and both the organization ID and project ID should be valid UUIDs.
 
 The command then writes these configurations to a file named 'config.ini' in the '.stellanow' directory of your home folder. If this directory or file does not exist, they will be created.
 
-### 'events'
+**'events'**
+
 The **'events'** command fetches the latest event specifications from the API and outputs a list of the events into the terminal prompt.
 
-#### Command usage:
+Command usage:
 
     stellanow events
 
 This will print a table of all available events with their metadata (EventID, Event Name, Is Active, Created At, Updated At).
 
-#### Command options:
+Command options:
 
 * No options required.
 
-### 'plan'
+**'plan'**
+
 The **'plan'** command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
 
-#### Command usage:
+Command usage:
 
     stellanow plan --input_dir .
 
 This will scan all the auto-generated files in the current directory and compare them with the latest specifications from the API.
 
-#### Command options:
+Command options:
 
 * **'--input_dir (-i)'**: The directory to read generated classes from. Defaults to the current directory.
 
-### 'generate'
+**'generate'**
+
 The **'generate'** command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
 
-#### Command usage:
+Command usage:
 
     stellanow generate --namespace MyApp.Messages --destination . --force --events Event1,Event2 --language csharp
 
 This will generate C# classes for events 'Event1' and 'Event2', placing them in the current directory. The generated classes will be in the namespace 'MyApp.Messages'. If a file for an event already exists, it will be overwritten due to the **'--force'** flag.
 
-#### Command options:
+Command options:
 
 * **'--namespace (-n)'**: The namespace for the generated classes. Defaults to an empty string.
 * **'--destination (-d)'**: The directory to save the generated classes. Defaults to the current directory.
 * **'--force (-f)'**: A flag indicating whether to overwrite existing files. Defaults to false.
 * **'--events (-e)'**: A list of specific events to generate. If this option is not provided, classes for all events will be generated.
 * **'--language (-l)'**: The programming language for the generated classes. Can be 'csharp'. Defaults to 'csharp'.
 
-### Common Command Options
+**Common Command Options**
 
 * **'--access_key'**: The access key credential for accessing the StellaNow API. This should be the same as your StellaNow account access key.
 * **'--access_token'**: The access token credential for accessing the StellaNow API. This should be the same as your StellaNow account access token.
 * **'--organization_id'**: The unique identifier (UUID) of the organization in StellaNow. This is used to scope the operations within the given organization's context.
 * **'--project_id'**: The unique identifier (UUID) of the project in StellaNow. This is used to scope the operations within the given project's context.
 * **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 * **'--verbose (-v)'**: Enables verbose mode, which outputs more detailed logging messages.
 
 These options allow for flexible command-line operation, as they let you provide command-specific details without altering your saved profile configurations. If these options are not specified in the command, the values saved in the specified profile (or the DEFAULT profile if none is specified) will be used.
 
 Please note that providing these options at the command line overrides the corresponding saved profile values for the duration of that command execution only. See **Credential Precedence Order** section for details.
 
-## Contact and Licensing
-For further assistance and support, please contact us at ***help@stella.systems***
+Contact and Licensing
+---------------------
+
+For further assistance and support, please contact us at **help@stella.systems**
 
 The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
```

### Comparing `stellanow_cli-0.0.2/setup.py` & `stellanow_cli-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/stellanow_cli/api/stellanow_api.py` & `stellanow_cli-0.0.3/stellanow_cli/api/stellanow_api.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/stellanow_cli/cli.py` & `stellanow_cli-0.0.3/stellanow_cli/cli.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/stellanow_cli/code_generators/code_generator.py` & `stellanow_cli-0.0.3/stellanow_cli/code_generators/code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/stellanow_cli/code_generators/csharp_code_generator.py` & `stellanow_cli-0.0.3/stellanow_cli/code_generators/csharp_code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/stellanow_cli/command_config.py` & `stellanow_cli-0.0.3/stellanow_cli/command_config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/stellanow_cli/config/config.py` & `stellanow_cli-0.0.3/stellanow_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/stellanow_cli/logger.py` & `stellanow_cli-0.0.3/stellanow_cli/logger.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/stellanow_cli/utils.py` & `stellanow_cli-0.0.3/stellanow_cli/utils.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/stellanow_cli/validate.py` & `stellanow_cli-0.0.3/stellanow_cli/validate.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/stellanow_cli.egg-info/PKG-INFO` & `stellanow_cli-0.0.3/stellanow_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,124 +1,140 @@
 Metadata-Version: 2.1
 Name: stellanow-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: A comprehensive Python package for data analysis and visualization.
 Requires-Python: ==3.10.*
 
-# StellaNow CLI Tool
+StellaNow CLI Tool
+==================
+
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
 
-## Installation
+Installation
+------------
+
 To install the StellaNow CLI tool, run the following command:
 
     pip install stellanow
 
 The tool is hosted on PYPI and can be installed via pip.
 
-## Usage
+Usage
+-----
+
 After installation, you can use the 'stellanow' command in your terminal to interact with StellaNow services. Here is how to use some of the available commands:
 
-### Configure
+**Configure**
+
 You can use the 'configure' command to setup the necessary credentials and configurations for a specific profile. The profile will store a particular set of configurations.
 
 Here is how to use the command:
 
     stellanow configure --profile YOUR_PROFILE_NAME
 
 If no profile is specified, the configurations will be stored under the 'DEFAULT' profile. Profile names are case-sensitive.
 
-### Environment Variables
+**Environment Variables**
+
 The stellanow CLI can also read the following environment variables:
 
     STELLANOW_ACCESS_KEY: Your access key.
     STELLANOW_ACCESS_TOKEN: Your access token.
 
-### Credentials Precedence Order
+**Credentials Precedence Order**
+
 In StellaNow CLI, there is a specific order of precedence for the way credentials and other settings are obtained. This means if a setting is provided in more than one place, the setting from the source with the highest precedence will be used. The order of precedence is:
 
     Environment Variables -> Command Line Options -> Configuration File
 
 * **Environment Variables**: These have the highest precedence. If a setting is provided as an environment variable, it will override any value provided as a command line option or in the configuration file.
 * **Command Line Options**: These have the second-highest precedence. If a setting is provided as a command line option, it will override any value provided in the configuration file.
 * **Configuration File**: This has the lowest precedence. Settings in the configuration file will be used if no value for the same setting is provided as an environment variable or as a command line option.
 
 * This order of precedence provides flexibility, allowing you to set default values in the configuration file but override them for specific operations with command line options or environment variables.
 
-## Commands
+Commands
+--------
+
+**'configure'**
 
-### 'configure'
 The **'configure'** command sets up the necessary credentials and configurations for a specific profile or for the DEFAULT profile if none is specified.
 
-#### Command usage:
+Command usage:
 
     stellanow configure --profile myProfile
 
-#### Command options:
+Command options:
 
 * **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 
 This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is 'myProfile'. If you do not specify a profile, the command will default to the 'DEFAULT' profile.
 
 The command validates the provided values to ensure they meet the expected formats: the access key should be a valid email address or a string containing only alphanumeric characters, dashes, and underscores; the access token should be a string with no whitespace and a length of 8-64 characters; and both the organization ID and project ID should be valid UUIDs.
 
 The command then writes these configurations to a file named 'config.ini' in the '.stellanow' directory of your home folder. If this directory or file does not exist, they will be created.
 
-### 'events'
+**'events'**
+
 The **'events'** command fetches the latest event specifications from the API and outputs a list of the events into the terminal prompt.
 
-#### Command usage:
+Command usage:
 
     stellanow events
 
 This will print a table of all available events with their metadata (EventID, Event Name, Is Active, Created At, Updated At).
 
-#### Command options:
+Command options:
 
 * No options required.
 
-### 'plan'
+**'plan'**
+
 The **'plan'** command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
 
-#### Command usage:
+Command usage:
 
     stellanow plan --input_dir .
 
 This will scan all the auto-generated files in the current directory and compare them with the latest specifications from the API.
 
-#### Command options:
+Command options:
 
 * **'--input_dir (-i)'**: The directory to read generated classes from. Defaults to the current directory.
 
-### 'generate'
+**'generate'**
+
 The **'generate'** command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
 
-#### Command usage:
+Command usage:
 
     stellanow generate --namespace MyApp.Messages --destination . --force --events Event1,Event2 --language csharp
 
 This will generate C# classes for events 'Event1' and 'Event2', placing them in the current directory. The generated classes will be in the namespace 'MyApp.Messages'. If a file for an event already exists, it will be overwritten due to the **'--force'** flag.
 
-#### Command options:
+Command options:
 
 * **'--namespace (-n)'**: The namespace for the generated classes. Defaults to an empty string.
 * **'--destination (-d)'**: The directory to save the generated classes. Defaults to the current directory.
 * **'--force (-f)'**: A flag indicating whether to overwrite existing files. Defaults to false.
 * **'--events (-e)'**: A list of specific events to generate. If this option is not provided, classes for all events will be generated.
 * **'--language (-l)'**: The programming language for the generated classes. Can be 'csharp'. Defaults to 'csharp'.
 
-### Common Command Options
+**Common Command Options**
 
 * **'--access_key'**: The access key credential for accessing the StellaNow API. This should be the same as your StellaNow account access key.
 * **'--access_token'**: The access token credential for accessing the StellaNow API. This should be the same as your StellaNow account access token.
 * **'--organization_id'**: The unique identifier (UUID) of the organization in StellaNow. This is used to scope the operations within the given organization's context.
 * **'--project_id'**: The unique identifier (UUID) of the project in StellaNow. This is used to scope the operations within the given project's context.
 * **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 * **'--verbose (-v)'**: Enables verbose mode, which outputs more detailed logging messages.
 
 These options allow for flexible command-line operation, as they let you provide command-specific details without altering your saved profile configurations. If these options are not specified in the command, the values saved in the specified profile (or the DEFAULT profile if none is specified) will be used.
 
 Please note that providing these options at the command line overrides the corresponding saved profile values for the duration of that command execution only. See **Credential Precedence Order** section for details.
 
-## Contact and Licensing
-For further assistance and support, please contact us at ***help@stella.systems***
+Contact and Licensing
+---------------------
+
+For further assistance and support, please contact us at **help@stella.systems**
 
 The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
```

### Comparing `stellanow_cli-0.0.2/stellanow_cli.egg-info/SOURCES.txt` & `stellanow_cli-0.0.3/stellanow_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.2/tests/test_command_configure.py` & `stellanow_cli-0.0.3/tests/test_command_configure.py`

 * *Files identical despite different names*

