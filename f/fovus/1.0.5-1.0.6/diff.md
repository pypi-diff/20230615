# Comparing `tmp/fovus-1.0.5-py3-none-any.whl.zip` & `tmp/fovus-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,49 +1,49 @@
-Zip file size: 47507 bytes, number of entries: 47
+Zip file size: 51660 bytes, number of entries: 47
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/__init__.py
 -rw-r--r--  2.0 unx       65 b- defN 23-Apr-05 06:40 fovus/root_config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/adapter/__init__.py
 -rw-r--r--  2.0 unx     3331 b- defN 23-Apr-05 06:40 fovus/adapter/aws_cognito_adapter.py
--rw-r--r--  2.0 unx    19085 b- defN 23-Jun-01 05:54 fovus/adapter/fovus_api_adapter.py
+-rw-r--r--  2.0 unx    22337 b- defN 23-Jun-15 01:02 fovus/adapter/fovus_api_adapter.py
 -rw-r--r--  2.0 unx     8700 b- defN 23-May-25 22:01 fovus/adapter/fovus_s3_adapter.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/cli/__init__.py
--rw-r--r--  2.0 unx    13450 b- defN 23-Jun-01 05:54 fovus/cli/cli_action_runner.py
+-rw-r--r--  2.0 unx    13717 b- defN 23-Jun-15 01:02 fovus/cli/cli_action_runner.py
 -rw-r--r--  2.0 unx      161 b- defN 23-Apr-05 06:56 fovus/cli/documenter.py
--rw-r--r--  2.0 unx      475 b- defN 23-Apr-05 06:40 fovus/cli/fovus_cli.py
--rw-r--r--  2.0 unx    25911 b- defN 23-Jun-01 05:54 fovus/cli/fovus_cli_argument_parser.py
+-rw-r--r--  2.0 unx      997 b- defN 23-Jun-15 01:02 fovus/cli/fovus_cli.py
+-rw-r--r--  2.0 unx    29103 b- defN 23-Jun-15 01:02 fovus/cli/fovus_cli_argument_parser.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/config/__init__.py
--rw-r--r--  2.0 unx      138 b- defN 23-Jun-01 05:56 fovus/config/config.py
+-rw-r--r--  2.0 unx      840 b- defN 23-Jun-15 01:40 fovus/config/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/constants/__init__.py
 -rw-r--r--  2.0 unx     1278 b- defN 23-Jun-01 05:54 fovus/constants/benchmark_constants.py
--rw-r--r--  2.0 unx       59 b- defN 23-Apr-05 06:40 fovus/constants/cli_action_runner_constants.py
--rw-r--r--  2.0 unx     8682 b- defN 23-Jun-01 05:54 fovus/constants/cli_constants.py
--rw-r--r--  2.0 unx     2100 b- defN 23-Jun-01 05:54 fovus/constants/fovus_api_constants.py
+-rw-r--r--  2.0 unx      485 b- defN 23-Jun-15 01:02 fovus/constants/cli_action_runner_constants.py
+-rw-r--r--  2.0 unx     9096 b- defN 23-Jun-15 01:02 fovus/constants/cli_constants.py
+-rw-r--r--  2.0 unx     2037 b- defN 23-Jun-15 01:02 fovus/constants/fovus_api_constants.py
 -rw-r--r--  2.0 unx      194 b- defN 23-Apr-05 06:40 fovus/constants/util_constants.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/exception/__init__.py
 -rw-r--r--  2.0 unx      291 b- defN 23-Apr-05 06:40 fovus/exception/status_code_exception.py
 -rw-r--r--  2.0 unx      183 b- defN 23-Apr-05 06:40 fovus/exception/system_exception.py
 -rw-r--r--  2.0 unx      174 b- defN 23-Apr-05 06:40 fovus/exception/user_exception.py
--rw-r--r--  2.0 unx     1054 b- defN 23-May-15 05:07 fovus/fovus_provided_configs/FOVUS_example_job_config_containerized.json
--rw-r--r--  2.0 unx     1112 b- defN 23-May-15 05:07 fovus/fovus_provided_configs/FOVUS_example_job_config_monolithic.json
--rw-r--r--  2.0 unx      829 b- defN 23-May-15 05:07 fovus/fovus_provided_configs/FOVUS_job_template_containerized.json
--rw-r--r--  2.0 unx     1185 b- defN 23-May-15 05:07 fovus/fovus_provided_configs/FOVUS_job_template_monolithic.json
--rw-r--r--  2.0 unx       42 b- defN 23-Apr-05 06:40 fovus/fovus_provided_configs/FOVUS_user_config_template.json
+-rw-r--r--  2.0 unx     1145 b- defN 23-Jun-15 01:02 fovus/fovus_provided_configs/FOVUS_example_job_config_containerized.json
+-rw-r--r--  2.0 unx     1203 b- defN 23-Jun-15 01:02 fovus/fovus_provided_configs/FOVUS_example_job_config_monolithic.json
+-rw-r--r--  2.0 unx      894 b- defN 23-Jun-15 01:02 fovus/fovus_provided_configs/FOVUS_job_template_containerized.json
+-rw-r--r--  2.0 unx     1250 b- defN 23-Jun-15 01:02 fovus/fovus_provided_configs/FOVUS_job_template_monolithic.json
+-rw-r--r--  2.0 unx       39 b- defN 23-Jun-15 01:02 fovus/fovus_provided_configs/FOVUS_user_config_template.json
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/fovus_provided_configs/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/schema/__init__.py
--rw-r--r--  2.0 unx    10183 b- defN 23-May-15 05:07 fovus/schema/create_job_schema.json
+-rw-r--r--  2.0 unx    11652 b- defN 23-Jun-15 01:02 fovus/schema/create_job_schema.json
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/util/__init__.py
 -rw-r--r--  2.0 unx     3389 b- defN 23-Apr-05 06:40 fovus/util/aws_util.py
 -rw-r--r--  2.0 unx      334 b- defN 23-Apr-05 06:40 fovus/util/cli_action_runner_util.py
--rw-r--r--  2.0 unx     4625 b- defN 23-Jun-01 05:54 fovus/util/file_util.py
--rw-r--r--  2.0 unx     7357 b- defN 23-Jun-01 05:54 fovus/util/fovus_api_util.py
--rw-r--r--  2.0 unx     1740 b- defN 23-Apr-05 06:40 fovus/util/fovus_cli_argument_parser_util.py
+-rw-r--r--  2.0 unx     5858 b- defN 23-Jun-15 01:02 fovus/util/file_util.py
+-rw-r--r--  2.0 unx    10774 b- defN 23-Jun-15 01:02 fovus/util/fovus_api_util.py
+-rw-r--r--  2.0 unx     1956 b- defN 23-Jun-15 01:02 fovus/util/fovus_cli_argument_parser_util.py
 -rw-r--r--  2.0 unx     1519 b- defN 23-Apr-05 06:40 fovus/util/fovus_s3_adapter_util.py
--rw-r--r--  2.0 unx      533 b- defN 23-Apr-05 06:40 fovus/util/util.py
+-rw-r--r--  2.0 unx      791 b- defN 23-Jun-15 01:02 fovus/util/util.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/validator/__init__.py
--rw-r--r--  2.0 unx     3732 b- defN 23-Jun-01 05:54 fovus/validator/fovus_api_validator.py
--rw-r--r--  2.0 unx    14101 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8883 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4184 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/RECORD
-47 files, 149228 bytes uncompressed, 40699 bytes compressed:  72.7%
+-rw-r--r--  2.0 unx     3782 b- defN 23-Jun-15 01:02 fovus/validator/fovus_api_validator.py
+-rw-r--r--  2.0 unx    14101 b- defN 23-Jun-15 01:59 fovus-1.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    10053 b- defN 23-Jun-15 01:59 fovus-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 01:59 fovus-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-15 01:59 fovus-1.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-15 01:59 fovus-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4187 b- defN 23-Jun-15 01:59 fovus-1.0.6.dist-info/RECORD
+47 files, 166065 bytes uncompressed, 44852 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -117,26 +117,26 @@
 
 Filename: fovus/validator/__init__.py
 Comment: 
 
 Filename: fovus/validator/fovus_api_validator.py
 Comment: 
 
-Filename: fovus-1.0.5.dist-info/LICENSE.txt
+Filename: fovus-1.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fovus-1.0.5.dist-info/METADATA
+Filename: fovus-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: fovus-1.0.5.dist-info/WHEEL
+Filename: fovus-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: fovus-1.0.5.dist-info/entry_points.txt
+Filename: fovus-1.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: fovus-1.0.5.dist-info/top_level.txt
+Filename: fovus-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: fovus-1.0.5.dist-info/RECORD
+Filename: fovus-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fovus/adapter/fovus_api_adapter.py

