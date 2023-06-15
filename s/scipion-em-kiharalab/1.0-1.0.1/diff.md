# Comparing `tmp/scipion-em-kiharalab-1.0.tar.gz` & `tmp/scipion-em-kiharalab-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-kiharalab-1.0.tar", last modified: Fri May  5 14:17:34 2023, max compression
+gzip compressed data, was "scipion-em-kiharalab-1.0.1.tar", last modified: Thu Jun 15 21:43:21 2023, max compression
```

## Comparing `scipion-em-kiharalab-1.0.tar` & `scipion-em-kiharalab-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:34.899150 scipion-em-kiharalab-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-05 14:17:34.895150 scipion-em-kiharalab-1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:34.895150 scipion-em-kiharalab-1.0/kiharalab/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10264 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2164 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/bibtex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2568 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    20905 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/install_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    52072 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/kiharalab_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:34.895150 scipion-em-kiharalab-1.0/kiharalab/protocols/
--rwxr-xr-x   0 runner    (1001) docker     (123)      459 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/protocols/protocol_daq.py
--rw-r--r--   0 runner    (1001) docker     (123)    34047 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/protocols/protocol_emap2sec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/protocols/protocol_mainmast_segment_map.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:34.895150 scipion-em-kiharalab-1.0/kiharalab/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/tests/test_daq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/tests/test_emap2sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/tests/test_mainmast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:34.895150 scipion-em-kiharalab-1.0/kiharalab/viewers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/viewers/viewer_daq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/viewers/viewer_emap2sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/viewers/viewer_mainmast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/kiharalab/wizards.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:34.895150 scipion-em-kiharalab-1.0/scipion_em_kiharalab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-05 14:17:34.000000 scipion-em-kiharalab-1.0/scipion_em_kiharalab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-05 14:17:34.000000 scipion-em-kiharalab-1.0/scipion_em_kiharalab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:17:34.000000 scipion-em-kiharalab-1.0/scipion_em_kiharalab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 14:17:34.000000 scipion-em-kiharalab-1.0/scipion_em_kiharalab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 14:17:34.000000 scipion-em-kiharalab-1.0/scipion_em_kiharalab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 14:17:34.000000 scipion-em-kiharalab-1.0/scipion_em_kiharalab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:17:34.899150 scipion-em-kiharalab-1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1386 2023-05-05 14:15:50.000000 scipion-em-kiharalab-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:43:21.094614 scipion-em-kiharalab-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-15 21:43:21.094614 scipion-em-kiharalab-1.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2688 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:43:21.090614 scipion-em-kiharalab-1.0.1/kiharalab/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10074 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2164 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/bibtex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2563 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22758 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/install_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52072 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/kiharalab_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:43:21.090614 scipion-em-kiharalab-1.0.1/kiharalab/protocols/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      459 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/protocols/protocol_daq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/protocols/protocol_emap2sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/protocols/protocol_mainmast_segment_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:43:21.090614 scipion-em-kiharalab-1.0.1/kiharalab/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/tests/test_daq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/tests/test_emap2sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/tests/test_mainmast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:43:21.090614 scipion-em-kiharalab-1.0.1/kiharalab/viewers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/viewers/viewer_daq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/viewers/viewer_emap2sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/viewers/viewer_mainmast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/kiharalab/wizards.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:43:21.094614 scipion-em-kiharalab-1.0.1/scipion_em_kiharalab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-15 21:43:21.000000 scipion-em-kiharalab-1.0.1/scipion_em_kiharalab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 21:43:21.000000 scipion-em-kiharalab-1.0.1/scipion_em_kiharalab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:43:21.000000 scipion-em-kiharalab-1.0.1/scipion_em_kiharalab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 21:43:21.000000 scipion-em-kiharalab-1.0.1/scipion_em_kiharalab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:43:21.000000 scipion-em-kiharalab-1.0.1/scipion_em_kiharalab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 21:43:21.000000 scipion-em-kiharalab-1.0.1/scipion_em_kiharalab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:43:21.094614 scipion-em-kiharalab-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2263 2023-06-15 21:41:37.000000 scipion-em-kiharalab-1.0.1/setup.py
```

### Comparing `scipion-em-kiharalab-1.0/LICENSE` & `scipion-em-kiharalab-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-kiharalab-1.0/kiharalab/__init__.py` & `scipion-em-kiharalab-1.0.1/kiharalab/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,55 +20,55 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-import pwem, shutil, os
+import pwem, os
 from .constants import *
 from .install_helper import InstallHelper
 
-__version__ = KIHARALAB_DEFAULT_VERSION
+__version__ = KIHARALAB_VERSION
 _logo = "kiharalab_logo.png"
 _references = ['genki2021DAQ']
 
 class Plugin(pwem.Plugin):
     """
-    Definition of class variables. For each protocol, a variable will be created.
-    _<protocolNameInLowercase>Home will contain the full path of the protocol, ending with a folder whose name will be <protocolNameFirstLetterLowercase>-<defaultProtocolVersion> variable.
+    Definition of class variables. For each package, a variable will be created.
+    _<packageNameInLowercase>Home will contain the full path of the package, ending with a folder whose name will be <packageNameFirstLetterLowercase>-<defaultPackageVersion> variable.
         For example: _emap2secHome = "~/Documents/scipion/software/em/emap2sec-1.0"
     
-    Inside that protocol, for each repo, there will also be another variable.
-    _<repoNameInLowercase>Repo will be a folder inside _<protocolNameInLowercase>Home and its name will be <repoName>.
-        For example: _emap2secplusRepo = "~/Documents/scipion/software/em/emap2sec-1.0/Emap2secPlus"
+    Inside that package, for each binary, there will also be another variable.
+    _<binaryNameInLowercase>Binary will be a folder inside _<packageNameInLowercase>Home and its name will be <binaryName>.
+        For example: _emap2secplusBinary = "~/Documents/scipion/software/em/emap2sec-1.0/Emap2secPlus"
     """
     # DAQ
     daqDefaultVersion = DAQ_DEFAULT_VERSION
     _daqHome = os.path.join(pwem.Config.EM_ROOT, 'daq-' + daqDefaultVersion)
-    _daqRepo = os.path.join(_daqHome, 'daq')
+    _daqBinary = os.path.join(_daqHome, 'daq')
 
     # Emap2sec
     emap2secDefaultVersion = EMAP2SEC_DEFAULT_VERSION
     _emap2secHome = os.path.join(pwem.Config.EM_ROOT, 'emap2sec-' + emap2secDefaultVersion)
-    _emap2secRepo = os.path.join(_emap2secHome, 'Emap2sec')
-    _emap2secplusRepo = os.path.join(_emap2secHome, 'Emap2secPlus')
+    _emap2secBinary = os.path.join(_emap2secHome, 'Emap2sec')
+    _emap2secplusBinary = os.path.join(_emap2secHome, 'Emap2secPlus')
 
     # MainMast
     mainmastDefaultVersion = MAINMAST_DEFAULT_VERSION
     _mainmastHome = os.path.join(pwem.Config.EM_ROOT, 'mainMast-' + mainmastDefaultVersion)
-    _mainmastRepo = os.path.join(_mainmastHome, 'MainMast')
+    _mainmastBinary = os.path.join(_mainmastHome, 'MainMast')
 
     @classmethod
     def _defineVariables(cls):
         """
         Return and write a home and conda enviroment variable in the config file.
-        Each protocol will have a variable called <protocolNameInUppercase>_HOME, and another called <protocolNameInUppercase>_ENV
-        <protocolNameInUppercase>_HOME will contain the path to the protocol installation. For example: "~/Documents/scipion/software/em/daq-1.0"
-        <protocolNameInUppercase>_ENV will contain the name of the conda enviroment for that protocol. For example: "daq-1.0"
+        Each package will have a variable called <packageNameInUppercase>_HOME, and another called <packageNameInUppercase>_ENV
+        <packageNameInUppercase>_HOME will contain the path to the package installation. For example: "~/Documents/scipion/software/em/daq-1.0"
+        <packageNameInUppercase>_ENV will contain the name of the conda enviroment for that package. For example: "daq-1.0"
         """
         # DAQ
         cls._defineEmVar(DAQ_HOME, cls._daqHome)
         cls._defineVar('DAQ_ENV', 'daq-' + cls.daqDefaultVersion)
 
         # Emap2sec
         cls._defineEmVar(EMAP2SEC_HOME, cls._emap2secHome)
@@ -90,52 +90,54 @@
     
     @classmethod    
     def addDAQ(cls, env):
         """
         This function provides the neccessary commands for installing DAQ.
         """
         # Defining protocol variables
-        protocolName = 'daq'
+        packageName = 'daq'
 
         # Instanciating installer
-        installer = InstallHelper()
+        installer = InstallHelper(packageName, packageVersion=cls.daqDefaultVersion)
 
         # Installing protocol
-        installer.getCloneCommand(cls._daqHome, 'https://github.com/kiharalab/DAQ.git', binaryFolderName=protocolName)\
-            .getCondaEnvCommand(protocolName, cls._daqHome, cls._daqRepo, pythonVersion='3.8.5')\
-            .addProtocolPackage(env, protocolName, dependencies=['git', 'conda', 'pip'])
+        installer.getCloneCommand('https://github.com/kiharalab/DAQ.git', binaryFolderName=packageName)\
+            .getCondaEnvCommand(pythonVersion='3.8.5', binaryPath=cls._daqBinary)\
+            .addPackage(env, dependencies=['git', 'conda', 'pip'])
 
     @classmethod    
     def addEmap2sec(cls, env):
         """
         This function provides the neccessary commands for installing Emap2sec.
         """
         # Defining protocol variables
-        protocolName = 'emap2sec'
+        packageName = 'emap2sec'
         emap2secFolderName = 'Emap2sec'
         emap2secPlusFolderName = 'Emap2secPlus'
 
         # Instanciating installer
-        installer = InstallHelper()
+        installer = InstallHelper(packageName, packageVersion=cls.emap2secDefaultVersion)
 
         # Defining extra files to download
