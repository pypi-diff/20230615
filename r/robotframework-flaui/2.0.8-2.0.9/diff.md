# Comparing `tmp/robotframework-flaui-2.0.8.tar.gz` & `tmp/robotframework-flaui-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-flaui-2.0.8.tar", last modified: Tue Apr  4 18:17:27 2023, max compression
+gzip compressed data, was "robotframework-flaui-2.0.9.tar", last modified: Wed Apr  5 00:28:25 2023, max compression
```

## Comparing `robotframework-flaui-2.0.8.tar` & `robotframework-flaui-2.0.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.884695 robotframework-flaui-2.0.8/
--rw-rw-rw-   0        0        0     1079 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/LICENSE
--rw-rw-rw-   0        0        0       40 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7853 2023-04-04 18:17:27.884695 robotframework-flaui-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6996 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/README.md
--rw-rw-rw-   0        0        0      103 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.806546 robotframework-flaui-2.0.8/robotframework_flaui.egg-info/
--rw-rw-rw-   0        0        0     7853 2023-04-04 18:17:27.000000 robotframework-flaui-2.0.8/robotframework_flaui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2891 2023-04-04 18:17:27.000000 robotframework-flaui-2.0.8/robotframework_flaui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 18:17:27.000000 robotframework-flaui-2.0.8/robotframework_flaui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-04-04 18:17:27.000000 robotframework-flaui-2.0.8/robotframework_flaui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-04 18:17:27.000000 robotframework-flaui-2.0.8/robotframework_flaui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 18:17:27.884695 robotframework-flaui-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2559 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.790967 robotframework-flaui-2.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.822193 robotframework-flaui-2.0.8/src/FlaUILibrary/
--rw-rw-rw-   0        0        0     8039 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.822193 robotframework-flaui-2.0.8/src/FlaUILibrary/bin/
--rw-rw-rw-   0        0        0   256512 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/bin/FlaUI.Core.dll
--rw-rw-rw-   0        0        0    76288 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/bin/FlaUI.UIA2.dll
--rw-rw-rw-   0        0        0   105984 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/bin/FlaUI.UIA3.dll
--rw-rw-rw-   0        0        0   151040 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.822193 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/
--rw-rw-rw-   0        0        0        0 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.822193 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/automation/
--rw-rw-rw-   0        0        0       46 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/automation/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/automation/uia.py
--rw-rw-rw-   0        0        0     1062 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/automation/uia2.py
--rw-rw-rw-   0        0        0     1062 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/automation/uia3.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.822193 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/enum/
--rw-rw-rw-   0        0        0       84 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/enum/__init__.py
--rw-rw-rw-   0        0        0      305 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/enum/interfacetype.py
--rw-rw-rw-   0        0        0      229 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/enum/treeitemaction.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.837818 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/exception/
--rw-rw-rw-   0        0        0       36 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/exception/__init__.py
--rw-rw-rw-   0        0        0     2525 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/exception/flauierror.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.837818 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/interface/
--rw-rw-rw-   0        0        0      158 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/interface/__init__.py
--rw-rw-rw-   0        0        0      737 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/interface/moduleinterface.py
--rw-rw-rw-   0        0        0      248 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/interface/valuecontainer.py
--rw-rw-rw-   0        0        0     1289 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.853443 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/
--rw-rw-rw-   0        0        0      484 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/__init__.py
--rw-rw-rw-   0        0        0     9161 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/application.py
--rw-rw-rw-   0        0        0     2512 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/checkbox.py
--rw-rw-rw-   0        0        0     2146 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/combobox.py
--rw-rw-rw-   0        0        0     2179 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/debug.py
--rw-rw-rw-   0        0        0    17419 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/element.py
--rw-rw-rw-   0        0        0     5767 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/grid.py
--rw-rw-rw-   0        0        0     4270 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/keyboard.py
--rw-rw-rw-   0        0        0     6061 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/mouse.py
--rw-rw-rw-   0        0        0    11810 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/property.py
--rw-rw-rw-   0        0        0     4605 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/screenshot.py
--rw-rw-rw-   0        0        0     8863 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/selector.py
--rw-rw-rw-   0        0        0     3224 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/tab.py
--rw-rw-rw-   0        0        0     2613 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/textbox.py
--rw-rw-rw-   0        0        0     1698 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/tooglebutton.py
--rw-rw-rw-   0        0        0     6711 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/tree.py
--rw-rw-rw-   0        0        0     2158 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/window.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.853443 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/util/
--rw-rw-rw-   0        0        0      140 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/util/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/util/converter.py
--rw-rw-rw-   0        0        0     7532 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/util/keyboardinputconverter.py
--rw-rw-rw-   0        0        0     5525 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/util/treeitems.py
--rw-rw-rw-   0        0        0     1728 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/util/treeitemsparser.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.869077 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/
--rw-rw-rw-   0        0        0      639 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/application.py
--rw-rw-rw-   0        0        0     2508 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/checkbox.py
--rw-rw-rw-   0        0        0     8813 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/combobox.py
--rw-rw-rw-   0        0        0     2352 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/debug.py
--rw-rw-rw-   0        0        0    15920 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/element.py
--rw-rw-rw-   0        0        0     4197 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/grid.py
--rw-rw-rw-   0        0        0     8994 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/keyboard.py
--rw-rw-rw-   0        0        0     6980 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/listbox.py
--rw-rw-rw-   0        0        0     7690 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/mouse.py
--rw-rw-rw-   0        0        0    28336 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/property.py
--rw-rw-rw-   0        0        0     2559 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/radiobutton.py
--rw-rw-rw-   0        0        0     2283 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/screenshot.py
--rw-rw-rw-   0        0        0     2399 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/tab.py
--rw-rw-rw-   0        0        0     2392 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/textbox.py
--rw-rw-rw-   0        0        0     1404 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/togglebutton.py
--rw-rw-rw-   0        0        0    13001 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/tree.py
--rw-rw-rw-   0        0        0     1230 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/window.py
--rw-rw-rw-   0        0        0      838 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/pythonnetwrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:17:27.884695 robotframework-flaui-2.0.8/src/FlaUILibrary/robotframework/
--rw-rw-rw-   0        0        0        0 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/robotframework/__init__.py
--rw-rw-rw-   0        0        0     1041 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/robotframework/robotlog.py
--rw-rw-rw-   0        0        0        0 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/robotframework/test.py
--rw-rw-rw-   0        0        0       18 2023-04-04 18:16:43.000000 robotframework-flaui-2.0.8/src/FlaUILibrary/version.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:25.020681 robotframework-flaui-2.0.9/
+-rw-rw-rw-   0        0        0     1079 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7821 2023-04-05 00:28:25.020681 robotframework-flaui-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6964 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/README.md
+-rw-rw-rw-   0        0        0      103 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:24.942542 robotframework-flaui-2.0.9/robotframework_flaui.egg-info/
+-rw-rw-rw-   0        0        0     7821 2023-04-05 00:28:24.000000 robotframework-flaui-2.0.9/robotframework_flaui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2891 2023-04-05 00:28:24.000000 robotframework-flaui-2.0.9/robotframework_flaui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-05 00:28:24.000000 robotframework-flaui-2.0.9/robotframework_flaui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-04-05 00:28:24.000000 robotframework-flaui-2.0.9/robotframework_flaui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-05 00:28:24.000000 robotframework-flaui-2.0.9/robotframework_flaui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-05 00:28:25.020681 robotframework-flaui-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1935 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:24.926922 robotframework-flaui-2.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:24.958189 robotframework-flaui-2.0.9/src/FlaUILibrary/
+-rw-rw-rw-   0        0        0     8039 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:24.958189 robotframework-flaui-2.0.9/src/FlaUILibrary/bin/
+-rw-rw-rw-   0        0        0   256512 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/bin/FlaUI.Core.dll
+-rw-rw-rw-   0        0        0    76288 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/bin/FlaUI.UIA2.dll
+-rw-rw-rw-   0        0        0   105984 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/bin/FlaUI.UIA3.dll
+-rw-rw-rw-   0        0        0   151040 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:24.958189 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/
+-rw-rw-rw-   0        0        0        0 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:24.973795 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/automation/
+-rw-rw-rw-   0        0        0       46 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/automation/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/automation/uia.py
+-rw-rw-rw-   0        0        0     1062 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/automation/uia2.py
+-rw-rw-rw-   0        0        0     1062 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/automation/uia3.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:24.973795 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/enum/
+-rw-rw-rw-   0        0        0       84 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/enum/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/enum/interfacetype.py
+-rw-rw-rw-   0        0        0      229 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/enum/treeitemaction.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:24.973795 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/exception/
+-rw-rw-rw-   0        0        0       36 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/exception/__init__.py
+-rw-rw-rw-   0        0        0     2525 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/exception/flauierror.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:24.973795 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/interface/
+-rw-rw-rw-   0        0        0      158 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/interface/__init__.py
+-rw-rw-rw-   0        0        0      737 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/interface/moduleinterface.py
+-rw-rw-rw-   0        0        0      248 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/interface/valuecontainer.py
+-rw-rw-rw-   0        0        0     1289 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:24.989427 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/
+-rw-rw-rw-   0        0        0      484 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/__init__.py
+-rw-rw-rw-   0        0        0     9161 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/application.py
+-rw-rw-rw-   0        0        0     2512 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/checkbox.py
+-rw-rw-rw-   0        0        0     2146 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/combobox.py
+-rw-rw-rw-   0        0        0     2179 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/debug.py
+-rw-rw-rw-   0        0        0    17419 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/element.py
+-rw-rw-rw-   0        0        0     5767 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/grid.py
+-rw-rw-rw-   0        0        0     4270 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/keyboard.py
+-rw-rw-rw-   0        0        0     6061 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/mouse.py
+-rw-rw-rw-   0        0        0    11810 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/property.py
+-rw-rw-rw-   0        0        0     4605 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/screenshot.py
+-rw-rw-rw-   0        0        0     8863 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/selector.py
+-rw-rw-rw-   0        0        0     3224 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/tab.py
+-rw-rw-rw-   0        0        0     2613 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/textbox.py
+-rw-rw-rw-   0        0        0     1698 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/tooglebutton.py
+-rw-rw-rw-   0        0        0     6711 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/tree.py
+-rw-rw-rw-   0        0        0     2158 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/window.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:25.005056 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/util/
+-rw-rw-rw-   0        0        0      140 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/util/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/util/converter.py
+-rw-rw-rw-   0        0        0     7532 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/util/keyboardinputconverter.py
+-rw-rw-rw-   0        0        0     5525 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/util/treeitems.py
+-rw-rw-rw-   0        0        0     1728 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/util/treeitemsparser.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:25.020681 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/
+-rw-rw-rw-   0        0        0      639 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/__init__.py
+-rw-rw-rw-   0        0        0     4822 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/application.py
+-rw-rw-rw-   0        0        0     2508 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/checkbox.py
+-rw-rw-rw-   0        0        0     8813 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/combobox.py
+-rw-rw-rw-   0        0        0     2352 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/debug.py
+-rw-rw-rw-   0        0        0    15920 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/element.py
+-rw-rw-rw-   0        0        0     4197 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/grid.py
+-rw-rw-rw-   0        0        0     8994 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/keyboard.py
+-rw-rw-rw-   0        0        0     6980 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/listbox.py
+-rw-rw-rw-   0        0        0     7690 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/mouse.py
+-rw-rw-rw-   0        0        0    28336 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/property.py
+-rw-rw-rw-   0        0        0     2559 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/radiobutton.py
+-rw-rw-rw-   0        0        0     2283 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/screenshot.py
+-rw-rw-rw-   0        0        0     2399 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/tab.py
+-rw-rw-rw-   0        0        0     2392 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/textbox.py
+-rw-rw-rw-   0        0        0     1404 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/togglebutton.py
+-rw-rw-rw-   0        0        0    13001 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/tree.py
+-rw-rw-rw-   0        0        0     1230 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/window.py
+-rw-rw-rw-   0        0        0      838 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/pythonnetwrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-05 00:28:25.020681 robotframework-flaui-2.0.9/src/FlaUILibrary/robotframework/
+-rw-rw-rw-   0        0        0        0 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/robotframework/__init__.py
+-rw-rw-rw-   0        0        0     1041 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/robotframework/robotlog.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/robotframework/test.py
+-rw-rw-rw-   0        0        0       18 2023-04-05 00:27:39.000000 robotframework-flaui-2.0.9/src/FlaUILibrary/version.py
```

### Comparing `robotframework-flaui-2.0.8/LICENSE` & `robotframework-flaui-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/PKG-INFO` & `robotframework-flaui-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-flaui
-Version: 2.0.8
+Version: 2.0.9
 Summary: Windows GUI testing library for Robot Framework
 Home-page: https://github.com/GDATASoftwareAG/robotframework-flaui
 Author: G DATA CyberDefense AG
 Author-email: opensource@gdata.de
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
@@ -34,16 +34,16 @@
 [tests_url]: https://ci.appveyor.com/project/GDATACyberDefenseAG/robotframework-flaui/build/tests
 
 [pypi]: https://img.shields.io/pypi/v/robotframework-flaui?style=flat-square
 [pypi_url]: https://pypi.org/pypi/robotframework-flaui
 
 [python_37]: https://img.shields.io/badge/Python-3.7-blue
 [python_38]: https://img.shields.io/badge/Python-3.8-blue
