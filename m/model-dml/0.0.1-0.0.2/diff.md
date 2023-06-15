# Comparing `tmp/model_dml-0.0.1.tar.gz` & `tmp/model_dml-0.0.2.tar.gz`

## Comparing `model_dml-0.0.1.tar` & `model_dml-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 model_dml-0.0.1/.flake8
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 model_dml-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 model_dml-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 model_dml-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 model_dml-0.0.1/build_requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 model_dml-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 model_dml-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 model_dml-0.0.1/.idea/modml.iml
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 model_dml-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 model_dml-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 model_dml-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 model_dml-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 model_dml-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 model_dml-0.0.1/src/model_dml/__init__.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 model_dml-0.0.1/src/model_dml/dml.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 model_dml-0.0.1/src/model_dml/py.typed
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 model_dml-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 model_dml-0.0.1/tests/test_main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 model_dml-0.0.1/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 model_dml-0.0.1/AUTHORS.rst
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 model_dml-0.0.1/LICENCE
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 model_dml-0.0.1/README.md
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 model_dml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 model_dml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 model_dml-0.0.2/.flake8
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 model_dml-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 model_dml-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 model_dml-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 model_dml-0.0.2/build_requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/modml.iml
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    13128 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 model_dml-0.0.2/src/model_dml/__init__.py
+-rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 model_dml-0.0.2/src/model_dml/dml.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 model_dml-0.0.2/src/model_dml/py.typed
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 model_dml-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 model_dml-0.0.2/tests/test_main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 model_dml-0.0.2/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 model_dml-0.0.2/AUTHORS.rst
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 model_dml-0.0.2/LICENCE
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 model_dml-0.0.2/README.md
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 model_dml-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 model_dml-0.0.2/PKG-INFO
```

### Comparing `model_dml-0.0.1/.gitlab-ci.yml` & `model_dml-0.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.1/CONTRIBUTING.md` & `model_dml-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.1/.idea/workspace.xml` & `model_dml-0.0.2/.idea/workspace.xml`

 * *Files 18% similar despite different names*

#### Comparing `model_dml-0.0.1/.idea/workspace.xml` & `model_dml-0.0.2/.idea/workspace.xml`

```diff
@@ -1,25 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="9719a552-d9bf-49c2-8d5a-a1017e61da6c" name="Changes" comment="add py.typed">
-      <change afterPath="$PROJECT_DIR$/src/model_ml/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/.gitlab-ci.yml" beforeDir="false" afterPath="$PROJECT_DIR$/.gitlab-ci.yml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/CONTRIBUTING.md" beforeDir="false" afterPath="$PROJECT_DIR$/CONTRIBUTING.md" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/modml/__init__.py" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/modml/dml.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/model_ml/dml.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/modml/py.typed" beforeDir="false" afterPath="$PROJECT_DIR$/src/model_ml/py.typed" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/conftest.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/conftest.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/test_main.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_main.py" afterDir="false"/>
-    </list>
+    <list default="true" id="9719a552-d9bf-49c2-8d5a-a1017e61da6c" name="Changes" comment="refactoring
+
+style
+better patterns"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="ChangesViewManager">
     <option name="groupingKeys">