+        firstLocation = "models/emap2sec_models_exp1"
+        secondLocation = "models/emap2sec_models_exp2"
         emap2secExtraFiles = [
-            ("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp1/checkpoint", "models/emap2sec_models_exp1"),
-            ("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp1/emap2sec_L1_exp.ckpt-108000.data-00000-of-00001", "models/emap2sec_models_exp1"),
-            ("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp1/emap2sec_L1_exp.ckpt-108000.index", "models/emap2sec_models_exp1"),
-            ("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp1/emap2sec_L1_exp.ckpt-108000.meta", "models/emap2sec_models_exp1"),
-            ("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp2/checkpoint", "models/emap2sec_models_exp2"),
-            ("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp2/emap2sec_L2_exp.ckpt-20000.data-00000-of-00001", "models/emap2sec_models_exp2"),
-            ("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp2/emap2sec_L2_exp.ckpt-20000.index", "models/emap2sec_models_exp2"),
-            ("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp2/emap2sec_L2_exp.ckpt-20000.meta", "models/emap2sec_models_exp2")
+            installer.getFileDict("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp1/checkpoint", path=firstLocation),
+            installer.getFileDict("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp1/emap2sec_L1_exp.ckpt-108000.data-00000-of-00001", path=firstLocation),
+            installer.getFileDict("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp1/emap2sec_L1_exp.ckpt-108000.index", path=firstLocation),
+            installer.getFileDict("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp1/emap2sec_L1_exp.ckpt-108000.meta", path=firstLocation),
+            installer.getFileDict("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp2/checkpoint", path=secondLocation),
+            installer.getFileDict("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp2/emap2sec_L2_exp.ckpt-20000.data-00000-of-00001", path=secondLocation),
+            installer.getFileDict("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp2/emap2sec_L2_exp.ckpt-20000.index", path=secondLocation),
+            installer.getFileDict("https://kiharalab.org/Emap2sec_models/emap2sec_models_exp2/emap2sec_L2_exp.ckpt-20000.meta", path=secondLocation)
         ]
 
         emap2secPlusExtraFiles = [
-            ("https://kiharalab.org/emsuites/emap2secplus_model/best_model.tar.gz", ''),
-            ("https://kiharalab.org/emsuites/emap2secplus_model/nocontour_best_model.tar.gz", '')
+            installer.getFileDict("https://kiharalab.org/emsuites/emap2secplus_model/best_model.tar.gz"),
+            installer.getFileDict("https://kiharalab.org/emsuites/emap2secplus_model/nocontour_best_model.tar.gz")
         ]
 
         # Defininig extra commands to run
         grantExecPermission = "chmod -R +x *"
         emap2secExtraCommands = [
             "mkdir -p results",
             grantExecPermission,
@@ -146,59 +148,53 @@
         emap2secPlusExtraCommands = [
             "tar -xf best_model.tar.gz && rm -f best_model.tar.gz",
             "tar -xf nocontour_best_model.tar.gz && rm -f nocontour_best_model.tar.gz",
             "cd process_map && make",
             grantExecPermission
         ]
 
-        # Getting dependencies
-        dependencies = ['git', 'conda', 'pip', 'wget', 'make', 'gcc', 'tar']
-
         # Installing protocol
-        installer.getCloneCommand(cls._emap2secHome, 'https://github.com/kiharalab/emap2sec.git', binaryFolderName=emap2secFolderName)\
-            .getCloneCommand(cls._emap2secHome, 'https://github.com/kiharalab/emap2secPlus.git', binaryFolderName=emap2secPlusFolderName)\
-            .getCondaEnvCommand(protocolName, cls._emap2secHome, binaryPath=cls._emap2secRepo, pythonVersion='3.6')\
-            .getCondaEnvCommand(protocolName, cls._emap2secHome, binaryPath=cls._emap2secplusRepo, binaryName='emap2secPlus', pythonVersion='3.6.9')\
-            .addCondaPackages(protocolName, packages=['pytorch==1.1.0', 'cudatoolkit=10.0'], binaryName='emap2secPlus', channel='pytorch')\
-            .getExtraFiles(protocolName, cls._emap2secHome, emap2secExtraFiles, workDir=cls._emap2secRepo)\
-            .getExtraFiles(protocolName, cls._emap2secHome, emap2secPlusExtraFiles, binaryName='emap2secPlus', workDir=cls._emap2secplusRepo)\
-            .addCommands(protocolName, emap2secExtraCommands, workDir=cls._emap2secRepo, protocolHome=cls._emap2secHome)\
-            .addCommands(protocolName, emap2secPlusExtraCommands, binaryName='emap2secPlus', workDir=cls._emap2secplusRepo, protocolHome=cls._emap2secHome)\
-            .addProtocolPackage(env, protocolName, dependencies=dependencies)
+        installer.getCloneCommand('https://github.com/kiharalab/emap2sec.git', binaryFolderName=emap2secFolderName)\
+            .getCloneCommand('https://github.com/kiharalab/emap2secPlus.git', binaryFolderName=emap2secPlusFolderName)\
+            .getCondaEnvCommand(binaryPath=cls._emap2secBinary, pythonVersion='3.6')\
+            .getCondaEnvCommand(binaryPath=cls._emap2secplusBinary, binaryName='emap2secPlus', pythonVersion='3.6.9')\
+            .addCondaPackages(packages=['pytorch==1.1.0', 'cudatoolkit=10.0'], binaryName='emap2secPlus', channel='pytorch')\
+            .getExtraFiles(emap2secExtraFiles, workDir=cls._emap2secBinary)\
+            .getExtraFiles(emap2secPlusExtraFiles, binaryName='emap2secPlus', workDir=cls._emap2secplusBinary)\
+            .addCommands(emap2secExtraCommands, workDir=cls._emap2secBinary)\
+            .addCommands(emap2secPlusExtraCommands, binaryName='emap2secPlus', workDir=cls._emap2secplusBinary)\
+            .addPackage(env, dependencies=['git', 'conda', 'pip', 'wget', 'make', 'gcc', 'tar'])
 
     @classmethod    
     def addMainMast(cls, env):
         """
         This function provides the neccessary commands for installing MainMast.
         """
         # Defining protocol variables
-        protocolName = 'mainMast'
+        packageName = 'mainMast'
 
         # Instanciating installer
-        installer = InstallHelper()
+        installer = InstallHelper(packageName, packageVersion=cls.mainmastDefaultVersion)
 
         # Extra commands
         grantExecPermission = "chmod -R +x *"
         cleanObjs = "rm -rf *.o"
         extraCommands = [
             cleanObjs + " MainmastSeg",
             grantExecPermission,
             "make",
             cleanObjs,
             grantExecPermission,
             "cd example1 && gunzip emd-0093.mrc.gz MAP_m4A.mrc.gz region0.mrc.gz region1.mrc.gz region2.mrc.gz region3.mrc.gz"
         ]
 
-        # Getting dependencies
-        dependencies = ['git', 'make', 'gcc', 'gzip']
-
         # Installing protocol
-        installer.getCloneCommand(cls._mainmastHome, 'https://github.com/kiharalab/MAINMASTseg.git', binaryFolderName='MainMast')\
-            .addCommands(protocolName, extraCommands, workDir=cls._mainmastRepo, protocolHome=cls._mainmastHome)\
-            .addProtocolPackage(env, protocolName, dependencies=dependencies)
+        installer.getCloneCommand('https://github.com/kiharalab/MAINMASTseg.git', binaryFolderName='MainMast')\
+            .addCommands(extraCommands, workDir=cls._mainmastBinary)\
+            .addPackage(env, dependencies=['git', 'make', 'gcc', 'gzip'])
 
     # ---------------------------------- Utils functions  -----------------------
     @classmethod
     def getProtocolEnvName(cls, protocolName, repoName=None):
         """
         This function returns the env name for a given protocol and repo.
         """
```

### Comparing `scipion-em-kiharalab-1.0/kiharalab/bibtex.py` & `scipion-em-kiharalab-1.0.1/kiharalab/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-kiharalab-1.0/kiharalab/constants.py` & `scipion-em-kiharalab-1.0.1/kiharalab/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 EMAP2SEC_HOME = 'EMAP2SEC_HOME'
 MAINMAST_HOME = 'MAINMAST_HOME'
 
 # Supported versions
 V1_0 = '1.0'
 
 # Plugin version
-KIHARALAB_DEFAULT_VERSION = V1_0
+KIHARALAB_VERSION = '1.0.1'
 
 # Protocol versions 
 DAQ_DEFAULT_VERSION = V1_0
 EMAP2SEC_DEFAULT_VERSION = V1_0
 MAINMAST_DEFAULT_VERSION = V1_0
 
 # Protocol repo versions
```

### Comparing `scipion-em-kiharalab-1.0/kiharalab/install_helper.py` & `scipion-em-kiharalab-1.0.1/kiharalab/install_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,220 +1,245 @@
-from typing import List, Tuple
+from typing import List, Tuple, Dict
 import pwem, os
 
 class InstallHelper():
     """
     ### This class is intended to be used to ease the plugin installation process.
 
     #### Usage:
     InstallHelper class needs to be instanciated before it can be used.
     After that, commands can be chained together to run them in the defined order.
-    The last command always needs to be addProtocolPackage().
+    The last command always needs to be addPackage().
 
     #### Example:
     installer = InstallHelper() # Instanciating class\n
-    installer.getCloneCommand('test-protocol', '/home/user/myCustomPath', 'github.com/myRepo') # Cloning GitHub repository\n
-    installer.getCondaenvCommand('test-protocol') # Creating conda enviroment\n
-    installer.addProtocolPackage(env, 'test-protocol') # Install package\n
+    installer.getCloneCommand('test-package', '/home/user/myCustomPath', 'github.com/myRepo') # Cloning GitHub repository\n
+    installer.getCondaenvCommand('test-package') # Creating conda enviroment\n
+    installer.addPackage(env, 'test-package') # Install package\n
 
     #### It can also be done in a single line:
-    installer.getCloneCommand('test-protocol', '/home/user/myCustomPath', 'github.com/myRepo').getCondaenvCommand('test-protocol').addProtocolPackage(env, 'test-protocol')\n
+    installer.getCloneCommand('test-package', '/home/user/myCustomPath', 'github.com/myRepo').getCondaenvCommand('test-package').addPackage(env, 'test-package')\n
 
-    #### If you want to check the command strings you are producing, use the function getCommandList() instead of addProtocolPackage() and assign it to a variable so you can print it.
+    #### If you want to check the command strings you are producing, use the function getCommandList() instead of addPackage() and assign it to a variable so you can print it.
     """
     # Global variables
     DEFAULT_VERSION = '1.0'
 
-    def __init__(self):
+    def __init__(self, packageName: str, packageHome: str=None, packageVersion: str=DEFAULT_VERSION):
         """
-        Constructor for the InstallHelper class.
+        ### Constructor for the InstallHelper class.
+
+        #### Parameters:
+        packageName (str): Name of the package.
+        packageHome (str): Optional. Path to the package. It can be absolute or relative to current directory.
+        packageVersion (str): Optional. Package version.
         """
         # Private list of tuples containing commands with targets
         self.__commandList = []
+        
+        # Package name, version, and home
+        self.__packageName = packageName
+        self.__packageVersion = packageVersion
+        self.__packageHome = packageHome if packageHome else os.path.join(pwem.Config.EM_ROOT, packageName + '-' + packageVersion)
     
     #--------------------------------------- PRIVATE FUNCTIONS ---------------------------------------#
     def __getTargetCommand(self, targetName: str) -> str:
         """
-        This private function returns the neccessary command to create a target file given its name.
-        Targets are always in uppercase and underscore format.
+        ### This private function returns the neccessary command to create a target file given its name.
+        ### Targets are always in uppercase and underscore format.
 
-        Parameters:
+        #### Parameters:
         targetName (str): Name of the target file.
 
-        Returns:
+        #### Returns:
         (str): The command needed to create the target file.
         """
         return 'touch {}'.format(targetName)
     
     def __getBinaryEnvName(self, binaryName: str, binaryVersion: str=DEFAULT_VERSION) -> str:
         """
-        This function returns the env name for a given protocol and repo.
+        ### This function returns the env name for a given package and repo.
 
-        Parameters:
-        binaryName (str): Name of the binary inside the protocol.
+        #### Parameters:
+        binaryName (str): Name of the binary inside the package.
         binaryVersion (str): Optional. Binary's version.
 
-        Returns:
+        #### Returns:
         (str): The enviroment name for this binary.
         """
         return binaryName + "-" + binaryVersion
     
     def __getEnvActivationCommand(self, binaryName: str, binaryVersion: str=DEFAULT_VERSION) -> str:
         """
-        Returns the conda activation command for the given enviroment.
+        ### Returns the conda activation command for the given enviroment.
 
-        Parameters:
-        binaryName (str): Name of the binary inside the protocol.
-        binaryVersion (str): Optional. Version of the binary inside the protocol.
+        #### Parameters:
+        binaryName (str): Name of the binary inside the package.
+        binaryVersion (str): Optional. Version of the binary inside the package.
+
+        #### Returns:
+        (str): The enviroment activation command.
         """
         return "conda activate " + self.__getBinaryEnvName(binaryName, binaryVersion=binaryVersion)
+    
+    def __getBinaryNameAndVersion(self, binaryName: str=None, binaryVersion: str=None)  -> Tuple[str, str]:
+        """
+        ### Returns the binary name and version from an optionally introduced binary name and version.
 
+        #### Parameters:
+        binaryName (str): Name of the binary inside the package.
+        binaryVersion (str): Optional. Version of the binary inside the package.
+
+        #### Returns:
+        tuple(str, str): The binary name and binary version.
+        """
+        binaryName = binaryName if binaryName else self.__packageName
+        binaryVersion = binaryVersion if binaryVersion else self.__packageVersion
+        return binaryName, binaryVersion
+    
     #--------------------------------------- PUBLIC FUNCTIONS ---------------------------------------#
     def getCommandList(self) -> List[Tuple[str, str]]:
         """
         ### This function returns the list of commands with targets for debugging purposes.
 
         #### Returns:
         (list[tuple[str, str]]): Command list with target files.
 
         #### Usage:
         commandList = installer.getCommandList()
         """
         return self.__commandList
-
-    def addCommand(self, command: str, targetName: str, workDir: str='', protocolHome: str=''):
+    
+    def addCommand(self, command: str, targetName: str, workDir: str=''):
         """
         ### This function adds the given command with target to the command list.
-        ### The target file needs to be located inside protocolHome's directory so Scipion can detect it.
+        ### The target file needs to be located inside packageHome's directory so Scipion can detect it.
 
         #### Parameters:
         command (str): Command to be added.
         targetName (str): Name of the target file to be produced after commands are completed successfully.
         workDir (str): Optional. Directory where the command will be executed from.
-        protocolHome (str): Optional. Protocol's root directory where target files are stored.
 
         #### Usage:
-        installer.addCommand('python3 myScript.py', 'MYSCRIPT_COMPLETED', workDir='/home/user/Documents/otherDirectory', protocolHome='/home/user/scipion/software/em/test-protocol-1.0')
+        installer.addCommand('python3 myScript.py', 'MYSCRIPT_COMPLETED', workDir='/home/user/Documents/otherDirectory')
 
         #### This function call will generate the following commands:
-        cd /home/user/Documents/otherDirectory && python3 myScript.py && touch /home/user/scipion/software/em/test-protocol-1.0/MYSCRIPT_COMPLETED
+        cd /home/user/Documents/otherDirectory && python3 myScript.py && touch /home/user/scipion/software/em/test-package-1.0/MYSCRIPT_COMPLETED
         """
         # Getting work directory
         workDirCmd = 'cd {} && '.format(workDir) if workDir else ''
 
         # Getting target name
-        fullTargetName = os.path.join(protocolHome, targetName) if protocolHome else targetName
+        fullTargetName = os.path.join(self.__packageHome, targetName)
 
         command = (workDirCmd + command) if workDir else command
         self.__commandList.append((command + " && {}".format(self.__getTargetCommand(fullTargetName)), targetName))
         return self
     
-    def addCommands(self, protocolName: str, commandList: List[str], binaryName: str=None, workDir:str='', protocolHome: str='', targetNames: List[str]=[]):
+    def addCommands(self, commandList: List[str], binaryName: str=None, workDir:str='', targetNames: List[str]=[]):
         """
         ### This function adds the given commands with targets to the command list.
 
         #### Parameters:
-        protocolName (str): Name of the protocol.
         commandList (list[str]): List containing the commands to add.
-        binaryName (str): Optional. Name of the binary.
+        binaryName (str): Optional. Name of the binary. Default is package name.
         workDir (str): Optional. Directory where the commands will be executed from.
-        protocolHome (str): Optional. Protocol's root directory where target files are stored.
         targetNames (list[str]): Optional. List containing the name of the target files for this commands.
 
         #### Usage:
-        installer.addCommands('test-protocol', ['python3 myScript.py', 'ls'], binaryName='myBinary', workDir='/home/user/Documents/otherDirectory',
-            protocolHome='/home/user/scipion/software/em/test-protocol-1.0', targetNames=['MYSCRIPT_COMPLETED', 'DIRECTORY_LISTED'])
+        installer.addCommands(['python3 myScript.py', 'ls'], binaryName='myBinary', workDir='/home/user/Documents/otherDirectory',
+            targetNames=['MYSCRIPT_COMPLETED', 'DIRECTORY_LISTED'])
 
         #### This function call will generate the following commands:
-        cd /home/user/Documents/otherDirectory && python3 myScript.py && touch /home/user/scipion/software/em/test-protocol-1.0/MYSCRIPT_COMPLETED\n
-        cd /home/user/Documents/otherDirectory && ls && touch /home/user/scipion/software/em/test-protocol-1.0/DIRECTORY_LISTED
+        cd /home/user/Documents/otherDirectory && python3 myScript.py && touch /home/user/scipion/software/em/test-package-1.0/MYSCRIPT_COMPLETED\n
+        cd /home/user/Documents/otherDirectory && ls && touch /home/user/scipion/software/em/test-package-1.0/DIRECTORY_LISTED
         """
         # Defining binary name
-        binaryName = binaryName if binaryName else protocolName
+        binaryName = self.__getBinaryNameAndVersion(binaryName=binaryName)[0]
 
         # Defining default target name preffix
         defaultTargetPreffix = '{}_EXTRA_COMMAND_'.format(binaryName.upper())
 
         # Executing commands
         for idx in range(len(commandList)):
             targetName = targetNames[idx] if targetNames else (defaultTargetPreffix + str(idx))
-            self.addCommand(commandList[idx], targetName, workDir=workDir, protocolHome=protocolHome)
+            self.addCommand(commandList[idx], targetName, workDir=workDir)
 
         return self
     
-    def getCloneCommand(self, protocolHome: str, url: str, binaryFolderName: str='', targeName: str=None):
+    def getCloneCommand(self, url: str, binaryFolderName: str='', targeName: str=None):
         """
         ### This function creates the neccessary command to clone a repository from Github.
 
         #### Parameters:
-        protocolHome (str): Path to the protocol. It can be absolute or relative to current directory.
         url (str): URL to the git repository.
         binaryFolderName (str): Optional. Name of the binary directory.
         targetName (str): Optional. Name of the target file for this command.
 
         #### Usage:
-        installer.getCloneCommand('/home/user/scipion/software/em/test-protocol-1.0', 'https://github.com/myRepo.git', binaryFolderName='myCustomBinary', targeName='BINARY_CLONED')
+        installer.getCloneCommand('https://github.com/myRepo.git', binaryFolderName='myCustomBinary', targeName='BINARY_CLONED')
 
         #### This function call will generate the following command:
-        cd /home/user/scipion/software/em/test-protocol-1.0 && git clone https://github.com/myRepo.git myCustomBinary && touch BINARY_CLONED
+        cd /home/user/scipion/software/em/test-package-1.0 && git clone https://github.com/myRepo.git myCustomBinary && touch BINARY_CLONED
         """
         # Defining target name
         targeName = targeName if targeName else '{}_CLONED'.format(binaryFolderName.upper())
 
         # Modifying binary name with a space for the command
         binaryFolderName = (' ' + binaryFolderName) if binaryFolderName else ''
 
         # Adding command
-        self.addCommand('git clone {}{}'.format(url, binaryFolderName), targeName, workDir=protocolHome)
+        self.addCommand('git clone {}{}'.format(url, binaryFolderName), targeName, workDir=self.__packageHome)
 
         return self
     
-    def getCondaEnvCommand(self, protocolName: str, protocolHome: str, binaryPath: str=None, binaryName: str=None, binaryVersion: str=DEFAULT_VERSION, pythonVersion: str=None, requirementsFile: bool=True,
+    def getCondaEnvCommand(self, binaryName: str=None, binaryPath: str=None, binaryVersion: str=None, pythonVersion: str=None, requirementsFile: bool=True,
                            requirementFileName: str='requirements.txt', requirementList: List[str]=[], extraCommands: List[str]=[], targetName: str=None):
         """
-        ### This function creates the command string for creating a Conda enviroment and installing required dependencies for a given binary inside a protocol.
+        ### This function creates the command string for creating a Conda enviroment and installing required dependencies for a given binary inside a package.
 
         #### Parameters:
-        protocolName (str): Name of the protocol.
-        protocolHome (str): Path to the protocol. It can be absolute or relative to current directory.
-        binaryPath (str): Path to the binary. It can be absolute or relative to current directory.
-        binaryName (str): Optional. Name of the binary.
-        binaryVersion (str): Optional. Binary's version.
-        pythonVersion (str): Optional. Python version needed for the protocol.
+        binaryName (str): Optional. Name of the binary. Default is package name.
+        binaryPath (str): Optional. Path to the binary. It can be absolute or relative to current directory.
+        binaryVersion (str): Optional. Binary's version. Default is package version.
+        pythonVersion (str): Optional. Python version needed for the package.
         requirementsFile (bool): Optional. Defines if a Python requirements file exists.
         requirementFileName (bool): Optional. Name of the Python requirements file.
         requirementList (list[str]): Optional. List of Python packages to be installed. Can be used together with requirements file, but packages cannot be repeated.
         extraCommands (list[str]): Optional. List of extra conda-related commands to execute within the conda enviroment.
         targetName (str): Optional. Name of the target file for this command.
 
         #### Usage:
-        installer.getCondaEnvCommand('test-protocol', '/home/user/scipion/software/em/test-protocol-1.0', '/home/user/scipion/software/em/test-protocol-1.0/myBinary',
-            binaryName='myBinary', binaryVersion='1.5', pythonVersion='3.11', requirementsFile=True, requirementFileName='requirements.txt', requirementList=['torch==1.2.0', 'numpy'],
+        installer.getCondaEnvCommand(binaryName='myBinary', binaryPath='/home/user/scipion/software/em/test-package-1.0/myBinary', binaryVersion='1.5', pythonVersion='3.11',
+            requirementsFile=True, requirementFileName='requirements.txt', requirementList=['torch==1.2.0', 'numpy'],
             extraCommands=['conda info --envs'], targetName='CONDA_ENV_CREATED')
 
         #### This function call will generate the following command:
         eval "$(/home/user/miniconda/bin/conda shell.bash hook)"&& conda create -y -n myBinary-1.5 python=3.11 && conda activate myBinary-1.5 &&
-        cd /home/user/scipion/software/em/test-protocol-1.0/myBinary && conda install pip -y && $CONDA_PREFIX/bin/pip install -r requirements.txt &&
-        $CONDA_PREFIX/bin/pip install torch==1.2.0 numpyconda info --envs && cd /home/user/scipion/software/em/test-protocol-1.0 && touch CONDA_ENV_CREATED
+        cd /home/user/scipion/software/em/test-package-1.0/myBinary && conda install pip -y && $CONDA_PREFIX/bin/pip install -r requirements.txt &&
+        $CONDA_PREFIX/bin/pip install torch==1.2.0 numpyconda info --envs && cd /home/user/scipion/software/em/test-package-1.0 && touch CONDA_ENV_CREATED
         #### The path in the first command (eval ...) might vary, depending on the value of CONDA_ACTIVATION_CMD in your scipion.conf file.
         """
-        # Binary name definition
-        binaryName = binaryName if binaryName else protocolName
+        # Binary name and version definition
+        binaryName, binaryVersion = self.__getBinaryNameAndVersion(binaryName=binaryName, binaryVersion=binaryVersion)
 
         # Conda env creation
         createEnvCmd = 'conda create -y -n {}{}'.format(self.__getBinaryEnvName(binaryName, binaryVersion=binaryVersion), (' python={}'.format(pythonVersion)) if pythonVersion else '')
 
         # Command to install pip
         pipInstallCmd = 'conda install pip -y'
 
         # Command prefix for Python packages installation
         requirementPrefixCmd = '$CONDA_PREFIX/bin/pip install'
 
+        # Requirements file name
+        requirementFileName = os.path.join(binaryPath, requirementFileName) if requirementFileName and binaryPath else requirementFileName
+
         # Command for installing Python packages with requirements file
-        installWithFile = requirementPrefixCmd + ' -r ' + requirementFileName if requirementsFile else ''
+        installWithFile = (requirementPrefixCmd + ' -r ' + requirementFileName) if requirementsFile else ''
 
         # Command for installing Python packages manually
         installManual = ' '.join(requirementList)
         installManual = (requirementPrefixCmd + " " + installManual) if installManual else ''
 
         # Only install pip and Python packages if requiremenst file or manual list has been provided
         pythonCommands = (' && ' + pipInstallCmd) if (installWithFile or installManual) else ''
@@ -222,141 +247,158 @@
             pythonCommands += ' && {}'.format(installWithFile) if installWithFile else ''
             pythonCommands += ' && {}'.format(installManual) if installManual else ''
         
         # Defining target name
         targetName = targetName if targetName else '{}_CONDA_ENV_CREATED'.format(binaryName.upper())
         
         # Crafting final command string
-        command = pwem.Plugin.getCondaActivationCmd() + ' ' + createEnvCmd              # Basic commands: hook and env creation
-        command += ' && ' + self.__getEnvActivationCommand(binaryName, binaryVersion=binaryVersion)   # Env activation
-        command += ' && cd {}'.format(binaryPath) if binaryPath else ''                 # cd to binary path if proceeds
-        command += pythonCommands                                                       # Python related commands
-        command += " && ".join(extraCommands)                                           # Extra conda commands
-        command += ' && cd {}'.format(protocolHome) if binaryPath else ''               # Return to protocol's root directory
+        command = pwem.Plugin.getCondaActivationCmd() + ' ' + createEnvCmd                          # Basic commands: hook and env creation
+        command += ' && ' + self.__getEnvActivationCommand(binaryName, binaryVersion=binaryVersion) # Env activation
+        command += ' && cd {}'.format(binaryPath) if binaryPath else ''                             # cd to binary path if proceeds
+        command += pythonCommands                                                                   # Python related commands
+        command += " && ".join(extraCommands)                                                       # Extra conda commands
+        command += ' && cd {}'.format(self.__packageHome) if binaryPath else ''                     # Return to package's root directory
         
         # Adding command
         self.addCommand(command, targetName)
         return self
     
-    def addCondaPackages(self, protocolName: str, packages: List[str], binaryName: str=None, binaryVersion: str=DEFAULT_VERSION, channel: str=None, targetName: str=None):
+    def addCondaPackages(self, packages: List[str], binaryName: str=None, binaryVersion: str=None, channel: str=None, targetName: str=None):
         """
         ### This function returns the command used for installing extra packages in a conda enviroment.
 
         #### Parameters:
-        binaryName (str): Name of the binary.
+        binaryName (str): Name of the binary. Default is package name.
         packages (list[str]): List of conda packages to install.
-        binaryVersion (str): Optional. Binary's version.
+        binaryVersion (str): Optional. Binary's version. Default is package version.
         channel (str): Optional. Channel to download the package from.
         targetName (str): Optional. Name of the target file for this command.
 
         #### Usage:
-        installer.addCondaPackages('test-protocol', packages=['pytorch==1.1.0', 'cudatoolkit=10.0'], binaryName='myBinary',
+        installer.addCondaPackages(packages=['pytorch==1.1.0', 'cudatoolkit=10.0'], binaryName='myBinary',
             binaryVersion='1.5', channel='conda-forge', targetName='CONDA_PACKAGES_INSTALLED')
 
         #### This function call will generate the following command:
         eval "$(/home/user/miniconda/bin/conda shell.bash hook)"&& conda activate myBinary-1.5 &&
         conda install -y pytorch==1.1.0 cudatoolkit=10.0 -c conda-forge && touch CONDA_PACKAGES_INSTALLED
         #### The path in the first command (eval ...) might vary, depending on the value of CONDA_ACTIVATION_CMD in your scipion.conf file.
         """
-        # Defining binary name
-        binaryName = binaryName if binaryName else protocolName
+        # Binary name and version definition
+        binaryName, binaryVersion = self.__getBinaryNameAndVersion(binaryName=binaryName, binaryVersion=binaryVersion)
 
         # Defininig target name
         targetName = targetName if targetName else '{}_CONDA_PACKAGES_INSTALLED'.format(binaryName.upper())
 
         # Adding installation command
         command = "{} {} && conda install -y {}".format(pwem.Plugin.getCondaActivationCmd(), self.__getEnvActivationCommand(binaryName, binaryVersion=binaryVersion), ' '.join(packages))
         if channel:
             command += " -c {}".format(channel)
         self.addCommand(command, targetName)
 
         return self
     
-    def getExtraFile(self, url: str, protocolHome: str, targetName: str, location: str=".", workDir: str=''):
+    def getExtraFile(self, url: str, targetName: str, location: str=".", workDir: str='', fileName: str=None):
         """
         ### This function creates the command to download with wget the file in the given link into the given path.
         ### The downloaded file will overwrite a local one if they have the same name.
         ### This is done to overwrite potential corrupt files whose download was not fully completed.
 
         #### Parameters:
         url (str): URL of the resource to download.
-        protocolHome (str): Path to the protocol. It can be absolute or relative to current directory.
         targetName (str): Name of the target file for this command.
         location (str): Optional. Location where the file will be downloaded. It can be absolute or relative to current directory.
         workDir (str): Optional. Directory where the file will be downloaded from.
+        fileName (str): Optional. Name of the file after the download. Use intended for cases when expected name differs from url name.
 
         #### Usage:
-        installer.getExtraFile('https://site.com/myfile.tar', '/home/user/scipion/software/em/test-protocol-1.0', 'FILE_DOWNLOADED', location='/home/user/scipion/software/em/test-protocol-1.0/subdirectory', workDir='/home/user')
+        installer.getExtraFile('https://site.com/myfile.tar', 'FILE_DOWNLOADED', location='/home/user/scipion/software/em/test-package-1.0/subdirectory', workDir='/home/user', fileName='test.tar')
 
         #### This function call will generate the following command:
-        cd /home/user && mkdir -p /home/user/scipion/software/em/test-protocol-1.0/subdirectory &&
-        wget -O /home/user/scipion/software/em/test-protocol-1.0/subdirectory/myfile.tar https://site.com/myfile.tar && touch /home/user/scipion/software/em/test-protocol-1.0/FILE_DOWNLOADED
+        cd /home/user && mkdir -p /home/user/scipion/software/em/test-package-1.0/subdirectory &&
+        wget -O /home/user/scipion/software/em/test-package-1.0/subdirectory/test.tar https://site.com/myfile.tar && touch /home/user/scipion/software/em/test-package-1.0/FILE_DOWNLOADED
         """
         # Getting filename for wget
-        fileName = os.path.basename(url)
+        fileName = fileName if fileName else os.path.basename(url)
         mkdirCmd = "mkdir -p {} && ".format(location) if location else ''
-        location = location if location else '.'
 
         downloadCmd = "{}wget -O {} {}".format(mkdirCmd, os.path.join(location, fileName), url)
-        self.addCommand(downloadCmd, targetName, workDir=workDir, protocolHome=protocolHome)
+        self.addCommand(downloadCmd, targetName, workDir=workDir)
     
         return self
-    
-    def getExtraFiles(self, protocolName: str, protocolHome: str, fileList: List[Tuple[str, str]], binaryName: str=None, workDir: str='', targetNames: List[str]=None):
+
+    def getExtraFiles(self, fileList: List[Dict[str, str]], binaryName: str=None, workDir: str='', targetNames: List[str]=None):
         """
         ### This function creates the command to download with wget the file in the given link into the given path.
         ### The downloaded file will overwrite a local one if they have the same name.
         ### This is done to overwrite potential corrupt files whose download was not fully completed.
 
         #### Parameters:
-        protocolName (str): Name of the protocol.
-        protocolHome (str): Path to the protocol. It can be absolute or relative to current directory.
-        fileList (list[tuple[str, str]]): List containing files to be downloaded. Example: [(url1, path1), (url2, path2)]
+        fileList (list[dict[str, str, str]]): List containing files to be downloaded. Example: [{'url': url1, 'path': path1, 'name': 'test.tar'}, {'url': url2, 'path': path2, 'name': 'test2.tar'}]
         binaryName (str): Optional. Name of the binary.
         Each file is a list contaning url and location to download it. Paths can be an empty string for default location.
         workDir (str): Optional. Directory where the files will be downloaded from.
         targetNames (list[str]): Optional. List containing the name of the target files for this commands.
 
         #### Usage:
-        installer..getExtraFiles('test-protocol', '/home/user/scipion/software/em/test-protocol-1.0',
+        installer.getExtraFiles(
             [
-                ('https://site.com/myfile.tar', '/home/user/scipion/software/em/test-protocol-1.0/subdirectory1'),
-                ('https://site.com/myfile.tar2', '/home/user/scipion/software/em/test-protocol-1.0/subdirectory2')
+                {'url': 'https://site.com/myfile.tar', 'path': '/home/user/scipion/software/em/test-package-1.0/subdirectory1', 'name': 'test.tar'},
+                {'url': 'https://site.com/myfile.tar2', 'path': '/home/user/scipion/software/em/test-package-1.0/subdirectory2', 'name': 'test2.tar2'}
             ],
             binaryName='myBinary', workDir='/home/user', targetNames=['DOWNLOADED_FILE_1', 'DOWNLOADED_FILE_2'])
 
         #### This function call will generate the following commands:
-        cd /home/user && mkdir -p /home/user/scipion/software/em/test-protocol-1.0/subdirectory1 &&
-        wget -O /home/user/scipion/software/em/test-protocol-1.0/subdirectory1/myfile.tar https://site.com/myfile.tar && touch /home/user/scipion/software/em/test-protocol-1.0/DOWNLOADED_FILE_1
+        cd /home/user && mkdir -p /home/user/scipion/software/em/test-package-1.0/subdirectory1 &&
+        wget -O /home/user/scipion/software/em/test-package-1.0/subdirectory1/test.tar https://site.com/myfile.tar && touch /home/user/scipion/software/em/test-package-1.0/DOWNLOADED_FILE_1
         
-        cd /home/user && mkdir -p /home/user/scipion/software/em/test-protocol-1.0/subdirectory2 &&
-        wget -O /home/user/scipion/software/em/test-protocol-1.0/subdirectory2/myfile.tar2 https://site.com/myfile.tar2 && touch /home/user/scipion/software/em/test-protocol-1.0/DOWNLOADED_FILE_2
+        cd /home/user && mkdir -p /home/user/scipion/software/em/test-package-1.0/subdirectory2 &&
+        wget -O /home/user/scipion/software/em/test-package-1.0/subdirectory2/test2.tar2 https://site.com/myfile.tar2 && touch /home/user/scipion/software/em/test-package-1.0/DOWNLOADED_FILE_2
         """
         # Defining binary name
-        binaryName = binaryName if binaryName else protocolName
+        binaryName = self.__getBinaryNameAndVersion(binaryName=binaryName)[0]
 
         # Default preffix for target names
         defaultTargetPreffix = "{}_FILE_".format(binaryName.upper())
 
         # For each file in the list, download file
         for idx in range(len(fileList)):
+            # Checking if file dictionary contains url
+            if 'url' not in fileList[idx]:
+                raise KeyError("ERROR: Download url has not been set for at least one file. You can create the appropiate dictionary calling function getFileDict.")
+            
+            # Getting proper file dictionary
+            kwargs = {}
+            if 'name' in fileList[idx]:
+                kwargs['name'] = fileList[idx]['name']
+            if 'path' in fileList[idx]:
+                kwargs['path'] = fileList[idx]['path']
+            downloadable = fileList[idx] if ('path' in fileList[idx] and 'name' in fileList[idx]) else self.getFileDict(fileList[idx]['url'], **kwargs)
+
             targetName = targetNames[idx] if targetNames else (defaultTargetPreffix + str(idx))
-            self.getExtraFile(fileList[idx][0], protocolHome, targetName, location=fileList[idx][1], workDir=workDir)
+            self.getExtraFile(downloadable['url'], targetName, location=downloadable['path'], workDir=workDir, fileName=downloadable['name'])
     
         return self
     
-    def addProtocolPackage(self, env, protocolName: str, protocolVersion: str=DEFAULT_VERSION, dependencies: List[str]=[], default: bool=True):
+    def addPackage(self, env, dependencies: List[str]=[], default: bool=True, **kwargs):
         """
-        ### This function adds the given protocol to scipion installation with some provided parameters.
+        ### This function adds the given package to scipion installation with some provided parameters.
         
         #### Parameters:
         env: Scipion enviroment.
-        protocolName (str): Name of the protocol.
-        protocolVersion (str): Protocol version.
-        dependencies (list[str]): Optional. List of dependencies the protocol has.
-        default (bool): Optional. Defines if this protocol version is automatically installed with the plugin.
-        Intended for cases where multiple versions of the same protocol coexist in the same plugin.
+        dependencies (list[str]): Optional. List of dependencies the package has.
+        default (bool): Optional. Defines if this package version is automatically installed with the plugin.
+        **kwargs: Optional. Other possible keyword parameters that will be directly passed to env.addPackage.
+        Intended for cases where multiple versions of the same package coexist in the same plugin.
 
         #### Usage:
-        installer.addProtocolPackage(env, 'test-protocol', protocolVersion='1.3', dependencies=['wget', 'conda'], default=True)
+        installer.addPackage(env, dependencies=['wget', 'conda'], default=True)
         """
-        env.addPackage(protocolName, version=protocolVersion, tar='void.tgz', commands=self.__commandList, neededProgs=dependencies, default=default)
+        env.addPackage(self.__packageName, version=self.__packageVersion, tar='void.tgz', commands=self.__commandList, neededProgs=dependencies, default=default, **kwargs)
+    
+    #--------------------------------------- PUBLIC UTILS FUNCTIONS ---------------------------------------#
+    def getFileDict(self, url: str, path: str='.', fileName: str=None) -> Dict[str, str]:
+        """ This function generates the dictionary for a downloadable file. """
+        # Getting file name
+        fileName = fileName if fileName else os.path.basename(url)
+
+        # Returning dictionary
+        return {'url': url, 'path': path, 'name': fileName}
```

### Comparing `scipion-em-kiharalab-1.0/kiharalab/kiharalab_logo.png` & `scipion-em-kiharalab-1.0.1/kiharalab/kiharalab_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-kiharalab-1.0/kiharalab/objects.py` & `scipion-em-kiharalab-1.0.1/kiharalab/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-kiharalab-1.0/kiharalab/protocols/protocol_daq.py` & `scipion-em-kiharalab-1.0.1/kiharalab/protocols/protocol_daq.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,21 +137,21 @@
         """
         outDir = self._getTmpPath('predictions')
         args = self.getDAQArgs()
 
         fullProgram = '{} {} && {}'\
             .format(Plugin.getCondaActivationCmd(), Plugin.getProtocolActivationCommand('daq'), 'python3')
         if not 'main.py' in args:
-            args = '{}/main.py {}'.format(Plugin._daqRepo, args)
-        self.runJob(fullProgram, args, cwd=Plugin._daqRepo)
+            args = '{}/main.py {}'.format(Plugin._daqBinary, args)
+        self.runJob(fullProgram, args, cwd=Plugin._daqBinary)
 
         if outDir is None:
             outDir = self._getExtraPath('predictions')
 
-        daqDir = os.path.join(Plugin._daqRepo, 'Predict_Result', self.getVolumeName())
+        daqDir = os.path.join(Plugin._daqBinary, 'Predict_Result', self.getVolumeName())
         shutil.copytree(daqDir, outDir)
         shutil.rmtree(daqDir)
     
     def createOutputStep(self):
         outStructFileName = self._getPath('outputStructure.cif')
         outDAQFile = os.path.abspath(self._getTmpPath('predictions/daq_score_w9.pdb'))
```

### Comparing `scipion-em-kiharalab-1.0/kiharalab/protocols/protocol_emap2sec.py` & `scipion-em-kiharalab-1.0.1/kiharalab/protocols/protocol_emap2sec.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,23 +37,22 @@
 from pyworkflow.utils import Message
 from pwem.protocols import EMProtocol
 from pwem.objects import AtomStruct
 from pwem.emlib.image import ImageHandler
 
 # Kiharalab imports
 from kiharalab import Plugin
-from kiharalab.constants import *
+from kiharalab.constants import EMAP2SEC_TYPE_EMAP2SEC, EMAP2SEC_NORM_GLOBAL, EMAP2SECPLUS_MODE_DETECT_STRUCTS, EMAP2SEC_TYPE_EMAP2SECPLUS
+from kiharalab.constants import EMAP2SECPLUS_TYPE_EXPERIMENTAL, EMAP2SECPLUS_MODE_DETECT_EVALUATE_STRUCTS, EMAP2SECPLUS_MODE_DETECT_DNA
+from kiharalab.constants import EMAP2SECPLUS_FOLD3, EMAP2SECPLUS_MODE_DETECT_EXPERIMENTAL_FOLD4, EMAP2SECPLUS_MODE_DETECT_DNA_EXPERIMENTAL_FOLD4
+from kiharalab.constants import EMAP2SECPLUS_MODE_DETECT_EVALUATE_EXPERIMENTAL_FOLD4, EMAP2SECPLUS_TYPE_SIMUL6A, EMAP2SECPLUS_TYPE_SIMUL10A, EMAP2SECPLUS_TYPE_SIMUL6_10A
 
 class ProtEmap2sec(EMProtocol):
-    ("Emap2sec is a computational tool using deep learning that can accurately identify protein secondary structures,"
-    " alpha helices, beta sheets, others (coils/turns), in cryo-Electron Microscopy (EM) maps of medium to low resolution.\n"
-    "Emap2sec+ also covers DNA/RNA.\n"
-    "Original software can be found in https://github.com/kiharalab/Emap2sec and https://github.com/kiharalab/Emap2secPlus\n\n"
-    "Output files can be visualized outside scipion with pymol, running 'pymol <output_pdb_file>' once pymol is installed.\n"
-    "Pymol can be installed from https://pymol.org/2/ or an open source version can be found in https://github.com/schrodinger/pymol-open-source\n")
+    ("Identifies protein secondary structures, in maps of medium to low resolution.\nEmap2sec+ also covers DNA/RNA.\n\n"
+    "Original software can be found in https://github.com/kiharalab/Emap2sec and https://github.com/kiharalab/Emap2secPlus\n")
     _label = 'Emap2sec'
     _possibleOutputs = {'outputAtomStruct': AtomStruct}
 
     # -------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         """
         Defines Emap2sec's input params.
@@ -65,17 +64,19 @@
                         help='Select the type of execution between Emap2sec and Emap2sec+.\n'
                         'Emap2sec+ can only be run on GPU, while Emap2sec runs on CPU.')
         form.addParam('inputVolume', params.PointerParam, pointerClass='Volume', allowsNull=False,
                         label="Input volume: ", help='Select the electron map to be processed.')
         form.addParam('cleanTmps', params.BooleanParam, default='True', label='Clean temporary files: ', expertLevel=params.LEVEL_ADVANCED,
                         help='Clean temporary files after finishing the execution.\nThis is useful to reduce unnecessary disk usage.')
 
+        # Execution type variable
+        executionType = 'executionType=='
         # -------------------------------------- Emap2sec params --------------------------------------
-        trimmapGroup = form.addGroup('Trimmap generation', condition='executionType==%d' % EMAP2SEC_TYPE_EMAP2SEC)
-        trimmapGroup.addParam('emap2secContour', params.FloatParam, label='Contour: ', condition='executionType==%d' % EMAP2SEC_TYPE_EMAP2SEC,
+        trimmapGroup = form.addGroup('Trimmap generation', condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SEC}')
+        trimmapGroup.addParam('emap2secContour', params.FloatParam, label='Contour: ', condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SEC}',
                         help='The level of isosurface to generate density values for.\n'
                             'You can use a value of 0.0 for simulated maps and the author recommended contour level for experimental EM maps.')
         trimmapGroup.addParam('sstep', params.IntParam, default='4', label='Stride size: ', expertLevel=params.LEVEL_ADVANCED,
                         help='This option sets the stride size of the sliding cube used for input data generation.\n'
                             'We recommend using a value of 4 that slides the cube by 4Å in each direction.\n'
                             'Decreasing this value by 1 produces 8 times more data (increase by a factor of 2 in each direction)'
                             ' and thus slows the running time down by 8 times so please be mindful lowering this value.')
@@ -86,60 +87,60 @@
                             'Please be mindful while increasing this option as it increases the portion of an EM map a single cube covers.'
                             ' Increasing this value also increases running time.')
         trimmapGroup.addParam('norm', params.EnumParam, display=params.EnumParam.DISPLAY_COMBO, default=EMAP2SEC_NORM_GLOBAL, label='Normalization type: ',
                         expertLevel=params.LEVEL_ADVANCED, choices=['Global', 'Local'],
                         help='Set this option to normalize density values of the sliding cube, used for input data generation,'
                             ' by global or local maximum density value.')
                        