-[python_39]: https://img.shields.io/badge/New%20Support-Python%203.9-blue
-[python_310]: https://img.shields.io/badge/New%20Support-Python%203.10-blue
+[python_39]: https://img.shields.io/badge/Python-3.9-blue
+[python_310]: https://img.shields.io/badge/Python-3.10-blue
 [python_311]: https://img.shields.io/badge/Experimental-Python%203.11-orange
 
 [rf3]: https://img.shields.io/badge/3-Supported-blue
 [rf4]: https://img.shields.io/badge/4-Supported-blue
 [rf5]: https://img.shields.io/badge/5-Supported-blue
 [rf6]: https://img.shields.io/badge/6-Supported-blue
```

### Comparing `robotframework-flaui-2.0.8/README.md` & `robotframework-flaui-2.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 [tests_url]: https://ci.appveyor.com/project/GDATACyberDefenseAG/robotframework-flaui/build/tests
 
 [pypi]: https://img.shields.io/pypi/v/robotframework-flaui?style=flat-square
 [pypi_url]: https://pypi.org/pypi/robotframework-flaui
 
 [python_37]: https://img.shields.io/badge/Python-3.7-blue
 [python_38]: https://img.shields.io/badge/Python-3.8-blue
-[python_39]: https://img.shields.io/badge/New%20Support-Python%203.9-blue
-[python_310]: https://img.shields.io/badge/New%20Support-Python%203.10-blue
+[python_39]: https://img.shields.io/badge/Python-3.9-blue
+[python_310]: https://img.shields.io/badge/Python-3.10-blue
 [python_311]: https://img.shields.io/badge/Experimental-Python%203.11-orange
 
 [rf3]: https://img.shields.io/badge/3-Supported-blue
 [rf4]: https://img.shields.io/badge/4-Supported-blue
 [rf5]: https://img.shields.io/badge/5-Supported-blue
 [rf6]: https://img.shields.io/badge/6-Supported-blue