```diff
@@ -15,85 +15,102 @@
 )
 from fovus.constants.cli_constants import (
     BENCHMARKING_PROFILE_NAME,
     COMPUTING_DEVICE,
     CPU,
     ENABLE_HYPERTHREADING,
     FOVUS_PROVIDED_CONFIGS,
+    IS_SINGLE_THREADED_TASK,
     JOB_CONFIG_CONTAINERIZED_TEMPLATE,
     JOB_CONFIG_FILE_PATH,
     JOB_NAME,
     MAX_GPU,
     MIN_GPU,
     MIN_GPU_MEM_GIB,
     MONOLITHIC_OVERRIDE,
     PATH_TO_CONFIG_FILE_IN_REPO,
+    SUPPORTED_CPU_ARCHITECTURES,
     TIMESTAMP,
     USER_ID,
     WORKSPACE_ID,
 )
 from fovus.constants.fovus_api_constants import (
-    APIS,
     AUTHORIZATION_HEADER,
-    BENCHMARK,
     BODY,
     BOUND_VALUE_CORRECTION_PRINT_ORDER,
     BP_HYPERTHREADING,
-    CREATE_JOB,
+    CONTAINERIZED,
     ENVIRONMENT,
-    FILE,
-    GET_FILE_DOWNLOAD_TOKEN,
-    GET_FILE_UPLOAD_TOKEN,
-    GET_JOB_INFO,
-    JOB,
+    IS_LICENSE_REQUIRED,
     JOB_STATUS,
+    LICENSE_ADDRESS,
     LICENSE_COUNT_PER_TASK,
     LICENSE_FEATURE,
-    LIST_BENCHMARK_PROFILE,
-    LIST_SOFTWARE,
     MONOLITHIC_LIST,
     PAYLOAD_CONSTRAINTS,
     PAYLOAD_JOB_CONSTRAINTS,
     PAYLOAD_JOB_NAME,
     PAYLOAD_TASK_CONSTRAINTS,
     PAYLOAD_TIMESTAMP,
     PAYLOAD_WORKSPACE_ID,
-    SOFTWARE,
     SOFTWARE_MAP,
     SOFTWARE_NAME,
     SOFTWARE_VERSION,
     SOFTWARE_VERSIONS,
     TIMEOUT_SECONDS,
     VENDOR_NAME,
+    Api,
+    ApiMethod,
 )
 from fovus.constants.util_constants import UTF8
 from fovus.exception.user_exception import UserException
 from fovus.root_config import ROOT_DIR
 from fovus.util.fovus_api_util import FovusApiUtil
 
 
 class FovusApiAdapter:
     def __init__(self, auth_type, auth_parameters, client_id):
         self.cognito_adapter = AwsCognitoAdapter()
         self.cognito_adapter.authenticate(auth_type, auth_parameters, client_id)
 
     def create_job(self, request):
         headers = self._get_api_authorization_header()
-        response = requests.post(APIS[JOB][CREATE_JOB], json=request, headers=headers, timeout=TIMEOUT_SECONDS)
+        response = requests.post(
+            FovusApiUtil.get_api_address(Api.JOB, ApiMethod.CREATE_JOB),
+            json=request,
+            headers=headers,
+            timeout=TIMEOUT_SECONDS,
+        )
         FovusApiUtil.confirm_successful_response(response.json(), self.__class__.__name__)
         return response.json()
 
     def make_dynamic_changes_to_create_job_request(self, request):
         self._make_dynamic_changes_to_software(request)
         self._validate_benchmarking_profile(request)
 
+    def _ensure_is_single_threaded_task_filled(self, request):
+        if (
+            request[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][COMPUTING_DEVICE] == CPU
+            and IS_SINGLE_THREADED_TASK not in request[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS]
+        ):
+            print(
+                f"Field '{IS_SINGLE_THREADED_TASK}' is now required in '{PAYLOAD_TASK_CONSTRAINTS}' for create job "
+                f"requests where '{COMPUTING_DEVICE}' is '{CPU}' and one of the following is true:"
+                f"\n\t- Job environment is '{CONTAINERIZED}'"
+                f"\n\t- Job environment is monolithic and any software in '{MONOLITHIC_LIST}' "
+                "does not require a license."
+                f"\nAutofilling '{IS_SINGLE_THREADED_TASK}' with default value of False."
+            )
+            request[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][IS_SINGLE_THREADED_TASK] = False
+
     def _make_dynamic_changes_to_software(self, request):
         print("Validating software...")
         if MONOLITHIC_LIST not in request[ENVIRONMENT]:
             print("Request is for a containerized job. Filling missing/empty vendorName fields is not required.")
+            self._ensure_is_single_threaded_task_filled(request)
             return
 
         list_software_response = self.list_software()
         for i, monolithic_list_item in enumerate(copy.deepcopy(request[ENVIRONMENT][MONOLITHIC_LIST])):
             software_name = monolithic_list_item[SOFTWARE_NAME]
             software_version = monolithic_list_item[SOFTWARE_VERSION]
             software_vendor = monolithic_list_item[VENDOR_NAME]
@@ -109,14 +126,19 @@
                     ):
                         if valid_software_vendor != software_vendor:
                             print(
                                 f"Replacing vendor name '{software_vendor}' with "
                                 f"'{valid_software_vendor}' for monolithic list item {monolithic_list_item}."
                             )
                             request[ENVIRONMENT][MONOLITHIC_LIST][i][VENDOR_NAME] = valid_software_vendor
+                        if list_software_response[SOFTWARE_MAP][valid_software_vendor][software_name][
+                            IS_LICENSE_REQUIRED
+                        ]:
+                            self._ensure_is_single_threaded_task_filled(request)
+                            self._confirm_required_fields_for_licensed_software(monolithic_list_item)
                         break  # Successful validation of current list item.
                     raise UserException(
                         HTTPStatus.BAD_REQUEST,
                         self.__class__.__name__,
                         f"Software version '{software_version}' for software name '{software_name}' is not valid. "
                         + "Valid software versions: "
                         + str(
@@ -133,14 +155,35 @@
                     HTTPStatus.BAD_REQUEST,
                     self.__class__.__name__,
                     f"Software name '{software_name}' is not valid. "
                     + "Valid software vendors and names (format: [{vendor: [name, ...]}, ...]): "
                     + str(valid_software_names),
                 )
 
+    def _confirm_required_fields_for_licensed_software(self, monolithic_list_item):
+        error_messages = []
+        if not monolithic_list_item.get(LICENSE_ADDRESS):
+            error_messages.append(f"Non-empty '{LICENSE_ADDRESS}'")
+        if not monolithic_list_item.get(LICENSE_FEATURE):
+            error_messages.append(f"Non-empty '{LICENSE_FEATURE}'")
+        if (
+            not isinstance(monolithic_list_item.get(LICENSE_COUNT_PER_TASK), int)
+            or monolithic_list_item.get(LICENSE_COUNT_PER_TASK) < 0
+        ):
+            error_messages.append(f"Non-negative integer '{LICENSE_COUNT_PER_TASK}'")
+        if error_messages:
+            raise UserException(
+                HTTPStatus.BAD_REQUEST,
+                self.__class__.__name__,
+                f"The following are required for {MONOLITHIC_LIST} item {monolithic_list_item} "
+                f"in order for license queue and auto-scaling to take effect:"
+                + "\n\t- "
+                + "\n\t- ".join(error_messages),
+            )
+
     def _validate_benchmarking_profile(self, request):  # pylint: disable=too-many-locals
         benchmarking_profile_name = request[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][BENCHMARKING_PROFILE_NAME]
         hyperthreading_enabled = request[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][ENABLE_HYPERTHREADING]
         print(
             f"Validating the benchmarking profile '{benchmarking_profile_name}' and "
             "updating values if necessary and possible..."
         )
@@ -154,14 +197,22 @@
             if benchmarking_profile_name == current_benchmarking_profile_name:
                 validations_config = FovusApiUtil.get_benchmark_validations_config(request)
                 bound_scaler = FovusApiUtil.get_benchmark_bound_scaler(
                     hyperthreading_enabled,
                     current_benchmarking_profile[BP_HYPERTHREADING],
                 )
                 FovusApiUtil.print_benchmark_hyperthreading_info(hyperthreading_enabled)
+                FovusApiUtil.validate_computing_device(
+                    request[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][COMPUTING_DEVICE],
+                    current_benchmarking_profile,
+                )
+                FovusApiUtil.validate_cpu_architectures(
+                    request[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][SUPPORTED_CPU_ARCHITECTURES],
+                    current_benchmarking_profile,
+                )
                 corrected_value_messages = {}
                 for validation_type in validations_config:  # pylint: disable=consider-using-dict-items
                     for bound_to_validate in validations_config[validation_type][BOUNDS]:
                         current_value = request[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][bound_to_validate]
                         benchmarking_profile_bounds = FovusApiUtil.get_benchmark_profile_bounds(
                             current_benchmarking_profile, bound_to_validate, bound_scaler
                         )
@@ -207,23 +258,29 @@
             f"Invalid benchmarking profile: '{benchmarking_profile_name}'. "
             + f"Valid benchmarking profiles: {valid_benchmarking_profile_names}",
         )
 
     def get_file_download_token(self, request):
         headers = self._get_api_authorization_header()
         response = requests.post(
-            APIS[FILE][GET_FILE_DOWNLOAD_TOKEN], json=request, headers=headers, timeout=TIMEOUT_SECONDS
+            FovusApiUtil.get_api_address(Api.FILE, ApiMethod.GET_FILE_DOWNLOAD_TOKEN),
+            json=request,
+            headers=headers,
+            timeout=TIMEOUT_SECONDS,
         )
         FovusApiUtil.confirm_successful_response(response.json(), self.__class__.__name__)
         return response.json()
 
     def get_file_upload_token(self, request):
         headers = self._get_api_authorization_header()
         response = requests.post(
-            APIS[FILE][GET_FILE_UPLOAD_TOKEN], json=request, headers=headers, timeout=TIMEOUT_SECONDS
+            FovusApiUtil.get_api_address(Api.FILE, ApiMethod.GET_FILE_UPLOAD_TOKEN),
+            json=request,
+            headers=headers,
+            timeout=TIMEOUT_SECONDS,
         )
         FovusApiUtil.confirm_successful_response(response.json(), self.__class__.__name__)
         return response.json()
 
     def get_temporary_s3_upload_credentials(self, cli_dict):
         upload_credentials = self.get_file_upload_token(self.get_file_upload_download_token_request(cli_dict))
         FovusApiUtil.confirm_successful_response(upload_credentials, self.__class__.__name__)
@@ -236,28 +293,37 @@
 
     def get_job_current_status(self, cli_dict, job_id):
         job_info = self.get_job_info(FovusApiAdapter.get_job_info_request(cli_dict, job_id))
         return job_info[BODY][JOB_STATUS]
 
     def get_job_info(self, request):
         headers = self._get_api_authorization_header()
-        response = requests.post(APIS[JOB][GET_JOB_INFO], json=request, headers=headers, timeout=TIMEOUT_SECONDS)
+        response = requests.post(
+            FovusApiUtil.get_api_address(Api.JOB, ApiMethod.GET_JOB_INFO),
+            json=request,
+            headers=headers,
+            timeout=TIMEOUT_SECONDS,
+        )
         FovusApiUtil.confirm_successful_response(response.json(), self.__class__.__name__)
         return response.json()
 
     def list_software(self):
         headers = self._get_api_authorization_header()
-        response = requests.get(APIS[SOFTWARE][LIST_SOFTWARE], headers=headers, timeout=TIMEOUT_SECONDS)
+        response = requests.get(
+            FovusApiUtil.get_api_address(Api.SOFTWARE, ApiMethod.LIST_SOFTWARE),
+            headers=headers,
+            timeout=TIMEOUT_SECONDS,
+        )
         FovusApiUtil.confirm_successful_response(response.json(), self.__class__.__name__)
         return response.json()
 
     def list_benchmarking_profile(self, workspace_id):
         headers = self._get_api_authorization_header()
         response = requests.get(
-            APIS[BENCHMARK][LIST_BENCHMARK_PROFILE],
+            FovusApiUtil.get_api_address(Api.BENCHMARK, ApiMethod.LIST_BENCHMARK_PROFILE),
             params={"workspaceId": workspace_id},
             headers=headers,
             timeout=TIMEOUT_SECONDS,
         )
         FovusApiUtil.confirm_successful_response(response.json(), self.__class__.__name__)
         return response.json()
```

## fovus/cli/cli_action_runner.py