-        form.addParam('proteinId', params.StringParam, label='Protein id:', condition='executionType==%d' % EMAP2SEC_TYPE_EMAP2SEC,
+        form.addParam('proteinId', params.StringParam, label='Protein id:', condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SEC}',
                         expertLevel=params.LEVEL_ADVANCED, help='Optional.\nUnique protein identifier. Either EMID or SCOPe ID can be used.'
                             '\nFor example, protein EMD-1733 in EMDB has the identifier 1733.')
         
         form.addParam('predict', params.BooleanParam, default='True', label='Show Secondary Structures predicted data: ',
-                        condition='executionType==%d' % EMAP2SEC_TYPE_EMAP2SEC, expertLevel=params.LEVEL_ADVANCED,
+                        condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SEC}', expertLevel=params.LEVEL_ADVANCED,
                         help='Show predicted data (Predicted secondary structures).')
         
         # -------------------------------------- Emap2sec+ params --------------------------------------
         form.addParam('mode', params.EnumParam, display=params.EnumParam.DISPLAY_COMBO, default=EMAP2SECPLUS_MODE_DETECT_STRUCTS, label='Mode: ',
-                        condition='executionType==%d' % EMAP2SEC_TYPE_EMAP2SECPLUS, expertLevel=params.LEVEL_ADVANCED,
+                        condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SECPLUS}', expertLevel=params.LEVEL_ADVANCED,
                         choices=['Detect structures', 'Detect-evaluate structures', 'Detect DNA/RNA & protein'],
                         help='Set this option to define the execution mode. The options are:\n\n'
                             '- Detect structures: Detect structures for EM Map\n\n'
                             '- Detect-evaluate structures: Detect and evaluate structures for EM map with pdb structure\n\n'
                             '- Detect DNA/RNA & protein: Detect DNA/RNA and protein for experimental maps. Only available with 4 fold models\n\n'
                             'For detect-evaluate mode, evaluation results will show up in summary box.')
         form.addParam('mapType', params.EnumParam, display=params.EnumParam.DISPLAY_COMBO, default=EMAP2SECPLUS_TYPE_EXPERIMENTAL, label='Map type: ',
-                        condition='executionType==%d' % EMAP2SEC_TYPE_EMAP2SECPLUS, expertLevel=params.LEVEL_ADVANCED,
+                        condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SECPLUS}', expertLevel=params.LEVEL_ADVANCED,
                         choices=['Simulated map at 6Å', 'Simulated map at 10Å', 'Simulated map at 6-10Å', 'Experimental map'],
                         help='Set this option to define the type of input map.')