```

### Comparing `robotframework-flaui-2.0.8/robotframework_flaui.egg-info/PKG-INFO` & `robotframework-flaui-2.0.9/robotframework_flaui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-flaui
-Version: 2.0.8
+Version: 2.0.9
 Summary: Windows GUI testing library for Robot Framework
 Home-page: https://github.com/GDATASoftwareAG/robotframework-flaui
 Author: G DATA CyberDefense AG
 Author-email: opensource@gdata.de
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
@@ -34,16 +34,16 @@
 [tests_url]: https://ci.appveyor.com/project/GDATACyberDefenseAG/robotframework-flaui/build/tests
 
 [pypi]: https://img.shields.io/pypi/v/robotframework-flaui?style=flat-square
 [pypi_url]: https://pypi.org/pypi/robotframework-flaui
 
 [python_37]: https://img.shields.io/badge/Python-3.7-blue
 [python_38]: https://img.shields.io/badge/Python-3.8-blue
-[python_39]: https://img.shields.io/badge/New%20Support-Python%203.9-blue
-[python_310]: https://img.shields.io/badge/New%20Support-Python%203.10-blue
+[python_39]: https://img.shields.io/badge/Python-3.9-blue
+[python_310]: https://img.shields.io/badge/Python-3.10-blue
 [python_311]: https://img.shields.io/badge/Experimental-Python%203.11-orange
 
 [rf3]: https://img.shields.io/badge/3-Supported-blue
 [rf4]: https://img.shields.io/badge/4-Supported-blue
 [rf5]: https://img.shields.io/badge/5-Supported-blue
 [rf6]: https://img.shields.io/badge/6-Supported-blue