```diff
@@ -2,22 +2,29 @@
 import os
 import shutil
 from http import HTTPStatus
 
 from fovus.adapter.aws_cognito_adapter import AwsCognitoAdapter, AwsCognitoAuthType
 from fovus.adapter.fovus_api_adapter import FovusApiAdapter
 from fovus.adapter.fovus_s3_adapter import JOB_DATA_FILENAME, FovusS3Adapter
-from fovus.config.config import DEFAULT_CLIENT_ID, DEFAULT_USER_POOL_ID
-from fovus.constants.cli_action_runner_constants import GENERIC_SUCCESS, OUTPUTS
+from fovus.config.config import Config
+from fovus.constants.cli_action_runner_constants import (
+    GENERIC_SUCCESS,
+    OUTPUTS,
+    USER_CONFIG_EMAIL_UPDATE_MESSAGE,
+)
 from fovus.constants.cli_constants import (
+    CLI_ARGUMENTS,
+    CLIENT_ID,
     CONFIGURE,
     CONFLICTING_CLI_ARGUMENT_SETS,
     CREATE_JOB_WITH_UPLOAD,
     DEFAULT_USER_CONFIG_FILE_PATH,
     DOWNLOAD_JOB_FILES,
+    EMAIL,
     FOVUS_PROVIDED_CONFIGS,
     GET_JOB_CURRENT_STATUS,
     JOB_CONFIG_FILE_PATH,
     JOB_FILE_ROOT_DIRECTORY,
     JOB_ID,
     OPEN_CONFIG_FOLDER,
     PATH_TO_CONFIG_FILE_IN_REPO,
@@ -25,25 +32,26 @@
     PATH_TO_CONFIG_ROOT,
     PATH_TO_JOB_CONFIGS,
     PATH_TO_JOB_LOGS,
     PATH_TO_USER_CONFIGS,
     UNIX_OPEN,
     USER_CONFIG_TEMPLATE_FILE_NAME,
     USER_ID,
+    USER_POOL_ID,
     USERNAME,
     WINDOWS_EXPLORER,
     WORKSPACE_ID,
 )
-from fovus.constants.fovus_api_constants import CREATE_JOB, PAYLOAD_WORKSPACE_ID
+from fovus.constants.fovus_api_constants import PAYLOAD_WORKSPACE_ID, ApiMethod
 from fovus.constants.util_constants import UTF8
 from fovus.exception.status_code_exception import StatusException
 from fovus.exception.user_exception import UserException
 from fovus.root_config import ROOT_DIR
 from fovus.util.cli_action_runner_util import CliActionRunnerUtil
-from fovus.util.file_util import FOVUS_JOB_INFO_FOLDER
+from fovus.util.file_util import FOVUS_JOB_INFO_FOLDER, FileUtil
 from fovus.util.fovus_api_util import FovusApiUtil
 from fovus.util.util import Util
 from fovus.validator.fovus_api_validator import FovusApiValidator
 
 
 class CliActionRunner:  # pylint: disable=too-few-public-methods
     def __init__(self, args_dict):
@@ -132,69 +140,76 @@
                 "Forbidden arguments: "
                 + ", ".join(CliActionRunnerUtil.get_argument_string_list_from_keys(forbidden_arguments))
                 + ".",
             )
         print(GENERIC_SUCCESS)
 
     def _confirm_user_config_data_present(self):
-        if not (self.args_dict.get(USERNAME) and self.args_dict.get(WORKSPACE_ID)):
+        if self.args_dict.get(USERNAME):
+            print(USER_CONFIG_EMAIL_UPDATE_MESSAGE)
+            Util.keep_prioritized_key_value_in_dict(self.args_dict, prioritized_key=EMAIL, fallback_key=USERNAME)
+        if not (self.args_dict.get(EMAIL) and self.args_dict.get(WORKSPACE_ID)):
             raise UserException(
                 HTTPStatus.BAD_REQUEST,
                 self.__class__.__name__,
-                "Username and workspace ID must be specified. This can be done in one of three ways:\n"
+                "Email and workspace ID must be specified. This can be done in one of three ways:\n"
                 + "1. Run the command 'fovus --configure' to create a default user config file.\n"
                 + "2. Specify the argument --user-config-file-path and point to a valid user config file.\n"
                 + "\t(run --open-config-folder to generate a template under ~/.fovus/user_configs/"
                 + USER_CONFIG_TEMPLATE_FILE_NAME
                 + "\n"
-                + "3. Specify the arguments --username and --workspace-id.\n",
+                + f"3. Specify the arguments {CLI_ARGUMENTS[EMAIL]} and {CLI_ARGUMENTS[WORKSPACE_ID]}.\n",
             )
 
     def _try_set_job_id(self):
-        if not self.args_dict.get(JOB_ID):
+        if self.args_dict.get(JOB_ID):
+            return
+
+        if self.args_dict.get(JOB_FILE_ROOT_DIRECTORY):
             print(
                 "Job ID not specified. Attempting to find job ID in "
                 + os.path.join(self.args_dict[JOB_FILE_ROOT_DIRECTORY], FOVUS_JOB_INFO_FOLDER, JOB_DATA_FILENAME)
                 + "..."
             )
             job_data_file_path = os.path.join(
                 self.args_dict[JOB_FILE_ROOT_DIRECTORY], FOVUS_JOB_INFO_FOLDER, JOB_DATA_FILENAME
             )
             if os.path.exists(job_data_file_path):
                 with open(job_data_file_path, encoding=UTF8) as file:
                     job_data = json.load(file)
                     self.args_dict[JOB_ID] = job_data.get(JOB_ID)
                     print("Job ID found: " + self.args_dict[JOB_ID])
-            else:
-                raise UserException(
-                    HTTPStatus.BAD_REQUEST,
-                    self.__class__.__name__,
-                    "Missing job ID. This can be provided as an argument (via --job-id) or through the job data "
-                    + "file, which is automatically generated when a job is created from the CLI.\n"
-                    + "When generated, the job data file is located at the following path:\n"
-                    + os.path.join(self.args_dict[JOB_FILE_ROOT_DIRECTORY], FOVUS_JOB_INFO_FOLDER, JOB_DATA_FILENAME)
-                    + ".",
-                )
+                    return
+
+        raise UserException(
+            HTTPStatus.BAD_REQUEST,
+            self.__class__.__name__,
+            (
+                "Missing job ID. This can be provided as an argument (via --job-id) or through the job data "
+                "file (via --job-file-root-directory), which is automatically generated in the "
+                "'job_root_folder/.fovus' directory when a job is created from the CLI."
+            ),
+        )
 
     def _configure(self):
         self._create_missing_directories()
         print(GENERIC_SUCCESS)
         self._create_missing_empty_config_files()
         print(GENERIC_SUCCESS)
 
         if os.path.exists(DEFAULT_USER_CONFIG_FILE_PATH):
             print("Default user config file already exists:")
-            with open(DEFAULT_USER_CONFIG_FILE_PATH, encoding=UTF8) as file:
-                print(json.dumps(json.load(file), indent=4))
+            default_user_config = FileUtil.get_default_user_config()
+            print(json.dumps(default_user_config, indent=4, sort_keys=True))
             if input("Overwrite? (y/n):") == "n":
                 return
 
         print("Setting up new default user config...")
         new_default_user_config = {}
-        new_default_user_config[USERNAME] = input("Username: ")
+        new_default_user_config[EMAIL] = input("Email: ")
         new_default_user_config[PAYLOAD_WORKSPACE_ID] = input("Workspace ID: ")
 
         with open(DEFAULT_USER_CONFIG_FILE_PATH, "w", encoding=UTF8) as file:
             json.dump(new_default_user_config, file, indent=4)
         print(GENERIC_SUCCESS)
         print("From now on, if no user config file is specified, this default config will be used.")
         print(OUTPUTS)
@@ -235,25 +250,25 @@
             )
         print(GENERIC_SUCCESS)
 
     def _create_job(self):
         print("Creating Fovus API adapter and Fovus S3 adapter and authenticating...")
         fovus_api_adapter = FovusApiAdapter(
             AwsCognitoAuthType.USER_SRP_AUTH,
-            AwsCognitoAdapter.get_user_srp_auth_parameters(self.args_dict[USERNAME], DEFAULT_USER_POOL_ID),
-            DEFAULT_CLIENT_ID,
+            AwsCognitoAdapter.get_user_srp_auth_parameters(self.args_dict[EMAIL], Config.get(USER_POOL_ID)),
+            Config.get(CLIENT_ID),
         )
         self._try_set_user_id(fovus_api_adapter)
         fovus_s3_adapter = FovusS3Adapter(fovus_api_adapter, self.args_dict, self.args_dict[JOB_FILE_ROOT_DIRECTORY])
         print(GENERIC_SUCCESS)
 
         print("Creating and validating create job request...")
         create_job_request = FovusApiAdapter.get_create_job_request(self.args_dict)
         fovus_api_adapter.make_dynamic_changes_to_create_job_request(create_job_request)
-        validator = FovusApiValidator(create_job_request, CREATE_JOB)
+        validator = FovusApiValidator(create_job_request, ApiMethod.CREATE_JOB)
         validator.validate()
         print(GENERIC_SUCCESS)
 
         fovus_s3_adapter.upload_files()
 
         print("Creating job...")
         fovus_api_adapter.create_job(create_job_request)
@@ -263,16 +278,16 @@
             "\n".join(("Job name:", create_job_request["jobName"], "Job ID:", FovusApiUtil.get_job_id(self.args_dict)))
         )
 
     def _download_job_files(self):
         print("Creating Fovus API adapter and Fovus S3 adapter and authenticating...")
         fovus_api_adapter = FovusApiAdapter(
             AwsCognitoAuthType.USER_SRP_AUTH,
-            AwsCognitoAdapter.get_user_srp_auth_parameters(self.args_dict[USERNAME], DEFAULT_USER_POOL_ID),
-            DEFAULT_CLIENT_ID,
+            AwsCognitoAdapter.get_user_srp_auth_parameters(self.args_dict[EMAIL], Config.get(USER_POOL_ID)),
+            Config.get(CLIENT_ID),
         )
         self._try_set_user_id(fovus_api_adapter)
         fovus_s3_adapter = FovusS3Adapter(fovus_api_adapter, self.args_dict, self.args_dict[JOB_FILE_ROOT_DIRECTORY])
         fovus_s3_adapter.download_files()
 
     def _create_missing_directories(self):
         print("Creating missing config directories (if any)")
@@ -286,16 +301,16 @@
             empty_config_json_file_path = os.path.abspath(os.path.join(ROOT_DIR, config[PATH_TO_CONFIG_FILE_IN_REPO]))
             shutil.copy(empty_config_json_file_path, config[PATH_TO_CONFIG_FILE_LOCAL])
 
     def _get_job_current_status(self):
         print("Getting job current status...")
         fovus_api_adapter = FovusApiAdapter(
             AwsCognitoAuthType.USER_SRP_AUTH,
-            AwsCognitoAdapter.get_user_srp_auth_parameters(self.args_dict[USERNAME], DEFAULT_USER_POOL_ID),
-            DEFAULT_CLIENT_ID,
+            AwsCognitoAdapter.get_user_srp_auth_parameters(self.args_dict[EMAIL], Config.get(USER_POOL_ID)),
+            Config.get(CLIENT_ID),
         )
         self._try_set_user_id(fovus_api_adapter)
         job_current_status = fovus_api_adapter.get_job_current_status(self.args_dict, self.args_dict[JOB_ID])
         print(GENERIC_SUCCESS)
         print(OUTPUTS)
         print("\n".join(("Job ID", self.args_dict[JOB_ID], "Job current status:", job_current_status)))
```

## fovus/cli/fovus_cli.py

```diff
@@ -1,21 +1,40 @@
 #!/usr/bin/env python3
 import sys
+import traceback
 
 from fovus.cli.cli_action_runner import CliActionRunner
 from fovus.cli.fovus_cli_argument_parser import FovusCliArgumentParser
 
 OK_RETURN_STATUS = 0
+ERROR_RETURN_STATUS = 1
 
 
 def main():
+    return_status = OK_RETURN_STATUS
+    debug = False
+    if "--debug" in sys.argv:
+        debug = True
+        sys.argv.remove("--debug")
+    try:
+        _main()
+    except Exception as exception:  # pylint: disable=broad-except
+        if debug:
+            print(traceback.format_exc())
+        else:
+            print(exception)
+        return_status = ERROR_RETURN_STATUS
+    finally:
+        return return_status  # pylint: disable=lost-exception
+
+
+def _main():
     parser = FovusCliArgumentParser()
     parser.parse_args()
     parser.merge_args_with_config()
+    parser.update_overridden_configs()
     cli_action_runner = CliActionRunner(parser.get_args_dict())
     cli_action_runner.run_actions()
 
-    return OK_RETURN_STATUS
-
 
 if __name__ == "__main__":
     sys.exit(main())
```

## fovus/cli/fovus_cli_argument_parser.py