-        form.addParam('gpuId', params.IntParam, default='0', label='GPU id: ', condition='executionType==%d' % EMAP2SEC_TYPE_EMAP2SECPLUS,
+        form.addParam('gpuId', params.IntParam, default='0', label='GPU id: ', condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SECPLUS}',
                         help='Select the GPU id where the process will run on.')
         form.addParam('emap2secplusContour', params.FloatParam, default='0.0', label='Contour: ',
-                        condition='executionType==%d' % EMAP2SEC_TYPE_EMAP2SECPLUS, help='Contour level for real map.\n'
+                        condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SECPLUS}', help='Contour level for real map.\n'
                             'You can use the author recommended contour level, which will be used by a specific model,'
                             ' or 0.0 to indicate that no contour is defined, which will use a general purpose model.')
         form.addParam('inputStruct', params.PointerParam,
-                        condition='(executionType==%d and mode==%d)' % (EMAP2SEC_TYPE_EMAP2SECPLUS, EMAP2SECPLUS_MODE_DETECT_EVALUATE_STRUCTS),
+                        condition=f'({executionType}{EMAP2SEC_TYPE_EMAP2SECPLUS} and mode=={EMAP2SECPLUS_MODE_DETECT_EVALUATE_STRUCTS})',
                         pointerClass='AtomStruct', allowsNull=False, label="Input atom struct: ", help='Select the atom struct to evaluate the model with.')
