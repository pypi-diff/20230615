# Comparing `tmp/myl-0.8.4.tar.gz` & `tmp/myl-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.8.4.tar", last modified: Wed Jun 14 17:13:06 2023, max compression
+gzip compressed data, was "myl-0.8.5.tar", last modified: Thu Jun 15 06:15:18 2023, max compression
```

## Comparing `myl-0.8.4.tar` & `myl-0.8.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:13:06.744591 myl-0.8.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:13:06.740591 myl-0.8.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 17:12:52.000000 myl-0.8.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:13:06.740591 myl-0.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 17:12:52.000000 myl-0.8.4/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 17:12:52.000000 myl-0.8.4/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-14 17:12:52.000000 myl-0.8.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 17:12:52.000000 myl-0.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 17:12:52.000000 myl-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43233 2023-06-14 17:13:06.744591 myl-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-14 17:12:52.000000 myl-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:13:06.740591 myl-0.8.4/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43233 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-14 17:12:52.000000 myl-0.8.4/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-14 17:12:52.000000 myl-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:13:06.744591 myl-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:15:18.023738 myl-0.8.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:15:18.019739 myl-0.8.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 06:15:06.000000 myl-0.8.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:15:18.019739 myl-0.8.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 06:15:06.000000 myl-0.8.5/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 06:15:06.000000 myl-0.8.5/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-15 06:15:06.000000 myl-0.8.5/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 06:15:06.000000 myl-0.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 06:15:06.000000 myl-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42933 2023-06-15 06:15:18.019739 myl-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-15 06:15:06.000000 myl-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:15:18.019739 myl-0.8.5/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42933 2023-06-15 06:15:17.000000 myl-0.8.5/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-15 06:15:18.000000 myl-0.8.5/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:15:17.000000 myl-0.8.5/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 06:15:17.000000 myl-0.8.5/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 06:15:17.000000 myl-0.8.5/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 06:15:17.000000 myl-0.8.5/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-15 06:15:06.000000 myl-0.8.5/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-15 06:15:06.000000 myl-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:15:18.023738 myl-0.8.5/setup.cfg
```

### Comparing `myl-0.8.4/.github/workflows/pypi.yaml` & `myl-0.8.5/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.8.4/.github/workflows/release.yaml` & `myl-0.8.5/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.8.4/LICENSE` & `myl-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.8.4/PKG-INFO` & `myl-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.4
+Version: 0.8.5
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,15 +703,15 @@
 - Fetch a specific number of messages
 - Mark messages as seen
 - Fetch messages from a specific folder
 - Search for specific strings in messages
 - Output HTML email
 - Output raw email
 - Fetch a specific mail by ID
-- Fetch a specific attachment (outputs to stdout)
+- Fetch a specific attachment
 
 ## 🚀 Installation
 
 To install myl, follow these steps:
 
 ```bash
 pipx install myl
@@ -727,48 +727,48 @@
 
 This command will display the help information for the `myl` command.
 
 Here are some examples of using flags with the `myl` command:
 
 ```bash
 # Connect to an IMAP server
-myl --server imap.example.com --username $username --password "$password"
+myl --server imap.example.com --port 143 --starttls --username "$username" --password "$password"
 
 # Use Google IMAP settings
 myl --google --username "$username" --password "$password"
 
 # Autodiscovery of the required server and port
 myl --auto --username "$username" --password "$password"
 
+# We won't repeat the server connection flags from here
+alias myl="command myl --auto --username \"$username\" --password \"$password\""
+
 # Fetch a specific number of messages
-myl --count 5 --username "$username" --password "$password"
+myl --count 5
 
 # Mark messages as seen
-myl --mark-seen --username "$username" --password "$password"
+myl --mark-seen
 
 # Fetch messages from a specific folder
-myl --folder "INBOX" --username "$username" --password "$password"
+myl --folder "INBOX"
 
 # Search for specific strings in messages
-myl --search "important" --username "$username" --password "$password"
-
-# Show raw email
-myl --raw --username "$username" --password "$password"
+myl --search "important"
 
 # Fetch a specific mail ID
-myl --username "$username" --password "$password" "$MAILID"
+myl "$MAILID"
 
 # Show HTML
-myl --html --username "$username" --password "$password" "$MAILID"
+myl --html "$MAILID"
 
 # raw email
