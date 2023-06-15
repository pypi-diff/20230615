# Comparing `tmp/dcentralab_qa_infra_automation-0.1.9.tar.gz` & `tmp/dcentralab_qa_infra_automation-0.2.0.tar.gz`

## Comparing `dcentralab_qa_infra_automation-0.1.9.tar` & `dcentralab_qa_infra_automation-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/vcs.xml
--rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/BasePage.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
--rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/.idea/vcs.xml
+-rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/BasePage.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.2.0/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.2.0/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-0.2.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/BasePage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/BasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,32 +20,32 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
-        return self.is_element_exist(GOT_IT_BUTTON)
+        return self.is_element_exist("GOT_IT_BUTTON", GOT_IT_BUTTON)
 
     def is_confirm_button_exist(self):
         """
         check is confirm button exist
         """
-        return self.is_element_exist(CONFIRM_BUTTON)
+        return self.is_element_exist("CONFIRM_BUTTON", CONFIRM_BUTTON)
 
     def click_on_confirm_button(self):
         """
         click on confirm button
         """
-        self.click(CONFIRM_BUTTON)
+        self.click("CONFIRM_BUTTON", CONFIRM_BUTTON)
 
     def is_got_it_button_exist(self):
         """
         check is confirm button exist
         """
-        return self.is_element_exist(GOT_IT_BUTTON)
+        return self.is_element_exist("GOT_IT_BUTTON", GOT_IT_BUTTON)
 
     def click_on_got_it_button(self):
         """
         click on confirm button
         """