-        form.addParam('classes', params.IntParam, default='4', label='Number of classes: ', condition='executionType==%d and mode!=%d' % (EMAP2SEC_TYPE_EMAP2SECPLUS, EMAP2SECPLUS_MODE_DETECT_DNA),
+        form.addParam('classes', params.IntParam, default='4', label='Number of classes: ', condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SECPLUS} and mode!={EMAP2SECPLUS_MODE_DETECT_DNA}',
                         expertLevel=params.LEVEL_ADVANCED, help='Select number of classes to differentiate between.\n'
                             'Not available for Detect DNA/RNA & protein mode.')
         form.addParam('fold', params.EnumParam, display=params.EnumParam.DISPLAY_COMBO, default=EMAP2SECPLUS_FOLD3, label='Fold model: ',
-                        condition='(executionType==%d and mode!=%d and mapType==%d)' % (EMAP2SEC_TYPE_EMAP2SECPLUS, EMAP2SECPLUS_MODE_DETECT_DNA, EMAP2SECPLUS_TYPE_EXPERIMENTAL),
+                        condition=f'({executionType}{EMAP2SEC_TYPE_EMAP2SECPLUS} and mode!={EMAP2SECPLUS_MODE_DETECT_DNA} and mapType=={EMAP2SECPLUS_TYPE_EXPERIMENTAL})',
                         expertLevel=params.LEVEL_ADVANCED, choices=['Fold 1', 'Fold 2', 'Fold 3', 'Fold 4'],
                         help='Set this option to specify the fold model used for detecting the experimental map.\n'
                             'This param is not available for DNA/RNA & protein detection.')
