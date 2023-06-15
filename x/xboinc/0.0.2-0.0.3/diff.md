# Comparing `tmp/xboinc-0.0.2.tar.gz` & `tmp/xboinc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xboinc-0.0.2.tar", max compression
+gzip compressed data, was "xboinc-0.0.3.tar", max compression
```

## Comparing `xboinc-0.0.2.tar` & `xboinc-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11356 2022-08-25 09:32:00.436120 xboinc-0.0.2/LICENSE
--rw-r--r--   0        0        0       74 2023-06-15 14:32:32.272596 xboinc-0.0.2/NOTICE
--rw-r--r--   0        0        0     6931 2023-03-03 10:01:23.334000 xboinc-0.0.2/README.md
--rw-r--r--   0        0        0      812 2023-06-15 14:32:32.272596 xboinc-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      308 2023-06-15 14:32:32.273595 xboinc-0.0.2/xboinc/__init__.py
--rw-r--r--   0        0        0     2112 2023-06-15 14:32:32.273595 xboinc-0.0.2/xboinc/default_tracker.py
--rw-r--r--   0        0        0     2648 2023-03-11 16:38:22.809319 xboinc-0.0.2/xboinc/eos.py
--rw-r--r--   0        0        0     3777 2023-06-15 14:32:32.273595 xboinc-0.0.2/xboinc/executable_src/main.c
--rw-r--r--   0        0        0       71 2023-02-15 13:32:40.914000 xboinc-0.0.2/xboinc/general.py
--rw-r--r--   0        0        0     2397 2023-06-15 14:32:32.273595 xboinc-0.0.2/xboinc/generate_executable_source.py
--rw-r--r--   0        0        0     2252 2023-06-15 14:32:32.273595 xboinc-0.0.2/xboinc/sim_data.py
--rw-r--r--   0        0        0     2203 2023-05-31 11:26:39.028175 xboinc-0.0.2/xboinc/submit.py
--rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 xboinc-0.0.2/setup.py
--rw-r--r--   0        0        0     7833 1970-01-01 00:00:00.000000 xboinc-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2022-08-25 09:32:00.436120 xboinc-0.0.3/LICENSE
+-rw-r--r--   0        0        0       74 2023-06-15 14:32:32.272596 xboinc-0.0.3/NOTICE
+-rw-r--r--   0        0        0     6931 2023-03-03 10:01:23.334000 xboinc-0.0.3/README.md
+-rw-r--r--   0        0        0      813 2023-06-15 14:42:02.615090 xboinc-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-06-15 14:42:02.615090 xboinc-0.0.3/xboinc/__init__.py
+-rw-r--r--   0        0        0     2112 2023-06-15 14:32:32.273595 xboinc-0.0.3/xboinc/default_tracker.py
+-rw-r--r--   0        0        0     2648 2023-03-11 16:38:22.809319 xboinc-0.0.3/xboinc/eos.py
+-rw-r--r--   0        0        0     3777 2023-06-15 14:32:32.273595 xboinc-0.0.3/xboinc/executable_src/main.c
+-rw-r--r--   0        0        0       71 2023-02-15 13:32:40.914000 xboinc-0.0.3/xboinc/general.py
+-rw-r--r--   0        0        0     2397 2023-06-15 14:32:32.273595 xboinc-0.0.3/xboinc/generate_executable_source.py
+-rw-r--r--   0        0        0     2252 2023-06-15 14:32:32.273595 xboinc-0.0.3/xboinc/sim_data.py
+-rw-r--r--   0        0        0     2203 2023-05-31 11:26:39.028175 xboinc-0.0.3/xboinc/submit.py
+-rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 xboinc-0.0.3/setup.py
+-rw-r--r--   0        0        0     7833 1970-01-01 00:00:00.000000 xboinc-0.0.3/PKG-INFO
```

### Comparing `xboinc-0.0.2/LICENSE` & `xboinc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xboinc-0.0.2/README.md` & `xboinc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xboinc-0.0.2/pyproject.toml` & `xboinc-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xboinc"
-version = "0.0.2"
+version = "0.0.3"
 description = "Xsuite BOINC interface"
 homepage = "https://github.com/xsuite/xboinc"
 repository = "https://github.com/xsuite/xboinc"
 authors = [
            "Frederik F. Van der Veken <frederik@cern.ch>",
            "Davide Di Croce <davide.di.croce@cern.ch>",
            "Giovanni Iadorala <giovanni.iadorala@cern.ch>"
@@ -26,8 +26,8 @@
 
 [tool.poetry.dev-dependencies]
 pytest = ">7"
 
 [build-system]
 # Needed for pip install -e (BTW: need pip version 22)
 requires = ["poetry-core>=1.0.8"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `xboinc-0.0.2/xboinc/default_tracker.py` & `xboinc-0.0.3/xboinc/default_tracker.py`

 * *Files identical despite different names*

### Comparing `xboinc-0.0.2/xboinc/eos.py` & `xboinc-0.0.3/xboinc/eos.py`

 * *Files identical despite different names*

### Comparing `xboinc-0.0.2/xboinc/executable_src/main.c` & `xboinc-0.0.3/xboinc/executable_src/main.c`

 * *Files identical despite different names*

### Comparing `xboinc-0.0.2/xboinc/generate_executable_source.py` & `xboinc-0.0.3/xboinc/generate_executable_source.py`

 * *Files identical despite different names*

### Comparing `xboinc-0.0.2/xboinc/sim_data.py` & `xboinc-0.0.3/xboinc/sim_data.py`

 * *Files identical despite different names*

### Comparing `xboinc-0.0.2/xboinc/submit.py` & `xboinc-0.0.3/xboinc/submit.py`

 * *Files identical despite different names*

### Comparing `xboinc-0.0.2/setup.py` & `xboinc-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'xfields>=0.12.1,<0.13.0',
  'xobjects>=0.2.6,<0.3.0',
  'xpart>=0.15.0,<0.16.0',
  'xtrack>=0.36.5,<0.37.0']
 
 setup_kwargs = {
     'name': 'xboinc',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Xsuite BOINC interface',
     'long_description': '# XBOINC\n\n## Python package for submitting track simulations in particle accelerators with BOINC system\n\n## INSTRUCTIONS FOR WINDOWS:\n\n### How to install boinc client/manager on Windows\n\nUse the installer at: https://boinc.berkeley.edu/download.php\n\n\n### Compile boinc api and examples from source on Windows\n\nWe use MSys2, in particular **MINGW64**\n\nFollow the instruction at https://www.msys2.org to install MSYS2 and GCC:\n```\npacman -S mingw-w64-x86_64-gcc\npacman -Suy\npacman -Suy  # you need indeed twice!\n```\n\nInstall git and python packages:\n```\npacman -S git\npacman -Sy mingw-w64-x86_64-python-numpy\npacman -Sy mingw-w64-x86_64-python-scipy\npacman -Sy mingw-w64-x86_64-python-pandas\npacman -Sy mingw-w64-x86_64-python-pip\npacman -Sy mingw-w64-x86_64-python-wheel\npacman -Sy vim\n```\n\n#### Compile BOINC\n```\npacman -S autotools\ncd\ngit clone https://github.com/BOINC/boinc\ncd boinc\nexport BOINC_DIR=$PWD\n \n./_autosetup\n \n./configure --disable-server --disable-client --disable-manager --disable-gui\n# This one takes very long\n \nmake\n# This also takes quite long\n```\n\n### Generate xboinc source and input files on windows\n\n```\ncd \nmkdir xsuite_packages\ncd xsuite_packages\ngit clone https://github.com/xsuite/xobjects.git\ngit clone https://github.com/xsuite/xpart.git\ngit clone https://github.com/xsuite/xtrack.git\ngit clone https://github.com/xsuite/xfields.git\ngit clone https://github.com/xsuite/xboinc.git\n\npip install --no-deps --no-build-isolation -e xtrack\npip install --no-deps --no-build-isolation -e xobjects\npip install --no-deps --no-build-isolation -e xpart\npip install --no-deps --no-build-isolation -e xfields\npip install --no-deps --no-build-isolation -e xboinc\n```\n\n#### Compile and generate input\n\n\n```bash\ncd xboinc/examples/000_build_executable\npython 000_build_executable.py\nbash 001msys2_compile_executable.sh\ncd ../002_lhc\npython 001_build_input.py\ncd ../003_boinc\necho $BOINC_DIR # Check if points into the BOINC source directory \npython 000_build_executable.py\nmake\n```\n\n#### Run/test the executable\n```\ncp ../002_lhc/xboinc_input.bin .\nchmod +x xboinc_executable\n./xboinc_executable\n```\n\n#### Running the test application with boinc server\nWe still work in MSYS2 (MINGW64)\n\nIn order to have it working we needed to have the file structure in C:\\PrgramData\\Boinc\n\n```\ncd /c/ProgramData/BOINC # This in WINDOWS is hidden\ncp ~/xsuite_packages/xboinc/examples/003_boinc/client_state_save.xml .\n```\nthen\n\n```\nnano account_test.xml \n```\n\nwrite\n```\n<account>\n    <master_url>http://test.test</master_url>\n    <project_name>test_project</project_name>\n</account>\n```\nthen \n```nano cc_config.xml```\nwrite\n```\n<cc_config>\n    <options>\n        <skip_cpu_benchmarks/>\n        <unsigned_apps_ok/>\n    </options>\n</cc_config>\n```\nThen make folder structure\n```\nmkdir projects/test.test\ncp ~/xsuite_packages/xboinc/examples/002_lhc/xboinc_input.bin projects/test.test/input.bin\ncp ~/xsuite_packages/xboinc/examples/003_boinc/xboinc_executable.exe projects/test.test/xboinc_executable\n```\n\nIn one terminal:\n`cp client_state_save.xml client_state.xml; ./../../Program\\ Files/BOINC/boinc.exe`\n\nIn another:\n`/c/Program\\ Files/BOINC/boincmgr.exe`\n\nIn case of problems stop boing client in the status bar:\n\n<img width="427" alt="image" src="https://user-images.githubusercontent.com/8049893/191972091-13fee31a-9dc8-459e-9f3f-3224c09bec47.png">\n\nYou can suspend using the activity menu:\n\n<img width="785" alt="image" src="https://user-images.githubusercontent.com/8049893/191973210-64e0c156-9565-41d9-9e8c-8e5eeef19b2b.png">\n\nYou can see the checkpoints in:\n\n<img width="835" alt="image" src="https://user-images.githubusercontent.com/8049893/191973307-498ce522-7542-4975-9e18-702bf449abd3.png">\n\nYou can restart from the same menu. \n\n\nWhen the job is finished, the result are saved in "projects/test.test/output.bin"\n\n\n## INSTRUCTIONS FOR UBUNTU:\n\n### How to install boinc client/manager on Ubuntu\nhttps://boinc.berkeley.edu/wiki/Installing_BOINC_on_Ubuntu\n\nBasically only:\n```\nsudo apt-get install aptitude\nsudo aptitude install boinc-client boinc-manager\n```\n#### Compile boinc api and examples from source on Ubuntu\n\nOn a fresh ubuntu installation I neede to:\n\n```\nsudo apt install make\nsudo apt install m4\nsudo apt install pkg-config\nsudo apt install autoconf\nsudo apt install libtool\nsudo apt install g++\n```\n\n```\ncd\ngit clone https://github.com/BOINC/boinc\ncd boinc\nexport BOINC_DIR=$PWD\n./_autosetup\n```\nFrom \nhttps://boinc.berkeley.edu/trac/wiki/BuildSystem\n\n"If you\'re developing or porting a BOINC application, you need only the API: "\n```\n./configure --disable-server --disable-client --disable-manager --disable-gui\n# This one takes very long\n```\nand then\n```\nmake\n# This also takes quite long\n```\n\n### Installing xsuite packages\n```\ncd\nwget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh\nbash Miniconda3-latest-Linux-x86_64.sh\nsource miniconda3/bin/activate\npip install numpy scipy matplotlib pandas ipython pytest\nmkdir xsuite_packages\ncd xsuite_packages\n\ngit clone https://github.com/xsuite/xobjects\ngit clone https://github.com/xsuite/xdeps\ngit clone https://github.com/xsuite/xpart\ngit clone https://github.com/xsuite/xtrack\ngit clone https://github.com/xsuite/xfields\ngit clone https://github.com/xsuite/xboinc\n\npip install -e xobjects\npip install -e xdeps\npip install -e xpart\npip install -e xtrack\npip install -e xfields\npip install -e xboinc\n```\n\n#### Compile and generate input\n\n```bash\ncd xboinc/examples/000_build_executable\npython 000_build_executable.py\nbash 001msys2_compile_executable.sh\ncd ../002_lhc\npython 001_build_input.py\ncd ../003_boinc\necho $BOINC_DIR # Check if points into the BOINC source directory \npython 000_build_executable.py\nmake\n```\n\n#### Run/test the executable\n```\ncp ../002_lhc/xboinc_input.bin .\nchmod +x xboinc_executable\n./xboinc_executable\n```\n\n### Running the test application with boinc server\n```\ncd\nmkdir xboinc_test\ncp ~/xsuite_packages/xboinc/examples/003_boinc/client_state_save.xml .\n```\nthen\n\n```\nvim account_test.xml \n```\n\nwrite\n```\n<account>\n    <master_url>http://test.test</master_url>\n    <project_name>test_project</project_name>\n</account>\n```\nthen \n```vim cc_config.xml```\nwrite\n```\n<cc_config>\n    <options>\n        <skip_cpu_benchmarks/>\n        <unsigned_apps_ok/>\n    </options>\n</cc_config>\n```\n\nAdd the same GUI RPC passwords in\n```\nvim gui_rpc_auth.cfg\n```\nand in\n```\nvim /etc/boinc-client/gui_rpc_auth.cfg\n```\n\nThen make folder structure\n```\nmkdir projects/test.test\ncp ~/xsuite_packages/xboinc/examples/002_lhc/xboinc_input.bin projects/test.test/input.bin\ncp ~/xsuite_packages/xboinc/examples/003_boinc/xboinc_executable.exe projects/test.test/xboinc_executable\n```\n\nIn one terminal:\n`cp client_state_save.xml client_state.xml; boinc --gui_rpc_port 31417`\n\nIn another:\n`boincmgr --gui_rpc_port 31417`\n\n!! Before running BOINC client or manager, kill the previous BOINC session\n```\nsudo /etc/init.d/boinc-client stop\n```\n',
     'author': 'Frederik F. Van der Veken',
     'author_email': 'frederik@cern.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/xsuite/xboinc',
```

### Comparing `xboinc-0.0.2/PKG-INFO` & `xboinc-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xboinc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Xsuite BOINC interface
 Home-page: https://github.com/xsuite/xboinc
 License: Apache 2.0
 Author: Frederik F. Van der Veken
 Author-email: frederik@cern.ch
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
```