```

### Comparing `robotframework-flaui-2.0.8/robotframework_flaui.egg-info/SOURCES.txt` & `robotframework-flaui-2.0.9/robotframework_flaui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/__init__.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/bin/FlaUI.Core.dll` & `robotframework-flaui-2.0.9/src/FlaUILibrary/bin/FlaUI.Core.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/bin/FlaUI.UIA2.dll` & `robotframework-flaui-2.0.9/src/FlaUILibrary/bin/FlaUI.UIA2.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/bin/FlaUI.UIA3.dll` & `robotframework-flaui-2.0.9/src/FlaUILibrary/bin/FlaUI.UIA3.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll` & `robotframework-flaui-2.0.9/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/automation/uia.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/automation/uia.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/automation/uia2.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/automation/uia2.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/automation/uia3.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/automation/uia3.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/exception/flauierror.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/exception/flauierror.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/interface/moduleinterface.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/interface/moduleinterface.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/application.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/application.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/checkbox.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/checkbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/combobox.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/combobox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/debug.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/debug.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/element.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/element.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/grid.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/grid.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/keyboard.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/keyboard.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/mouse.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/mouse.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/property.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/property.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/screenshot.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/screenshot.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/selector.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/selector.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/tab.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/tab.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/textbox.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/textbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/tooglebutton.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/tooglebutton.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/tree.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/tree.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/module/window.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/module/window.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/util/converter.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/util/converter.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/util/keyboardinputconverter.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/util/keyboardinputconverter.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/util/treeitems.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/util/treeitems.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/flaui/util/treeitemsparser.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/flaui/util/treeitemsparser.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/__init__.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/application.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/application.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/checkbox.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/checkbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/combobox.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/combobox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/debug.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/debug.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/element.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/element.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/grid.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/grid.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/keyboard.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/keyboard.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/listbox.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/listbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/mouse.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/mouse.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/property.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/property.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/radiobutton.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/radiobutton.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/screenshot.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/screenshot.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/tab.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/tab.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/textbox.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/textbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/togglebutton.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/togglebutton.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/tree.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/tree.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/keywords/window.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/keywords/window.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/pythonnetwrapper.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/pythonnetwrapper.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-2.0.8/src/FlaUILibrary/robotframework/robotlog.py` & `robotframework-flaui-2.0.9/src/FlaUILibrary/robotframework/robotlog.py`

 * *Files identical despite different names*