```diff
@@ -1,29 +1,36 @@
 #!/usr/bin/env python3
 import argparse
 import json
 import os
+import sys
+from http import HTTPStatus
 
+from fovus.config.config import Config
 from fovus.constants.cli_constants import (
     BENCHMARKING_PROFILE_NAME,
     BOOLEAN_ARGS,
     CLI_ARGUMENTS,
+    CLIENT_ID,
     COMPUTING_DEVICE,
     CONFIGURE,
     CPU,
     CREATE_JOB_WITH_UPLOAD,
     DEFAULT_USER_CONFIG_FILE_PATH,
+    DOMAIN_NAME,
     DOWNLOAD_JOB_FILES,
+    EMAIL,
     ENABLE_HYPERTHREADING,
     EXCLUDE_INPUT,
     EXCLUDE_OUTPUT,
     GET_JOB_CURRENT_STATUS,
     GPU,
     INCLUDE_INPUT,
     INCLUDE_OUTPUT,
+    IS_SINGLE_THREADED_TASK,
     IS_SUBJECT_TO_AVAILABLE_RESOURCES,
     JOB_CONFIG_FILE_PATH,
     JOB_FILE_ROOT_DIRECTORY,
     JOB_ID,
     JOB_NAME,
     LICENSE_TIMEOUT_HOURS,
     MAX_GPU,
@@ -41,24 +48,28 @@
     PARALLELISM_OPTIMIZATION,
     RUN_COMMAND,
     SCALABLE_PARALLELISM,
     STORAGE_GIB,
     SUPPORTED_CPU_ARCHITECTURES,
     TIME_TO_COST_PRIORITY_RATIO,
     USER_CONFIG_FILE_PATH,
+    USER_POOL_ID,
     USERNAME,
     WALLTIME_HOURS,
     WORKSPACE_ID,
 )
 from fovus.constants.util_constants import UTF8
+from fovus.exception.user_exception import UserException
 from fovus.util.cli_action_runner_util import CliActionRunnerUtil
+from fovus.util.file_util import FileUtil
 from fovus.util.fovus_cli_argument_parser_util import FovusCliArgumentParserUtil
 
 OK_RETURN_STATUS = 0
 
+IF_IS_SINGLE_THREADED_NOTE = "(or multiple single-threaded tasks on each compute node if isSingleThreadedTask is true)"
 JOB_DIRECTORY_REQUIRES_FOVUS_FOLDER_NOTE_WITH_DIRECTORY_AND_JOB_ID_EXPLANATION = (
     "(Note: If the job file directory is provided, the directory must contain a .fovus "
     "folder, which is automatically generated when a job is created with the Fovus CLI. "
     "If both a job file directory and job ID are provided, the job ID will be used.)"
 )
 USED_FOR_OVERRIDING_JOB_CONFIG_VALUES = (
     "(Note: Used for overriding job config values. If this value is provided in the job "
@@ -212,21 +223,22 @@
             + "filepath does "
             + "not match any expression, it will not be downloaded. "
             + " ".join((WILDCARD_EXPLANATION, ANY_NUMBER_OF_EXPRESSIONS)),
         )
 
         # User config.
         self.parser.add_argument(
-            *CLI_ARGUMENTS[USERNAME],
-            dest=USERNAME,
+            *CLI_ARGUMENTS[EMAIL],
+            dest=EMAIL,
             default=None,
             type=str,
-            metavar=FovusCliArgumentParserUtil.camel_to_snake(USERNAME).upper(),
+            metavar=FovusCliArgumentParserUtil.camel_to_snake(EMAIL).upper(),
             help=f"The email address used for your Fovus account. {USED_FOR_OVERRIDING_USER_CONFIG_VALUES}",
         )
+
         self.parser.add_argument(
             *CLI_ARGUMENTS[WORKSPACE_ID],
             dest=WORKSPACE_ID,
             default=None,
             type=str,
             metavar=FovusCliArgumentParserUtil.camel_to_snake(WORKSPACE_ID).upper(),
             help="The ID for the workspace you would like to use. The workspace ID can be found by clicking on the "
@@ -269,14 +281,25 @@
             default=None,
             type=str,
             metavar=FovusCliArgumentParserUtil.camel_to_snake(JOB_ID).upper(),
             help="Job ID. Used for checking job status and downloading job files if the root file directory is not "
             + "provided.",
         )
         self.parser.add_argument(
+            *CLI_ARGUMENTS[IS_SINGLE_THREADED_TASK],
+            dest=IS_SINGLE_THREADED_TASK,
+            default=None,
+            type=str,
+            choices=["true", "false"],
+            metavar=FovusCliArgumentParserUtil.camel_to_snake(IS_SINGLE_THREADED_TASK).upper(),
+            help="Set true if and only if each task uses only a single CPU thread (vCPU) at a maximum. "
+            + "Setting it true allows multiple tasks to be deployed onto the same compute node to maximize the "
+            + "task-level parallelism and the utilization of all CPU threads (vCPUs).",
+        )
+        self.parser.add_argument(
             *CLI_ARGUMENTS[LICENSE_TIMEOUT_HOURS],
             dest=LICENSE_TIMEOUT_HOURS,
             default=None,
             type=float,
             metavar=FovusCliArgumentParserUtil.camel_to_snake(LICENSE_TIMEOUT_HOURS).upper(),
             help="For license-required jobs, the maximum time the job is allowed to be waiting in a queue for "
             + "deployment when no license is available. A job will be terminated once the timeout timer expires. "
@@ -323,38 +346,40 @@
         )
         self.parser.add_argument(
             *CLI_ARGUMENTS[MIN_VCPU],
             dest=MIN_VCPU,
             default=None,
             type=int,
             metavar="MIN_VCPU",
-            help="The minimum number of vCPUs required to parallelize the execution of each task. A vCPU refers "
-            + "to a thread of a CPU core. Only values supported by the selected BP are allowed. "
+            help="The minimum number of vCPUs required to parallelize the execution of each task "
+            f"{IF_IS_SINGLE_THREADED_NOTE}. A vCPU refers to a thread "
+            "of a CPU core. Only values supported by the selected BP are allowed. "
             + USED_FOR_OVERRIDING_JOB_CONFIG_VALUES,
         )
         self.parser.add_argument(
             *CLI_ARGUMENTS[MAX_VCPU],
             dest=MAX_VCPU,
             default=None,
             type=int,
             metavar="MAX_VCPU",
-            help="The maximum number of vCPUs allowed to parallelize the execution of each task. A vCPU refers "
-            + "to a thread of a CPU core. Only values supported by the selected BP are allowed. "
+            help="The maximum number of vCPUs allowed to parallelize the execution of each task "
+            f"{IF_IS_SINGLE_THREADED_NOTE}. A vCPU refers to a thread "
+            "of a CPU core. Only values supported by the selected BP are allowed. "
             + USED_FOR_OVERRIDING_JOB_CONFIG_VALUES,
         )
         self.parser.add_argument(
             *CLI_ARGUMENTS[MIN_VCPU_MEM_GIB],
             dest=MIN_VCPU_MEM_GIB,
             default=None,
             type=float,
             metavar="MIN_VCPU_MEM_GIB",
-            help="The minimum total size of system memory required to support the execution of each task, summing "
-            + "the required memory size for each vCPU. Format: Real (e.g., 10.5). Only values supported by the "
-            + "selected BP are allowed. "
-            + USED_FOR_OVERRIDING_JOB_CONFIG_VALUES,
+            help="The minimum total size of system memory required to support the execution of each task "
+            f"{IF_IS_SINGLE_THREADED_NOTE}, summing the "
+            "required memory size for each vCPU. Format: Real (e.g., 10.5). Only values supported by the selected "
+            "BP are allowed. " + USED_FOR_OVERRIDING_JOB_CONFIG_VALUES,
         )
         self.parser.add_argument(
             *CLI_ARGUMENTS[OUTPUT_FILE_LIST],
             dest=OUTPUT_FILE_LIST,
             default=None,
             type=str,
             nargs="+",
@@ -420,16 +445,17 @@
         )
         self.parser.add_argument(
             *CLI_ARGUMENTS[STORAGE_GIB],
             dest=STORAGE_GIB,
             default=None,
             type=int,
             metavar="STORAGE_GIB",
-            help="The total size of local SSD storage required to support the execution of each task. "
-            + f"Format: Integer. Range: [1, 65536]. {USED_FOR_OVERRIDING_JOB_CONFIG_VALUES}",
+            help="The total size of local SSD storage required to support the execution of each task "
+            f"{IF_IS_SINGLE_THREADED_NOTE}. Format: Integer. "
+            "Range: [1, 65536]. " + USED_FOR_OVERRIDING_JOB_CONFIG_VALUES,
         )
         self.parser.add_argument(
             *CLI_ARGUMENTS[IS_SUBJECT_TO_AVAILABLE_RESOURCES],
             dest=IS_SUBJECT_TO_AVAILABLE_RESOURCES,
             default=None,
             type=str,
             choices=["true", "false"],
@@ -487,48 +513,102 @@
             type=float,
             metavar=FovusCliArgumentParserUtil.camel_to_snake(WALLTIME_HOURS).upper(),
             help="The maximum time each task is allowed to run. A task will be terminated without a condition "
             + "once the walltime timer expires. Format: Real (e.g., 1.5). Range: >0. "
             + USED_FOR_OVERRIDING_JOB_CONFIG_VALUES,
         )
 
+        # Development overrides
+        self.parser.add_argument(
+            *CLI_ARGUMENTS[CLIENT_ID],
+            dest=CLIENT_ID,
+            default=None,
+            type=str,
+            metavar=FovusCliArgumentParserUtil.camel_to_snake(CLIENT_ID).upper(),
+            help="Cognito client ID.",
+        )
+        self.parser.add_argument(
+            *CLI_ARGUMENTS[DOMAIN_NAME],
+            dest=DOMAIN_NAME,
+            default=None,
+            type=str,
+            metavar=FovusCliArgumentParserUtil.camel_to_snake(DOMAIN_NAME).upper(),
+            help="Fovus API endpoint.",
+        )
+        self.parser.add_argument(
+            *CLI_ARGUMENTS[USER_POOL_ID],
+            dest=USER_POOL_ID,
+            default=None,
+            type=str,
+            metavar=FovusCliArgumentParserUtil.camel_to_snake(USER_POOL_ID).upper(),
+            help="Cognito user pool ID.",
+        )
+
     def parse_args(self):
+        self._confirm_args_are_valid()
         args = self.parser.parse_args()
         self.args_dict = vars(args)
         self._convert_boolean_args_to_bool()
         FovusCliArgumentParserUtil.set_timestamp(self.args_dict)
 
+    def _confirm_args_are_valid(self):
+        for arg in sys.argv:
+            if arg in CLI_ARGUMENTS[USERNAME]:
+                raise UserException(
+                    HTTPStatus.BAD_REQUEST,
+                    self.__class__.__name__,
+                    f"Arguments {CLI_ARGUMENTS[USERNAME]} are no longer supported. "
+                    f"Please use {CLI_ARGUMENTS[EMAIL]} instead.",
+                )
+
     def _convert_boolean_args_to_bool(self):
         for key in self.args_dict:
             if key in BOOLEAN_ARGS:
                 if self.args_dict[key] == "true":
                     self.args_dict[key] = True
                 elif self.args_dict[key] == "false":
                     self.args_dict[key] = False
 
     def get_args_dict(self):
         return self.args_dict
 
     def merge_args_with_config(self):
         for config_filepath in self._get_config_list():
-            with open(os.path.expanduser(config_filepath), encoding=UTF8) as file:
-                config = json.load(file)
-                for config_key in config:
-                    # Config file JSON keys are expected to be camelCase,
-                    # but all internal dictionary keys are snake_case.
-                    config_key_snake_case = FovusCliArgumentParserUtil.camel_to_snake(config_key)
-                    if FovusCliArgumentParserUtil.key_isnt_password(
-                        config_key
-                    ) and self._should_add_config_entry_to_args_dict(config_key_snake_case):
-                        self.args_dict[config_key_snake_case] = config[config_key]
+            config = {}
+            if config_filepath == DEFAULT_USER_CONFIG_FILE_PATH:
+                config = FileUtil.get_default_user_config()
+            else:
+                with open(os.path.expanduser(config_filepath), encoding=UTF8) as file:
+                    config = json.load(file)
+
+            for config_key in config:
+                # Config file JSON keys are expected to be camelCase,
+                # but all internal dictionary keys are snake_case.
+                config_key_snake_case = FovusCliArgumentParserUtil.camel_to_snake(config_key)
+                if FovusCliArgumentParserUtil.key_isnt_password(
+                    config_key
+                ) and self._should_add_config_entry_to_args_dict(config_key_snake_case):
+                    self.args_dict[config_key_snake_case] = config[config_key]
 
     def _get_config_list(self):
         config_list = []
         for key in [USER_CONFIG_FILE_PATH]:
             if key in self.args_dict and self.args_dict[key]:
                 config_list.append(self.args_dict[key])
-        if os.path.exists(os.path.expanduser(DEFAULT_USER_CONFIG_FILE_PATH)):
+        if os.path.exists(os.path.expanduser(DEFAULT_USER_CONFIG_FILE_PATH)) and [
+            arg not in self.args_dict for arg in CLI_ARGUMENTS[USER_CONFIG_FILE_PATH]
+        ]:
             config_list.append(DEFAULT_USER_CONFIG_FILE_PATH)
         return config_list
 
     def _should_add_config_entry_to_args_dict(self, key):
         return not (key in self.args_dict and self.args_dict[key])
+
+    def update_overridden_configs(self):
+        for config in Config.editable_configs():
+            config_override = self.args_dict.get(config)
+            if config_override:
+                print(
+                    f"CLI override found for config: {config}. "
+                    f"Overriding default value of '{Config.get(config)}' with '{config_override}'."
+                )
+                Config.set(config, config_override)
```