-        form.addParam('customModel', params.FolderParam, label='Custom model path: ', condition='executionType==%d and (fold==%d or mode==%d)' % (EMAP2SEC_TYPE_EMAP2SECPLUS, 3, EMAP2SECPLUS_MODE_DETECT_DNA),
+        form.addParam('customModel', params.FolderParam, label='Custom model path: ', condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SECPLUS} and (fold=={3} or mode=={EMAP2SECPLUS_MODE_DETECT_DNA})',
                         expertLevel=params.LEVEL_ADVANCED,
                         help='Set this option to specify the path to a custom model to be used by Emap2sec+.\n'
                             'The model needs to have the same directory and file structure as the models included with this protocol.\n'
                             'This means that, for each file or folder that exists within the example model, a file or folder (same type of element) with the same name must exist.\n'
                             'You can download a sample model to check the folder structure from https://kiharalab.org/emsuites/emap2secplus_model/nocontour_best_model.tar.gz\n'
                             'Custom models can only be used with 4 fold networks.')
-        form.addParam('getConfident', params.BooleanParam, default='True', label='Get confident results: ', expertLevel=params.LEVEL_ADVANCED, condition='executionType==%d' % EMAP2SEC_TYPE_EMAP2SECPLUS,
+        form.addParam('getConfident', params.BooleanParam, default='True', label='Get confident results: ', expertLevel=params.LEVEL_ADVANCED, condition=f'{executionType}{EMAP2SEC_TYPE_EMAP2SECPLUS}',
                         help='Only accept as valid predictions the ones with a 90%+ probability.')
 
     # --------------------------- STEPS functions ------------------------------
     def _insertAllSteps(self):
         """
         This method defines the functions that will be run during the execution of this protocol.
         """
@@ -204,72 +205,72 @@
         """
         # Building commands before actual protocol execution
         # Enviroment activation command. Needed to execute before every other standalone command.
         envActivationCommand = "{} {}".format(Plugin.getCondaActivationCmd(), Plugin.getProtocolActivationCommand('emap2sec'))
         
         # If custom output directory is specified, create it if it does not exist
         if outDir:
-            self.runJob("mkdir -p", outDir, cwd=Plugin._emap2secRepo)
+            self.runJob("mkdir -p", outDir, cwd=Plugin._emap2secBinary)
 
         # Command to move to Emap2sec's repo's root directory.
         # Needed to be executed before the actual workflow commands
         moveToRepoCommand = "cd"
-        self.runJob(moveToRepoCommand, Plugin._emap2secRepo, cwd=Plugin._emap2secRepo)
+        self.runJob(moveToRepoCommand, Plugin._emap2secBinary, cwd=Plugin._emap2secBinary)
 
         # Trimapp generation command
         trimappCommand = "data_generate/map2train"
-        self.runJob(trimappCommand, args[0], cwd=Plugin._emap2secRepo)
+        self.runJob(trimappCommand, args[0], cwd=Plugin._emap2secBinary)
 
         # Dataset generation command
         datasetCommand = "{} && python data_generate/dataset.py".format(envActivationCommand)
-        self.runJob(datasetCommand, args[1], cwd=Plugin._emap2secRepo)
+        self.runJob(datasetCommand, args[1], cwd=Plugin._emap2secBinary)
 
         # Input file for Emap2sec.py
-        self.runJob("echo", args[2], cwd=Plugin._emap2secRepo)
+        self.runJob("echo", args[2], cwd=Plugin._emap2secBinary)
 
         # Emap2sec execution command
         emap2secCommand = "{} && python emap2sec/Emap2sec.py".format(envActivationCommand)
-        self.runJob(emap2secCommand, args[3], cwd=Plugin._emap2secRepo)
+        self.runJob(emap2secCommand, args[3], cwd=Plugin._emap2secBinary)
         
         # Secondary structures visualization command
         visualCommand = "Visual/Visual.pl"
-        self.runJob(visualCommand, args[4], cwd=Plugin._emap2secRepo)
+        self.runJob(visualCommand, args[4], cwd=Plugin._emap2secBinary)
 
         # Remove temporary files
         if clean:
             for tmp_file in args[5]:
-                self.runJob("rm -rf", tmp_file, cwd=Plugin._emap2secRepo)
+                self.runJob("rm -rf", tmp_file, cwd=Plugin._emap2secBinary)
     
     # ---------------------------------- Emap2sec+ ----------------------------------
     def runEmap2secPlus(self, args, clean=True):
         """
         Run Emap2secPlus script from a given protocol.
         """
         # Building commands before actual protocol execution
         # Enviroment activation command. Needed to execute befor every other standalone command.
         envActivationCommand = "{} {}".format(Plugin.getCondaActivationCmd(), Plugin.getProtocolActivationCommand('emap2sec', 'emap2secPlus'))
         
         # Command to move to Emap2sec+'s repo's root directory.
         # Needed to be executed once before the actual workflow commands
         moveToRepoCommand = "cd"
-        self.runJob(moveToRepoCommand, Plugin._emap2secplusRepo, cwd=Plugin._emap2secplusRepo)
+        self.runJob(moveToRepoCommand, Plugin._emap2secplusBinary, cwd=Plugin._emap2secplusBinary)
 
         # Emap2sec+ execution command
         runCommand = "{} && python3 main.py".format(envActivationCommand)
-        self.runJob(runCommand, args[0], cwd=Plugin._emap2secplusRepo)
+        self.runJob(runCommand, args[0], cwd=Plugin._emap2secplusBinary)
 
         # Output file/s relocation
-        self.runJob("mv", args[1][0] + ' ' + args[1][1], cwd=Plugin._emap2secplusRepo)
+        self.runJob("mv", args[1][0] + ' ' + args[1][1], cwd=Plugin._emap2secplusBinary)
         if len(args[1]) == 4:
-            self.runJob("mv", args[1][2] + ' ' + args[1][3], cwd=Plugin._emap2secplusRepo)
+            self.runJob("mv", args[1][2] + ' ' + args[1][3], cwd=Plugin._emap2secplusBinary)
 
         # Remove temporary files
         if clean:
             for tmp_file in args[2]:
-                self.runJob("rm -rf", tmp_file, cwd=Plugin._emap2secplusRepo)
+                self.runJob("rm -rf", tmp_file, cwd=Plugin._emap2secplusBinary)
     # --------------------------- INFO functions -----------------------------------
     def _summary(self):
         """
         This method usually returns a summary of the text provided by '_methods'.
         """
         summary = []
 
@@ -278,15 +279,15 @@
             metricsFilename = os.path.join(self.getOutputPath(), self.getEmap2secPlusMetricsFile())
             try:
                 metricsFile = open(metricsFilename, 'r')
                 summary.append('Model evaluation results:')
                 for line in metricsFile:
                     summary.append(line)
                 metricsFile.close()
-            except:
+            except FileNotFoundError:
                 summary.append('Metric results not ready yet.')
         
         return summary
 
     def _methods(self):
         """
         This method returns a text intended to be copied and pasted in the paper section 'materials & methods'.
@@ -304,16 +305,16 @@
         This method validates the received params and checks that they all fullfill the requirements needed to run the protocol.
         """
         errors = []
         if self.executionType.get() == EMAP2SEC_TYPE_EMAP2SECPLUS:
             # Detecting if host machine has Nvidia drivers installed
             try:
                 # If no Nvidia drivers are present, the following command will reuturn an error
-                subprocess.check_output(['nvidia-smi'])
-            except Exception as e:
+                subprocess.run(['nvidia-smi'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+            except Exception:
                 errors.append('No Nvidia drivers detected on this machine.\n'
                     'Emap2sec+ needs an Nvidia GPU to run.')
 
         return errors
 
     # --------------------------- UTILS functions -----------------------------------
     def getProtocolPrefix(self):
@@ -438,22 +439,22 @@
         return args
 
     # -------------------------------- Emap2sec specific functions --------------------------------
     def getTrimmapArgs(self):
         """
         This method returns a list with the arguments neccessary for the trimmap generation for the volume.
         """
-        file = self.getConvertedVolumeAbsolutePath()
+        inputfFile = self.getConvertedVolumeAbsolutePath()
         return '{} -c {} -sstep {} -vw {} {} > data/{}trimmap'\
-        .format(file,
+        .format(inputfFile,
             self.emap2secContour.get(),
             self.sstep.get(),
             self.vw.get(),
             '-gnorm' if self.norm.get() == EMAP2SEC_NORM_GLOBAL else '-Inorm',
-            self.getProtocolFilePrefix(file))
+            self.getProtocolFilePrefix(inputfFile))
     
     def getDatasetArgs(self):
         """
         This method returns the arguments neccessary for the dataset generation.
         """
         outputPefix = 'data/{}'.format(self.getProtocolFilePrefix(self.getVolumeAbsolutePath()))
         proteinId = (' ' + self.proteinId.get()) if self.proteinId.get() else ''
@@ -473,20 +474,20 @@
         """
         return 'data/{}input.txt --prefix results/{}'.format(self.getProtocolPrefix(), self.getProtocolPrefix())
 
     def getVisualArgs(self):
         """
         This method returns the arguments neccessary for the Secondary Structure visualization.
         """
-        file = self.getVolumeAbsolutePath()
+        inputFile = self.getVolumeAbsolutePath()
         return 'data/{}trimmap results/{}outputP2_{}dataset -p > {}'\
-                .format(self.getProtocolFilePrefix(file),
+                .format(self.getProtocolFilePrefix(inputFile),
                     self.getProtocolPrefix(),
-                    self.getProtocolFilePrefix(file),
-                    self.getOutputFile(file))
+                    self.getProtocolFilePrefix(inputFile),
+                    self.getOutputFile(inputFile))
     
     # -------------------------------- Emap2sec+ specific functions --------------------------------
     def getFoldModel(self):
         """
         This method returns the real fold value selected by the user.
         That is the value returned by the form + 1, because input param list starts by 1 but arrays start by 0.
         """
@@ -564,18 +565,26 @@
 
         return param
     
     def getEmap2secPlusTypePath(self):
         """
         This method returns the first folder for the output path for Emap2sec+, matching the map type.
         """
-        return ('SIMU6' if self.mapType.get() == EMAP2SECPLUS_TYPE_SIMUL6A else
-            ('SIMU10' if self.mapType.get() == EMAP2SECPLUS_TYPE_SIMUL10A else
-            ('SIMU_MIX' if self.mapType.get() == EMAP2SECPLUS_TYPE_SIMUL6_10A else 'REAL'))
-        )
+        # Obtaining map type
+        if self.mapType.get() == EMAP2SECPLUS_TYPE_SIMUL6A:
+            mapType = 'SIMU6'
+        elif self.mapType.get() == EMAP2SECPLUS_TYPE_SIMUL10A:
+            mapType = 'SIMU10'
+        elif self.mapType.get() == EMAP2SECPLUS_TYPE_SIMUL6_10A:
+            mapType = 'SIMU_MIX'
+        else:
+            mapType = 'REAL'
+
+        # Returning resulting type
+        return mapType
     
     def getEmap2secPlusDefaultOutputPath(self, base=False):
         """
         This method returns the default output file path for Emap2sec+.
         """
         # Checking if selected mode is DNA/RNA & protein prediction (causes path format changes)
         modeIsDNA = self.getMode() == EMAP2SECPLUS_MODE_DETECT_DNA_EXPERIMENTAL_FOLD4
@@ -585,16 +594,17 @@
         filePath = os.path.splitext(self.getVolumeName(self.getVolumeAbsolutePath()))[0]
         basePath = os.path.join(self.getOutputPath(),
                 'Binary' if modeIsDNA else '',
                 self.getEmap2secPlusTypePath(),
                 foldPath if not modeIsDNA else '',
                 filePath
             )
+        finalPath = 'Phase2' if not modeIsDNA else 'Final'
 
-        return basePath if base else os.path.join(basePath, 'Phase2' if not modeIsDNA else 'Final')
+        return basePath if base else os.path.join(basePath, finalPath)
     
     def getEmap2secPlusOutputFile(self, clean=True):
         """
         This method returns the default output file name for Emap2sec+.
         """
         inputFile = self.getVolumeAbsolutePath()
         volumeName = os.path.splitext(self.getCleanVolumeName(inputFile) if clean else self.getVolumeName(inputFile))[0]
@@ -621,8 +631,8 @@
         ]
 
         # If evaluation mode, also move metrics report file
         if self.mode.get() == EMAP2SECPLUS_MODE_DETECT_EVALUATE_STRUCTS:
             params.append(os.path.join(self.getEmap2secPlusDefaultOutputPath(base=True), self.getEmap2secPlusMetricsFile(clean=False)))
             params.append(os.path.join(self.getOutputPath(), self.getEmap2secPlusMetricsFile()))
 
