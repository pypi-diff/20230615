# Comparing `tmp/ipyautoui-0.5.4.tar.gz` & `tmp/ipyautoui-0.5.5.tar.gz`

## Comparing `ipyautoui-0.5.4.tar` & `ipyautoui-0.5.5.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/_dev_sys_path_append.py
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/_utils.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/_utils_debounce.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/_version.py
--rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autodisplay.py
--rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autodisplay_renderers.py
--rw-r--r--   0        0        0    29199 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autoipywidget.py
--rw-r--r--   0        0        0    21750 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/automapschema.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/automapschema.yaml
--rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autoui.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autovjsf.py
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autowidgets.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/basemodel.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/constants.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/env.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/mydocstring_display.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/test_schema.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/vjsf.vue
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/__init__.py
--rw-r--r--   0        0        0    41006 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/autogrid.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/buttonbars.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/decision_branch.py
--rw-r--r--   0        0        0    25595 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/editgrid.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/filechooser.py
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/filesindir.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/fileupload.py
--rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/iterable.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/loadproject.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/markdown_widget.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/modelrun.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/multiselect_search.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/outputlogging.py
--rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/selectdir.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/showhide.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/showopenurl.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/title_description.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/urlimagelink.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/widgetcaller_error.py
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/workingdir.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/complex_serialization.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/core_ipywidgets.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/editable_datagrid.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nested.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/override_ipywidgets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_array.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_array_enum.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_enum.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_simple.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/ruleset.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/LICENSE
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/README.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/_dev_sys_path_append.py
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/_utils.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/_utils_debounce.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/_version.py
+-rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autodisplay.py
+-rw-r--r--   0        0        0    14178 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autodisplay_renderers.py
+-rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autoipywidget.py
+-rw-r--r--   0        0        0    21750 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/automapschema.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/automapschema.yaml
+-rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autoui.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autovjsf.py
+-rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autowidgets.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/basemodel.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/constants.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/env.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/mydocstring_display.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/test_schema.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/vjsf.vue
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/__init__.py
+-rw-r--r--   0        0        0    41006 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/autogrid.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/buttonbars.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/decision_branch.py
+-rw-r--r--   0        0        0    25595 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/editgrid.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/filechooser.py
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/filesindir.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/fileupload.py
+-rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/iterable.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/loadproject.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/markdown_widget.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/modelrun.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/multiselect_search.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/outputlogging.py
+-rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/selectdir.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/selectfrom.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/showhide.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/showopenurl.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/title_description.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/urlimagelink.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/widgetcaller_error.py
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/workingdir.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/complex_serialization.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/core_ipywidgets.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/editable_datagrid.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nested.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/override_ipywidgets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_array.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_array_enum.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_enum.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_simple.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/ruleset.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/LICENSE
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/README.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/PKG-INFO
```

### Comparing `ipyautoui-0.5.4/src/ipyautoui/__init__.py` & `ipyautoui-0.5.5/src/ipyautoui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/_dev_sys_path_append.py` & `ipyautoui-0.5.5/src/ipyautoui/_dev_sys_path_append.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/_utils.py` & `ipyautoui-0.5.5/src/ipyautoui/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,14 +421,15 @@
     """get file extension including compound json files"""
     return "".join(pathlib.Path(fpth).suffixes).lower()
 
 
 def st_mtime_string(path):
     """st_mtime_string for a given path"""
     try:
+        import time
         t = path.stat().st_mtime
         return time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(t))
     except:
         return "####-##-## ##:##:##"
 
 
 def check_installed(package_name):
```

### Comparing `ipyautoui-0.5.4/src/ipyautoui/_utils_debounce.py` & `ipyautoui-0.5.5/src/ipyautoui/_utils_debounce.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/autodisplay.py` & `ipyautoui-0.5.5/src/ipyautoui/autodisplay.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/autodisplay_renderers.py` & `ipyautoui-0.5.5/src/ipyautoui/autodisplay_renderers.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,20 +446,20 @@
     return HTML(
         f"""
 {s}
 """
     )
 
 
-def preview_pdf(path: pathlib.Path):
+def preview_pdf(path: pathlib.Path):  # TODO: facillitate passing kwargs...
     if not isinstance(path, pathlib.PurePath):
         path = pathlib.Path(path)
 
     path = os.path.relpath(path, start=ENV.IPYAUTOUI_ROOTDIR)