## fovus/config/config.py

```diff
@@ -1,4 +1,31 @@
-# Prod
-DOMAIN_NAME = "https://api.fovus.co"
-DEFAULT_CLIENT_ID = "353su1970rpnfcigu09j9078c0"
-DEFAULT_USER_POOL_ID = "us-east-1_fVH5TjPp5"
+# Dev
+import copy
+from http import HTTPStatus
+
+from fovus.constants.cli_constants import CLIENT_ID, DOMAIN_NAME, USER_POOL_ID
+from fovus.exception.user_exception import UserException
+
+
+class Config:
+    __conf = {
+        # Prod
+        CLIENT_ID: "353su1970rpnfcigu09j9078c0",
+        DOMAIN_NAME: "https://api.fovus.co",
+        USER_POOL_ID: "us-east-1_fVH5TjPp5",
+    }
+    __setters = [DOMAIN_NAME, CLIENT_ID, USER_POOL_ID]
+
+    @staticmethod
+    def get(key):
+        return Config.__conf[key]
+
+    @staticmethod
+    def set(key, value):
+        if key in Config.__setters:
+            Config.__conf[key] = value
+        else:
+            raise UserException(HTTPStatus.INTERNAL_SERVER_ERROR, Config.__name__, f"Key '{key}' is not in Config.")
+
+    @staticmethod
+    def editable_configs():
+        return copy.copy(Config.__setters)
```

## fovus/constants/cli_action_runner_constants.py

```diff
@@ -1,2 +1,11 @@
+from fovus.constants.cli_constants import EMAIL, USERNAME
+
 GENERIC_SUCCESS = "Success!"
 OUTPUTS = "==== Outputs ===="
+
+USER_CONFIG_EMAIL_UPDATE_MESSAGE = (
+    f"Your config uses the {USERNAME} key instead of the {EMAIL} key or contains both. "
+    f"User configs should use the {EMAIL} key instead of the {USERNAME} key. "
+    f"\n\t- If both the {EMAIL} key and {USERNAME} key are present, the {EMAIL} key/value pair will be used. "
+    f"\n\t- This will not affect CLI behavior."
+)
```

## fovus/constants/cli_constants.py

```diff
@@ -1,35 +1,35 @@
 import os
 
-# Parsed argument keys.
-CLIENT_ID = "client_id"
+# Parsed argument keys
 CONFIGURE = "configure"
 CREATE_JOB_WITH_UPLOAD = "create_job_with_upload"
 DOWNLOAD_JOB_FILES = "download_job_files"
+EMAIL = "email"
 EXCLUDE_INPUT = "exclude_input"
 EXCLUDE_OUTPUT = "exclude_output"
 GET_JOB_CURRENT_STATUS = "get_job_current_status"
 INCLUDE_INPUT = "include_input"
 INCLUDE_OUTPUT = "include_output"
 JOB_CONFIG_FILE_PATH = "job_config_file_path"
 JOB_FILE_ROOT_DIRECTORY = "job_file_root_directory"
 JOB_ID = "job_id"
 JOB_NAME = "job_name"
 OPEN_CONFIG_FOLDER = "open_config_folder"
 TIMESTAMP = "timestamp"
 USERNAME = "username"
 USER_CONFIG_FILE_PATH = "user_config_file_path"
 USER_ID = "user_id"
-USER_POOL_ID = "user_pool_id"
 WORKSPACE_ID = "workspace_id"
 
-# Job config overrides.
+# Job config overrides
 BENCHMARKING_PROFILE_ID = "benchmarkingProfileId"
 BENCHMARKING_PROFILE_NAME = "benchmarkingProfileName"
 COMPUTING_DEVICE = "computingDevice"
+IS_SINGLE_THREADED_TASK = "isSingleThreadedTask"
 LICENSE_TIMEOUT_HOURS = "licenseTimeoutHours"
 MONOLITHIC_OVERRIDE = "monolithicOverride"
 MIN_GPU = "minGpu"
 MAX_GPU = "maxGpu"
 MIN_GPU_MEM_GIB = "minGpuMemGiB"
 MIN_VCPU = "minvCpu"
 MAX_VCPU = "maxvCpu"
@@ -44,56 +44,63 @@
 STORAGE_GIB = "storageGiB"
 IS_SUBJECT_TO_AVAILABLE_RESOURCES = "isSubjectToAvailableResources"
 ENABLE_HYPERTHREADING = "enableHyperthreading"
 SUPPORTED_CPU_ARCHITECTURES = "supportedCpuArchitectures"
 TIME_TO_COST_PRIORITY_RATIO = "timeToCostPriorityRatio"
 WALLTIME_HOURS = "walltimeHours"
 
-# Additional arguments (if required).
+# Development overrides
+CLIENT_ID = "clientId"
+DOMAIN_NAME = "domainName"
+USER_POOL_ID = "userPoolId"
+
+# Additional arguments (if required)
 MONOLITHIC_OVERRIDE_ADDITIONAL_ARGUMENTS = {
     "default": [],
     "action": "append",
     "nargs": 4,
     "metavar": ("VENDOR_NAME", "SOFTWARE_NAME", "LICENSE_FEATURE", "NEW_LICENSE_COUNT"),
 }
 
 # Argument groups
 BOOLEAN_ARGS = (
     SCALABLE_PARALLELISM,
     PARALLELISM_OPTIMIZATION,
     SCALING_OUT,
     IS_SUBJECT_TO_AVAILABLE_RESOURCES,
     ENABLE_HYPERTHREADING,
+    IS_SINGLE_THREADED_TASK,
 )
 
 # CLI arguments
 CLI_ARGUMENTS = {
-    CLIENT_ID: ("--client-id", "--clientId", "-cid"),
+    # Parsed argument keys
     CONFIGURE: ("--configure", "-c"),
     CREATE_JOB_WITH_UPLOAD: ("--create-job-with-upload", "--createJobWithUpload", "-cjwu"),
     DOWNLOAD_JOB_FILES: ("--download-job-files", "--downloadJobFiles", "-djf"),
+    EMAIL: ("--email", "-e"),
     EXCLUDE_INPUT: ("--exclude-input", "--excludeInput", "-ei"),
     EXCLUDE_OUTPUT: ("--exclude-output", "--excludeOutput", "-eo"),
     GET_JOB_CURRENT_STATUS: ("--get-job-current-status", "--getJobCurrentStatus", "-gjcs"),
     INCLUDE_INPUT: ("--include-input", "--includeInput", "-ii"),
     INCLUDE_OUTPUT: ("--include-output", "--includeOutput", "-io"),
     JOB_CONFIG_FILE_PATH: ("--job-config-file-path", "--jobConfigFilePath", "-jcfp"),
     JOB_FILE_ROOT_DIRECTORY: ("--job-file-root-directory", "--jobFileRootDirectory", "-jfdr"),
     OPEN_CONFIG_FOLDER: ("--open-config-folder", "--openConfigFolder", "-ocf"),
     USERNAME: ("--username", "-u"),
     USER_CONFIG_FILE_PATH: ("--user-config-file-path", "--userConfigFilePath", "-ucfp"),
     USER_ID: ("--user-id", "--userId", "-uid"),
-    USER_POOL_ID: ("--user-pool-id", "--userPoolId", "-upi"),
     WORKSPACE_ID: ("--workspace-id", "--workspaceId", "-wid"),
-    # Job config overrides.
+    # Job config overrides
     BENCHMARKING_PROFILE_ID: ("--benchmarking-profile-id", "--benchmarkingProfileId", "-bpi"),
     BENCHMARKING_PROFILE_NAME: ("--benchmarking-profile-name", "--benchmarkingProfileName", "-bpn"),
     COMPUTING_DEVICE: ("--computing-device", "--computingDevice", "-cd"),
     JOB_NAME: ("--job-name", "--jobName", "-jn"),
     JOB_ID: ("--job-id", "--jobId", "-jid"),
+    IS_SINGLE_THREADED_TASK: ("--is-single-threaded-task", "--isSingleThreadedTask", "-istt"),
     LICENSE_TIMEOUT_HOURS: ("--license-timeout-hours", "--licenseTimeoutHours", "-lth"),
     MONOLITHIC_OVERRIDE: ("--monolithic-override", "--monolithicOverride", "-mo"),
     MIN_GPU: ("--min-gpu", "--minGpu"),
     MAX_GPU: ("--max-gpu", "--maxGpu"),
     MIN_GPU_MEM_GIB: ("--min-gpu-mem-gib", "--minGpuMemGiB", "-mgpuMemGiB"),
     MIN_VCPU: ("--min-vcpu", "--minvCpu", "--min-cpu"),
     MAX_VCPU: ("--max-vcpu", "--maxvCpu", "--max-cpu"),
@@ -111,14 +118,18 @@
         "--isSubjectToAvailableResources",
         "-istar",
     ),
     ENABLE_HYPERTHREADING: ("--enable-hyperthreading", "--enableHyperthreading", "--hyperthreading", "-ht"),
     SUPPORTED_CPU_ARCHITECTURES: ("--supported-cpu-architectures", "--supportedCpuArchitectures", "-sca"),
     TIME_TO_COST_PRIORITY_RATIO: ("--time-to-cost-priority-ratio", "--timeToCostPriorityRatio", "-tcr"),
     WALLTIME_HOURS: ("--walltime-hours", "--walltimeHours", "-wh"),
+    # Development overrides
+    CLIENT_ID: ("--client-id", "--clientId", "-cid"),
+    DOMAIN_NAME: ("--domain-name", "--domainName", "-dn"),
+    USER_POOL_ID: ("--user-pool-id", "--userPoolId", "-upi"),
 }
 
 CONFLICTING_CLI_ARGUMENT_SETS = [
     (
         CONFIGURE,
         OPEN_CONFIG_FOLDER,
         CREATE_JOB_WITH_UPLOAD,
@@ -128,14 +139,15 @@
     (INCLUDE_INPUT, EXCLUDE_INPUT),
     (INCLUDE_OUTPUT, EXCLUDE_OUTPUT),
 ]
 
 # Job types
 CPU = "cpu"
 GPU = "cpu+gpu"
+GPU_INTERNAL_REPRESENTATION = "gpu"
 
 PASSWORD_ENVIRONMENT_VARIABLE_KEY = "FOVUS_CLI_PASSWORD"  # nosec
 PATH_TO_CONFIG_ROOT = os.path.join(os.path.expanduser("~"), ".fovus")
 PATH_TO_JOB_CONFIGS = os.path.join(PATH_TO_CONFIG_ROOT, "job_configs")
 PATH_TO_USER_CONFIGS = os.path.join(PATH_TO_CONFIG_ROOT, "user_configs")
 PATH_TO_JOB_LOGS = os.path.join(PATH_TO_CONFIG_ROOT, "job_logs")
 UNIX_OPEN = "open"
```

## fovus/constants/fovus_api_constants.py