-        self.click(GOT_IT_BUTTON)
+        self.click("GOT_IT_BUTTON", GOT_IT_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,20 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         @return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
     def click_on_confirm_button(self):
         """
         click on confirm button
         """
         try:
             self.is_element_exist_with_custom_timeout(CONFIRM_BUTTON, pytest.properties.get("timeout") / 10)
-            self.click(CONFIRM_BUTTON)
+            self.click("CONFIRM_BUTTON", CONFIRM_BUTTON)
         except:
             # Close chrome extension popup
             self.driver.close()
             pytest.logger.info("coinbase wallet already connected")
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,14 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         @return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
     def click_on_connect_button(self):
         """
         click on connect button
         """
-        self.click(CONNECT_BUTTON)
+        self.click("CONNECT_BUTTON", CONNECT_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,33 +24,33 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         @return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
     def insert_password(self):
         """
         insert password
         """
-        self.enter_text(PASSWORD_INPUT, pytest.wallets_data.get("coinbase_password"))
+        self.enter_text("PASSWORD_INPUT", PASSWORD_INPUT, pytest.wallets_data.get("coinbase_password"))
 
     def verify_password(self):
         """
         verify password
         """
-        self.enter_text(VERIFY_PASSWORD_INPUT, pytest.wallets_data.get("coinbase_password"))
+        self.enter_text("VERIFY_PASSWORD_INPUT", VERIFY_PASSWORD_INPUT, pytest.wallets_data.get("coinbase_password"))
 
     def click_on_agree_terms_checkbox(self):
         """
         click on agree terms checkbox
         """
-        self.click(AGREE_TERMS_CHECKBOX)
+        self.click("AGREE_TERMS_CHECKBOX", AGREE_TERMS_CHECKBOX)
 
     def click_on_submit(self):
         """
         click on submit
         """
-        self.click(SUBMIT_BUTTON)
+        self.click("SUBMIT_BUTTON", SUBMIT_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,14 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         @return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
     def click_on_already_have_a_wallet(self):
         """
         click on already have a wallet
         """
-        self.click(ALREADY_HAVE_WALLET_LINK)
+        self.click("ALREADY_HAVE_WALLET_LINK", ALREADY_HAVE_WALLET_LINK)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         @return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
     def insert_recovery_phrase(self):
         """
         enter recovery phrase
         """
-        self.enter_text(ENTER_WORD_SEED_PHRASE, pytest.wallets_data.get("secret_recovery_phrase"))
+        self.enter_text("ENTER_WORD_SEED_PHRASE", ENTER_WORD_SEED_PHRASE, pytest.wallets_data.get("secret_recovery_phrase"))
 
     def click_on_import_wallet(self):
         """
         click on import wallet
         """
         self.click("IMPORT_WALLET_BUTTON", IMPORT_WALLET_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
-receive crypto to your username page
+welcome to metamask page
 
 @Author: Efrat Cohen
-@Date: 02.2023
+@Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(text(),'Receive crypto to your username')]")
-DENY_BUTTON = (By.XPATH, "//*[contains(text(),'Deny')]")
+TITLE = (By.XPATH, "//*[contains(text(),'Welcome to MetaMask')]")
+GET_STARTED_BUTTON = (By.XPATH, "//*[contains(text(),'Get started')]")
+CONNECT_WALLET_POPUP = (By.XPATH, "//*[contains(@class,'permissions-connect-header__title')]")
 
 
-class ReceiveCryptoToUsernamePage(BasePage):
+class WelcomeToMetamaskPage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
-        @return: true if on page, otherwise return false
+        :return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
-    def click_on_deny(self):
-        self.click(DENY_BUTTON)
+    def click_on_get_started(self):
+        """
+        click on get started button
+        """
+        self.click("GET_STARTED_BUTTON", GET_STARTED_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,14 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         @return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
     def click_on_enter_recovery_phrase(self):
         """
         click on enter recovery phrase
         """
-        self.click(ENTER_RECOVERY_PHRASE)
+        self.click("ENTER_RECOVERY_PHRASE", ENTER_RECOVERY_PHRASE)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,20 +19,20 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
-        return self.is_element_exist(CONFIRM_BUTTON)
+        return self.is_element_exist("CONFIRM_BUTTON", CONFIRM_BUTTON)
 
     def is_confirm_button_exist(self):
         """
         check is confirm button exist
         """
-        return self.is_element_exist(CONFIRM_BUTTON)
+        return self.is_element_exist("CONFIRM_BUTTON", CONFIRM_BUTTON)
 
     def click_on_confirm_button(self):
         """
         click on confirm button
         """
-        self.click(CONFIRM_BUTTON)
+        self.click("CONFIRM_BUTTON", CONFIRM_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,14 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
     def click_on_all_done(self):
         """
         click on all done button
         """
-        self.click(ALL_DONE_BUTTON)
+        self.click("ALL_DONE_BUTTON", ALL_DONE_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,20 +21,20 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
     def click_on_next_button(self):
         """
         click on next button
         """
-        self.click(NEXT_BUTTON)
+        self.click("NEXT_BUTTON", NEXT_BUTTON)
 
     def click_on_connect_button(self):
         """
         click on connect button
         """
-        self.click(CONNECT_BUTTON)
+        self.click("CONNECT_BUTTON", CONNECT_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py`

 * *Files 25% similar despite different names*

```diff
@@ -36,49 +36,49 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
     def insert_secret_recovery_phrase(self):
         """
         insert secret recovery phrase
         """
-        self.enter_text(SECRET_RECOVERY_PHRASE_0, pytest.wallets_data.get("secret_recovery_phrase_0"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_1, pytest.wallets_data.get("secret_recovery_phrase_1"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_2, pytest.wallets_data.get("secret_recovery_phrase_2"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_3, pytest.wallets_data.get("secret_recovery_phrase_3"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_4, pytest.wallets_data.get("secret_recovery_phrase_4"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_5, pytest.wallets_data.get("secret_recovery_phrase_5"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_6, pytest.wallets_data.get("secret_recovery_phrase_6"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_7, pytest.wallets_data.get("secret_recovery_phrase_7"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_8, pytest.wallets_data.get("secret_recovery_phrase_8"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_9, pytest.wallets_data.get("secret_recovery_phrase_9"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_10, pytest.wallets_data.get("secret_recovery_phrase_10"))
-        self.enter_text(SECRET_RECOVERY_PHRASE_11, pytest.wallets_data.get("secret_recovery_phrase_11"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_0", SECRET_RECOVERY_PHRASE_0, pytest.wallets_data.get("secret_recovery_phrase_0"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_1", SECRET_RECOVERY_PHRASE_1, pytest.wallets_data.get("secret_recovery_phrase_1"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_2", SECRET_RECOVERY_PHRASE_2, pytest.wallets_data.get("secret_recovery_phrase_2"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_3", SECRET_RECOVERY_PHRASE_3, pytest.wallets_data.get("secret_recovery_phrase_3"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_4", SECRET_RECOVERY_PHRASE_4, pytest.wallets_data.get("secret_recovery_phrase_4"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_5", SECRET_RECOVERY_PHRASE_5, pytest.wallets_data.get("secret_recovery_phrase_5"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_6", SECRET_RECOVERY_PHRASE_6, pytest.wallets_data.get("secret_recovery_phrase_6"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_7", SECRET_RECOVERY_PHRASE_7, pytest.wallets_data.get("secret_recovery_phrase_7"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_8", SECRET_RECOVERY_PHRASE_8, pytest.wallets_data.get("secret_recovery_phrase_8"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_9", SECRET_RECOVERY_PHRASE_9, pytest.wallets_data.get("secret_recovery_phrase_9"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_10", SECRET_RECOVERY_PHRASE_10, pytest.wallets_data.get("secret_recovery_phrase_10"))
+        self.enter_text("SECRET_RECOVERY_PHRASE_11", SECRET_RECOVERY_PHRASE_11, pytest.wallets_data.get("secret_recovery_phrase_11"))
 
     def insert_password(self):
         """
         insert password
         """
-        self.enter_text(PASSWORD_INPUT, pytest.wallets_data.get("password"))
+        self.enter_text("PASSWORD_INPUT", PASSWORD_INPUT, pytest.wallets_data.get("password"))
 
     def insert_confirm_password(self):
         """
         insert confirm password
         """
-        self.enter_text(CONFIRM_PASSWORD_INPUT, pytest.wallets_data.get("password"))
+        self.enter_text("CONFIRM_PASSWORD_INPUT", CONFIRM_PASSWORD_INPUT, pytest.wallets_data.get("password"))
 
     def agree_terms_of_use(self):
         """
         click on agree terms of use checkbox
         """
-        self.click(AGREE_TERMS_CHECKBOX)
+        self.click("AGREE_TERMS_CHECKBOX", AGREE_TERMS_CHECKBOX)
 
     def click_on_submit_import_button(self):
         """
         click on import - submit the import form
         """
-        self.click(SUBMIT_IMPORT_BUTTON)
+        self.click("SUBMIT_IMPORT_BUTTON", SUBMIT_IMPORT_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
-improve metamask page
+new to metamask page
 
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(@class,'metametrics-opt-in__title')]")
-I_AGREE_BUTTON = (By.XPATH, "//*[contains(text(),'I agree')]")
+TITLE = (By.XPATH, "//*[contains(@class,'select-action__body-header')]")
+IMPORT_WALLET_BUTTON = (By.XPATH, "//*[contains(text(),'Import wallet')]")
 
 
-class ImproveMetamaskPage(BasePage):
+class NewToMetamaskPage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
-    def click_on_i_agree_button(self):
+    def click_on_import_wallet(self):
         """
-        click on i agree button
+        click on import wallet
         """
-        self.click(I_AGREE_BUTTON)
+        self.click("IMPORT_WALLET_BUTTON", IMPORT_WALLET_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
-new to metamask page
+wallet connected home page
 
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(@class,'select-action__body-header')]")
-IMPORT_WALLET_BUTTON = (By.XPATH, "//*[contains(text(),'Import wallet')]")
+TITLE = (By.XPATH, "//*[contains(@class,'selected-account__name')]")
 
 
-class NewToMetamaskPage(BasePage):
+class WalletConnectedHomePage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
-
-    def click_on_import_wallet(self):
-        """
-        click on import wallet
-        """
-        self.click(IMPORT_WALLET_BUTTON)
+        return self.is_element_exist("TITLE", TITLE)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,14 @@
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
 
     def click_on_switch_network(self):
         """
         click on switch network button
         """
-        self.click(SWITCH_NETWORK_BUTTON)
+        self.click("SWITCH_NETWORK_BUTTON", SWITCH_NETWORK_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
-wallet connected home page
+receive crypto to your username page
 
 @Author: Efrat Cohen
-@Date: 12.2022
+@Date: 02.2023
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(@class,'selected-account__name')]")
+TITLE = (By.XPATH, "//*[contains(text(),'Receive crypto to your username')]")
+DENY_BUTTON = (By.XPATH, "//*[contains(text(),'Deny')]")
 
 
-class WalletConnectedHomePage(BasePage):
+class ReceiveCryptoToUsernamePage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
-        :return: true if on page, otherwise return false
+        @return: true if on page, otherwise return false
         """
-        return self.is_element_exist(TITLE)
+        return self.is_element_exist("TITLE", TITLE)
+
+    def click_on_deny(self):
+        self.click("DENY_BUTTON", DENY_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py` & `dcentralab_qa_infra_automation-0.2.0/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/LICENSE` & `dcentralab_qa_infra_automation-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.9/pyproject.toml` & `dcentralab_qa_infra_automation-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-0.1.9/PKG-INFO` & `dcentralab_qa_infra_automation-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 0.1.9
+Version: 0.2.0
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