@@ -40,28 +32,34 @@
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2QWFWRRpPhcbDZybVWHB99EabuE"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "WebServerToolWindowFactoryState": "false",
-    "git-widget-placeholder": "main",
-    "last_opened_file_path": "/home/dturba/PycharmProjects/modml/tests",
-    "node.js.detected.package.eslint": "true",
-    "node.js.detected.package.tslint": "true",
-    "node.js.selected.package.eslint": "(autodetect)",
-    "node.js.selected.package.tslint": "(autodetect)",
-    "nodejs_package_manager_path": "npm",
-    "vue.rearranger.settings.migration": "true"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;WebServerToolWindowFactoryState&quot;: &quot;false&quot;,
+    &quot;git-widget-placeholder&quot;: &quot;main&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/home/dturba/PycharmProjects/modml&quot;,
+    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
+    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
+    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
+    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;,
+    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;project.propVCSSupport.DirectoryMappings&quot;,
+    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
+  },
+  &quot;keyToStringList&quot;: {
+    &quot;com.intellij.ide.scratch.ScratchImplUtil$2/New Scratch File&quot;: [
+      &quot;Python&quot;
+    ]
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$"/>
     </key>
   </component>
   <component name="RunManager" selected="Python tests.pytest in modml">
     <configuration name="main" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
@@ -82,14 +80,59 @@
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
+    <configuration name="scratch_17" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+      <module name="modml"/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <envs>
+        <env name="PYTHONUNBUFFERED" value="1"/>
+      </envs>
+      <option name="SDK_HOME" value="$PROJECT_DIR$/venv/bin/python"/>
+      <option name="SDK_NAME" value="Python 3.11 (modml)"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
+      <option name="IS_MODULE_SDK" value="false"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
+      <option name="SCRIPT_NAME" value="$APPLICATION_CONFIG_DIR$/scratches/scratch_17.py"/>
+      <option name="PARAMETERS" value=""/>
+      <option name="SHOW_COMMAND_LINE" value="false"/>
+      <option name="EMULATE_TERMINAL" value="false"/>
+      <option name="MODULE_MODE" value="false"/>
+      <option name="REDIRECT_INPUT" value="false"/>
+      <option name="INPUT_FILE" value=""/>
+      <method v="2"/>
+    </configuration>
+    <configuration name="scratch_18" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+      <module name="modml"/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <envs>
+        <env name="PYTHONUNBUFFERED" value="1"/>
+      </envs>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$APPLICATION_CONFIG_DIR$/scratches"/>
+      <option name="IS_MODULE_SDK" value="false"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
+      <option name="SCRIPT_NAME" value="$APPLICATION_CONFIG_DIR$/scratches/scratch_18.py"/>
+      <option name="PARAMETERS" value=""/>
+      <option name="SHOW_COMMAND_LINE" value="false"/>
+      <option name="EMULATE_TERMINAL" value="false"/>
+      <option name="MODULE_MODE" value="false"/>
+      <option name="REDIRECT_INPUT" value="false"/>
+      <option name="INPUT_FILE" value=""/>
+      <method v="2"/>
+    </configuration>
     <configuration name="pytest in modml" type="tests" factoryName="py.test" nameIsGenerated="true">
       <module name="modml"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value="$PROJECT_DIR$/venv/bin/python"/>
       <option name="SDK_NAME" value="Python 3.11 (modml)"/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
@@ -102,30 +145,41 @@
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;$PROJECT_DIR$&quot;"/>
       <option name="_new_targetType" value="&quot;PATH&quot;"/>
       <method v="2"/>
     </configuration>
     <list>
       <item itemvalue="Python.main"/>
+      <item itemvalue="Python.scratch_18"/>
+      <item itemvalue="Python.scratch_17"/>
       <item itemvalue="Python tests.pytest in modml"/>
     </list>
+    <recent_temporary>
+      <list>
+        <item itemvalue="Python.scratch_18"/>
+        <item itemvalue="Python.scratch_17"/>
+      </list>
+    </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="9719a552-d9bf-49c2-8d5a-a1017e61da6c" name="Changes" comment=""/>
       <created>1685461462049</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1685461462049</updated>
       <workItem from="1685461464247" duration="1101000"/>
       <workItem from="1685462663359" duration="5550000"/>
       <workItem from="1685603428109" duration="2499000"/>
       <workItem from="1685606118080" duration="1090000"/>
-      <workItem from="1685614943201" duration="989000"/>
+      <workItem from="1685614943201" duration="1308000"/>
+      <workItem from="1685628682946" duration="3814000"/>
+      <workItem from="1685690462755" duration="2044000"/>
+      <workItem from="1685941744569" duration="14000"/>
     </task>
     <task id="LOCAL-00001" summary="first commit">
       <created>1685476645393</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1685476645393</updated>
@@ -163,15 +217,32 @@
     <task id="LOCAL-00006" summary="add py.typed">
       <created>1685606400665</created>
       <option name="number" value="00006"/>
       <option name="presentableId" value="LOCAL-00006"/>
       <option name="project" value="LOCAL"/>
       <updated>1685606400665</updated>
     </task>
-    <option name="localTasksCounter" value="7"/>
+    <task id="LOCAL-00007" summary="change project name from modml to model_dml">
+      <created>1685616137914</created>
+      <option name="number" value="00007"/>
+      <option name="presentableId" value="LOCAL-00007"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1685616137914</updated>
+    </task>
+    <task id="LOCAL-00008" summary="refactoring
+
+style
+better patterns">
+      <created>1685693425612</created>
+      <option name="number" value="00008"/>
+      <option name="presentableId" value="LOCAL-00008"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1685693425612</updated>
+    </task>
+    <option name="localTasksCounter" value="9"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -189,13 +260,23 @@
     <MESSAGE value="update README.md"/>
     <MESSAGE value="fix README.md indentation"/>
     <MESSAGE value="fix mypy python_version pyproject.toml config"/>
     <MESSAGE value="update .gitlab-ci.yml
 
 Add run CI when pyproject.toml is changed"/>
     <MESSAGE value="add py.typed"/>
-    <option name="LAST_COMMIT_MESSAGE" value="add py.typed"/>
+    <MESSAGE value="change project name from modml to model_dml"/>
+    <MESSAGE value="refactoring
+
+style
+better patterns"/>
+    <option name="LAST_COMMIT_MESSAGE" value="refactoring
+
+style
+better patterns"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
-    <SUITE FILE_PATH="coverage/modml$pytest_in_modml.coverage" NAME="pytest in modml Coverage Results" MODIFIED="1685615845439" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/modml$pytest_in_modml.coverage" NAME="pytest in modml Coverage Results" MODIFIED="1685693371429" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/modml$scratch_18.coverage" NAME="scratch_18 Coverage Results" MODIFIED="1685692634853" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$APPLICATION_CONFIG_DIR$/scratches"/>
+    <SUITE FILE_PATH="coverage/modml$scratch_17.coverage" NAME="scratch_17 Coverage Results" MODIFIED="1685660010224" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
   </component>
 </project>
```

### Comparing `model_dml-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `model_dml-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.1/src/model_dml/dml.py` & `model_dml-0.0.2/src/model_dml/dml.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,118 +38,93 @@
             session.execute(stmt, values)
 
     @classmethod
     def _insert_returning_result(
         cls,
         values: AnyExecuteParams,
         returning: typing.Sequence[COLUMNS_CLAUSE_ARGUMENT] = (),
-    ) -> sqlalchemy.Result[COLUMNS_CLAUSE_ARGUMENT]:
+    ) -> sqlalchemy.Result[typing.Any]:
         stmt = sqlalchemy.insert(cls).returning(*returning)
         with cls.session_maker().begin() as session:
             result = session.execute(stmt, values)
         return result
 
     @classmethod
     def _insert_returning_scalar(
         cls,
         values: AnyExecuteParams,
         returning: typing.Sequence[COLUMNS_CLAUSE_ARGUMENT] = (),
-    ) -> sqlalchemy.ScalarResult[COLUMNS_CLAUSE_ARGUMENT]:
+    ) -> sqlalchemy.ScalarResult[typing.Any]:
         stmt = sqlalchemy.insert(cls).returning(*returning)
         with cls.session_maker().begin() as session:
             result = session.scalars(stmt, values)
         return result
 
     @classmethod
     def insert(
         cls,
         values: AnyExecuteParams,
         returning: typing.Sequence[COLUMNS_CLAUSE_ARGUMENT] = (),
-    ) -> typing.Union[
-        sqlalchemy.ScalarResult[COLUMNS_CLAUSE_ARGUMENT],
-        sqlalchemy.Result[COLUMNS_CLAUSE_ARGUMENT],
-        None,
-    ]:
+    ) -> typing.Union[sqlalchemy.ScalarResult[typing.Any], sqlalchemy.Result[typing.Any], None,]:
         match returning:
             case [one, two, *more]:
                 return cls._insert_returning_result(values, [one, two, *more])
-            case [one, *more]:
-                return cls._insert_returning_scalar(values, [one, *more])
+            case [one]:
+                return cls._insert_returning_scalar(values, [one])
             case _:
                 return cls._insert_no_returning(values)
 
 
 class Update(SessionMakerMixin):
     @classmethod
     def _update_no_returning(
         cls,
         where: typing.Sequence[sqlalchemy.ColumnExpressionArgument[bool]],
         values: AnyExecuteParams,
     ) -> None:
         stmt = sqlalchemy.update(cls).where(*where)
         with cls.session_maker().begin() as session:
-            session.execute(
-                stmt,
-                values,
-            )
+            session.execute(stmt, values)
 
     @classmethod
     def _update_returning_scalar(
         cls,
         where: typing.Sequence[sqlalchemy.ColumnExpressionArgument[bool]],
         values: AnyExecuteParams,
         returning: typing.Sequence[COLUMNS_CLAUSE_ARGUMENT],
-    ) -> sqlalchemy.ScalarResult[COLUMNS_CLAUSE_ARGUMENT]:
+    ) -> sqlalchemy.ScalarResult[typing.Any]:
         stmt = sqlalchemy.update(cls).where(*where).returning(*returning)
         with cls.session_maker().begin() as session:
-            result = session.scalars(
-                stmt,
-                values,
-            )
+            result = session.scalars(stmt, values)
         return result
 
     @classmethod
     def _update_returning_result(
         cls,
         where: typing.Sequence[sqlalchemy.ColumnExpressionArgument[bool]],
         values: AnyExecuteParams,
         returning: typing.Sequence[COLUMNS_CLAUSE_ARGUMENT],
-    ) -> sqlalchemy.Result[COLUMNS_CLAUSE_ARGUMENT]:
+    ) -> sqlalchemy.Result[typing.Any]:
         stmt = sqlalchemy.update(cls).where(*where).returning(*returning)
         with cls.session_maker().begin() as session:
-            result = session.execute(
-                stmt,
-                values,
-            )
+            result = session.execute(stmt, values)
         return result
 
     @classmethod
     def update(
         cls,
         where: typing.Sequence[sqlalchemy.ColumnExpressionArgument[bool]],
         values: AnyExecuteParams,
         returning: typing.Sequence[COLUMNS_CLAUSE_ARGUMENT] = (),
-    ) -> typing.Union[
-        sqlalchemy.ScalarResult[COLUMNS_CLAUSE_ARGUMENT],
-        sqlalchemy.Result[COLUMNS_CLAUSE_ARGUMENT],
-        None,
-    ]:
+    ) -> typing.Union[sqlalchemy.ScalarResult[typing.Any], sqlalchemy.Result[typing.Any], None,]:
         match returning:
             case [one, two, *more]:
                 return cls._update_returning_result(where, values, [one, two, *more])
-            case [
-                one,
-            ]:
-                return cls._update_returning_scalar(
-                    where,
-                    values,
-                    [
-                        one,
-                    ],
-                )
+            case [one]:
+                return cls._update_returning_scalar(where, values, [one])
             case _:
                 return cls._update_no_returning(where, values)
 
 
 class Delete(SessionMakerMixin):
     @classmethod
     def _delete_no_returning(
@@ -161,50 +136,46 @@
             session.execute(stmt)
 
     @classmethod
     def _delete_returning_scalar(
         cls,
         where: typing.Sequence[sqlalchemy.ColumnExpressionArgument[bool]],
         returning: typing.Sequence[COLUMNS_CLAUSE_ARGUMENT] = (),
-    ) -> sqlalchemy.ScalarResult[COLUMNS_CLAUSE_ARGUMENT]:
+    ) -> sqlalchemy.ScalarResult[typing.Any]:
         stmt = sqlalchemy.delete(cls).where(*where).returning(*returning)
         with cls.session_maker().begin() as session:
             result = session.scalars(stmt)
         return result
 
     @classmethod
     def _delete_returning_result(
         cls,
         where: typing.Sequence[sqlalchemy.ColumnExpressionArgument[bool]],
         returning: typing.Sequence[COLUMNS_CLAUSE_ARGUMENT] = (),
-    ) -> sqlalchemy.Result[COLUMNS_CLAUSE_ARGUMENT]:
+    ) -> sqlalchemy.Result[typing.Any]:
         stmt = sqlalchemy.delete(cls).where(*where).returning(*returning)
         with cls.session_maker().begin() as session:
             result = session.execute(stmt)
         return result
 
     @classmethod
     def delete(
         cls,
         where: typing.Sequence[sqlalchemy.ColumnExpressionArgument[bool]],
         returning: typing.Sequence[COLUMNS_CLAUSE_ARGUMENT] = (),
-    ) -> typing.Union[
-        sqlalchemy.ScalarResult[COLUMNS_CLAUSE_ARGUMENT],
-        sqlalchemy.Result[COLUMNS_CLAUSE_ARGUMENT],
-        None,
-    ]:
+    ) -> typing.Union[sqlalchemy.ScalarResult[typing.Any], sqlalchemy.Result[typing.Any], None,]:
         """
         :param where: filters affected row, send empty sequence to affect all rows explicitly
         :param returning: select returned columns, leave empty or send empty sequence for no return
             values, if only one value is provided, result will be scalar
         """
         match returning:
             case [one, two, *more]:
                 return cls._delete_returning_result(where, [one, two, *more])
-            case [one, *more]:
-                return cls._delete_returning_scalar(where, [one, *more])
+            case [one]:
+                return cls._delete_returning_scalar(where, [one])
             case _:
                 return cls._delete_no_returning(where)
 
 
 class DML(Insert, Update, Delete):
     """helper class that package all dml method implementations insert, update and delete"""
```

### Comparing `model_dml-0.0.1/tests/conftest.py` & `model_dml-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.1/tests/test_main.py` & `model_dml-0.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.1/.gitignore` & `model_dml-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.1/LICENCE` & `model_dml-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.1/README.md` & `model_dml-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,14 @@
     id: sqlalchemy.orm.Mapped[int] = sqlalchemy.orm.mapped_column(primary_key=True)
     name: sqlalchemy.orm.Mapped[str] = sqlalchemy.orm.mapped_column(sqlalchemy.String(30))
 ```
 
 ### Use the DML methods
 
 ```python
-user = User.insert(dict(name="John"))
-user = User.insert({'name': "Jane"})
+User.insert(dict(name="John"))
+User.insert({'name': "Jane"})
 user = User.insert({'name': "Jack"}, returning=[User.id, User.name])
 ```
 
 [Using a sessionmaker]: https://docs.sqlalchemy.org/en/20/orm/session_basics.html#using-a-sessionmaker
 [sessionmaker documentation and example]: https://docs.sqlalchemy.org/en/20/orm/session_api.html#sqlalchemy.orm.sessionmaker
```

### Comparing `model_dml-0.0.1/pyproject.toml` & `model_dml-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "model_dml"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Dorian Turba", email = "contact.5oldw@8shield.net" },
 ]
 description = "A package for SQLAlchemy models DML mixins."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `model_dml-0.0.1/PKG-INFO` & `model_dml-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model_dml
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for SQLAlchemy models DML mixins.
 Project-URL: Homepage, https://lab.frogg.it/dorianturba/model_dml
 Project-URL: Bug Tracker, https://lab.frogg.it/dorianturba/model_dml
 Author-email: Dorian Turba <contact.5oldw@8shield.net>
 License-File: AUTHORS.rst
 License-File: LICENCE
 Classifier: Development Status :: 3 - Alpha
@@ -99,14 +99,14 @@
     id: sqlalchemy.orm.Mapped[int] = sqlalchemy.orm.mapped_column(primary_key=True)
     name: sqlalchemy.orm.Mapped[str] = sqlalchemy.orm.mapped_column(sqlalchemy.String(30))
 ```
 
 ### Use the DML methods
 
 ```python
-user = User.insert(dict(name="John"))
-user = User.insert({'name': "Jane"})
+User.insert(dict(name="John"))
+User.insert({'name': "Jane"})
 user = User.insert({'name': "Jack"}, returning=[User.id, User.name])
 ```
 
 [Using a sessionmaker]: https://docs.sqlalchemy.org/en/20/orm/session_basics.html#using-a-sessionmaker
 [sessionmaker documentation and example]: https://docs.sqlalchemy.org/en/20/orm/session_api.html#sqlalchemy.orm.sessionmaker
```