```diff
@@ -1,56 +1,56 @@
 # API
-from fovus.config.config import DOMAIN_NAME
-from fovus.constants.cli_constants import MAX_VCPU, MIN_VCPU
+from enum import Enum
+
+from fovus.constants.cli_constants import (
+    CPU,
+    GPU,
+    GPU_INTERNAL_REPRESENTATION,
+    MAX_VCPU,
+    MIN_VCPU,
+)
 
 COGNITO_REGION = "us-east-1"
 TIMEOUT_SECONDS = 10
 
-# API
-JOB = "job"
-FILE = "file"
-SOFTWARE = "software"
-BENCHMARK = "benchmark"
-__APIS = {
-    JOB: DOMAIN_NAME + "/job",
-    FILE: DOMAIN_NAME + "/file",
-    SOFTWARE: DOMAIN_NAME + "/software",
-    BENCHMARK: DOMAIN_NAME + "/benchmark",
-}
 
-CREATE_JOB = "CREATE_JOB"
-GET_JOB_INFO = "GET_JOB_STATUS"
+# API: Access through FovusApiUtil.get_api_address function to allow domain override via CLI.
+class Api(Enum):
+    JOB = "job"
+    FILE = "file"
+    SOFTWARE = "software"
+    BENCHMARK = "benchmark"
 
-GET_FILE_DOWNLOAD_TOKEN = "GET_FILE_DOWNLOAD_TOKEN"  # nosec
-GET_FILE_UPLOAD_TOKEN = "GET_FILE_UPLOAD_TOKEN"  # nosec
 
-LIST_SOFTWARE = "LIST_SOFTWARE"
+class ApiMethod(Enum):
+    CREATE_JOB = "create-job"
+    GET_JOB_INFO = "get-job-info"
+    GET_FILE_DOWNLOAD_TOKEN = "get-file-download-token"  # nosec
+    GET_FILE_UPLOAD_TOKEN = "get-file-upload-token"  # nosec
+    LIST_SOFTWARE = "list-software"
+    LIST_BENCHMARK_PROFILE = "list-benchmark-profile"
 
-LIST_BENCHMARK_PROFILE = "LIST_BENCHMARK_PROFILE"
-
-APIS = {
-    JOB: {CREATE_JOB: __APIS[JOB] + "/create-job", GET_JOB_INFO: __APIS[JOB] + "/get-job-info"},
-    FILE: {
-        GET_FILE_DOWNLOAD_TOKEN: __APIS[FILE] + "/get-file-download-token",
-        GET_FILE_UPLOAD_TOKEN: __APIS[FILE] + "/get-file-upload-token",
-    },
-    SOFTWARE: {
-        LIST_SOFTWARE: __APIS[SOFTWARE] + "/list-software",
-    },
-    BENCHMARK: {LIST_BENCHMARK_PROFILE: __APIS[BENCHMARK] + "/list-benchmark-profile"},
-}
 
 # Benchmarking
 BOUNDS_TO_SCALE = (MIN_VCPU, MAX_VCPU)
 BOUND_VALUE_CORRECTION_PRINT_ORDER = ("minvCpu", "maxvCpu", "minvCpuMemGiB", "minGpu", "maxGpu", "minGpuMemGiB")
+X86_64 = "x86-64"
+SUPPORTED_ARCHITECTURES = {
+    CPU: (X86_64,),
+}
+COMPUTING_DEVICE_TO_BP_COMPUTING_DEVICE = {
+    CPU: CPU,
+    GPU: GPU_INTERNAL_REPRESENTATION,
+}
 
 # Payload
 AUTHORIZATION_HEADER = "Authorization"
 CONTAINERIZED = "containerized"
 ENVIRONMENT = "environment"
+LICENSE_ADDRESS = "licenseAddress"
 LICENSE_COUNT_PER_TASK = "licenseCountPerTask"
 LICENSE_FEATURE = "licenseFeature"
 MONOLITHIC_LIST = "monolithicList"
 PAYLOAD_CONSTRAINTS = "constraints"
 PAYLOAD_JOB_CONSTRAINTS = "jobConstraints"
 PAYLOAD_JOB_NAME = "jobName"
 PAYLOAD_TASK_CONSTRAINTS = "taskConstraints"
@@ -60,12 +60,15 @@
 SOFTWARE_NAME = "softwareName"
 SOFTWARE_VERSION = "softwareVersion"
 STATUS_CODE = "statusCode"
 VENDOR_NAME = "vendorName"
 
 # Response
 BODY = "body"
+GPU_RANGE = "gpuRange"
 BP_HYPERTHREADING = "bpHyperthreading"
+SUPPORTED_PROCESSOR_ARCHITECTURES = "supportedProcessorArchitectures"
 ERROR_MESSAGE = "errorMessage"
+IS_LICENSE_REQUIRED = "isLicenseRequired"
 JOB_STATUS = "jobStatus"
 SOFTWARE_MAP = "softwareMap"
 SOFTWARE_VERSIONS = "softwareVersions"
```

## fovus/fovus_provided_configs/FOVUS_example_job_config_containerized.json

### Pretty-printed

 * *Similarity: 0.9962121212121212%*

 * *Differences: {"'constraints'": "{'taskConstraints': {'isSingleThreadedTask': False}}"}*

```diff
@@ -8,14 +8,15 @@
             "supportedCpuArchitectures": [
                 "x86-64",
                 "arm-64"
             ],
             "timeToCostPriorityRatio": "0.9/0.1"
         },
         "taskConstraints": {
+            "isSingleThreadedTask": false,
             "maxGpu": 0,
             "maxvCpu": 192,
             "minGpu": 0,
             "minGpuMemGiB": 0,
             "minvCpu": 1,
             "minvCpuMemGiB": 1,
             "parallelismOptimization": false,
```

## fovus/fovus_provided_configs/FOVUS_example_job_config_monolithic.json

### Pretty-printed

 * *Similarity: 0.9962121212121212%*

 * *Differences: {"'constraints'": "{'taskConstraints': {'isSingleThreadedTask': False}}"}*

```diff
@@ -9,14 +9,15 @@
             "supportedCpuArchitectures": [
                 "x86-64",
                 "arm-64"
             ],
             "timeToCostPriorityRatio": "0.9/0.1"
         },
         "taskConstraints": {
+            "isSingleThreadedTask": false,
             "maxGpu": 0,
             "maxvCpu": 192,
             "minGpu": 0,
             "minGpuMemGiB": 0,
             "minvCpu": 1,
             "minvCpuMemGiB": 1,
             "parallelismOptimization": false,
```

## fovus/fovus_provided_configs/FOVUS_job_template_containerized.json

### Pretty-printed

 * *Similarity: 0.9962121212121212%*

 * *Differences: {"'constraints'": "{'taskConstraints': {'isSingleThreadedTask': False}}"}*

```diff
@@ -7,14 +7,15 @@
             "isSubjectToAvailableResources": false,
             "supportedCpuArchitectures": [
                 ""
             ],
             "timeToCostPriorityRatio": ""
         },
         "taskConstraints": {
+            "isSingleThreadedTask": false,
             "maxGpu": 0,
             "maxvCpu": 192,
             "minGpu": 0,
             "minGpuMemGiB": 0,
             "minvCpu": 1,
             "minvCpuMemGiB": 1,
             "parallelismOptimization": false,
```

## fovus/fovus_provided_configs/FOVUS_job_template_monolithic.json

### Pretty-printed

 * *Similarity: 0.9962121212121212%*

 * *Differences: {"'constraints'": "{'taskConstraints': {'isSingleThreadedTask': False}}"}*

```diff
@@ -8,14 +8,15 @@
             "licenseTimeoutHours": 1,
             "supportedCpuArchitectures": [
                 ""
             ],
             "timeToCostPriorityRatio": ""
         },
         "taskConstraints": {
+            "isSingleThreadedTask": false,
             "maxGpu": 0,
             "maxvCpu": 192,
             "minGpu": 0,
             "minGpuMemGiB": 0,
             "minvCpu": 1,
             "minvCpuMemGiB": 1,
             "parallelismOptimization": false,
```

## fovus/fovus_provided_configs/FOVUS_user_config_template.json

### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'email'": "''", 'delete': "['username']"}*

```diff
@@ -1,4 +1,4 @@
 {
-    "username": "",
+    "email": "",
     "workspaceId": ""
 }
```

## fovus/schema/create_job_schema.json

### Pretty-printed

 * *Similarity: 0.9999983258928571%*

 * *Differences: {"'properties'": "{'environment': {'properties': {'monolithicList': {'items': {'required': "*

 * *                 "{delete: [4, 3, 2]}}}}}, 'constraints': {'properties': {'jobConstraints': "*

 * *                 "{'properties': {'supportedCpuArchitectures': {'items': {delete: ['enum']}}}}}}}"}*

```diff
@@ -51,18 +51,14 @@
                             ],
                             "title": "The isSubjectToAvailableResources Schema.",
                             "type": "boolean"
                         },
                         "supportedCpuArchitectures": {
                             "default": [],
                             "items": {
-                                "enum": [
-                                    "x86-64",
-                                    "arm-64"
-                                ],
                                 "examples": [
                                     [
                                         "x86-64"
                                     ],
                                     [
                                         "x86-64",
                                         "arm-64"
@@ -321,18 +317,15 @@
                                 ],
                                 "title": "The vendorName Schema",
                                 "type": "string"
                             }
                         },
                         "required": [
                             "softwareName",
-                            "softwareVersion",
-                            "licenseAddress",
-                            "licenseFeature",
-                            "licenseCountPerTask"
+                            "softwareVersion"
                         ],
                         "title": "A Schema",
                         "type": "object"
                     },
                     "title": "The monolithicList Schema",
                     "type": "array"
                 }
```

## fovus/util/file_util.py

```diff
@@ -1,12 +1,16 @@
 import fnmatch
 import hashlib
+import json
 import os
 from http import HTTPStatus
 
+from fovus.constants.cli_action_runner_constants import USER_CONFIG_EMAIL_UPDATE_MESSAGE
+from fovus.constants.cli_constants import DEFAULT_USER_CONFIG_FILE_PATH, EMAIL, USERNAME
+from fovus.constants.util_constants import UTF8
 from fovus.exception.user_exception import UserException
 from fovus.util.util import Util
 
 FOVUS_JOB_INFO_FOLDER = ".fovus"
 
 
 class FileUtil:
@@ -115,7 +119,25 @@
         for directory in directories:
             local_directory_path = os.path.join(local_root_directory_path, directory)
             os.makedirs(local_directory_path, exist_ok=True)
 
     @staticmethod
     def windows_to_unix_path(path):
         return path.replace("\\", "/")
+
+    @staticmethod
+    def get_default_user_config():
+        default_user_config = {}
+        with open(DEFAULT_USER_CONFIG_FILE_PATH, encoding=UTF8) as file:
+            default_user_config = json.load(file)
+        if USERNAME in default_user_config:
+            print(
+                f"{USER_CONFIG_EMAIL_UPDATE_MESSAGE}"
+                "\nSince the user config being used is the default config, "
+                f"automatically updating the {USERNAME} key to the {EMAIL} key. "
+                f"\n\t- If both {EMAIL} and {USERNAME} are present, the {EMAIL} key/value pair will be kept and "
+                f"the {USERNAME} key/value pair will be removed."
+            )
+            Util.keep_prioritized_key_value_in_dict(default_user_config, prioritized_key=EMAIL, fallback_key=USERNAME)
+            with open(DEFAULT_USER_CONFIG_FILE_PATH, "w", encoding=UTF8) as file:
+                json.dump(default_user_config, file, indent=4, sort_keys=True)
+        return default_user_config
```

## fovus/util/fovus_api_util.py