-    return IFrame(path, width=1000, height=600)
+    return IFrame(path, width=1000, height=1000)
 
 
 DEFAULT_FILE_RENDERERS = frozenmap(
     **{
         ".csv": preview_csv,
         ".xlsx": PreviewExcel,
         ".json": preview_json,
```

### Comparing `ipyautoui-0.5.4/src/ipyautoui/autoipywidget.py` & `ipyautoui-0.5.5/src/ipyautoui/autoipywidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     wi = ShowHide(
         fn_display=lambda: widget,
         title=label,
         auto_open=auto_open,
         button_width="300px",
     )
     if contains_nullable:
-        return w.HBox([SPACER, wi])
+        return w.HBox([SPACER, wi], layout={"width": "100%"})
     else:
         return wi
 
 
 def add_spacer_to_form_with_nullables(children, widget, contains_nullable):
     if contains_nullable and not isinstance(widget, Nullable):
         children = [SPACER] + children
@@ -198,15 +198,17 @@
     Returns:
         _type_: a widget box that is added to the list of children in AutoObject
     """
     if nested_widgets is None:
         nested_widgets = []
     if align_horizontal:
         if True in [isinstance(widget, w) for w in nested_widgets]:
-            return horizontal_row_nested(widget, label, auto_open=auto_open, contains_nullable=contains_nullable)
+            return horizontal_row_nested(
+                widget, label, auto_open=auto_open, contains_nullable=contains_nullable
+            )
         else:
             return horizontal_row_simple(
                 widget, label, contains_nullable=contains_nullable
             )
     else:
         return vertical_row(widget, label, contains_nullable=contains_nullable)
 
@@ -621,14 +623,24 @@
         self._format_rows()
         if value is not None:
             self.value = value
         else:
             self._value = self.di_widgets_value
         self.savebuttonbar.unsaved_changes = False
 
+    def show_nested(self):
+        for r in self.rows:
+            if isinstance(r, ShowHide):
+                r.show()
+
+    def hide_nested(self):
+        for r in self.rows:
+            if isinstance(r, ShowHide):
+                r.hide()
+
     @property
     def default_order(self):
         try:
             return list(self.di_widgets.keys())
         except:
             None
```

### Comparing `ipyautoui-0.5.4/src/ipyautoui/automapschema.py` & `ipyautoui-0.5.5/src/ipyautoui/automapschema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/automapschema.yaml` & `ipyautoui-0.5.5/src/ipyautoui/automapschema.yaml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/autoui.py` & `ipyautoui-0.5.5/src/ipyautoui/autoui.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/autovjsf.py` & `ipyautoui-0.5.5/src/ipyautoui/autovjsf.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/autowidgets.py` & `ipyautoui-0.5.5/src/ipyautoui/autowidgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #
 # %load_ext lab_black
 
 """
 extends standard ipywidgets to facilitate initialisation from jsonschema
 """
 
-from ipyautoui.constants import MAP_JSONSCHEMA_TO_IPYWIDGET
+from ipyautoui.constants import MAP_JSONSCHEMA_TO_IPYWIDGET, BUTTON_WIDTH_MIN
 import ipywidgets as w
 import traitlets as tr
 from copy import deepcopy
 from ipyautoui.custom import (
     modelrun,
     markdown_widget,
     filechooser,
@@ -100,15 +100,15 @@
 
     def __init__(self, widget_type, schema, *args, **kwargs):
         self.schema = schema
         self.caller = create_widget_caller(schema)
         # ^ TODO: should this be in a higher-level func?
         #         ui = nullable(w.IntSlider)(value=30) # this doesn't work bu maybe should...
         self.nullable = tr.Bool(default_value=True)
-        self.bn = w.ToggleButton(icon="toggle-on", layout={"width": "40px"})
+        self.bn = w.ToggleButton(icon="toggle-on", layout={"width": BUTTON_WIDTH_MIN})
         self.show_none = w.Text(**SHOW_NONE_KWARGS)
         if "nullable" in kwargs.keys():
             self.nullable = kwargs["nullable"]
             kwargs.pop("nullable")
         if "value" in kwargs.keys():
             value = kwargs["value"]
         elif len(args) > 0:
```

### Comparing `ipyautoui-0.5.4/src/ipyautoui/basemodel.py` & `ipyautoui-0.5.5/src/ipyautoui/basemodel.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/constants.py` & `ipyautoui-0.5.5/src/ipyautoui/constants.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo.py` & `ipyautoui-0.5.5/src/ipyautoui/demo.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/env.py` & `ipyautoui-0.5.5/src/ipyautoui/env.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/mydocstring_display.py` & `ipyautoui-0.5.5/src/ipyautoui/mydocstring_display.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/test_schema.py` & `ipyautoui-0.5.5/src/ipyautoui/test_schema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/vjsf.vue` & `ipyautoui-0.5.5/src/ipyautoui/vjsf.vue`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/autogrid.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/autogrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/buttonbars.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/buttonbars.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/decision_branch.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/decision_branch.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/editgrid.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/editgrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/filechooser.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/filechooser.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/filesindir.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/filesindir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/fileupload.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/fileupload.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/iterable.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/iterable.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/loadproject.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/loadproject.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/markdown_widget.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/markdown_widget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/modelrun.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/modelrun.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/multiselect_search.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/multiselect_search.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/outputlogging.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/outputlogging.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/selectdir.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/selectdir.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 #     language: python
 #     name: python3
 # ---
 
 # +
 # %run ../_dev_sys_path_append.py
 # %run __init__.py
-#
 # %load_ext lab_black
+
 from IPython.display import display
 from ipyautoui.basemodel import BaseModel
 from ipyautoui.basemodel import file
 from ipyautoui._utils import file
 
 setattr(BaseModel, "file", file)
 from pydantic import validator, Field, ValidationError
```

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/showhide.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/showhide.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 # jupyter:
 #   jupytext:
 #     formats: py:light
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.13.8
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # %run ../_dev_sys_path_append.py
-# %run __init__.py
-#
-# %run ../__init__.py
+# # %run __init__.py
+# # %run ../__init__.py
 # %load_ext lab_black
 
 # +
 import ipywidgets as w
-import traitlets as t
+import traitlets as tr
 from IPython.display import clear_output, display
 from ipyautoui.constants import KWARGS_COLLAPSE, KWARGS_DISPLAY
 import typing as ty
 
 
 class ShowHide(w.VBox):
     """simple show/hide widget that displays output of a callable that is pass as the input"""
 
-    fn_display = t.Callable()
-    title = t.Unicode()
+    fn_display = tr.Callable()
+    is_show = tr.Bool()
+    title = tr.Unicode()
 
-    @t.default("fn_display")
+    @tr.default("fn_display")
     def _fn_display(self):
         return lambda: print("display")
 
     def __init__(
         self,
         fn_display: ty.Callable = lambda: w.HTML("😲"),
         title: str = "title",
@@ -67,23 +67,37 @@
             self.btn_display.layout.width = self.button_width
         self.html_title = w.HTML()
         self.out = w.Output()
         self.out.layout.display = "None"
         self.hbx_title.children = [self.btn_display, self.html_title]
         self.children = [self.hbx_title, self.out]
         self._observe_fn_display("asd")
+        self._init_controls()
 
-    @t.observe("title")
+    def _init_controls(self):
+        self.btn_display.observe(self.check_is_show, "value")
+
+    def check_is_show(self, on_change):
+        self.is_show = on_change["new"]
+
+    def show(self):
+        self.btn_display.value = True
+
+    def hide(self):
+        self.btn_display.value = False
+
+    @tr.observe("title")
     def _observe_title(self, change):
         self.html_title.value = self.title
 
-    @t.observe("fn_display")
+    @tr.observe("fn_display")
     def _observe_fn_display(self, change):
         self.btn_display.unobserve(None)
         self.btn_display.observe(self.display_out, "value")
+        self.btn_display.observe(self.check_is_show, "value")
 
     def display_out(self, click):
         with self.out:
             if self.btn_display.value:
                 {
                     setattr(self.btn_display, k, v)
                     for k, v in KWARGS_COLLAPSE.items()
@@ -102,7 +116,9 @@
                 clear_output()
 
 
 # -
 if __name__ == "__main__":
     d = ShowHide(auto_open=True)
     display(d)
+
+
```

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/showopenurl.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/showopenurl.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/title_description.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/title_description.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/urlimagelink.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/urlimagelink.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/widgetcaller_error.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/widgetcaller_error.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/custom/workingdir.py` & `ipyautoui-0.5.5/src/ipyautoui/custom/workingdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/__init__.py` & `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/complex_serialization.py` & `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/complex_serialization.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/core_ipywidgets.py` & `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/editable_datagrid.py` & `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nested.py` & `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nested.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nested_editable_datagrid.py` & `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nested_editable_datagrid.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     integer: int = Field(1)
     floater: float = Field(3.1415, column_width=70)
     something_else: float = Field(324, column_width=100)
 
 
 class NestedEditableGrid(BaseModel):
     title: str = "My editable Dataframe"
-    reference: str = "some ref data"
+    reference: ty.Optional[str] = None  # TODO: this creates formatting issue
     grid: ty.List[DataFrameCols] = Field(
         default=DATAGRID_TEST_VALUE,
-        # default_factory=lambda: DATAGRID_TEST_VALUE, # TODO: AutoUi isn't getting data when set using default_factory. make this work!
         format="DataFrame",
         global_decimal_places=2,
+        # default_factory=lambda: DATAGRID_TEST_VALUE, # TODO: AutoUi isn't getting data when set using default_factory. make this work!
     )
```

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py` & `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_array_enum.py` & `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_array_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_enum.py` & `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/ruleset.py` & `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/ruleset.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/.gitignore` & `ipyautoui-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/LICENSE` & `ipyautoui-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/README.md` & `ipyautoui-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/pyproject.toml` & `ipyautoui-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.4/PKG-INFO` & `ipyautoui-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyautoui
-Version: 0.5.4
+Version: 0.5.5
 Summary: wrapper that sits on top of ipywidgets and other ipy widget libraries to template / automate the creation of widget forms. Uses pydantic to create defined data-container and serialisation to JSON. Includes example patterns for adding new custom widgets.
 Project-URL: Homepage, https://github.com/maxfordham/ipyautoui
 Author-email: John Gunstone <gunstone.john@gmail.com>
 License-File: LICENSE
 Keywords: ipyautoui
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