-        return params
+        return params
```

### Comparing `scipion-em-kiharalab-1.0/kiharalab/protocols/protocol_mainmast_segment_map.py` & `scipion-em-kiharalab-1.0.1/kiharalab/protocols/protocol_mainmast_segment_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,24 +20,34 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
+# General imports
 import os, glob
 import numpy as np
 
+# Base Scipion imports
 from pwem.protocols import EMProtocol
 from pyworkflow.protocol import params
 from pwem.emlib.image import ImageHandler
 from pwem.objects import Volume, SetOfVolumes
 
+# Plugin imports
 from kiharalab import Plugin as Mainmast
-from phenix import Plugin as Phenix
+try:
+    from phenix import Plugin as Phenix
+except ModuleNotFoundError:
+    raise ModuleNotFoundError("Plugin scipion-em-phenix is not installed!\n"
+                              "You can find it at https://github.com/scipion-em/scipion-em-phenix")
+
+# Constants
+REGIONS_PATTERN = "region*.mrc"
 
 class ProtMainMastSegmentMap(EMProtocol):
     """Protcol to perform the segmentation of maps into different regions by using
     mainmast software.
     For more information, follow the next link:
     http://kiharalab.org/mainmast_seg/index.html"""
     _label = 'segment map'
@@ -103,18 +113,18 @@
         self.runSegmentation(args, cwd=self._getExtraPath())
 
     def createOutputStep(self):
         """
         This method processes the output files generated by the protocol and imports them into Scipion objects.
         """
         # Getting region files
-        regionFiles = sorted(glob.glob(self._getExtraPath("region*.mrc")))
+        regionFiles = sorted(glob.glob(self._getExtraPath(REGIONS_PATTERN)))
         if len(regionFiles) == 0:
             # If region files were not found, throw an exception and cancel execution
-            raise Exception("Region files were not generated after MainMast's execution."
+            raise FileNotFoundError("Region files were not generated after MainMast's execution."
                 " This could be caused by an insufficient amount of dynamic memory being available to the process, "
                 "specially if the execution only took some seconds. Try providing more RAM to your system, or"
                 " to Scipion if any memory limits have been set.")
         
         if self.combine.get():
             # If combine is selected, return object is of type Volume
             ih = ImageHandler()
@@ -163,30 +173,30 @@
             self.cleanTmpfiles(self.getTmpFiles())
     
     # --------------------------- EXECUTION functions -----------------------------------
     def runSegmentation(self, args, cwd=None):
         """
         Run segmentation phase for MainMast.
         """
-        mainMastCall = os.path.join(Mainmast._mainmastRepo, 'MainmastSeg')
+        mainMastCall = os.path.join(Mainmast._mainmastBinary, 'MainmastSeg')
         self.runJob(mainMastCall, args, cwd=cwd)
     
     def convertMatrix(self, args, cwd=None):
         """
         Run matrix conversion phase for MainMast.
         """
-        convertCall = os.path.join(Mainmast._mainmastRepo, 'conv_ncs.pl')
+        convertCall = os.path.join(Mainmast._mainmastBinary, 'conv_ncs.pl')
         self.runJob(convertCall, args, cwd=cwd)
 
     def cleanTmpfiles(self, tmpFiles=[]):
         """
         This method removes all temporary files to reduce disk usage.
         """
         for tmp_file in tmpFiles:
-            self.runJob("rm -rf", tmp_file, cwd=Mainmast._mainmastRepo)
+            self.runJob("rm -rf", tmp_file, cwd=Mainmast._mainmastBinary)
 
     # --------------------------- UTILS functions ------------------------------
     def scapePath(self, path):
         """
         This function returns the given path with all the spaces in folder names scaped to avoid errors.
         """
         # os.path.baspath adds '\\' when finding a foldername with '\ ', so '\\\' needs to be replaced with ''
@@ -217,30 +227,30 @@
             self.getExtraFileAbsolutePath('contour.cif'),
             self.getExtraFileAbsolutePath('sym_mat.txt'),
             self.getExtraFileAbsolutePath('symmetry_from_map.ncs_spec')
         ]
 
         # if combine is selected, region files are not needed any more
         if self.combine.get():
-            regionFiles = sorted(glob.glob(self.getExtraFileAbsolutePath("region*.mrc")))
+            regionFiles = sorted(glob.glob(self.getExtraFileAbsolutePath(REGIONS_PATTERN)))
             for regionFile in regionFiles:
                 tmpFiles.append(regionFile)
 
         return tmpFiles
 
     # --------------------------- INFO functions -----------------------------------
     def _summary(self):
         """
         This method returns a summary of the text provided by '_methods'.
         """
         summary = []
         summary.append("Input Volume provided: %s\n"
                        % self.inputVolume.get().getFileName())
         if self.getOutputsSize() >= 1:
-            regions = len(glob.glob(self._getExtraPath("region*.mrc")))
+            regions = len(glob.glob(self._getExtraPath(REGIONS_PATTERN)))
             if hasattr(self, 'outputMasks'):
                 msg = ("A total of %d regions have been segmented" % regions)
                 summary.append(msg)
             if hasattr(self, 'outputMask'):
                 msg = ("Output regions combined to an indentifier mask with %d different "
                        "regions" % regions)
                 summary.append(msg)