```diff
@@ -1,38 +1,47 @@
 import operator
 from http import HTTPStatus
 
 import boto3
 
+from fovus.config.config import Config
 from fovus.constants.benchmark_constants import (
+    BENCHMARK_NAME,
     BOUNDS,
     CORRECTABLE_COMPARISON,
     CORRECTABLE_LIST_COMPREHENSION,
     DEFAULT_BOOLEANS_TO_VALIDATE,
     DEFAULT_LOWER_BOUNDS_TO_VALIDATE,
     DEFAULT_UPPER_BOUNDS_TO_VALIDATE,
     GPU_LOWER_BOUNDS_TO_VALIDATE,
     GPU_UPPER_BOUNDS_TO_VALIDATE,
     INCORRECTABLE_COMPARISON,
     INCORRECTABLE_LIST_COMPREHENSION,
     LIST_BENCHMARKING_FIELD_BY_CREATE_JOB_REQUEST_FIELD,
 )
 from fovus.constants.cli_constants import (
     COMPUTING_DEVICE,
+    CPU,
+    DOMAIN_NAME,
     GPU,
     JOB_ID,
+    SUPPORTED_CPU_ARCHITECTURES,
     TIMESTAMP,
     USER_ID,
 )
 from fovus.constants.fovus_api_constants import (
     BOUNDS_TO_SCALE,
     ERROR_MESSAGE,
+    GPU_RANGE,
     PAYLOAD_CONSTRAINTS,
     PAYLOAD_JOB_CONSTRAINTS,
     STATUS_CODE,
+    SUPPORTED_PROCESSOR_ARCHITECTURES,
+    Api,
+    ApiMethod,
 )
 from fovus.constants.util_constants import (
     SERVER_ERROR_PREFIX,
     SUCCESS_STATUS_CODES,
     USER_ERROR_PREFIX,
 )
 from fovus.exception.system_exception import SystemException
@@ -174,7 +183,73 @@
             f"{bound_to_validate} is {benchmarking_profile_item_bound}"
         )
         if bound_to_validate in BOUNDS_TO_SCALE:
             hyperthreading_enabled_print = "enabled" if hyperthreading_enabled else "disabled"
             message += f" given that hyperthreading is {hyperthreading_enabled_print}"
         message += f". Overriding current value of {current_value} with " f"{benchmarking_profile_item_bound}."
         return message
+
+    @staticmethod
+    def validate_computing_device(input_computing_device, benchmarking_profile_item):
+        computing_device_should_be = ""
+        if (
+            GPU_RANGE not in benchmarking_profile_item or not benchmarking_profile_item[GPU_RANGE]
+        ) and input_computing_device == GPU:
+            computing_device_should_be = CPU
+        if (
+            GPU_RANGE in benchmarking_profile_item and benchmarking_profile_item[GPU_RANGE]
+        ) and input_computing_device == CPU:
+            computing_device_should_be = GPU
+
+        if computing_device_should_be:
+            raise UserException(
+                HTTPStatus.BAD_REQUEST,
+                FovusApiUtil.__name__,
+                f"Invalid value for {COMPUTING_DEVICE}. "
+                + FovusApiUtil.get_formatted_benchmark_supported_message(
+                    benchmarking_profile_item[BENCHMARK_NAME], "computing devices", [computing_device_should_be]
+                ),
+            )
+
+    @staticmethod
+    def validate_cpu_architectures(input_cpu_architectures, benchmarking_profile_item):
+        supported_architectures = []
+        valid_input_cpu_architectures = []
+        for supported_computing_device_and_architecture in benchmarking_profile_item[SUPPORTED_PROCESSOR_ARCHITECTURES]:
+            supported_architecture = supported_computing_device_and_architecture.split("-", maxsplit=1)[1]
+            supported_architectures.append(supported_architecture)
+            if supported_architecture in input_cpu_architectures:
+                valid_input_cpu_architectures.append(supported_architecture)
+
+        if valid_input_cpu_architectures:
+            if len(valid_input_cpu_architectures) < len(input_cpu_architectures):
+                print(
+                    f"Create job request contains values for {SUPPORTED_CPU_ARCHITECTURES} not supported by the "
+                    f"benchmarking profile {benchmarking_profile_item[BENCHMARK_NAME]}. "
+                    f"\n\t- "
+                    + FovusApiUtil.get_formatted_benchmark_supported_message(
+                        benchmarking_profile_item[BENCHMARK_NAME], "CPU architectures", supported_architectures
+                    )
+                    + f"\n\t- The following request values have been removed: "
+                    f"{list(set(input_cpu_architectures) - set(valid_input_cpu_architectures))}"
+                )
+            return
+
+        raise UserException(
+            HTTPStatus.BAD_REQUEST,
+            FovusApiUtil.__name__,
+            f"Invalid value of {SUPPORTED_CPU_ARCHITECTURES}. "
+            + FovusApiUtil.get_formatted_benchmark_supported_message(
+                benchmarking_profile_item[BENCHMARK_NAME], "CPU architectures", supported_architectures
+            ),
+        )
+
+    @staticmethod
+    def get_formatted_benchmark_supported_message(benchmark_name, field_readable, supported_values: tuple):
+        return (
+            f"The benchmarking profile '{benchmark_name}' only supports the "
+            f"following {field_readable}: {supported_values}."
+        )
+
+    @staticmethod
+    def get_api_address(api: Api, api_method: ApiMethod):
+        return "/".join((Config.get(DOMAIN_NAME), api.value, api_method.value))
```

## fovus/util/fovus_cli_argument_parser_util.py

```diff
@@ -15,15 +15,17 @@
     def validate_password_exists():
         if not os.environ.get(PASSWORD_ENVIRONMENT_VARIABLE_KEY):
             raise UserException(
                 HTTPStatus.BAD_REQUEST,
                 FovusCliArgumentParserUtil.__name__,
                 f"Password must be set in environment variable {PASSWORD_ENVIRONMENT_VARIABLE_KEY}."
                 + "\nTo set on Unix-based systems, run the following command: "
-                + f'export {PASSWORD_ENVIRONMENT_VARIABLE_KEY}="your_password_here"'
+                + f"export {PASSWORD_ENVIRONMENT_VARIABLE_KEY}='your_password_here'"
+                + "\n\t- If you are using a Unix-based system and your password contains a single quote ('), "
+                + "replace all instances of the single quote with the following character sequence: '''"
                 + "\nTo set on Windows, run the following command then close and reopen command prompt: "
                 + f'setx {PASSWORD_ENVIRONMENT_VARIABLE_KEY} "your_password_here"',
             )
 
     @staticmethod
     def get_password():
         return os.environ.get(PASSWORD_ENVIRONMENT_VARIABLE_KEY)
```

## fovus/util/util.py

```diff
@@ -19,7 +19,13 @@
     @staticmethod
     def is_unix():
         return os.name == UNIX_OS_NAME
 
     @staticmethod
     def is_windows():
         return os.name == WINDOWS_OS_NAME
+
+    @staticmethod
+    def keep_prioritized_key_value_in_dict(dictionary, prioritized_key, fallback_key):
+        if not dictionary.get(prioritized_key):
+            dictionary[prioritized_key] = dictionary[fallback_key]
+        del dictionary[fallback_key]
```

## fovus/validator/fovus_api_validator.py

```diff
@@ -13,27 +13,28 @@
     SCALABLE_PARALLELISM,
 )
 from fovus.constants.fovus_api_constants import (
     PAYLOAD_CONSTRAINTS,
     PAYLOAD_JOB_CONSTRAINTS,
     PAYLOAD_TASK_CONSTRAINTS,
     PAYLOAD_TIME_COST_PRIORITY_RATIO,
+    ApiMethod,
 )
 from fovus.constants.util_constants import UTF8
 from fovus.exception.user_exception import UserException
 from fovus.root_config import ROOT_DIR
 
 SCHEMA_PATH_PREFIX = "schema/"
 SCHEMA_PATH_SUFFIX = "_schema.json"
 
 
 class FovusApiValidator:  # pylint: disable=too-few-public-methods
-    def __init__(self, payload, api_method):
+    def __init__(self, payload, api_method: ApiMethod):
         self.payload = payload
-        self.api_method = api_method
+        self.api_method = api_method.value.replace("-", "_")
 
     def validate(self):
         self._validate_schema()
         self._validate_time_cost_to_priority_ratio()
         self._validate_parallelism_optimization_allowed_value()
         self._validate_min_max_vcpu()
         self._validate_min_max_gpu()
```

## Comparing `fovus-1.0.5.dist-info/LICENSE.txt` & `fovus-1.0.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fovus-1.0.5.dist-info/METADATA` & `fovus-1.0.6.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fovus
-Version: 1.0.5
+Version: 1.0.6
 Summary: The Fovus Python CLI
 Author: Fovus Corporation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: boto3 (>=1.26.60)
 Requires-Dist: jsonschema (>=3.2.0)
@@ -27,14 +27,20 @@
 Requires-Dist: pydocstringformatter ; extra == 'dev'
 Requires-Dist: pylint ; extra == 'dev'
 Requires-Dist: pyupgrade ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage ; extra == 'test'
 
