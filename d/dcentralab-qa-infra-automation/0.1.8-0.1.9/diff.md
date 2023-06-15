# Comparing `tmp/dcentralab_qa_infra_automation-0.1.8.tar.gz` & `tmp/dcentralab_qa_infra_automation-0.1.9.tar.gz`

## Comparing `dcentralab_qa_infra_automation-0.1.8.tar` & `dcentralab_qa_infra_automation-0.1.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/vcs.xml
--rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/BasePage.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
--rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/vcs.xml
+-rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/BasePage.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.9/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-0.1.8/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.1.9/.idea/workspace.xml`

 * *Files 6% similar despite different names*

#### Comparing `dcentralab_qa_infra_automation-0.1.8/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.1.9/.idea/workspace.xml`

```diff
@@ -24,14 +24,15 @@
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/Loggers.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/Loggers.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriverWithMetamaskExtension.py" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/seleniumPythonFramework_VeriSoft/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
```

### Comparing `dcentralab_qa_infra_automation-0.1.8/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-0.1.9/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,23 +33,25 @@
     # Returns JSON object as a dictionary
     tokens = json.load(f)
     # Store the data in pytest global variables
     pytest.tokens = tokens
     # Closing file
     f.close()
 
-    # Init farms JSON data
-    # Opening farms JSON file
-    f = open(pytest.user_dir + '/testsData/farms.json')
-    # Returns JSON object as a dictionary
-    farms_data = json.load(f)
-    # Store the data in pytest global variables
-    pytest.farms_data = farms_data
-    # Closing file
-    f.close()
+    # Init farms file only in tokensfarm project
+    if "tokensfarm" in pytest.user_dir:
+        # Init farms JSON data
+        # Opening farms JSON file
+        f = open(pytest.user_dir + '/testsData/farms.json')
+        # Returns JSON object as a dictionary
+        farms_data = json.load(f)
+        # Store the data in pytest global variables
+        pytest.farms_data = farms_data
+        # Closing file
+        f.close()
 
     # Init wallets JSON data
     # Opening wallets JSON file
     f = open(pytest.user_dir + '/testsData/wallets.json')
     # Returns JSON object as a dictionary
     wallets_data = json.load(f)
     # Store the data in pytest global variables
```

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
 confirm coinbase wallet page
 
 @Author: Efrat Cohen
 @Date: 08.2023
```

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,9 +34,9 @@
         """
         self.enter_text(ENTER_WORD_SEED_PHRASE, pytest.wallets_data.get("secret_recovery_phrase"))
 
     def click_on_import_wallet(self):
         """
         click on import wallet
         """
-        self.click(IMPORT_WALLET_BUTTON)
+        self.click("IMPORT_WALLET_BUTTON", IMPORT_WALLET_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py` & `dcentralab_qa_infra_automation-0.1.9/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/LICENSE` & `dcentralab_qa_infra_automation-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.8/pyproject.toml` & `dcentralab_qa_infra_automation-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-0.1.8/PKG-INFO` & `dcentralab_qa_infra_automation-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 0.1.8
+Version: 0.1.9
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