@@ -254,15 +264,15 @@
         """
         methodsMsgs = []
         methodsMsgs.append('*Input volume:* %s' % self.inputVolume.get().getFileName())
         methodsMsgs.append('*Map symmetry:* %s' % self.sym.get())
         methodsMsgs.append('*Map threshold:* %d' % self.threshold.get())
         methodsMsgs.append('*Regions combined:* %r' % self.combine.get())
         if self.getOutputsSize() >= 1:
-            regions = len(glob.glob(self._getExtraPath("region*.mrc")))
+            regions = len(glob.glob(self._getExtraPath(REGIONS_PATTERN)))
             msg = ("*Regions segmented:* %d" % regions)
             methodsMsgs.append(msg)
         else:
             methodsMsgs.append("Segmentation not ready yet.")
         return methodsMsgs
     
     def _validate(self):
```

### Comparing `scipion-em-kiharalab-1.0/kiharalab/protocols.conf` & `scipion-em-kiharalab-1.0.1/kiharalab/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-kiharalab-1.0/kiharalab/tests/__init__.py` & `scipion-em-kiharalab-1.0.1/kiharalab/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-kiharalab-1.0/kiharalab/tests/test_daq.py` & `scipion-em-kiharalab-1.0.1/kiharalab/tests/test_daq.py`

 * *Files identical despite different names*

### Comparing `scipion-em-kiharalab-1.0/kiharalab/tests/test_emap2sec.py` & `scipion-em-kiharalab-1.0.1/kiharalab/tests/test_emap2sec.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 # **************************************************************************
 
 import os
 from pyworkflow.tests import BaseTest, setupTestProject, DataSet
 from pwem.protocols import ProtImportVolumes, ProtImportPdb
 from ..protocols import ProtEmap2sec
 from kiharalab import Plugin
-from kiharalab.constants import *
+from kiharalab.constants import EMAP2SEC_TYPE_EMAP2SEC, EMAP2SEC_TYPE_EMAP2SECPLUS
+from kiharalab.constants import EMAP2SECPLUS_MODE_DETECT_STRUCTS, EMAP2SECPLUS_MODE_DETECT_EVALUATE_STRUCTS
 
 class TestEmap2sec(BaseTest):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.tmpFiles = []
         cls.ds = DataSet.getDataSet('model_building_tutorial')
@@ -56,15 +57,15 @@
         cls.launchProtocol(protImportVolumes)
 
         # Storing results
         cls.protImportVolumePredict = protImportVolumes
 
         # Creating arguments for import volumes protocol for evaluation purposes
         args = {
-            'filesPath': os.path.join(Plugin._emap2secRepo, 'data', '1733.mrc'),
+            'filesPath': os.path.join(Plugin._emap2secBinary, 'data', '1733.mrc'),
             'samplingRate': 1.36825,
             'setOrigCoord': False
         }
 
         # Creating and launching import volumes protocol
         protImportVolumes = cls.newProtocol(ProtImportVolumes, **args)
         cls.launchProtocol(protImportVolumes)
@@ -73,15 +74,15 @@
         cls.protImportVolumeEvaluate = protImportVolumes
     
     @classmethod
     def _runImportPDB(cls):
         # Creating arguments for import pdb protocol
         args = {
             'inputPdbData': 1,
-            'pdbFile': os.path.join(Plugin._emap2secRepo, 'data', '3c91.pdb'),
+            'pdbFile': os.path.join(Plugin._emap2secBinary, 'data', '3c91.pdb'),
             'inputVolume': cls.protImportVolumeEvaluate.outputVolume
         }
 
         # Creating and launching import pdb protocol
         protImportPDB = cls.newProtocol(ProtImportPdb, **args)
         cls.launchProtocol(protImportPDB)
```

### Comparing `scipion-em-kiharalab-1.0/kiharalab/tests/test_mainmast.py` & `scipion-em-kiharalab-1.0.1/kiharalab/tests/test_mainmast.py`

 * *Files identical despite different names*

### Comparing `scipion-em-kiharalab-1.0/kiharalab/viewers/viewer_daq.py` & `scipion-em-kiharalab-1.0.1/kiharalab/viewers/viewer_daq.py`

 * *Files identical despite different names*

### Comparing `scipion-em-kiharalab-1.0/kiharalab/viewers/viewer_emap2sec.py` & `scipion-em-kiharalab-1.0.1/kiharalab/viewers/viewer_emap2sec.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,24 +20,25 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
+# General imports
 import os
 from shutil import which
 
+# Base Scipion viewer imports
 import pyworkflow.viewer as pwviewer
+from pwem.viewers.viewer_chimera import Chimera, ChimeraView
 
-import pwem.viewers as viewers
-from pwem.viewers.viewer_chimera import ChimeraView
-
+# Plugin imports
 from ..protocols.protocol_emap2sec import ProtEmap2sec
-from kiharalab.constants import *
+from kiharalab.constants import EMAP2SEC_TYPE_EMAP2SECPLUS, EMAP2SECPLUS_MODE_DETECT_EVALUATE_STRUCTS
 
 class Emap2secViewer(pwviewer.Viewer):
     """
     Wrapper to visualize different outputs of MAINMASTseg software.
     """
     _environments = [pwviewer.DESKTOP_TKINTER]
     _targets = [ProtEmap2sec]
@@ -54,42 +55,45 @@
         return views
 
     def _validate(self):
         """
         This function validates the installation of Chimera so the files can be visualized.
         """
         errors = []
-        if (which(viewers.viewer_chimera.Chimera.getProgram()) is None):
+        if (which(Chimera.getProgram()) is None):
             errors.append("Chimera is not available. Please install it to visualize.")
         return errors
     
     def chimeraViewFile(self, axis=False):
         """
         This function creates the Chimera file needed to visualize the results.
         """
         # Creating cxc file for Chimera commands
         filePath = os.path.abspath(self.protocol._getExtraPath('chimera.cxc'))
         inputVolume = self.protocol.getVolumeAbsolutePath()
 
+        # Open command
+        openCommandPrefix = 'open'
+
         f = open(filePath, "w")
         # Adding axis to file if requested
         if axis:
             builFileName = os.path.abspath(self.protocol._getExtraPath("axis.bild"))
-            viewers.viewer_chimera.Chimera.createCoordinateAxisFile(self.protocol.inputVolume.get().getDim()[0],
+            Chimera.createCoordinateAxisFile(self.protocol.inputVolume.get().getDim()[0],
                 bildFileName=os.path.abspath(self.protocol._getExtraPath("axis.bild")),
                 sampling=self.protocol.inputVolume.get().getSamplingRate())
-            f.write('open %s\n' % builFileName)
+            f.write(f'{openCommandPrefix} {builFileName}\n')
             
             # Setting center of coordinates for the axis
             f.write('cofr 0,0,0\n')
 
         # Adding input Volume
-        f.write('open %s\n' % inputVolume)
+        f.write(f'{openCommandPrefix} {inputVolume}\n')
         # Adding output Atom Struct
-        f.write('open %s\n' % self.protocol.getOutputFile(inputVolume))
+        f.write(f'{openCommandPrefix} {self.protocol.getOutputFile(inputVolume)}\n')
         # If evaluation mode on Emap2sec+, add reference pdb
         if self.protocol.executionType.get() == EMAP2SEC_TYPE_EMAP2SECPLUS and self.protocol.mode.get() == EMAP2SECPLUS_MODE_DETECT_EVALUATE_STRUCTS:
-            f.write('open %s\n' % self.protocol.getStructAbsolutePath())
+            f.write(f'{openCommandPrefix} {self.protocol.getStructAbsolutePath()}\n')
         f.close()
 
         # Returning written file 
         return filePath
```

### Comparing `scipion-em-kiharalab-1.0/kiharalab/viewers/viewer_mainmast.py` & `scipion-em-kiharalab-1.0.1/kiharalab/viewers/viewer_mainmast.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,37 +20,38 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
+# General imports
 import os, glob
 
+# Base Scipion viewer imports
 import pyworkflow.viewer as pwviewer
+from pwem.viewers.views import ObjectView
+from pwem.viewers.viewer_chimera import Chimera, ChimeraView
 
-import pwem.viewers as viewers
-import pwem.viewers.views as vi
-from pwem.viewers.viewer_chimera import ChimeraView
-
+# Plugin imports
 from ..protocols.protocol_mainmast_segment_map import ProtMainMastSegmentMap
 
 class MainMastViewer(pwviewer.Viewer):
     """
     Wrapper to visualize different outputs of MAINMASTseg software.
     """
     _environments = [pwviewer.DESKTOP_TKINTER]
     _targets = [ProtMainMastSegmentMap]
 
     def __init__(self, **kwargs):
         pwviewer.Viewer.__init__(self, **kwargs)
         self._views = []
 
     def _getObjView(self, obj, fn, viewParams={}):
-        return vi.ObjectView(
+        return ObjectView(
             self._project, obj.strId(), fn, viewParams=viewParams)
 
     def _visualize(self, obj, **kwargs):
         views = []
         cls = type(obj)
 
         if issubclass(cls, ProtMainMastSegmentMap):
@@ -72,15 +73,15 @@
             volumeIdx = idx + 1
             f.write('open %s\n' % os.path.abspath(segmentation))
             f.write('volume #%d step 1 level %f\n' % (volumeIdx, self.protocol.threshold.get()))
 
         # Adding axis to file if requested
         if axis:
             builFileName = os.path.abspath(self.protocol._getExtraPath("axis.bild"))
-            viewers.viewer_chimera.Chimera.createCoordinateAxisFile(self.protocol.inputVolume.get().getDim()[0],
+            Chimera.createCoordinateAxisFile(self.protocol.inputVolume.get().getDim()[0],
                 bildFileName=os.path.abspath(self.protocol._getExtraPath("axis.bild")),
                 sampling=self.protocol.inputVolume.get().getSamplingRate())
             f.write('open %s\n' % builFileName)
 
             # Setting center of coordinates for the axis
             f.write('cofr 0,0,0\n')
```

### Comparing `scipion-em-kiharalab-1.0/kiharalab/wizards.py` & `scipion-em-kiharalab-1.0.1/kiharalab/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-kiharalab-1.0/scipion_em_kiharalab.egg-info/SOURCES.txt` & `scipion-em-kiharalab-1.0.1/scipion_em_kiharalab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CHANGES.txt
+CHANGES.rst
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 kiharalab/__init__.py
 kiharalab/bibtex.py
```

### Comparing `scipion-em-kiharalab-1.0/setup.py` & `scipion-em-kiharalab-1.0.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,17 +25,38 @@
 
 setup(
     name='scipion-em-kiharalab',  # Required
     version=__version__,  # Required
     description='Scipion plugin in order to use ther kiharalab software',  # Required
     long_description=long_description,  # Optional
     url='https://github.com/scipion-em/scipion-em-kiharalab',  # Optional
-    author='Daniel Del Hoyo',  # Optional
-    author_email='ddelhoyo@cnb.csic.es',  # Optional
+    author='Daniel Del Hoyo, Martín Salinas',  # Optional
+    author_email='ddelhoyo@cnb.csic.es, martin.salinas@cnb.csic.es',  # Optional
     keywords='scipion kiharalab scipion-3.0 EM',  # Optional
+    classifiers=[  # Optional
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        'Development Status :: 4 - Beta',
+
+        # Indicate who your project is intended for
+        #   'Intended Audience :: Users',
+
+        # Pick your license as you wish
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
+        'Programming Language :: Python :: 3'
+    ],
     packages=find_packages(),
     install_requires=[requirements],
     entry_points={'pyworkflow.plugin': 'kiharalab = kiharalab'},
     package_data={  # Optional
        'kiharalab': [_logo, 'protocols.conf'],
+    },
+    project_urls={  # Optional
+        'Bug Reports': 'https://github.com/scipion-em/scipion-em-kiharalab/issues',
+        'Pull Requests': 'https://github.com/scipion-em/scipion-em-kiharalab/pulls',
     }
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