+## Getting Started with Fovus CLI
+
+The official CLI tool for interacting with the Fovus Serverless HPC SaaS. Installation, setup, and usage documentation is provided here. Further detail is available via the CLI `--help` command or at our [CLI documentation website](https://fovus.github.io/).
+
+Features include job creation (with validation), job status checking, and job file downloading. In addition, reusable job and user configurations with optional command-line overriding are supported. Additional features are detailed in this README and in our help documentation (linked above).
+
 ## Installation
 
 ### Prerequisites
 
 1. Python and pip installation: https://www.python.org/downloads/
     1. Click the "Download Python" button.
     2. If you have an option of installing pip, select that option. (This should be the default.)
@@ -55,45 +61,57 @@
 
 ### User config
 
 A user config is for a pre-existing user that is *already set up in the Fovus web UI*.
 
 The following values can be viewed on the Fovus web UI by clicking on your profile icon in the top right of the page:
 
-- `username`: the email address used for your account.
-- `workspaceId`: the ID for the workspace you would like to use. The workspace ID can be found by clicking on the user icon in the web UI. 
+- `email`: the email address used for your account.
+- `workspaceId`: the ID for the workspace you would like to use. The workspace ID can be found by clicking on the user icon in the web UI.
 
 Set up your CLI user config with the following command:
 
 ```
 fovus --configure
 ```
 
 Note:
 
 1. This user config will save to `~/.fovus/user_configs/FOVUS_default_user_config.json`.
 2. To view all your configs, use `fovus --open-config-folder`.
 3. The user config can also be provided in the following ways (these will override default user config):
-    1. Using the following parameters: `--username your_username` and `--workspace-id your_workspace_id`.
+    1. Using the following parameters: `--email your_email` and `--workspace-id your_workspace_id`.
     2. Using the following parameter: `--user-config-file-path /path/to/your/user_config.json`
 
 ### Password environment variable
 
 Export your Fovus password as an environment variable by following the instructions for your system:
 
 Unix-based systems
 ```
 export FOVUS_CLI_PASSWORD='your_password_here'
 ```
 
+Note: if you are using a Unix-based system and your password contains a single quote `'`,
+replace all instances of the single quote `'` with the following character sequence: `'\''`.
+
 Windows
 
 1. Run `setx FOVUS_CLI_PASSWORD "your_password_here"` in command prompt
 2. Close your command prompt and open a new one (to refresh the environment variables)
 
+### Post-installation setup
+
+Run `fovus --configure` and follow the prompts. If this results in an error, see below for common errors
+
+#### Windows - Python can't find script
+
+1. Run `echo %USERPROFILE%\AppData\Roaming\Python\PythonXX\Scripts`, replacing `PythonXX` with your version (can find using `python--version`). For example, if your python version is 3.11.2, replace `PythonXX` with `Python311`
+2. Run `setx PATH "%PATH%;C:\path\to\scripts"`, replacing `C:\path\to\scripts` with the modified output from step 1.
+3. Close and reopen your command prompt.
 
 ## Basic usage
 
 See the "Advanced Usage" section for additional options regarding file inclusion/exclusion for create job and download job files.
 
 ### Viewing your config files
 ```
@@ -103,29 +121,33 @@
 Note:
 
 1. Contains empty job and user config files for reference and copying.
 
 ### Creating jobs
 This command will upload files from the specified directory to Fovus and create a job.
 
-Upon job creation, a `.fovus` folder will be created in your local file root directory, which will contain a `job_data.json` file (i.e., `/path/to/job/file/root/directory/.fovus/job_data.json`. This json is used to facilitate checking job status and downloading job files by tracking the job's `jobID`.
+Upon job creation:
+
+1. The following will be validated: your job configuration structure (if provided as JSON), your job configuration values against your chosen benchmarking profile, and your software configurations (if job is monolithic).
+2. A `.fovus` folder will be created in your local file root directory, which will contain a `job_data.json` file (i.e., `/path/to/job/file/root/directory/.fovus/job_data.json`. This json is used to facilitate checking job status and downloading job files by tracking the job's `jobID`.
 
 ```
 fovus --create-job --job-config-file-path "/path/to/job/config/file.json" --job-file-root-directory "/path/to/job/file/root/directory"
 ```
 
 Note:
 
 1. To create your own job template, do the following:
     1. Open the fovus config folder with `--open-config-folder`.
     2. Make a copy of either `~/.fovus/job_configs/FOVUS_job_template_containerized.json` or `~/.fovus/job_configs FOVUS_job_template_monolithic.json`.
     3. ***IMPORTANT: rename your copy, or it will be overwritten.***
     4. Fill in the fields.
 2. Each subdirectory in your job file root directory will be treated as its own task.
-3. You can add the optional argument `--job-name "your_job_name_here"` to set a custom job name.
+    1. Spaces are not allowed in task directory names.
+4. You can add the optional argument `--job-name "your_job_name_here"` to set a custom job name.
 
 ### Getting job status
 
 If you created the job using the Fovus CLI on the same local machine (i.e., the `.fovus` folder was created in your job root directory -- see "Creating job" section for details):
 
 ```
 fovus --get-job-current-status --job-file-root-directory "/path/to/job/file/root/directory
@@ -151,15 +173,15 @@
 
 ```
 fovus --download-job-files --job-file-root-directory "/path/to/job/file/root/directory" --job-id "your_job_id"
 ```
 
 Note:
 
-1. Only new or updated files will be downloaded.
+1. Only new or updated files will be downloaded (checked using file hash).
 
 ## Advanced usage
 
 ### Include/Exclude file patterns
 
 When creating a job, the arguments `--include-input` and `--exclude-input` are available to you. These arguments are used to include/exclude filepaths for upload/download. Valid values for these arguments are alphanumeric along with the wildcards: * (matches any number of characters), ? (matches any single character).
 
@@ -204,17 +226,7 @@
 To do this, use the command `--monolithic-override "vendor_name" "software_name" "license_feature" "your_new_license_count_here"`.
 
 Note:
 
 1. The monolithicList object must already exist in the job config JSON.
 2. The vendor name, software name, and license feature are used to reference the specific object within the list and do not override existing values.
 3. If an object that does not match the given vendor name, software name, and license feature does not exist, an error will be thrown.
-
-## Troubleshooting
-
-### Windows - Python can't find script
-
-Windows
-
-1. Run `echo %USERPROFILE%\AppData\Roaming\Python\PythonXX\Scripts`, replacing `PythonXX` with your version (can find using `python--version`). For example, if my python version is 3.11.2, I will replace `PythonXX` with `Python311`
-2. Run `setx PATH "%PATH%;C:\path\to\scripts"`, replacing `C:\path\to\scripts` with the modified output from step 1.
-3. Close and reopen your command prompt.
```

## Comparing `fovus-1.0.5.dist-info/RECORD` & `fovus-1.0.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 fovus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/root_config.py,sha256=onsSNaAhzMvRK8o82IkASh4EVkyMxVMPBlUXcUq1Lcg,65
 fovus/adapter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/adapter/aws_cognito_adapter.py,sha256=RsqnPW2spH2DKn6mDf4cgbd3KwICANS4uL7vt0zo6k8,3331
-fovus/adapter/fovus_api_adapter.py,sha256=Y-NGC9vBM0gBJblxfYQfvqttacx7YOWATBT7YkcGkQM,19085
+fovus/adapter/fovus_api_adapter.py,sha256=3exODyU12GfxupKbm3QI4wwQ9f1KlULsgwFsBwyBsRI,22337
 fovus/adapter/fovus_s3_adapter.py,sha256=0O5IUT1WUk_i2GAoy_J3lZB0Onh4M2z6U-hX_lr1Lxs,8700
 fovus/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fovus/cli/cli_action_runner.py,sha256=o2SHIqdEOvUkhlUY-ZtoHacCEt3LzrY4HFCOLNrtOU8,13450
+fovus/cli/cli_action_runner.py,sha256=mLvAVdtUChtgNibFxVL1oRIHzkSjhPf6ZdHf6c7qU5s,13717
 fovus/cli/documenter.py,sha256=uzpu25Wd8YXirM7oQPLG3hqgAZa2_H_YPz0i522qxyo,161
-fovus/cli/fovus_cli.py,sha256=6YyqZ6-gzmH2eXVlwwbg-jl4P_lRJn77qx1_cG_432U,475
-fovus/cli/fovus_cli_argument_parser.py,sha256=OgTmDTokaquT9qIcnMDy3Z5Aco7xaLuNDnv6ru85Z9g,25911
+fovus/cli/fovus_cli.py,sha256=JGO28oDHjwO7E8-5f-di09eEmOVQbrfk8FrmLZkC-dk,997
+fovus/cli/fovus_cli_argument_parser.py,sha256=sZ8TuM7WshU0SXahb7TzzGXEaA5HnmNyWxr7vRW18fw,29103
 fovus/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fovus/config/config.py,sha256=LhikS-z0_0IL8uGJVDSf-HfPfq0a6_C3oOixw320sYM,138
+fovus/config/config.py,sha256=7pE82qidwfnY9lczL-rFoPq6jFP5Gp1LL5dGRZ2qeNY,840
 fovus/constants/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/constants/benchmark_constants.py,sha256=liNu-qvuo6VFfwud2upeYakuk9fVvSOe60EX0KyCdx0,1278
-fovus/constants/cli_action_runner_constants.py,sha256=k_k3fQ1SgcMpm3Gm12Mhii4DVh3-AlHKeJMh5MreeMs,59
-fovus/constants/cli_constants.py,sha256=1raw6jGzntHYdBEckvhU8gGuaNoOJ_jdLFYjZoVpRMY,8682
-fovus/constants/fovus_api_constants.py,sha256=so5TuaeO7r2ggQJwsUm1BReEtFxTI2lHlsna_92fcCI,2100
+fovus/constants/cli_action_runner_constants.py,sha256=PQkh9gznZCcc-cNtddO748WkLgPh6Rms9ug6ib0E7CE,485
+fovus/constants/cli_constants.py,sha256=Vj0870qgZuzIH6jUdrI8LD_QVwrOdfZH45OORnmYyeI,9096
+fovus/constants/fovus_api_constants.py,sha256=ECIlbBiP5jK-ab-nSLJDZ6cv0H50nLDD7plWKILooSI,2037
 fovus/constants/util_constants.py,sha256=tcIzvskdO_N9aYrNLLoqoASG76AVeiuexcfzG-IouPQ,194
 fovus/exception/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/exception/status_code_exception.py,sha256=HXfQ6E3gGSEg2dUxS6ccPN5kAgCC33nVzCuAy_zxN7o,291
 fovus/exception/system_exception.py,sha256=lzoDivDErUE47Cz3v9U1AhbzI4MQHTeYbvmn02myOHA,183
 fovus/exception/user_exception.py,sha256=Un3pq8s1a7gXdZ8MoHNhxE5xZz_fO4cBy4lE2n7uEzg,174
-fovus/fovus_provided_configs/FOVUS_example_job_config_containerized.json,sha256=FXKEiSlgg1-3NaDm5Sm0IuAJHyaTMV78yjwZ-PB651A,1054
-fovus/fovus_provided_configs/FOVUS_example_job_config_monolithic.json,sha256=S-wGqqE657jOq6ki83VeNcwefvIOtBnkZDgc5u-JGTk,1112
-fovus/fovus_provided_configs/FOVUS_job_template_containerized.json,sha256=SJ-7bWiZOvXf_p-2h7NsmU74ivi-watBe9KQnt-Hrzw,829
-fovus/fovus_provided_configs/FOVUS_job_template_monolithic.json,sha256=h9I-jDj6yktqpSFDMpHdDyuCxBYeSst9CibHZBzXKIA,1185
-fovus/fovus_provided_configs/FOVUS_user_config_template.json,sha256=HMCwX1ffMaUFonqxfv94c1ZlianfRTXal3BsYMxuRAE,42
+fovus/fovus_provided_configs/FOVUS_example_job_config_containerized.json,sha256=86akGvwLh-Ew_JYIMEEE_9AA6zsHhvYWezHn7n5ILsw,1145
+fovus/fovus_provided_configs/FOVUS_example_job_config_monolithic.json,sha256=6TbAK4Cx9bPg9Ugw_O1U-vpKhL9pH84-K49-Nki9YL8,1203
+fovus/fovus_provided_configs/FOVUS_job_template_containerized.json,sha256=KxaVEc8ilPa7tUV0wywMEKWqh6BCD8HkXBUm6r5kBYE,894
+fovus/fovus_provided_configs/FOVUS_job_template_monolithic.json,sha256=yAgBJioVl3p37H5C5XWCuqy3KZs59GQ7P3qu9lqxNOM,1250
+fovus/fovus_provided_configs/FOVUS_user_config_template.json,sha256=H7ePuIRbzYaTdL__NWh6XwRidLuN4Tue3yHY2lOArs4,39
 fovus/fovus_provided_configs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/schema/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fovus/schema/create_job_schema.json,sha256=rxVBkIytO6qvcLd_qmHtxkKJMvDb5SFFS33BUwOzSfQ,10183
+fovus/schema/create_job_schema.json,sha256=47IKcgmBu1y0j4edTW6LYnRvzTdy_hox99yuLkZe-k0,11652
 fovus/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/util/aws_util.py,sha256=KX6DJIkwZ8ruToI8O0fK0TYEVxfyZI-p3NkRSSbGuVg,3389
 fovus/util/cli_action_runner_util.py,sha256=cPVVedOavu7nO_bbRS8wlipc2PCB-Q94BAMV3aopOYo,334
-fovus/util/file_util.py,sha256=S_sE2yzOrIEyDy6BjBW615lGWzTNx6yLhhGcaChxRis,4625
-fovus/util/fovus_api_util.py,sha256=1xb-lo8toBwZ1Pm5PHJ6POJ-LMsDvFFom64tqRNCfOQ,7357
-fovus/util/fovus_cli_argument_parser_util.py,sha256=kuVUIibYr_9crVH34aX-MotOwj_KBBt8R_bbbrEmiIw,1740
+fovus/util/file_util.py,sha256=kMO8Sr5XV7zQHaYcpgPcR-dZw5SV-naL4V8GVJp2aRA,5858
+fovus/util/fovus_api_util.py,sha256=n_kOqBU78sUrKM8kU02ejxP-l9p239QrztI5p1U-b9M,10774
+fovus/util/fovus_cli_argument_parser_util.py,sha256=XRLoaMCulYzh_Ew85imIwcZwb-8bEYT_gIpiodjwOuo,1956
 fovus/util/fovus_s3_adapter_util.py,sha256=WQwqgaeVttAUTJ2MyO9KFXpaIsVFwzcUM3K6xZ5oeFU,1519
-fovus/util/util.py,sha256=i_mzAJDsIvvWEEOTVGYckYZInZe6EddwyJiiVQca7R4,533
+fovus/util/util.py,sha256=ij6HD8nFdmGiuVhYQdrq7lSt7zbUZVvs1W1ABdc4syo,791
 fovus/validator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fovus/validator/fovus_api_validator.py,sha256=3_epp3QpaRmDColc2u0NwpAC9ud-EhivAKLM5EW8hNA,3732
-fovus-1.0.5.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
-fovus-1.0.5.dist-info/METADATA,sha256=Zug2BVdRkvAdGdaaxRQD_Bz0eNLFpCLCvIVHuqOL0F0,8883
-fovus-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fovus-1.0.5.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
-fovus-1.0.5.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
-fovus-1.0.5.dist-info/RECORD,,
+fovus/validator/fovus_api_validator.py,sha256=6LL7RCBPUse_-a1MeZR6wulaUoUtg1Pj6Fpg_IuUtsU,3782
+fovus-1.0.6.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
+fovus-1.0.6.dist-info/METADATA,sha256=D_pn2Ew9Nb-FEyhVzmWdFUAEB6IDXkrRdU7qm3Pi_s0,10053
+fovus-1.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fovus-1.0.6.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
+fovus-1.0.6.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
+fovus-1.0.6.dist-info/RECORD,,
```