-myl --raw --username "$username" --password "$password" "$MAILID" > email.eml
+myl --raw "$MAILID" > email.eml
 
 # Fetch a specific attachment (outputs to stdout)
-myl --username "$username" --password "$password" "$MAILID" "$ATT" > att.txt
+myl "$MAILID" "$ATT" > att.txt
 ```
 
 Please replace `imap.example.com`, `$username`, `$password`, `$MAILID`,
 and `$ATT` with your actual IMAP server details, username, password,
 mail ID, and attachment name.
 
 ## 📜 License
```

### Comparing `myl-0.8.4/myl.egg-info/PKG-INFO` & `myl-0.8.5/myl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.4
+Version: 0.8.5
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,15 +703,15 @@
 - Fetch a specific number of messages
 - Mark messages as seen
 - Fetch messages from a specific folder
 - Search for specific strings in messages
 - Output HTML email
 - Output raw email
 - Fetch a specific mail by ID
-- Fetch a specific attachment (outputs to stdout)
+- Fetch a specific attachment
 
 ## 🚀 Installation
 
 To install myl, follow these steps:
 
 ```bash
 pipx install myl
@@ -727,48 +727,48 @@
 
 This command will display the help information for the `myl` command.
 
 Here are some examples of using flags with the `myl` command:
 
 ```bash
 # Connect to an IMAP server
-myl --server imap.example.com --username $username --password "$password"
+myl --server imap.example.com --port 143 --starttls --username "$username" --password "$password"
 
 # Use Google IMAP settings
 myl --google --username "$username" --password "$password"
 
 # Autodiscovery of the required server and port
 myl --auto --username "$username" --password "$password"
 
+# We won't repeat the server connection flags from here
+alias myl="command myl --auto --username \"$username\" --password \"$password\""
+
 # Fetch a specific number of messages
-myl --count 5 --username "$username" --password "$password"
+myl --count 5
 
 # Mark messages as seen
-myl --mark-seen --username "$username" --password "$password"
+myl --mark-seen
 
 # Fetch messages from a specific folder
-myl --folder "INBOX" --username "$username" --password "$password"
+myl --folder "INBOX"
 
 # Search for specific strings in messages
-myl --search "important" --username "$username" --password "$password"
-
-# Show raw email
-myl --raw --username "$username" --password "$password"
+myl --search "important"
 
 # Fetch a specific mail ID
-myl --username "$username" --password "$password" "$MAILID"
+myl "$MAILID"
 
 # Show HTML
-myl --html --username "$username" --password "$password" "$MAILID"
+myl --html "$MAILID"
 
 # raw email
-myl --raw --username "$username" --password "$password" "$MAILID" > email.eml
+myl --raw "$MAILID" > email.eml
 
 # Fetch a specific attachment (outputs to stdout)
-myl --username "$username" --password "$password" "$MAILID" "$ATT" > att.txt
+myl "$MAILID" "$ATT" > att.txt
 ```
 
 Please replace `imap.example.com`, `$username`, `$password`, `$MAILID`,
 and `$ATT` with your actual IMAP server details, username, password,
 mail ID, and attachment name.
 
 ## 📜 License
```

### Comparing `myl-0.8.4/myl.py` & `myl-0.8.5/myl.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         if args.sent or args.folder == "Sent":
             args.folder = GMAIL_SENT_FOLDER
         # elif args.folder == "INBOX":
         #     args.folder = GMAIL_ALL_FOLDER
     else:
         if args.auto:
             try:
-                settings = autodiscover(args.username).get("imap")
+                settings = autodiscover(args.username, password=args.password).get("imap")
             except Exception:
                 error_msg("Failed to autodiscover IMAP settings")
                 if args.debug:
                     console.print_exception(show_locals=True)
                 return 1
             LOGGER.debug(f"Discovered settings: {settings})")
             args.server = settings.get("server")
```

### Comparing `myl-0.8.4/pyproject.toml` & `myl-0.8.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 keywords = ["imap", "email"]
 license = {file = "LICENSE"}
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "imap-tools == 1.0.0",
-  "myl-discovery == 0.4.0",
+  "myl-discovery == 0.5.2",
   "rich == 13.4.2",
 ]
-version = "0.8.4"
+version = "0.8.5"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

