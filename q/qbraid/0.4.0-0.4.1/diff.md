# Comparing `tmp/qbraid-0.4.0.tar.gz` & `tmp/qbraid-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-0.4.0.tar", last modified: Tue May 16 22:30:19 2023, max compression
+gzip compressed data, was "qbraid-0.4.1.tar", last modified: Thu Jun 15 21:38:37 2023, max compression
```

## Comparing `qbraid-0.4.0.tar` & `qbraid-0.4.1.tar`

### file list

```diff
@@ -1,272 +1,284 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.753776 qbraid-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-16 22:30:06.000000 qbraid-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 22:30:06.000000 qbraid-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 22:30:06.000000 qbraid-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-16 22:30:19.753776 qbraid-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-05-16 22:30:06.000000 qbraid-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.713776 qbraid-0.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.713776 qbraid-0.4.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.713776 qbraid-0.4.0/docs/_static/account/
--rw-r--r--   0 runner    (1001) docker     (123)    80371 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/account/account_access_key.png
--rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/account/account_profile_details.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.713776 qbraid-0.4.0/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.721776 qbraid-0.4.0/docs/_static/environments/
--rw-r--r--   0 runner    (1001) docker     (123)   358114 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_add.png
--rw-r--r--   0 runner    (1001) docker     (123)   236606 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_add_package.png
--rw-r--r--   0 runner    (1001) docker     (123)   112288 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_create.png
--rw-r--r--   0 runner    (1001) docker     (123)    41898 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_custom_installing.png
--rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_custom_pkgs.png
--rw-r--r--   0 runner    (1001) docker     (123)   497786 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_install.png
--rw-r--r--   0 runner    (1001) docker     (123)   450900 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_installing.png
--rw-r--r--   0 runner    (1001) docker     (123)   394044 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_more.png
--rw-r--r--   0 runner    (1001) docker     (123)   545265 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_new.png
--rw-r--r--   0 runner    (1001) docker     (123)   148896 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_pkg_install.png
--rw-r--r--   0 runner    (1001) docker     (123)    47510 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_share.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.721776 qbraid-0.4.0/docs/_static/errors/
--rw-r--r--   0 runner    (1001) docker     (123)   108308 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/errors/sidebar_glitch.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.721776 qbraid-0.4.0/docs/_static/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/0_file_control_panel.png
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/1_top_bar_token.png
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/2_request_token.png
--rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/3_copy_token.png
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/4_jupyter_server.png
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/5_existing_uri.png
--rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/6_example_user.png
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/7_notebook_kernel.png
--rw-r--r--   0 runner    (1001) docker     (123)    34868 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/8_select_kernel.png
--rw-r--r--   0 runner    (1001) docker     (123)    85020 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/os.png
--rw-r--r--   0 runner    (1001) docker     (123)    34944 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/vscode_graphic.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.721776 qbraid-0.4.0/docs/_static/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)   411673 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/jobs/jobs_ionq.png
--rw-r--r--   0 runner    (1001) docker     (123)   592257 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/jobs/jobs_sdk.png
--rw-r--r--   0 runner    (1001) docker     (123)    85873 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/jobs/jobs_tag.png
--rw-r--r--   0 runner    (1001) docker     (123)   154811 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.725776 qbraid-0.4.0/docs/_static/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/file_browser.png
--rw-r--r--   0 runner    (1001) docker     (123)   451731 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/kernel_activate.png
--rw-r--r--   0 runner    (1001) docker     (123)   510341 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/kernel_deactivate.png
--rw-r--r--   0 runner    (1001) docker     (123)   290430 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/kernel_nb.png
--rw-r--r--   0 runner    (1001) docker     (123)   346617 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/kernel_switch.png
--rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/share_notebook.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.725776 qbraid-0.4.0/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (123)    36600 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/braket.png
--rw-r--r--   0 runner    (1001) docker     (123)    53519 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/pyquil.png
--rw-r--r--   0 runner    (1001) docker     (123)    28492 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/pytket.png
--rw-r--r--   0 runner    (1001) docker     (123)   125852 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/qasm.png
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/qiskit.png
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/xanadu.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.729776 qbraid-0.4.0/docs/_static/sdk-files/
--rw-r--r--   0 runner    (1001) docker     (123)   447304 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/sdk-files/get_devices.png
--rw-r--r--   0 runner    (1001) docker     (123)    53194 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/sdk-files/plot_counts.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.729776 qbraid-0.4.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.devices.aws.rst
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.devices.ibm.rst
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_braket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_pyquil.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_pytket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_qiskit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.733776 qbraid-0.4.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/envs-activate.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/envs-list.rst
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/envs-uninstall.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/envs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs-add.rst
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs-disable.rst
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs-enable.rst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs-get-credits.rst
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs-list.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/kernels.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.733776 qbraid-0.4.0/docs/lab/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/account.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/environments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/integrations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/quantumjobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/system.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/troubleshoot.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.733776 qbraid-0.4.0/docs/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/sdk/circuits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/sdk/devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/sdk/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/sdk/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/sdk/results.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-16 22:30:06.000000 qbraid-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.737776 qbraid-0.4.0/qbraid/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/_qprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.737776 qbraid-0.4.0/qbraid/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/job_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.737776 qbraid-0.4.0/qbraid/api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/tests/test_api_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/tests/test_api_thirdparty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.737776 qbraid-0.4.0/qbraid/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/devices/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/aws/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/aws/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/aws/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/devices/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/devices/ibm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/tests/test_ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/status_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/devices/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/display_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/get_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/interface/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/calculate_unitary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/convert_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/programs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/interface/qbraid_braket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_braket/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_braket/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/interface/qbraid_cirq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_cirq/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_cirq/circuits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/interface/qbraid_cirq/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_cirq/tests/test_cirq_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_cirq/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/qbraid_pyquil/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pyquil/programs.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pyquil/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/qbraid_pytket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pytket/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pytket/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/qbraid_qasm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qasm/circuits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/qbraid_qasm/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qasm/test/test_qasm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qasm/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/qbraid_qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qiskit/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qiskit/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/tests/test_calculate_unitary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/tests/test_convert_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/tests/test_programs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/tests/test_top_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/transpiler/cirq_braket/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_from_braket_qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/custom_gates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/_gate_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_from_braket_qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_to_braket_measure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/tests/test_conversions_pyquil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_conversions_pytket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_to_pytket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/_gate_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/_gate_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_conversions_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_from_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_to_qiskit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/code/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/code/qasm_to_braket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/code/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/code/tests/test_qasm_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/custom_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/tests/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/abc_qprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/braket_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/cirq_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/pyquil_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/pytket_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/qasm_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/qiskit_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.737776 qbraid-0.4.0/qbraid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-16 22:30:06.000000 qbraid-0.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-16 22:30:06.000000 qbraid-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-16 22:30:19.753776 qbraid-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-16 22:30:06.000000 qbraid-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.753776 qbraid-0.4.0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-16 22:30:06.000000 qbraid-0.4.0/tools/verify_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-16 22:30:06.000000 qbraid-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.069667 qbraid-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-15 21:38:22.000000 qbraid-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 21:38:22.000000 qbraid-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-15 21:38:22.000000 qbraid-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-06-15 21:38:37.069667 qbraid-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-15 21:38:22.000000 qbraid-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.025667 qbraid-0.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.025667 qbraid-0.4.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.025667 qbraid-0.4.1/docs/_static/account/
+-rw-r--r--   0 runner    (1001) docker     (123)    80371 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/account/account_access_key.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/account/account_profile_details.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.029667 qbraid-0.4.1/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.033667 qbraid-0.4.1/docs/_static/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)   358114 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_add.png
+-rw-r--r--   0 runner    (1001) docker     (123)   236606 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_add_package.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112288 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_create.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41898 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_custom_installing.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_custom_pkgs.png
+-rw-r--r--   0 runner    (1001) docker     (123)   497786 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_install.png
+-rw-r--r--   0 runner    (1001) docker     (123)   450900 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_installing.png
+-rw-r--r--   0 runner    (1001) docker     (123)   394044 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_more.png
+-rw-r--r--   0 runner    (1001) docker     (123)   545265 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_new.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148896 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_pkg_install.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47510 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/environments/env_share.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.033667 qbraid-0.4.1/docs/_static/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)   108308 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/errors/sidebar_glitch.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.037667 qbraid-0.4.1/docs/_static/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/0_file_control_panel.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/1_top_bar_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/2_request_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/3_copy_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/4_jupyter_server.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/5_existing_uri.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/6_example_user.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/7_notebook_kernel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34868 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/8_select_kernel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85020 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/os.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34944 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/integrations/vscode_graphic.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.037667 qbraid-0.4.1/docs/_static/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)   411673 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/jobs/jobs_ionq.png
+-rw-r--r--   0 runner    (1001) docker     (123)   592257 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/jobs/jobs_sdk.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85873 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/jobs/jobs_tag.png
+-rw-r--r--   0 runner    (1001) docker     (123)   154811 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.041667 qbraid-0.4.1/docs/_static/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/notebooks/file_browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)   451731 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/notebooks/kernel_activate.png
+-rw-r--r--   0 runner    (1001) docker     (123)   510341 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/notebooks/kernel_deactivate.png
+-rw-r--r--   0 runner    (1001) docker     (123)   290430 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/notebooks/kernel_nb.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346617 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/notebooks/kernel_switch.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/notebooks/share_notebook.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.045667 qbraid-0.4.1/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36600 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/pkg-logos/braket.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53519 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/pkg-logos/pyquil.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28492 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/pkg-logos/pytket.png
+-rw-r--r--   0 runner    (1001) docker     (123)   125852 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/pkg-logos/qasm.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/pkg-logos/qiskit.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/pkg-logos/xanadu.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.045667 qbraid-0.4.1/docs/_static/sdk-files/
+-rw-r--r--   0 runner    (1001) docker     (123)   447304 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/sdk-files/get_devices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53194 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/_static/sdk-files/plot_counts.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.049667 qbraid-0.4.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.devices.aws.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.devices.ibm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.transpiler.cirq_braket.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.transpiler.cirq_pyquil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.transpiler.cirq_pytket.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.transpiler.cirq_qiskit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.transpiler.cirq_utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/api/qbraid.transpiler.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.053667 qbraid-0.4.1/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/envs-activate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/envs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/envs-uninstall.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/envs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/jobs-add.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/jobs-disable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/jobs-enable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/jobs-get-credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/jobs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/kernels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/cli/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.053667 qbraid-0.4.1/docs/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/lab/account.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/lab/environments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/lab/files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/lab/integrations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/lab/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/lab/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/lab/quantumjobs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/lab/system.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/lab/troubleshoot.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.053667 qbraid-0.4.1/docs/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/sdk/circuits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/sdk/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/sdk/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/sdk/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-15 21:38:22.000000 qbraid-0.4.1/docs/sdk/results.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-15 21:38:22.000000 qbraid-0.4.1/ecosystem.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-15 21:38:22.000000 qbraid-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.053667 qbraid-0.4.1/qbraid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/_qprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.057667 qbraid-0.4.1/qbraid/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/api/job_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/api/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/api/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.057667 qbraid-0.4.1/qbraid/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/api/tests/test_api_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/api/tests/test_api_thirdparty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.057667 qbraid-0.4.1/qbraid/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.057667 qbraid-0.4.1/qbraid/devices/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/aws/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/aws/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/aws/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.057667 qbraid-0.4.1/qbraid/devices/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/ibm/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/ibm/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/ibm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/ibm/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.057667 qbraid-0.4.1/qbraid/devices/ibm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/ibm/tests/test_ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/ionq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/status_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.057667 qbraid-0.4.1/qbraid/devices/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/tests/test_braket_ionq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/devices/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/display_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/get_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.057667 qbraid-0.4.1/qbraid/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/calculate_unitary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/convert_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/programs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/interface/qbraid_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_braket/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_braket/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/interface/qbraid_cirq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_cirq/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_cirq/circuits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/interface/qbraid_cirq/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_cirq/tests/test_cirq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_cirq/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/interface/qbraid_pyquil/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_pyquil/programs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_pyquil/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/interface/qbraid_pytket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_pytket/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_pytket/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/interface/qbraid_qasm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_qasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_qasm/circuit_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_qasm/circuits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/interface/qbraid_qasm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_qasm/tests/test_circuit_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_qasm/tests/test_qasm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_qasm/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/interface/qbraid_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_qiskit/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/qbraid_qiskit/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/interface/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/tests/test_calculate_unitary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/tests/test_convert_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/interface/tests/test_programs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/tests/test_top_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.061667 qbraid-0.4.1/qbraid/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/cirq_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_braket/convert_from_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_braket/convert_from_braket_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_braket/convert_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_braket/custom_gates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/_gate_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/test_from_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/test_from_braket_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/test_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/test_to_braket_measure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/cirq_pyquil/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_pyquil/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/cirq_pyquil/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_pyquil/tests/test_conversions_pyquil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/cirq_pytket/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_pytket/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/cirq_pytket/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_pytket/tests/test_conversions_pytket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_pytket/tests/test_to_pytket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/cirq_qasm/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qasm/qasm_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23183 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qasm/qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qasm/qasm_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qasm/qelib1_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/cirq_qasm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qasm/tests/_gate_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qasm/tests/test_qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qasm/tests/test_qasm_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/tests/_gate_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/tests/test_conversions_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/tests/test_from_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/tests/test_to_qiskit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/code/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/code/qasm_to_braket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.065667 qbraid-0.4.1/qbraid/transpiler/code/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/code/tests/test_qasm_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/custom_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.069667 qbraid-0.4.1/qbraid/transpiler/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.069667 qbraid-0.4.1/qbraid/transpiler/tests/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/tests/coverage/test_coverage_from_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/tests/coverage/test_coverage_from_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/tests/coverage/test_coverage_from_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/tests/coverage/test_coverage_from_pytket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/tests/coverage/test_coverage_from_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/tests/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.069667 qbraid-0.4.1/qbraid/transpiler/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/wrappers/abc_qprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/wrappers/braket_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/wrappers/cirq_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/wrappers/pyquil_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/wrappers/pytket_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/wrappers/qasm_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/transpiler/wrappers/qiskit_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-15 21:38:22.000000 qbraid-0.4.1/qbraid/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.053667 qbraid-0.4.1/qbraid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-06-15 21:38:36.000000 qbraid-0.4.1/qbraid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-15 21:38:37.000000 qbraid-0.4.1/qbraid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:38:36.000000 qbraid-0.4.1/qbraid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-15 21:38:36.000000 qbraid-0.4.1/qbraid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-15 21:38:36.000000 qbraid-0.4.1/qbraid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 21:38:36.000000 qbraid-0.4.1/qbraid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-15 21:38:22.000000 qbraid-0.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-15 21:38:22.000000 qbraid-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-15 21:38:37.069667 qbraid-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-15 21:38:22.000000 qbraid-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:38:37.069667 qbraid-0.4.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-15 21:38:22.000000 qbraid-0.4.1/tools/verify_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-15 21:38:22.000000 qbraid-0.4.1/tox.ini
```

### Comparing `qbraid-0.4.0/CONTRIBUTING.md` & `qbraid-0.4.1/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 The following is a summary of important commands and protocols for developers contributing to qBraid. Note that all
 commands assume a Debian environment, and that all commands (except the initial repository cloning command) assume
 your current working directory is the qBraid repo root.
 
 ## Pull request checklist
 
-1. `tox -e unit-tests`: All unit tests are passing. New + modified code has corresponding unit tests and satisfy `codecov` checks.
+1. `tox -e unit-tests`: All unit tests are passing. New + modified code has corresponding unit tests and satisfy `codecov` checks. To run remote tests (i.e. those requiring qBraid/AWS/IBM credentials), set environment variable `QBRAID_RUN_REMOTE_TESTS=True`.
 2. `tox -e docs`: Doc builds are passing. New + modified code has appropriate docstrings and tree stubs are updated, if applicable.
 3. `tox -e linters`: Code passes linters and formatters checks. Any exceptions or updates to code style configs are documented.
 4. `python tools/verify_headers.py`: New files have appropriate licensing headers. Running headers script passes checks.
 
 ## Installing from source
 
 You can install the qBraid-SDK from source by cloning this repository and running a pip install command in the root directory:
```

### Comparing `qbraid-0.4.0/LICENSE` & `qbraid-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/PKG-INFO` & `qbraid-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Home-page: https://github.com/qBraid/qBraid/
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
-License: Restricted
+License: GPL v3.0
 Keywords: qbraid,quantum
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,14 +24,15 @@
 
 <img width=full alt="qbraid-sdk-header" src="https://user-images.githubusercontent.com/46977852/224456452-605e51f2-193d-4789-863e-e51cdd4b0a54.png">
 
 [![CI](https://github.com/qBraid/qBraid/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/qBraid/qBraid/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/qBraid/qBraid/branch/main/graph/badge.svg?token=1UTM0XZB7A)](https://codecov.io/gh/qBraid/qBraid)
 [![Documentation Status](https://readthedocs.com/projects/qbraid-qbraid/badge/?version=latest)](https://docs.qbraid.com/en/latest/?badge=latest)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid.svg?color=blue)](https://pypi.org/project/qbraid/)
+[![License](https://img.shields.io/github/license/qBraid/qbraid.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The qBraid-SDK is a Python toolkit for cross-framework abstraction,
 transpilation, and execution of quantum programs.
 
 [<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git)
 
@@ -44,15 +45,15 @@
   circuit-building package, and **execute** on any backend that interfaces with
   a supported frontend.
 - Benchmark, compare, interpret results. Built-in **compatible** post-processing
   enables comparing results between runs and **across backends**.
 
 ## Installation & Setup
 
-<img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/669bd6f3-bbef-428c-9b59-b421c940262e">
+<img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/c82d61b4-2518-4c7e-8f48-05106afa708e">
 
 For the best experience, install the qBraid-SDK environment on
 [lab.qbraid.com](https://lab.qbraid.com). Login (or
 [create an account](https://account.qbraid.com)) and follow the steps to
 [install an environment](https://docs.qbraid.com/en/latest/lab/environments.html#install-environment).
 
 Using the SDK on qBraid Lab means direct, pre-configured access to all
@@ -92,15 +93,15 @@
 ### Transpiler
 
 Construct a quantum program of any supported program type,
 
 ```python
 >>> from qbraid import QPROGRAM_LIBS
 >>> QPROGRAM_LIBS
-['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm']
+['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm2']
 ```
 
 and use the `circuit_wrapper()` to convert to any other supported program type:
 
 ```python
 >>> from qbraid import circuit_wrapper
 >>> from qbraid.interface import random_circuit
@@ -164,16 +165,15 @@
 >>> aws_result.measurement_counts()
 {'00': 483, '01': 14, '10': 486, '11': 17}
 >>> ibm_result.measurement_counts()
 {'00': 496, '01': 12, '10': 479, '11': 13}
 ```
 
 ## Local account setup
-<img mg align="right" width="350" alt="api_key" src="https://github.com/qBraid/qBraid/assets/32727721/d087c404-e9c7-4a0b-b2a5-a58f2e483cce">
-
+<img mg align="right" width="350" alt="api_key" src="https://github.com/qBraid/qBraid/assets/46977852/86235d04-4b12-40e0-befe-1eeacaac9104">
 
 To use the qBraid-SDK locally (outside of qBraid Lab), you must add your account
 credentials:
 
 1. Create a qBraid account or log in to your existing account by visiting
    [account.qbraid.com](https://account.qbraid.com/v2)
 2. Copy your API Key token from the left side of
@@ -239,16 +239,18 @@
 
 - Interested in contributing code, or making a PR? See
   [CONTRIBUTING.md](CONTRIBUTING.md)
 - For feature requests and bug reports:
   [Submit an issue](https://github.com/qBraid/qBraid/issues)
 - For discussions, and specific questions about the qBraid SDK, qBraid Lab, or
   other topics, [join our discord community](https://discord.gg/gwBebaBZZX)
-- For questions that are more suited for a forum, use the `qbraid` tag on
-  [Stack Exchange](https://quantumcomputing.stackexchange.com/)
+- For questions that are more suited for a forum, post to
+  [Quantum Computing Stack Exchange](https://quantumcomputing.stackexchange.com/)
+  with the [`qbraid`](https://quantumcomputing.stackexchange.com/questions/tagged/qbraid) tag.
+  
 - Want your open-source project featured as its own runtime environment on
   qBraid Lab? Fill out our
   [New Environment Request Form](https://forms.gle/a4v7Kdn7G7bs9jYD8)
 
 ## License
 
 [GNU General Public License v3.0](LICENSE)
```

### Comparing `qbraid-0.4.0/README.md` & `qbraid-0.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <img width=full alt="qbraid-sdk-header" src="https://user-images.githubusercontent.com/46977852/224456452-605e51f2-193d-4789-863e-e51cdd4b0a54.png">
 
 [![CI](https://github.com/qBraid/qBraid/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/qBraid/qBraid/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/qBraid/qBraid/branch/main/graph/badge.svg?token=1UTM0XZB7A)](https://codecov.io/gh/qBraid/qBraid)
 [![Documentation Status](https://readthedocs.com/projects/qbraid-qbraid/badge/?version=latest)](https://docs.qbraid.com/en/latest/?badge=latest)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid.svg?color=blue)](https://pypi.org/project/qbraid/)
+[![License](https://img.shields.io/github/license/qBraid/qbraid.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The qBraid-SDK is a Python toolkit for cross-framework abstraction,
 transpilation, and execution of quantum programs.
 
 [<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git)
 
@@ -20,15 +21,15 @@
   circuit-building package, and **execute** on any backend that interfaces with
   a supported frontend.
 - Benchmark, compare, interpret results. Built-in **compatible** post-processing
   enables comparing results between runs and **across backends**.
 
 ## Installation & Setup
 
-<img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/669bd6f3-bbef-428c-9b59-b421c940262e">
+<img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/c82d61b4-2518-4c7e-8f48-05106afa708e">
 
 For the best experience, install the qBraid-SDK environment on
 [lab.qbraid.com](https://lab.qbraid.com). Login (or
 [create an account](https://account.qbraid.com)) and follow the steps to
 [install an environment](https://docs.qbraid.com/en/latest/lab/environments.html#install-environment).
 
 Using the SDK on qBraid Lab means direct, pre-configured access to all
@@ -68,15 +69,15 @@
 ### Transpiler
 
 Construct a quantum program of any supported program type,
 
 ```python
 >>> from qbraid import QPROGRAM_LIBS
 >>> QPROGRAM_LIBS
-['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm']
+['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm2']
 ```
 
 and use the `circuit_wrapper()` to convert to any other supported program type:
 
 ```python
 >>> from qbraid import circuit_wrapper
 >>> from qbraid.interface import random_circuit
@@ -140,16 +141,15 @@
 >>> aws_result.measurement_counts()
 {'00': 483, '01': 14, '10': 486, '11': 17}
 >>> ibm_result.measurement_counts()
 {'00': 496, '01': 12, '10': 479, '11': 13}
 ```
 
 ## Local account setup
-<img mg align="right" width="350" alt="api_key" src="https://github.com/qBraid/qBraid/assets/32727721/d087c404-e9c7-4a0b-b2a5-a58f2e483cce">
-
+<img mg align="right" width="350" alt="api_key" src="https://github.com/qBraid/qBraid/assets/46977852/86235d04-4b12-40e0-befe-1eeacaac9104">
 
 To use the qBraid-SDK locally (outside of qBraid Lab), you must add your account
 credentials:
 
 1. Create a qBraid account or log in to your existing account by visiting
    [account.qbraid.com](https://account.qbraid.com/v2)
 2. Copy your API Key token from the left side of
@@ -215,16 +215,18 @@
 
 - Interested in contributing code, or making a PR? See
   [CONTRIBUTING.md](CONTRIBUTING.md)
 - For feature requests and bug reports:
   [Submit an issue](https://github.com/qBraid/qBraid/issues)
 - For discussions, and specific questions about the qBraid SDK, qBraid Lab, or
   other topics, [join our discord community](https://discord.gg/gwBebaBZZX)
-- For questions that are more suited for a forum, use the `qbraid` tag on
-  [Stack Exchange](https://quantumcomputing.stackexchange.com/)
+- For questions that are more suited for a forum, post to
+  [Quantum Computing Stack Exchange](https://quantumcomputing.stackexchange.com/)
+  with the [`qbraid`](https://quantumcomputing.stackexchange.com/questions/tagged/qbraid) tag.
+  
 - Want your open-source project featured as its own runtime environment on
   qBraid Lab? Fill out our
   [New Environment Request Form](https://forms.gle/a4v7Kdn7G7bs9jYD8)
 
 ## License
 
 [GNU General Public License v3.0](LICENSE)
```

### Comparing `qbraid-0.4.0/docs/_static/account/account_access_key.png` & `qbraid-0.4.1/docs/_static/account/account_access_key.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/account/account_profile_details.png` & `qbraid-0.4.1/docs/_static/account/account_profile_details.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/cards/jupyter.png` & `qbraid-0.4.1/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/cards/python.png` & `qbraid-0.4.1/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/cards/terminal.png` & `qbraid-0.4.1/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_add.png` & `qbraid-0.4.1/docs/_static/environments/env_add.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_add_package.png` & `qbraid-0.4.1/docs/_static/environments/env_add_package.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_create.png` & `qbraid-0.4.1/docs/_static/environments/env_create.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_custom_installing.png` & `qbraid-0.4.1/docs/_static/environments/env_custom_installing.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_custom_pkgs.png` & `qbraid-0.4.1/docs/_static/environments/env_custom_pkgs.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_install.png` & `qbraid-0.4.1/docs/_static/environments/env_install.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_installing.png` & `qbraid-0.4.1/docs/_static/environments/env_installing.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_more.png` & `qbraid-0.4.1/docs/_static/environments/env_more.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_new.png` & `qbraid-0.4.1/docs/_static/environments/env_new.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_pkg_install.png` & `qbraid-0.4.1/docs/_static/environments/env_pkg_install.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/environments/env_share.png` & `qbraid-0.4.1/docs/_static/environments/env_share.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/errors/sidebar_glitch.png` & `qbraid-0.4.1/docs/_static/errors/sidebar_glitch.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/favicon.ico` & `qbraid-0.4.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/0_file_control_panel.png` & `qbraid-0.4.1/docs/_static/integrations/0_file_control_panel.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/1_top_bar_token.png` & `qbraid-0.4.1/docs/_static/integrations/1_top_bar_token.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/2_request_token.png` & `qbraid-0.4.1/docs/_static/integrations/2_request_token.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/3_copy_token.png` & `qbraid-0.4.1/docs/_static/integrations/3_copy_token.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/4_jupyter_server.png` & `qbraid-0.4.1/docs/_static/integrations/4_jupyter_server.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/5_existing_uri.png` & `qbraid-0.4.1/docs/_static/integrations/5_existing_uri.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/6_example_user.png` & `qbraid-0.4.1/docs/_static/integrations/6_example_user.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/7_notebook_kernel.png` & `qbraid-0.4.1/docs/_static/integrations/7_notebook_kernel.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/8_select_kernel.png` & `qbraid-0.4.1/docs/_static/integrations/8_select_kernel.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/os.png` & `qbraid-0.4.1/docs/_static/integrations/os.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/integrations/vscode_graphic.png` & `qbraid-0.4.1/docs/_static/integrations/vscode_graphic.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/jobs/jobs_ionq.png` & `qbraid-0.4.1/docs/_static/jobs/jobs_ionq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/jobs/jobs_sdk.png` & `qbraid-0.4.1/docs/_static/jobs/jobs_sdk.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/jobs/jobs_tag.png` & `qbraid-0.4.1/docs/_static/jobs/jobs_tag.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/logo.png` & `qbraid-0.4.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/notebooks/file_browser.png` & `qbraid-0.4.1/docs/_static/notebooks/file_browser.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/notebooks/kernel_activate.png` & `qbraid-0.4.1/docs/_static/notebooks/kernel_activate.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/notebooks/kernel_deactivate.png` & `qbraid-0.4.1/docs/_static/notebooks/kernel_deactivate.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/notebooks/kernel_nb.png` & `qbraid-0.4.1/docs/_static/notebooks/kernel_nb.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/notebooks/kernel_switch.png` & `qbraid-0.4.1/docs/_static/notebooks/kernel_switch.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/notebooks/share_notebook.png` & `qbraid-0.4.1/docs/_static/notebooks/share_notebook.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/pkg-logos/braket.png` & `qbraid-0.4.1/docs/_static/pkg-logos/braket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/pkg-logos/cirq.png` & `qbraid-0.4.1/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/pkg-logos/pyquil.png` & `qbraid-0.4.1/docs/_static/pkg-logos/pyquil.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/pkg-logos/pytket.png` & `qbraid-0.4.1/docs/_static/pkg-logos/pytket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/pkg-logos/qasm.png` & `qbraid-0.4.1/docs/_static/pkg-logos/qasm.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/pkg-logos/qiskit.png` & `qbraid-0.4.1/docs/_static/pkg-logos/qiskit.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/pkg-logos/xanadu.png` & `qbraid-0.4.1/docs/_static/pkg-logos/xanadu.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/sdk-files/get_devices.png` & `qbraid-0.4.1/docs/_static/sdk-files/get_devices.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/_static/sdk-files/plot_counts.png` & `qbraid-0.4.1/docs/_static/sdk-files/plot_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/api/qbraid.devices.aws.rst` & `qbraid-0.4.1/docs/api/qbraid.devices.aws.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/api/qbraid.devices.ibm.rst` & `qbraid-0.4.1/docs/api/qbraid.devices.ibm.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/api/qbraid.interface.rst` & `qbraid-0.4.1/docs/api/qbraid.interface.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_braket.rst` & `qbraid-0.4.1/docs/api/qbraid.transpiler.cirq_braket.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_utils.rst` & `qbraid-0.4.1/docs/api/qbraid.transpiler.cirq_utils.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/api/qbraid.transpiler.rst` & `qbraid-0.4.1/docs/api/qbraid.transpiler.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/envs-activate.rst` & `qbraid-0.4.1/docs/cli/envs-activate.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/envs-list.rst` & `qbraid-0.4.1/docs/cli/envs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/envs-uninstall.rst` & `qbraid-0.4.1/docs/cli/envs-uninstall.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/envs.rst` & `qbraid-0.4.1/docs/cli/envs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/jobs-add.rst` & `qbraid-0.4.1/docs/cli/jobs-add.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/jobs-disable.rst` & `qbraid-0.4.1/docs/cli/jobs-disable.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/jobs-enable.rst` & `qbraid-0.4.1/docs/cli/jobs-enable.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/jobs-list.rst` & `qbraid-0.4.1/docs/cli/jobs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/jobs.rst` & `qbraid-0.4.1/docs/cli/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/kernels.rst` & `qbraid-0.4.1/docs/cli/kernels.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/cli/qbraid.rst` & `qbraid-0.4.1/docs/cli/qbraid.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/conf.py` & `qbraid-0.4.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.autodoc",
     "sphinx_autodoc_typehints",
     "sphinx.ext.autosummary",
     "sphinx.ext.todo",
     "sphinx.ext.mathjax",
     "sphinx.ext.coverage",
-    # "sphinx.ext.viewcode", # Hide source code link
+    "sphinx.ext.viewcode", # Hide source code link
 ]
 
 # set_type_checking_flag = True
 autodoc_member_order = "bysource"
 autoclass_content = "both"
 autodoc_mock_imports = ["cirq", "qiskit", "braket", "numpy", "requests", "requests.Session"]
 napoleon_numpy_docstring = False
```

### Comparing `qbraid-0.4.0/docs/index.rst` & `qbraid-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/lab/account.rst` & `qbraid-0.4.1/docs/lab/account.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/lab/environments.rst` & `qbraid-0.4.1/docs/lab/environments.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/lab/files.rst` & `qbraid-0.4.1/docs/lab/files.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/lab/integrations.rst` & `qbraid-0.4.1/docs/lab/integrations.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/lab/notebooks.rst` & `qbraid-0.4.1/docs/lab/notebooks.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/lab/overview.rst` & `qbraid-0.4.1/docs/lab/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/lab/quantumjobs.rst` & `qbraid-0.4.1/docs/lab/quantumjobs.rst`

 * *Files 1% similar despite different names*

```diff
@@ -101,13 +101,13 @@
     # Job ID (arn) copied over from sidebar
     task = AwsQuantumTask(arn="arn:aws:braket:us-east-1:..." )
 
     task.result()
     ...
 
 On qBraid, the devices you can access are not restricted by your choice of programming framework. Target any of our 20+ supported QPUs and simulators
-from Qiskit, Amazon Braket, Cirq, pyQuil, or OpenQASM using the `qBraid SDK <../sdk/devices.html>`_.
+from Qiskit, Amazon Braket, Cirq, pyQuil, or OpenQASM 2 using the `qBraid SDK <../sdk/devices.html>`_.
 
 .. seealso::
 
     - `Using access codes to connect to quantum devices on qBraid | Demo <https://youtu.be/K4vb2fzmSZQ>`_
     - `qBraid Quantum Jobs Lab Demo Notebook <https://github.com/qBraid/qbraid-lab-demo/blob/main/qbraid_quantum_jobs.ipynb>`_
```

### Comparing `qbraid-0.4.0/docs/lab/system.rst` & `qbraid-0.4.1/docs/lab/system.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/lab/troubleshoot.rst` & `qbraid-0.4.1/docs/lab/troubleshoot.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/sdk/circuits.rst` & `qbraid-0.4.1/docs/sdk/circuits.rst`

 * *Files 0% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 other circuit-based convenience features.
 
 Program Types
 --------------
 
 Supported frontend program types include `Qiskit <QiskitQuantumCircuit>`_,
 `Amazon Braket <BraketCircuit>`_, `Cirq <CirqCircuit>`_, `PyQuil <PyQuilProgram>`_,
-`PyTKET <PyTKETCircuit>`_, and `OpenQASM <OpenQASMString>`_:
+`PyTKET <PyTKETCircuit>`_, and `OpenQASM 2 <OpenQASMString>`_:
 
 .. code-block:: python
     
     >>> from qbraid import QPROGRAM_TYPES
     >>> for k in QPROGRAM_TYPES:
     ...     print(k)
     ...
     braket.circuits.circuit.Circuit
     cirq.circuits.circuit.Circuit
     qiskit.circuit.quantumcircuit.QuantumCircuit
     pyquil.quil.Program
     pytket._tket.circuit.Circuit
-    qasm
+    qasm2
 
 
 .. _QiskitQuantumCircuit: https://qiskit.org/documentation/stubs/qiskit.circuit.QuantumCircuit.html
 .. _BraketCircuit: https://docs.aws.amazon.com/braket/latest/developerguide/braket-constructing-circuit.html
 .. _CirqCircuit: https://quantumai.google/reference/python/cirq/circuits/Circuit
 .. _PyQuilProgram: https://pyquil-docs.rigetti.com/en/stable/basics.html
 .. _PyTKETCircuit: https://cqcl.github.io/tket/pytket/api/circuit_class.html
```

### Comparing `qbraid-0.4.0/docs/sdk/devices.rst` & `qbraid-0.4.1/docs/sdk/devices.rst`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     >>> from qbraid import get_devices
     >>> get_devices(filters={"vendor": "AWS", "type": "QPU"}, refresh=True)
     Device status updated 0 minutes ago
 
     Device ID                           Status
     ---------                           ------
-    aws_ionq                            ONLINE
+    aws_ionq_aria1                      ONLINE
     aws_oqc_lucy                        ONLINE
     aws_quera_aquila                    ONLINE
     aws_rigetti_aspen_m2                OFFLINE
     aws_rigetti_aspen_m3                ONLINE
     aws_xanadu_borealis                 ONLINE
 
 Each supported device is associated with its own qBraid ID. The next section will cover
```

### Comparing `qbraid-0.4.0/docs/sdk/jobs.rst` & `qbraid-0.4.1/docs/sdk/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/docs/sdk/overview.rst` & `qbraid-0.4.1/docs/sdk/overview.rst`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 Construct a quantum program of any supported program type:
 
 .. code-block:: python
    
    >>> from qbraid import QPROGRAM_LIBS
    >>> from qbraid.interface import random_circuit
    >>> QPROGRAM_LIBS
-   ['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm']
+   ['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm2']
    >>> circuit = random_circuit("qiskit", num_qubits=1, measure=True)
 
 Search for quantum backend(s) on which to execute your program:
 
 .. code-block:: python
 
    >>> from qbraid import get_devices
```

### Comparing `qbraid-0.4.0/docs/sdk/results.rst` & `qbraid-0.4.1/docs/sdk/results.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/pyproject.toml` & `qbraid-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/__init__.py` & `qbraid-0.4.1/qbraid/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/_version.py` & `qbraid-0.4.1/qbraid/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
 """
 Module containing version information
 
 Version number (major.minor.patch[-label])
 
 """
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `qbraid-0.4.0/qbraid/_warnings.py` & `qbraid-0.4.1/qbraid/_warnings.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,28 +31,34 @@
 
 def _check_version():
     """Emits UserWarning if updated package version exists in qBraid API
     compared to local copy."""
 
     # pylint: disable=import-outside-toplevel
     from ._version import __version__ as version_local
+    from .api.job_api import _running_in_lab
     from .api.session import QbraidSession
 
+    if not _running_in_lab():
+        return
+
     session = QbraidSession()
     version_api = session.get("/public/lab/get-sdk-version", params={}).json()
 
     if _warn_new_version(version_local, version_api):
         warnings.warn(
             f"You are using qbraid version {version_local}; however, version {version_api} "
             "is available. To avoid compatibility issues, consider upgrading by uninstalling "
             "and reinstalling the qBraid-SDK environment.",
             UserWarning,
         )
 
 
+# coverage: ignore
 warnings.filterwarnings("ignore", category=SyntaxWarning)
 warnings.filterwarnings("ignore", category=UserWarning, message="Setuptools is replacing distutils")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 warnings.filterwarnings("ignore", category=PendingDeprecationWarning)
+warnings.filterwarnings("ignore", category=RuntimeWarning, module="numpy")
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-# _check_version()
+_check_version()
```

### Comparing `qbraid-0.4.0/qbraid/api/__init__.py` & `qbraid-0.4.1/qbraid/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/api/exceptions.py` & `qbraid-0.4.1/qbraid/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/api/job_api.py` & `qbraid-0.4.1/qbraid/api/job_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,90 +9,106 @@
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for interacting with the qBraid Jobs API.
 
 """
 import os
+import sys
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 from .session import QbraidSession
 
 if TYPE_CHECKING:
     import qbraid
 
+SLUG = "qbraid_sdk_9j9sjy"  # qBraid Lab environment ID.
+ENVS_PATH = os.getenv("QBRAID_USR_ENVS") or os.path.join(
+    os.path.expanduser("~"), ".qbraid", "environments"
+)
+SLUG_PATH = os.path.join(ENVS_PATH, SLUG)
+
+
+def _running_in_lab():
+    """Checks if you are running qBraid-SDK in qBraid Lab environment.
+
+    See https://docs.qbraid.com/en/latest/lab/environments.html
+    """
+    python_exe = os.path.join(SLUG_PATH, "pyenv", "bin", "python")
+    return sys.executable == python_exe
+
 
 def _qbraid_jobs_enabled():
     """Returns True if running qBraid Lab and qBraid Quantum Jobs
-    proxy is enabled. Otherwise, returns False."""
-    qbraid_envs_path = os.path.join(os.path.expanduser("~"), ".qbraid", "environments")
-    slug_dir_proxy_file = os.path.join(qbraid_envs_path, "qbraid_sdk_9j9sjy", "qbraid", "proxy")
-
-    # Location of proxy file for SDK environment in qBraid Lab.
-    if os.path.isfile(slug_dir_proxy_file):
-        with open(slug_dir_proxy_file) as f:  # pylint: disable=unspecified-encoding
+    proxy is enabled. Otherwise, returns False.
+
+    See https://docs.qbraid.com/en/latest/lab/quantumjobs.html
+    """
+    proxy_file = os.path.join(SLUG_PATH, "qbraid", "proxy")
+    if os.path.isfile(proxy_file):
+        with open(proxy_file) as f:  # pylint: disable=unspecified-encoding
             firstline = f.readline().rstrip()
-            if firstline == "active = true":  # check if proxy is active or not
-                return True
+            return "active = true" in firstline  # check if proxy is active or not
     return False
 
 
 def init_job(
     vendor_job_id: str,
     device: "qbraid.devices.DeviceLikeWrapper",
-    circuit: "qbraid.transpiler.QuantumProgramWrapper",
+    circuits: "qbraid.transpiler.QuantumProgramWrapper",
     shots: int,
 ) -> str:
     """Initialize data dictionary for new qbraid job and
     create associated MongoDB job document.
 
     Args:
         vendor_job_id: Job ID provided by device vendor
         device: Wrapped quantum device
-        circuit: Wrapped quantum circuit
+        circuit: Wrapped quantum circuit list
         shots: Number of shots
 
     Returns:
         The qbraid job ID associated with this job
 
     """
     session = QbraidSession()
 
     # One of the features of qBraid Quantum Jobs is the ability to send
-    # jobs without any credentials using the qBraid Lab platform. In short,
-    # the qBraid CLI allows you to enable/disable API proxies for environments
-    # that use IBMQ and/or Amazon Braket (Botocore). A ``qbraid`` directory
-    # exists for each such environment that contains information about how to
-    # toggle the proxies, along with their status. If the qBraid Quantum Jobs
-    # proxy is enabled, a MongoDB document has already been created for this job. So,
-    # instead of creating a new job document, we instead query the user jobs
-    # for the ``vendorJobId`` (for Amazon Braket this is the QuantumTask arn),
-    # and return the correspondong ``qbraidJobId``.
-    if _qbraid_jobs_enabled():
+    # jobs without any credentials using the qBraid Lab platform. If the
+    # qBraid Quantum Jobs proxy is enabled, a document has already been
+    # created for this job. So, instead creating a duplicate, we query the
+    # user jobs for the `vendorJobId` and return the correspondong `qbraidJobId`.
+    if _running_in_lab() and _qbraid_jobs_enabled():
         job = session.post("/get-user-jobs", json={"vendorJobId": vendor_job_id}).json()[0]
         return job["qbraidJobId"]
 
-    # Create a new MongoDB document for the user job.  The qBraid API creates
-    # a unique Job ID, which is collected in the response. We use dummy variables
-    # for each of the status fields, which will be updated via the ``get_job_data``
-    # function upon instantiation of the ``JobLikeWrapper`` object.
+    # Create a new document for the user job. The qBraid API creates a unique
+    # Job ID, which is collected in the response. We use dummy variables for
+    # each of the status fields, which will be updated via the `get_job_data`
+    # function upon instantiation of the `JobLikeWrapper` object.
     init_data = {
         "qbraidJobId": "",
         "vendorJobId": vendor_job_id,
         "qbraidDeviceId": device.id,
         "vendorDeviceId": device.vendor_device_id,
-        "circuitNumQubits": circuit.num_qubits,
-        "circuitDepth": circuit.depth,
         "shots": shots,
         "createdAt": datetime.utcnow(),
         "status": "UNKNOWN",  # this will be set after we get back the job ID and check status
-        "qbraidStatus": "INITIALIZING",
+        "qbraidStatus": "INITIALIZING",  # TODO use qbraid Enums for status values
+        "email": os.getenv("JUPYTERHUB_USER") or session.user_email,
     }
-    init_data["email"] = os.getenv("JUPYTERHUB_USER")  # this env variable exists in Lab by default.
+
+    if len(circuits) == 1:
+        init_data["circuitNumQubits"] = circuits[0].num_qubits
+        init_data["circuitDepth"]: circuits[0].depth
+    else:
+        init_data["circuitBatchNumQubits"] = ([circuit.num_qubits for circuit in circuits],)
+        init_data["circuitBatchDepth"] = [circuit.depth for circuit in circuits]
+
     return session.post("/init-job", data=init_data).json()
 
 
 def get_job_data(qbraid_job_id: str, update: dict = None) -> dict:
     """Update a new MongoDB job document.
 
     Args:
```

### Comparing `qbraid-0.4.0/qbraid/api/retry.py` & `qbraid-0.4.1/qbraid/api/retry.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         response=None,
         error=None,
         _pool=None,
         _stacktrace=None,
     ):
         """Overwrites parent class increment method for logging."""
         if logger.getEffectiveLevel() is logging.DEBUG:
+            # coverage: ignore
             status = data = headers = None
             if response:
                 status = response.status
                 data = response.data
                 headers = response.headers
             logger.debug(
                 "Retrying method=%s, url=%s, status=%s, error=%s, data=%s, headers=%s",
```

### Comparing `qbraid-0.4.0/qbraid/api/session.py` & `qbraid-0.4.1/qbraid/api/session.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/api/tests/test_api_config.py` & `qbraid-0.4.1/qbraid/api/tests/test_api_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 ibmq_token = os.getenv("QISKIT_IBM_TOKEN")
 qbraid_refresh_token = os.getenv("REFRESH")
 qbraid_api_key = os.getenv("QBRAID_API_KEY")
 
 # This is the only environment variable that actually exists in qBraid Lab
 qbraid_user = os.getenv("JUPYTERHUB_USER")
 
+# Skip tests if IBM/AWS account auth/creds not configured
+skip_remote_tests: bool = os.getenv("QBRAID_RUN_REMOTE_TESTS") is None
+REASON = "QBRAID_RUN_REMOTE_TESTS not set (requires configuration of qBraid storage)"
+
 config_lst = [
     # (config_name, config_value, section, filepath)
     ["aws_access_key_id", aws_access_key_id, "default", aws_cred_path],
     ["aws_secret_access_key", aws_secret_access_key, "default", aws_cred_path],
     ["region", "us-east-1", "default", aws_config_path],
     ["output", "json", "default", aws_config_path],
     ["token", ibmq_token, "ibmq", qiskitrc_path],
@@ -76,15 +80,16 @@
         if section not in config.sections():
             config.add_section(section)
         config.set(section, config_name, str(config_value))
         with open(filepath, "w", encoding="utf-8") as cfgfile:
             config.write(cfgfile)
 
 
-set_config()
+if not skip_remote_tests:
+    set_config()
 
 
 def test_api_error():
     """Test raising error when making invalid API request."""
     with pytest.raises(RequestsApiError):
         session = QbraidSession()
         session.request("POST", "not a url")
@@ -94,21 +99,23 @@
     """Test initializing QbraidSession with attributes set from user-provided values."""
     refresh_token = "test123"
     session = QbraidSession(refresh_token=refresh_token)
     assert session.refresh_token == refresh_token
     del session
 
 
+@pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_qbraid_session_api_key():
     """Test initializing QbraidSession without args and then saving config."""
     session = QbraidSession()
     session.save_config(api_key=qbraid_api_key, user_email=qbraid_user)
     assert session.get_config_variable("api-key") == qbraid_api_key
 
 
+@pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_qbraid_session_save_config():
     """Test initializing QbraidSession without args and then saving config."""
     session = QbraidSession()
     session.save_config(user_email=qbraid_user, refresh_token=qbraid_refresh_token)
     assert session.get_config_variable("email") == qbraid_user
     assert session.get_config_variable("refresh-token") == qbraid_refresh_token
```

### Comparing `qbraid-0.4.0/qbraid/api/tests/test_api_thirdparty.py` & `qbraid-0.4.1/qbraid/api/tests/test_api_thirdparty.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 or relate to qBraid other third-party APIs.
 
 """
 import os
 
 import pytest
 
-from qbraid.api.job_api import _qbraid_jobs_enabled
+from qbraid.api.job_api import _qbraid_jobs_enabled, _running_in_lab
 from qbraid.api.session import STATUS_FORCELIST, PostForcelistRetry, QbraidSession
 
 
-def test_check_braket_proxy():
-    """Test function that checks whether braket proxy is active."""
+def test_running_in_lab():
+    assert not _running_in_lab()
+
+
+def test_check_quantum_jobs_enabled():
+    """Test function that checks whether quantum jobs is enabled in qBraid Lab."""
     qbraid_envs_path = os.path.join(os.path.expanduser("~"), ".qbraid", "environments")
     proxy_dir = os.path.join(qbraid_envs_path, "qbraid_sdk_9j9sjy", "qbraid")
     proxy_file = os.path.join(proxy_dir, "proxy")
     os.makedirs(proxy_dir, exist_ok=True)
     if os.path.exists(proxy_file):
         os.remove(proxy_file)
     assert _qbraid_jobs_enabled() is False
```

### Comparing `qbraid-0.4.0/qbraid/devices/__init__.py` & `qbraid-0.4.1/qbraid/devices/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,15 +27,17 @@
    DeviceType
    JobError
    JobStateError
    JobLikeWrapper
    JobStatus
    ResultWrapper
    is_status_final
+   braket_ionq_compilation
 
 
 """
 from .device import DeviceLikeWrapper
 from .enums import DeviceStatus, DeviceType, JobStatus, is_status_final
 from .exceptions import DeviceError, JobError, JobStateError
+from .ionq import braket_ionq_compilation
 from .job import JobLikeWrapper
 from .result import ResultWrapper
```

### Comparing `qbraid-0.4.0/qbraid/devices/aws/__init__.py` & `qbraid-0.4.1/qbraid/devices/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/devices/aws/device.py` & `qbraid-0.4.1/qbraid/devices/aws/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,17 +228,18 @@
             shots (int): The number of times to run the task on the device.
 
         Returns:
             The job like object for the run.
 
         """
         run_input, qbraid_circuit = self._compat_run_input(run_input)
+
         if "s3_destination_folder" not in kwargs:
             kwargs["s3_destination_folder"] = self._default_s3_folder
         aws_quantum_task = self.vendor_dlo.run(run_input, *args, **kwargs)
         metadata = aws_quantum_task.metadata()
         shots = 0 if "shots" not in metadata else metadata["shots"]
         vendor_job_id = aws_quantum_task.metadata()["quantumTaskArn"]
-        job_id = init_job(vendor_job_id, self, qbraid_circuit, shots)
+        job_id = init_job(vendor_job_id, self, [qbraid_circuit], shots)
         return AwsQuantumTaskWrapper(
             job_id, vendor_job_id=vendor_job_id, device=self, vendor_jlo=aws_quantum_task
         )
```

### Comparing `qbraid-0.4.0/qbraid/devices/aws/job.py` & `qbraid-0.4.1/qbraid/devices/aws/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     def _get_vendor_jlo(self):
         """Return the job like object that is being wrapped."""
         return AwsQuantumTask(self.vendor_job_id)
 
     def _get_status(self):
         """Returns status from Braket QuantumTask object metadata."""
-        return self.vendor_jlo.metadata()["status"]
+        return self.vendor_jlo.state()
 
     def result(self) -> AwsGateModelResultWrapper:
         """Return the results of the job."""
         if self.status() not in JOB_FINAL:
             logging.info("Result will be available when job has reached final state.")
         return AwsGateModelResultWrapper(self.vendor_jlo.result())
```

### Comparing `qbraid-0.4.0/qbraid/devices/aws/result.py` & `qbraid-0.4.1/qbraid/devices/aws/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/devices/device.py` & `qbraid-0.4.1/qbraid/devices/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING  # pylint: disable=unused-import
 
 from qbraid import circuit_wrapper
 
 from .exceptions import DeviceError
+from .ionq import braket_ionq_compilation
 
 if TYPE_CHECKING:
     import qbraid
 
 
 class DeviceLikeWrapper(ABC):
     """Abstract interface for device-like classes."""
@@ -40,15 +41,15 @@
             runPackage (str): The software package used to access the device
             objArg (str): The vendor device id/arn to supply as arg to vendor device-like object
             type (str): The type of the device, "QPU" or "Simulator"
             numberQubits (int): The number of qubits in the device (if applicable)
 
         """
         self._info = kwargs
-        self._qubits = self._info["numberQubits"]
+        self._qubits = self._info.get("numberQubits")
         self.vendor_device_id = self._info.pop("objArg")
         self.vendor_dlo = self._get_device()
 
     def _compat_run_input(self, run_input: "qbraid.QPROGRAM") -> "qbraid.QPROGRAM":
         """Checks if ``run_input`` is compatible with device and calls transpiler if necessary.
 
         Returns:
@@ -65,16 +66,23 @@
         input_run_package = run_input.__module__.split(".")[0]
         qbraid_circuit = circuit_wrapper(run_input)
         if self.num_qubits and qbraid_circuit.num_qubits > self.num_qubits:
             raise DeviceError(
                 f"Number of qubits in circuit ({qbraid_circuit.num_qubits}) exceeds "
                 f"number of qubits in device ({self.num_qubits})."
             )
-        if input_run_package != device_run_package:
-            run_input = qbraid_circuit.transpile(device_run_package)
+
+        if self._info["provider"] == "IonQ" and self._info["name"] == "Harmony":
+            if input_run_package not in ["pytket", "braket"]:
+                run_input = qbraid_circuit.transpile(device_run_package)
+            run_input = braket_ionq_compilation(run_input)
+        else:
+            if input_run_package != device_run_package:
+                run_input = qbraid_circuit.transpile(device_run_package)
+
         compat_run_input = self._vendor_compat_run_input(run_input)
         return compat_run_input, qbraid_circuit
 
     @abstractmethod
     def _vendor_compat_run_input(self, run_input):
         """Applies any software/device specific modifications to run input."""
```

### Comparing `qbraid-0.4.0/qbraid/devices/enums.py` & `qbraid-0.4.1/qbraid/devices/enums.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/devices/exceptions.py` & `qbraid-0.4.1/qbraid/devices/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/devices/ibm/__init__.py` & `qbraid-0.4.1/qbraid/devices/ibm/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/devices/ibm/device.py` & `qbraid-0.4.1/qbraid/devices/ibm/device.py`

 * *Files 20% similar despite different names*

```diff
@@ -98,12 +98,52 @@
         shots = backend.options.get("shots") if "shots" not in kwargs else kwargs.pop("shots")
         memory = (
             True if "memory" not in kwargs else kwargs.pop("memory")
         )  # Needed to get measurements
         transpiled = transpile(run_input, backend=backend)
         qiskit_job = backend.run(transpiled, shots=shots, memory=memory, **kwargs)
         qiskit_job_id = qiskit_job.job_id()
-        qbraid_job_id = init_job(qiskit_job_id, self, qbraid_circuit, shots)
+        qbraid_job_id = init_job(qiskit_job_id, self, [qbraid_circuit], shots)
+        qbraid_job = IBMJobWrapper(
+            qbraid_job_id, vendor_job_id=qiskit_job_id, device=self, vendor_jlo=qiskit_job
+        )
+        return qbraid_job
+
+    def run_batch(self, run_input, **kwargs):
+        """Runs circuit(s) on qiskit backend via :meth:`~qiskit.execute`
+
+        Uses the :meth:`~qiskit.execute` method to create a :class:`~qiskit.providers.Job` object,
+        applies a :class:`~qbraid.devices.ibm.IBMJobWrapper`, and return the result.
+
+        Args:
+            run_input: A circuit object list to run on the wrapped device.
+
+        Keyword Args:
+            shots (int): The number of times to run the task on the device. Default is 1024.
+
+
+        Returns:
+            qbraid.devices.ibm.IBMJobWrapper: The job like object for the run.
+
+        """
+        backend = self.vendor_dlo
+        qbraid_circuit_batch = []
+        run_input_batch = []
+        for circuit in run_input:
+            run_input, qbraid_circuit = self._compat_run_input(circuit)
+            run_input_batch.append(run_input)
+            qbraid_circuit_batch.append(qbraid_circuit)
+
+        shots = backend.options.get("shots") if "shots" not in kwargs else kwargs.pop("shots")
+        memory = (
+            True if "memory" not in kwargs else kwargs.pop("memory")
+        )  # Needed to get measurements
+        transpiled = transpile(run_input_batch, backend=backend)
+        qiskit_job = backend.run(transpiled, shots=shots, memory=memory, **kwargs)
+        qiskit_job_id = qiskit_job.job_id()
+
+        # to change to batch
+        qbraid_job_id = init_job(qiskit_job_id, self, qbraid_circuit_batch, shots)
         qbraid_job = IBMJobWrapper(
             qbraid_job_id, vendor_job_id=qiskit_job_id, device=self, vendor_jlo=qiskit_job
         )
         return qbraid_job
```

### Comparing `qbraid-0.4.0/qbraid/devices/ibm/job.py` & `qbraid-0.4.1/qbraid/devices/ibm/job.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 Module defining IBMJobWrapper Class
 
 """
 import logging
 
 from qiskit_ibm_provider import IBMBackend
+from qiskit_ibm_provider.job.exceptions import IBMJobInvalidStateError
 
 from qbraid.devices.enums import JOB_FINAL
 from qbraid.devices.exceptions import JobError, JobStateError
 from qbraid.devices.job import JobLikeWrapper
 
 from .result import IBMResultWrapper
 
@@ -52,8 +53,11 @@
         return IBMResultWrapper(self.vendor_jlo.result())
 
     def cancel(self):
         """Attempt to cancel the job."""
         status = self.status()
         if status in JOB_FINAL:
             raise JobStateError(f"Cannot cancel quantum job in the {status} state.")
-        return self.vendor_jlo.cancel()
+        try:
+            return self.vendor_jlo.cancel()
+        except IBMJobInvalidStateError as err:
+            raise JobStateError from err
```

### Comparing `qbraid-0.4.0/qbraid/devices/ibm/provider.py` & `qbraid-0.4.1/qbraid/devices/ibm/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/devices/ibm/result.py` & `qbraid-0.4.1/qbraid/transpiler/wrappers/braket_circuit.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module defining IBMResultWrapper Class
+Module defining BraketCircuitWrapper Class
 
 """
-import numpy as np
+from braket.circuits.circuit import Circuit as BKCircuit
 
-from qbraid.devices.result import ResultWrapper
+from qbraid.transpiler.wrappers.abc_qprogram import QuantumProgramWrapper
 
 
-class IBMResultWrapper(ResultWrapper):
-    """Qiskit ``Result`` wrapper class."""
+class BraketCircuitWrapper(QuantumProgramWrapper):
+    """Wrapper class for Amazon Braket ``Circuit`` objects."""
 
-    def measurements(self):
-        """Return measurements as list"""
-        qiskit_meas = self.vendor_rlo.get_memory()
-        qbraid_meas = []
-        for str_shot in qiskit_meas:
-            lst_shot = [int(x) for x in list(str_shot)]
-            qbraid_meas.append(lst_shot)
-        return np.array(qbraid_meas)
-
-    def raw_counts(self):
-        """Returns the histogram data of the run"""
-        return self.vendor_rlo.get_counts()
+    def __init__(self, circuit: BKCircuit):
+        """Create a BraketCircuitWrapper
+
+        Args:
+            circuit: the circuit object to be wrapped
+
+        """
+        super().__init__(circuit)
+
+        self._qubits = circuit.qubits
+        self._num_qubits = len(self.qubits)
+        self._depth = circuit.depth
+        self._package = "braket"
+        self._program_type = "Circuit"
```

### Comparing `qbraid-0.4.0/qbraid/devices/ibm/tests/test_ibm_provider.py` & `qbraid-0.4.1/qbraid/devices/ibm/tests/test_ibm_provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 import os
 
 import pytest
 from qiskit_ibm_provider import IBMProvider
 
 from qbraid.devices.ibm.provider import ibm_least_busy_qpu, ibm_provider, ibm_to_qbraid_id
 
+# Skip tests if IBM/AWS account auth/creds not configured
+skip_remote_tests: bool = os.getenv("QBRAID_RUN_REMOTE_TESTS") is None
+REASON = "QBRAID_RUN_REMOTE_TESTS not set (requires configuration of IBM storage)"
+
 backend_id_data = [
     ("ibm_nairobi", "ibm_q_nairobi"),
     ("ibmq_belem", "ibm_q_belem"),
     ("simulator_extended_stabilizer", "ibm_q_simulator_extended_stabilizer"),
 ]
 
 
@@ -30,18 +34,20 @@
 def test_get_qbraid_id(data):
     """Test converting backend name to qbraid_id."""
     original, expected = data
     result = ibm_to_qbraid_id(original)
     assert result == expected
 
 
+@pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_ibm_provider():
     """Test getting IBMQ provider using qiskit_ibm_provider package."""
     ibmq_token = os.getenv("QISKIT_IBM_TOKEN", None)
     provider = ibm_provider(token=ibmq_token)
     assert isinstance(provider, IBMProvider)
 
 
+@pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_ibm_least_busy():
     """Test returning qbraid ID of least busy IBMQ QPU."""
     qbraid_id = ibm_least_busy_qpu()
     assert qbraid_id[:6] == "ibm_q_"
```

### Comparing `qbraid-0.4.0/qbraid/devices/job.py` & `qbraid-0.4.1/qbraid/devices/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/devices/result.py` & `qbraid-0.4.1/qbraid/devices/result.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,13 +57,17 @@
     @abstractmethod
     def raw_counts(self):
         """Returns raw histogram data of the run"""
 
     def measurement_counts(self):
         """Returns the sorted histogram data of the run"""
         raw_counts = self.raw_counts()
-        return _format_counts(raw_counts)
+        if isinstance(raw_counts, dict):
+            return _format_counts(raw_counts)
+        return [_format_counts(counts) for counts in raw_counts]
 
     def plot_counts(self):
         """Plot histogram of measurement counts"""
         counts = self.measurement_counts()
-        return plot_histogram(counts)
+        if isinstance(counts, dict):
+            return plot_histogram(counts)
+        return [plot_histogram(count) for count in counts]
```

### Comparing `qbraid-0.4.0/qbraid/devices/status_maps.py` & `qbraid-0.4.1/qbraid/devices/status_maps.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/devices/tests/test_devices.py` & `qbraid-0.4.1/qbraid/devices/tests/test_devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Unit tests for the qbraid device layer.
 
 """
+import os
+
 import cirq
 import numpy as np
 import pytest
 from braket.aws import AwsDevice
 from braket.circuits import Circuit as BraketCircuit
 from braket.tasks.quantum_task import QuantumTask as AwsQuantumTask
 from qiskit import QuantumCircuit as QiskitCircuit
@@ -31,23 +33,31 @@
     IBMBackendWrapper,
     IBMJobWrapper,
     ibm_least_busy_qpu,
     ibm_to_qbraid_id,
 )
 from qbraid.interface import random_circuit
 
+# Skip tests if IBM/AWS account auth/creds not configured
+skip_remote_tests: bool = os.getenv("QBRAID_RUN_REMOTE_TESTS") is None
+REASON = "QBRAID_RUN_REMOTE_TESTS not set (requires configuration of IBM/AWS storage)"
+pytestmark = pytest.mark.skipif(skip_remote_tests, reason=REASON)
+
 
 def device_wrapper_inputs(vendor: str):
     """Returns list of tuples containing all device_wrapper inputs for given vendor."""
     session = QbraidSession()
     devices = session.get("/public/lab/get-devices", params={}).json()
     input_list = []
+    deprecated = ["aws_ionq"]
     for document in devices:
         if document["vendor"] == vendor:
-            input_list.append(document["qbraid_id"])
+            qbraid_id = document["qbraid_id"]
+            if qbraid_id not in deprecated:
+                input_list.append(qbraid_id)
     return input_list
 
 
 def ibm_devices():
     provider = IBMProvider()
     backends = provider.backends()
     qbraid_devices = device_wrapper_inputs("IBM")
@@ -56,16 +66,16 @@
 
 
 """
 Device wrapper tests: initialization
 Coverage: all vendors, all available devices
 """
 
-inputs_braket_dw = device_wrapper_inputs("AWS")
-inputs_qiskit_dw = ibm_devices()
+inputs_braket_dw = [] if skip_remote_tests else device_wrapper_inputs("AWS")
+inputs_qiskit_dw = [] if skip_remote_tests else ibm_devices()
 
 
 def test_job_wrapper_type():
     """Test that job wrapper creates object of original job type"""
     device = device_wrapper("aws_dm_sim")
     circuit = random_circuit("qiskit")
     job_0 = device.run(circuit, shots=10)
@@ -179,14 +189,24 @@
     qbraid_device = device_wrapper(device_id)
     qbraid_job = qbraid_device.run(circuit, shots=10)
     vendor_job = qbraid_job.vendor_jlo
     assert isinstance(qbraid_job, IBMJobWrapper)
     assert isinstance(vendor_job, IBMJob)
 
 
+@pytest.mark.parametrize("device_id", inputs_qiskit_run)
+def test_run_batch_qiskit_device_wrapper(device_id):
+    """Test run_batch method from wrapped Qiskit backends"""
+    qbraid_device = device_wrapper(device_id)
+    qbraid_job = qbraid_device.run_batch(circuits_qiskit_run, shots=10)
+    vendor_job = qbraid_job.vendor_jlo
+    assert isinstance(qbraid_job, IBMJobWrapper)
+    assert isinstance(vendor_job, IBMJob)
+
+
 @pytest.mark.parametrize("circuit", circuits_braket_run)
 @pytest.mark.parametrize("device_id", inputs_braket_run)
 def test_run_braket_device_wrapper(device_id, circuit):
     """Test run method of wrapped Braket devices"""
     qbraid_device = device_wrapper(device_id)
     qbraid_job = qbraid_device.run(circuit, shots=10)
     vendor_job = qbraid_job.vendor_jlo
@@ -210,14 +230,33 @@
         status = qbraid_job.status()
         status_final = is_status_final(status)
         count += 1
     with pytest.raises(JobStateError):
         qbraid_job.cancel()
 
 
+@pytest.mark.parametrize("device_id", ["ibm_q_simulator_statevector"])
+def test_cancel_completed_batch_error(device_id):
+    """Test that cancelling a batch job that has already reached its
+    final state raises an error."""
+    import time
+
+    qbraid_device = device_wrapper(device_id)
+    qbraid_job = qbraid_device.run_batch(circuits_qiskit_run, shots=10)
+    status_final = False
+    count = 0
+    while not status_final and count < 10:
+        time.sleep(2)
+        status = qbraid_job.status()
+        status_final = is_status_final(status)
+        count += 1
+    with pytest.raises(JobStateError):
+        qbraid_job.cancel()
+
+
 def test_circuit_too_many_qubits():
     """Test that run method raises exception when input circuit
     num qubits exceeds that of wrapped Qiskit device."""
     two_qubit_circuit = QiskitCircuit(6)
     two_qubit_circuit.h([0, 1])
     two_qubit_circuit.cx(0, 5)
     one_qubit_device = device_wrapper("ibm_q_belem")
@@ -237,25 +276,13 @@
     circuit = random_circuit("qiskit")
     job = device.run(circuit, shots=10)
     job.wait_for_final_state()
     status = job.status()
     assert is_status_final(status)
 
 
-@pytest.mark.parametrize("device_id", ["ibm_q_simulator_statevector", "aws_sv_sim"])
-def test_result_wrapper_measurements(device_id):
-    """Test result wrapper measurements method."""
-    circuit = random_circuit("qiskit", num_qubits=3, depth=3, measure=True)
-    sim = device_wrapper(device_id).run(circuit, shots=10)
-    qbraid_result = sim.result()
-    counts = qbraid_result.measurement_counts()
-    measurements = qbraid_result.measurements()
-    assert isinstance(counts, dict)
-    assert measurements.shape == (10, 3)
-
-
 def test_aws_device_available():
     """Test BraketDeviceWrapper avaliable output identical"""
     device = device_wrapper("aws_dm_sim")
     is_available_bool, is_available_time = device.is_available
     assert is_available_bool == device._get_device().is_available
     assert len(is_available_time.split(":")) == 3
```

### Comparing `qbraid-0.4.0/qbraid/devices/tests/test_enums.py` & `qbraid-0.4.1/qbraid/devices/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/display_utils.py` & `qbraid-0.4.1/qbraid/display_utils.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/exceptions.py` & `qbraid-0.4.1/qbraid/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/get_devices.py` & `qbraid-0.4.1/qbraid/get_devices.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/get_jobs.py` & `qbraid-0.4.1/qbraid/get_jobs.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/__init__.py` & `qbraid-0.4.1/qbraid/interface/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 .. currentmodule:: qbraid.interface
 
 .. autosummary::
    :toctree: ../stubs/
 
    to_unitary
    unitary_to_little_endian
+   random_unitary_matrix
    convert_to_contiguous
    circuits_allclose
    random_circuit
    circuit_drawer
    ContiguousConversionError
    UnitaryCalculationError
 
 """
 from .calculate_unitary import (
     UnitaryCalculationError,
     circuits_allclose,
+    random_unitary_matrix,
     to_unitary,
     unitary_to_little_endian,
 )
 from .convert_to_contiguous import ContiguousConversionError, convert_to_contiguous
 from .draw import circuit_drawer
 from .programs import random_circuit
```

### Comparing `qbraid-0.4.0/qbraid/interface/calculate_unitary.py` & `qbraid-0.4.1/qbraid/interface/calculate_unitary.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     Returns:
         Matrix representation of the input quantum program.
     """
     to_unitary_function: Callable[[Any], np.ndarray]
 
     if isinstance(program, str):
-        package = "qasm"
+        package = "qasm2"
     else:
         try:
             package = program.__module__
         except AttributeError as err:
             raise ProgramTypeError(program) from err
 
     # pylint: disable=import-outside-toplevel
@@ -71,15 +71,15 @@
         from qbraid.interface.qbraid_pyquil.tools import _unitary_from_pyquil
 
         to_unitary_function = _unitary_from_pyquil
     elif "pytket" in package:
         from qbraid.interface.qbraid_pytket.tools import _unitary_from_pytket
 
         to_unitary_function = _unitary_from_pytket
-    elif "qasm" in package:
+    elif "qasm2" in package:
         from qbraid.interface.qbraid_qasm.tools import _unitary_from_qasm
 
         to_unitary_function = _unitary_from_qasm
     else:
         raise ProgramTypeError(program)
 
     program_input = convert_to_contiguous(program) if ensure_contiguous else program
@@ -145,7 +145,23 @@
         raise ValueError("Input matrix must be unitary.")
     num_qubits = int(np.log2(rank))
     tensor_be = matrix.reshape([2] * 2 * num_qubits)
     indicies_in = list(reversed(range(num_qubits)))
     indicies_out = [i + num_qubits for i in indicies_in]
     tensor_le = np.einsum(tensor_be, indicies_in + indicies_out)
     return tensor_le.reshape([rank, rank])
+
+
+def random_unitary_matrix(dim: int) -> np.ndarray:
+    """Create a random (complex) unitary matrix of order `dim`
+
+    Args:
+        dim: integer square matrix dimension
+
+    Returns:
+        random unitary matrix of shape dim x dim
+    """
+    # Create a random complex matrix of size dim x dim
+    matrix = np.random.randn(dim, dim) + 1j * np.random.randn(dim, dim)
+    # Use the QR decomposition to get a random unitary matrix
+    unitary, _ = np.linalg.qr(matrix)
+    return unitary
```

### Comparing `qbraid-0.4.0/qbraid/interface/convert_to_contiguous.py` & `qbraid-0.4.1/qbraid/interface/convert_to_contiguous.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     Returns:
         :data:`~qbraid.QPROGRAM`: Program of the same type as the input quantum program.
 
     """
     conversion_function: Callable[[Any], QPROGRAM]
 
     if isinstance(program, str):
-        package = "qasm"
+        package = "qasm2"
     else:
         try:
             package = program.__module__
         except AttributeError as err:
             raise ProgramTypeError(program) from err
 
     # pylint: disable=import-outside-toplevel
@@ -69,15 +69,15 @@
         from qbraid.interface.qbraid_braket.tools import _convert_to_contiguous_braket
 
         conversion_function = _convert_to_contiguous_braket
     elif "pytket" in package:
         from qbraid.interface.qbraid_pytket.tools import _convert_to_contiguous_pytket
 
         conversion_function = _convert_to_contiguous_pytket
-    elif "qasm" in package:
+    elif "qasm2" in package:
         from qbraid.interface.qbraid_qasm.tools import _convert_to_contiguous_qasm
 
         conversion_function = _convert_to_contiguous_qasm
     else:
         raise ProgramTypeError(program)
 
     try:
```

### Comparing `qbraid-0.4.0/qbraid/interface/draw.py` & `qbraid-0.4.1/qbraid/interface/draw.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,20 @@
         :data:`~.qbraid.QPROGRAM`: Supported quantum program
 
     Raises:
         ProgramTypeError: If quantum program is not of a supported type
     """
     # todo: visualization from supportive framework
     if isinstance(program, str):
-        package = "qasm"
+        if "OPENQASM 2.0" in program:
+            package = "qasm2"
+        elif "OPENQASM 3.0" in program:
+            package = "qasm3"
+        else:
+            raise ProgramTypeError("Input of type string must represent a valid OpenQASM program.")
     else:
         try:
             package = program.__module__
         except AttributeError as err:
             raise ProgramTypeError(program) from err
 
     # pylint: disable=import-outside-toplevel
@@ -92,8 +97,21 @@
 
             # coverage: ignore
             return render_circuit_as_html(program, **kwargs)
         raise VisualizationError(
             'The only valid option for pytket are "jupyter", "view_browser", "html"'
         )
 
+    if package == "qasm3":
+        from .qbraid_qasm.circuit_drawer import draw_circuit
+
+        # coverage: ignore
+        return print(draw_circuit(program))
+
+    if package == "qasm2":
+        from .qbraid_qasm.tools import convert_to_qasm3
+
+        # coverage: ignore
+        qasm3_str = convert_to_qasm3(program)
+        return print(draw_circuit(qasm3_str))
+
     raise ProgramTypeError(package)
```

### Comparing `qbraid-0.4.0/qbraid/interface/programs.py` & `qbraid-0.4.1/qbraid/interface/programs.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,47 +31,47 @@
 
 def bell_data() -> QROGRAM_TEST_TYPE:
     """Returns bell circuit/program in each supported package."""
     from qbraid.interface.qbraid_braket.circuits import braket_bell
     from qbraid.interface.qbraid_cirq.circuits import cirq_bell
     from qbraid.interface.qbraid_pyquil.programs import pyquil_bell
     from qbraid.interface.qbraid_pytket.circuits import pytket_bell
-    from qbraid.interface.qbraid_qasm.circuits import qasm_bell
+    from qbraid.interface.qbraid_qasm.circuits import qasm2_bell
     from qbraid.interface.qbraid_qiskit.circuits import qiskit_bell
 
     unitary = to_unitary(cirq_bell())
 
     circuits = {
         "braket": braket_bell,
         "cirq": cirq_bell,
         "pyquil": pyquil_bell,
         "qiskit": qiskit_bell,
         "pytket": pytket_bell,
-        "qasm": qasm_bell,
+        "qasm2": qasm2_bell,
     }
 
     return circuits, unitary
 
 
 def shared15_data() -> QROGRAM_TEST_TYPE:
     """Returns shared gates circuit/program in each supported package."""
     from qbraid.interface.qbraid_braket.circuits import braket_shared15
     from qbraid.interface.qbraid_cirq.circuits import cirq_shared15
     from qbraid.interface.qbraid_pytket.circuits import pytket_shared15
-    from qbraid.interface.qbraid_qasm.circuits import qasm_shared15
+    from qbraid.interface.qbraid_qasm.circuits import qasm2_shared15
     from qbraid.interface.qbraid_qiskit.circuits import qiskit_shared15
 
     unitary = to_unitary(cirq_shared15())
 
     circuits = {
         "braket": braket_shared15,
         "cirq": cirq_shared15,
         "qiskit": qiskit_shared15,
         "pytket": pytket_shared15,
-        "qasm": qasm_shared15,
+        "qasm2": qasm2_shared15,
     }
 
     return circuits, unitary
 
 
 def random_circuit(
     package: str, num_qubits: Optional[int] = None, depth: Optional[int] = None, **kwargs
@@ -93,15 +93,19 @@
 
     """
     # todo: custom random gate
     if package not in QPROGRAM_LIBS:
         raise PackageValueError(package)
     num_qubits = np.random.randint(1, 4) if num_qubits is None else num_qubits
     depth = np.random.randint(1, 4) if depth is None else depth
-    if package == "qiskit":
+    if package == "qasm3":
+        from qbraid.interface.qbraid_qasm.circuits import _qasm3_random
+
+        rand_circuit = _qasm3_random(num_qubits, depth, **kwargs)
+    elif package == "qiskit":
         from qbraid.interface.qbraid_qiskit.circuits import _qiskit_random
 
         rand_circuit = _qiskit_random(num_qubits, depth, **kwargs)
     else:
         from qbraid.interface.qbraid_cirq.circuits import _cirq_random
 
         rand_circuit = _cirq_random(num_qubits, depth, **kwargs)
```

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_braket/circuits.py` & `qbraid-0.4.1/qbraid/interface/qbraid_braket/circuits.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_braket/tools.py` & `qbraid-0.4.1/qbraid/interface/qbraid_braket/tools.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_cirq/_utils.py` & `qbraid-0.4.1/qbraid/interface/qbraid_cirq/_utils.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_cirq/circuits.py` & `qbraid-0.4.1/qbraid/interface/qbraid_cirq/circuits.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_cirq/tests/test_cirq_utils.py` & `qbraid-0.4.1/qbraid/interface/qbraid_cirq/tests/test_cirq_utils.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_cirq/tools.py` & `qbraid-0.4.1/qbraid/interface/qbraid_cirq/tools.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_pyquil/programs.py` & `qbraid-0.4.1/qbraid/interface/qbraid_pyquil/programs.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_pyquil/tools.py` & `qbraid-0.4.1/qbraid/interface/qbraid_pyquil/tools.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_pytket/circuits.py` & `qbraid-0.4.1/qbraid/interface/qbraid_pytket/circuits.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_pytket/tools.py` & `qbraid-0.4.1/qbraid/interface/qbraid_pytket/tools.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_qiskit/circuits.py` & `qbraid-0.4.1/qbraid/interface/qbraid_qiskit/circuits.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/qbraid_qiskit/tools.py` & `qbraid-0.4.1/qbraid/interface/qbraid_qiskit/tools.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/tests/test_calculate_unitary.py` & `qbraid-0.4.1/qbraid/interface/tests/test_calculate_unitary.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 """
 from itertools import chain, combinations
 
 import numpy as np
 import pytest
 from braket.circuits import Circuit, Instruction, gates
 from pytket.circuit import Circuit as TKCircuit
-from pytket.circuit import OpType
 
 from qbraid.exceptions import ProgramTypeError
-from qbraid.interface.calculate_unitary import to_unitary, unitary_to_little_endian
+from qbraid.interface.calculate_unitary import (
+    random_unitary_matrix,
+    to_unitary,
+    unitary_to_little_endian,
+)
 from qbraid.interface.convert_to_contiguous import convert_to_contiguous
 
 
 def get_subsets(nqubits):
     """Return list of all combinations up to number nqubits"""
     qubits = list(range(0, nqubits))
     combos = lambda x: combinations(qubits, x)
@@ -110,17 +113,22 @@
     if flat:
         assert c_unitary.shape[0] == 2**2
     else:
         assert c_unitary.shape[0] == 2**4
 
 
 def test_qasm_depth():
-    from qbraid.interface.qbraid_qasm.circuits import qasm_bell, qasm_shared15
+    from qbraid.interface.qbraid_qasm.circuits import qasm2_bell, qasm2_shared15
     from qbraid.interface.qbraid_qasm.tools import qasm_depth
 
-    assert qasm_depth(qasm_bell()) == 2
-    assert qasm_depth(qasm_shared15()) == 22
+    assert qasm_depth(qasm2_bell()) == 2
+    assert qasm_depth(qasm2_shared15()) == 22
 
 
 def test_unitary_raises():
     with pytest.raises(ProgramTypeError):
         to_unitary(None)
+
+
+def test_random_unitary():
+    matrix = random_unitary_matrix(2)
+    assert np.allclose(matrix @ matrix.conj().T, np.eye(2))
```

### Comparing `qbraid-0.4.0/qbraid/interface/tests/test_convert_to_contiguous.py` & `qbraid-0.4.1/qbraid/interface/tests/test_convert_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/interface/tests/test_programs.py` & `qbraid-0.4.1/qbraid/interface/tests/test_programs.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,43 +22,43 @@
 
 map, _ = bell_data()
 braket_bell = map["braket"]()
 cirq_bell = map["cirq"]()
 pyquil_bell = map["pyquil"]()
 qiskit_bell = map["qiskit"]()
 pytket_bell = map["pytket"]()
-qasm_bell = map["qasm"]()
+qasm2_bell = map["qasm2"]()
 
 map, _ = shared15_data()
 braket_shared15 = map["braket"]()
 cirq_shared15 = map["cirq"]()
 qiskit_shared15 = map["qiskit"]()
 pytket_shared15 = map["pytket"]()
-qasm_shared15 = map["qasm"]()
+qasm2_shared15 = map["qasm2"]()
 
 
 def test_bell():
     """Test the equality of bell circuits"""
 
     eq1 = circuits_allclose(braket_bell, cirq_bell, strict_gphase=True)
     eq2 = circuits_allclose(cirq_bell, pyquil_bell, strict_gphase=True)
     eq3 = circuits_allclose(pyquil_bell, qiskit_bell, strict_gphase=True)
     eq4 = circuits_allclose(qiskit_bell, pytket_bell, strict_gphase=True)
-    eq5 = circuits_allclose(pytket_bell, qasm_bell, strict_gphase=True)
+    eq5 = circuits_allclose(pytket_bell, qasm2_bell, strict_gphase=True)
 
     assert eq1 and eq2 and eq3 and eq4 and eq5
 
 
 def test_shared15():
     """Test the equality of shared gates circuits"""
 
     eq1 = circuits_allclose(braket_shared15, cirq_shared15, strict_gphase=True)
     eq2 = circuits_allclose(cirq_shared15, qiskit_shared15, strict_gphase=True)
     eq3 = circuits_allclose(qiskit_shared15, pytket_shared15, strict_gphase=True)
-    eq4 = circuits_allclose(pytket_shared15, qasm_shared15, strict_gphase=True)
+    eq4 = circuits_allclose(pytket_shared15, qasm2_shared15, strict_gphase=True)
 
     assert eq1 and eq2 and eq3 and eq4
 
 
 @pytest.mark.parametrize("package", ["braket", "cirq", "qiskit"])
 def test_random(package):
     """Test generating random circuits"""
@@ -86,15 +86,15 @@
      ┌───┐└─┬─┘
 q_1: ┤ H ├──■──
      └───┘     """
     result = circuit_drawer(qiskit_bell, output="text")
     assert result.__str__() == expected
 
 
-@pytest.mark.parametrize("package", ["braket", "cirq", "qiskit", "pytket", "pyquil", "qasm"])
+@pytest.mark.parametrize("package", ["braket", "cirq", "qiskit", "pytket", "pyquil", "qasm2"])
 def test_braket_bell_draw(capfd, package):
     """Test that draw function standard output is of the expected length."""
     circuit_wrapper(eval(f"{package}_bell")).draw(package="braket", output="ascii")
 
     out, err = capfd.readouterr()
     print(out, err)
     assert len(err) == 0
@@ -106,23 +106,23 @@
 
 def test_braket_raises():
     """Test that non-supported output raises error"""
     with pytest.raises(VisualizationError):
         circuit_drawer(braket_bell, output="bad_input")
 
 
-@pytest.mark.parametrize("package", ["braket", "cirq", "qiskit", "pytket", "pyquil", "qasm"])
+@pytest.mark.parametrize("package", ["braket", "cirq", "qiskit", "pytket", "pyquil", "qasm2"])
 def test_cirq_bell_text_draw(capfd, package):
     """Test that draw function standard output is of the expected length."""
     circuit_wrapper(eval(f"{package}_bell")).draw(package="cirq", output="text")
 
     out, err = capfd.readouterr()
     print(out, err)
     assert len(err) == 0
-    if package == "pytket" or package == "qasm":  # todo: there is "q_n" represent number of qubit
+    if package == "pytket" or package == "qasm2":  # todo: there is "q_n" represent number of qubit
         assert len(out) == 48
     else:
         assert len(out) == 42
 
 
 def test_cirq_bell_svg_draw():
     """Test svg_source"""
@@ -131,15 +131,15 @@
 
 
 def test_cirq_raises():
     with pytest.raises(VisualizationError):
         circuit_drawer(cirq_bell, output="bad_input")
 
 
-@pytest.mark.parametrize("package", ["braket", "cirq", "qiskit", "pytket", "pyquil", "qasm"])
+@pytest.mark.parametrize("package", ["braket", "cirq", "qiskit", "pytket", "pyquil", "qasm2"])
 def test_pyquil_bell_draw(capfd, package):
     """Test that draw function standard output is of the expected length."""
     circuit_wrapper(eval(f"{package}_bell")).draw(package="pyquil", output="text")
 
     out, err = capfd.readouterr()
     print(out, err)
     assert len(err) == 0
@@ -148,13 +148,13 @@
 
 def test_pyquil_raises():
     with pytest.raises(VisualizationError):
         circuit_drawer(pyquil_bell, output="bad_input")
 
 
 def test_pytket_draw():
-    assert len(circuit_drawer(pytket_bell, output="html")) == 1922
+    assert len(circuit_drawer(pytket_bell, output="html")) == 2381
 
 
 def test_pytket_raises():
     with pytest.raises(VisualizationError):
         circuit_drawer(pytket_bell, output="bad_input")
```

### Comparing `qbraid-0.4.0/qbraid/tests/test_top_level.py` & `qbraid-0.4.1/qbraid/tests/test_top_level.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,28 +8,33 @@
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Unit tests for qbraid top-level functionality
 
 """
+import os
 import sys
 from unittest.mock import Mock
 
 import pytest
 
 from qbraid import __version__
 from qbraid._warnings import _warn_new_version
 from qbraid.display_utils import running_in_jupyter, update_progress_bar
 from qbraid.exceptions import PackageValueError
 from qbraid.get_devices import get_devices
 from qbraid.get_jobs import _display_jobs_jupyter, get_jobs
 
 # pylint: disable=missing-function-docstring,redefined-outer-name
 
+# Skip tests if IBM/AWS account auth/creds not configured
+skip_remote_tests: bool = os.getenv("QBRAID_RUN_REMOTE_TESTS") is None
+REASON = "QBRAID_RUN_REMOTE_TESTS not set (requires configuration of qBraid/AWS/IBM storage)"
+
 check_version_data = [
     # local, API, warn
     ("0.1.0", "0.1.1", True),
     ("1.0.7", "1.0.8", True),
     ("1.3.2", "2.0.6", True),
     ("0.1.0", "0.1.0", False),
     ("0.2.4.dev1", "0.2.4", False),
@@ -101,25 +106,27 @@
 
 
 def test_ipython_imported_and_in_jupyter():
     _mock_ipython(MockIPython("non-empty kernel"))
     assert running_in_jupyter()
 
 
+@pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_get_jobs_no_results(capfd):
     """Test ``get_jobs`` stdout for results == 0.
     When no results are found, a single line is printed.
     """
     _mock_ipython(MockIPython(None))
     get_jobs(filters={"circuitNumQubits": -1})
     out, err = capfd.readouterr()
     assert out == "No jobs found matching given criteria\n"
     assert len(err) == 0
 
 
+@pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_get_jobs_results(capfd):
     """Test ``get_jobs`` stdout for results > 0.
     When results returned, output format is as follows:
     (1) Progress bar
     (2) Message
     (3) Empty line
     (4) Section titles
@@ -135,14 +142,15 @@
     get_jobs(filters={"numResults": num_results})
     out, err = capfd.readouterr()
     lines_out = len(out.split("\n"))
     assert lines_out == lines_expected
     assert len(err) == 0
 
 
+@pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_display_jobs_in_jupyter(capfd):
     _mock_ipython(MockIPython("non-empty kernel"))
     data = []
     for index, value in enumerate(job_status_list):
         job_id = f"job_{index}"
         timestamp = f"timestamp_{index}"
         status_str = value
@@ -151,14 +159,15 @@
     msg = "test123"
     _display_jobs_jupyter(data, msg)
     out, err = capfd.readouterr()
     assert "IPython.core.display.HTML object" in out
     assert len(err) == 0
 
 
+@pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_get_jobs_in_jupyter(capfd):
     _mock_ipython(MockIPython("non-empty kernel"))
     get_jobs()
     out, err = capfd.readouterr()
     assert "IPython.core.display.HTML object" in out
     assert len(err) == 0
 
@@ -191,14 +200,15 @@
     lines_expected = 5 + num_results
     out, err = capfd.readouterr()
     lines_out = len(out.split("\n"))
     assert lines_out == lines_expected
     assert len(err) == 0
 
 
+@pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_get_devices_refresh_results(capfd):
     """Test ``get_devices`` stdout for results > 0, with refresh.
     When results returned, output format is as follows:
     (1) Progress bar
     (2) Empty line
     (3) Message
     (4) Empty line
```

### Comparing `qbraid-0.4.0/qbraid/transpiler/__init__.py` & `qbraid-0.4.1/qbraid/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_from_braket.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_braket/convert_from_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_from_braket_qasm.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_braket/convert_from_braket_qasm.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,34 +10,31 @@
 
 """
 Module for converting Braket circuits to Cirq circuit via OpenQASM
 
 """
 
 from braket.circuits import Circuit as BKCircuit
+from braket.circuits.serialization import IRType
 from cirq import Circuit
 from cirq.contrib.qasm_import.exception import QasmException
 
 from qbraid.interface import convert_to_contiguous
 from qbraid.transpiler.cirq_qasm import from_qasm
 from qbraid.transpiler.exceptions import CircuitConversionError
 
 QASMType = str
 
 
 def to_qasm(circuit: BKCircuit) -> QASMType:
-    """Converts a `braket.circuits.Circuit` to an OpenQASM string.
+    """Converts a `braket.circuits.Circuit` to an OpenQASM 2.0 string.
+    *DEPRECATAION NOTICE*: incomplete function, to be removed in next release.
 
-    Args:
-        circuit: Amazon Braket quantum circuit
-
-    Returns:
-        The OpenQASM string equivalent to the circuit
+    .. code-block:: python
 
-    Example:
         >>> from braket.circuits import Circuit
         >>> circuit = Circuit().h(0).cnot(0,1).cnot(1,2)
         >>> print(circuit)
         T  : |0|1|2|
 
         q0 : -H-C---
                 |
@@ -52,19 +49,21 @@
 
         qreg q[3];
 
         h q[0];
         cx q[0],q[1];
         cx q[1],q[2];
 
-    """
-    # OpenQASM 3.0 conversion
-    # from braket.circuits.serialization import IRType
-    # return circuit.to_ir(IRType.OPENQASM).source
+    Args:
+        circuit: Amazon Braket quantum circuit
 
+    Returns:
+        The OpenQASM string equivalent to the circuit
+
+    """
     # A mapping from Amazon Braket gates to QASM gates
     gates = {
         "cnot": "cx",
         "ccnot": "ccx",
         "i": "id",
         "phaseshift": "p",
         "si": "sdg",
@@ -101,14 +100,58 @@
         for t in range(1, len(targets)):
             code += f", q[{targets[t]}]"
         code += ";\n"
 
     return code
 
 
+def braket_to_qasm3(circuit: BKCircuit) -> QASMType:
+    """Converts a ``braket.circuits.Circuit`` to an OpenQASM 3.0 string.
+
+    .. code-block:: python
+
+        >>> from braket.circuits import Circuit
+        >>> circuit = Circuit().h(0).cnot(0,1).cnot(1,2)
+        >>> print(circuit)
+        T  : |0|1|2|
+
+        q0 : -H-C---
+                |
+        q1 : ---X-C-
+                  |
+        q2 : -----X-
+
+        T  : |0|1|2|
+        >>> print(circuit_to_qasm3(circuit))
+        OPENQASM 3.0;
+        bit[3] b;
+        qubit[3] q;
+        h q[0];
+        cnot q[0], q[1];
+        cnot q[1], q[2];
+        b[0] = measure q[0];
+        b[1] = measure q[1];
+        b[2] = measure q[2];
+
+    Args:
+        circuit: Amazon Braket quantum circuit
+
+    Returns:
+        The OpenQASM 3.0 string equivalent to the circuit
+
+    Raises:
+        CircuitConversionError: If braket to qasm conversion fails
+
+    """
+    try:
+        return circuit.to_ir(IRType.OPENQASM).source
+    except Exception as err:
+        raise CircuitConversionError("Error converting braket circuit to qasm3 string") from err
+
+
 def from_braket(circuit: BKCircuit) -> Circuit:
     """Returns a Cirq circuit equivalent to the input Braket circuit.
 
     Note: The returned Cirq circuit acts on cirq.LineQubit's with indices equal
     to the qubit indices of the Braket circuit.
 
     Args:
```

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_to_braket.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_braket/convert_to_braket.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,16 @@
                 )
             ]
 
         if isinstance(gate, cirq_ops.PhaseDampingChannel):
             return [BKInstruction(braket_noise_gate.PhaseDamping(operation.gate._gamma), target)]
 
         matrix = protocols.unitary(gate)
-        return _to_one_qubit_braket_instruction(matrix, target, gate_name=str(gate))
+        gate_name = "U" if isinstance(gate, cirq_ops.MatrixGate) else str(gate)
+        return _to_one_qubit_braket_instruction(matrix, target, gate_name=gate_name)
 
     if isinstance(operation, np.ndarray):
         return instruction_from_matrix(operation, target, gate_name)
 
     if isinstance(operation, cirq_ops.Operation):
         gate = operation.gate
     elif isinstance(operation, cirq_ops.Gate):
```

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_braket/custom_gates.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_braket/custom_gates.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/_gate_archive.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/_gate_archive.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_from_braket.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/test_from_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_from_braket_qasm.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/test_from_braket_qasm.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import numpy as np
 import pytest
 from braket.circuits import Circuit as BKCircuit
 from braket.circuits import Instruction
 from braket.circuits import gates as braket_gates
 
 from qbraid.interface import circuits_allclose
-from qbraid.transpiler.cirq_braket.convert_from_braket_qasm import from_braket
+from qbraid.transpiler.cirq_braket.convert_from_braket_qasm import braket_to_qasm3, from_braket
 from qbraid.transpiler.exceptions import CircuitConversionError
 
 
 def test_from_braket_bell_circuit():
     """Test converting bell circuit"""
     # pylint: disable-next=no-member
     braket_circuit = BKCircuit().h(0).cnot(0, 1)
@@ -119,7 +119,22 @@
         instr = Instruction(
             braket_gates.Unitary(_rotation_of_pi_over_7(num_qubits)),
             target=list(range(num_qubits)),
         )
         braket_circuit.add_instruction(instr)
         with pytest.raises(CircuitConversionError):
             from_braket(braket_circuit)
+
+
+def test_braket_to_qasm3__bell_circuit():
+    """Test converting braket bell circuit to OpenQASM 3.0 string"""
+    qasm_expected = """
+OPENQASM 3.0;
+bit[2] b;
+qubit[2] q;
+h q[0];
+cnot q[0], q[1];
+b[0] = measure q[0];
+b[1] = measure q[1];
+"""
+    bell = BKCircuit().h(0).cnot(0, 1)
+    assert qasm_expected.strip("\n") == braket_to_qasm3(bell)
```

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_to_braket.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/test_to_braket.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 """
 import numpy as np
 import pytest
 from braket.circuits import noises as braket_noise_gate
 from cirq import Circuit, LineQubit, ops, testing
 
-from qbraid.interface import circuits_allclose
+from qbraid.interface import circuits_allclose, random_unitary_matrix
 from qbraid.transpiler.cirq_braket.convert_to_braket import to_braket
 
 
 @pytest.mark.parametrize("qreg", (LineQubit.range(2), [LineQubit(1), LineQubit(6)]))
 def test_to_braket_bell_circuit(qreg):
     """Test converting bell circuit"""
     cirq_circuit = Circuit(ops.H(qreg[0]), ops.CNOT(*qreg))
@@ -277,7 +277,14 @@
     K1 = np.sqrt(0.2) * np.kron(np.array([[0, 1], [1, 0]]), np.array([[0, 1], [1, 0]]))
     cirq_circuit = Circuit(ops.KrausChannel([K0, K1]).on(*LineQubit.range(2)))
     braket_circuit = to_braket(cirq_circuit)
     Gate = braket_circuit.instructions[0].operator
     assert type(Gate) == braket_noise_gate.Kraus
     assert Gate.qubit_count == 2
     assert np.allclose(Gate._matrices, [K0, K1])
+
+
+def test_braket_unitary_display_name():
+    """Test braket unitary gate uses correct display name"""
+    unitary = random_unitary_matrix(2)
+    braket_circuit = to_braket(Circuit(ops.MatrixGate(unitary).on(LineQubit(0))))
+    assert braket_circuit.instructions[0].operator.ascii_symbols[0] == "U"
```

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_to_braket_measure.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_braket/tests/test_to_braket_measure.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/__init__.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_pyquil/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/conversions.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_pyquil/conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/tests/test_conversions_pyquil.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_pyquil/tests/test_conversions_pyquil.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_pytket/__init__.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_pytket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_pytket/conversions.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_pytket/conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_conversions_pytket.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_pytket/tests/test_conversions_pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_to_pytket.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_pytket/tests/test_to_pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/__init__.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_conversions.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qasm/qasm_conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_parser.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qasm/qasm_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -278,14 +278,16 @@
             qasm_gate='ch', cirq_gate=ops.ControlledGate(ops.H), num_params=0, num_args=2
         ),
         'swap': QasmGateStatement(qasm_gate='swap', cirq_gate=ops.SWAP, num_params=0, num_args=2),
         'cswap': QasmGateStatement(
             qasm_gate='cswap', num_params=0, num_args=3, cirq_gate=ops.CSWAP
         ),
         'ccx': QasmGateStatement(qasm_gate='ccx', num_params=0, num_args=3, cirq_gate=ops.CCX),
+        'c3x': QasmGateStatement(qasm_gate='c3x', num_params=0, num_args=4, cirq_gate=ops.ControlledGate(ops.CCX)),
+        'c4x': QasmGateStatement(qasm_gate='c4x', num_params=0, num_args=5, cirq_gate=ops.ControlledGate(ops.ControlledGate(ops.CCX))),
         'sdg': QasmGateStatement(qasm_gate='sdg', num_params=0, num_args=1, cirq_gate=ops.S**-1),
         'csdg': QasmGateStatement(qasm_gate='csdg', num_params=0, num_args=2, cirq_gate=ops.ControlledGate(ops.S**-1)),
         'tdg': QasmGateStatement(qasm_gate='tdg', num_params=0, num_args=1, cirq_gate=ops.T**-1),
         'crz': QasmGateStatement(
             qasm_gate='crz',
             cirq_gate=(lambda params: ops.ControlledGate(ops.rz(params[0]))),
             num_params=1,
@@ -299,14 +301,17 @@
         ),
         'csx': QasmGateStatement(
             qasm_gate='csx', num_params=0, num_args=2, cirq_gate=ops.ControlledGate(ops.XPowGate(exponent=0.5))
         ),
         'c3sx': QasmGateStatement(
             qasm_gate='c3sx', num_params=0, num_args=4, cirq_gate=ops.ControlledGate(ops.ControlledGate(ops.ControlledGate(ops.XPowGate(exponent=0.5))))
         ),
+        'c3sqrtx': QasmGateStatement(
+            qasm_gate='c3sqrtx', num_params=0, num_args=4, cirq_gate=ops.ControlledGate(ops.ControlledGate(ops.ControlledGate(ops.XPowGate(exponent=0.5))))
+        ),
         'cu1': QasmGateStatement(
             qasm_gate='cu1',
             cirq_gate=(lambda params: ops.ControlledGate(ops.ZPowGate(exponent=params[0] / np.pi))),
             num_params=1,
             num_args=2,
         ),
         'cu3': QasmGateStatement(
```

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/_gate_archive.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qasm/tests/_gate_archive.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_parser.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qasm/tests/test_qasm_parser.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_preprocess.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qasm/tests/test_qasm_preprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,15 +32,33 @@
 ecr q[3],q[0];
 rzx_6320157840(2.3200048200765524) q[2],q[1];
 rccx q[1],q[2],q[3];
 csx q[0],q[1];
 rxx(5.603791034636421) q[2],q[0];
 """
 
-qasm_lst = [qasm_0]
+qasm_1 = """
+OPENQASM 2.0;
+include "qelib1.inc";
+qreg q[5];
+rccx q[1],q[2],q[0];
+cu(5.64,3.60,3.73, 5.68) q[1],q[0];
+c3x q[1],q[3],q[0],q[2];
+c3sqrtx q[3],q[1],q[2],q[0];
+c4x q[2],q[0],q[1],q[4],q[3];
+rc3x q[1],q[2],q[0],q[3];
+"""
+
+qasm_lst = [qasm_0, qasm_1]
+
+def strings_equal(s1, s2):
+    """Check if two strings are equal, ignoring spaces and newlines."""
+    s1_clean = s1.replace(" ", "").replace("\n", "")
+    s2_clean = s2.replace(" ", "").replace("\n", "")
+    return s1_clean == s2_clean
 
 
 @pytest.mark.parametrize("qasm_str", qasm_lst)
 def test_preprocess_qasm(qasm_str):
     """Test converting qasm string to format supported by Cirq parser"""
     qiskit_circuit = QuantumCircuit().from_qasm_str(qasm_str)
     supported_qasm = convert_to_supported_qasm(qasm_str)
@@ -149,80 +167,122 @@
 measure b[3] -> ans[3];
 measure cout[0] -> ans[4];
 // quantum ripple-carry adder from Cuccaro et al, quant-ph/0410184
 """
     )
 
 
-@pytest.mark.skip("Conversion test for when update to qiskit>=0.43.0")
 def test_convert_qasm_one_param():
     """Test converting qasm string from one-parameter gate"""
-    assert (
-        convert_to_supported_qasm(
-            """
+
+    qasm_in = """
 OPENQASM 2.0;
 include "qelib1.inc";
 gate ryy(param0) q0,q1 { rx(pi/2) q0; rx(pi/2) q1; cx q0,q1; rz(param0) q1; cx q0,q1; rx(-pi/2) q0; rx(-pi/2) q1; }
 qreg q[2];
 ryy(2.0425171585294746) q[1],q[0];
 """
-        )
-        == """
+    expected_out = """
 OPENQASM 2.0;
 include "qelib1.inc";
 qreg q[2];
 rx(pi/2) q[1];
 rx(pi/2) q[0];
 cx q[1],q[0];
 rz(2.0425171585294746) q[0];
 cx q[1],q[0];
 rx(-pi/2) q[1];
 rx(-pi/2) q[0];
 """
-    )
+    qasm_out = convert_to_supported_qasm(qasm_in)
+    print(qasm_out)
+    assert strings_equal(qasm_out, expected_out)
 
 
-@pytest.mark.skip("Conversion test for when update to qiskit>=0.43.0")
 def test_convert_qasm_two_param():
     """Test converting qasm string from two-parameter gate"""
-    assert (
-        convert_to_supported_qasm(
-            """
+
+    qasm_in = """
 OPENQASM 2.0;
 include "qelib1.inc";
 gate xx_minus_yy(param0,param1) q0,q1 { rz(-1.0*param1) q1; ry(param0/2) q0; }
 qreg q[2];
 xx_minus_yy(2.00367210595874,5.07865952845335) q[0],q[1];
 """
-        )
-        == """
+    expected_out = """
 OPENQASM 2.0;
 include "qelib1.inc";
 qreg q[2];
-rz(-5.07865952845335) q[1];
-ry(1.00367210595874) q[0];
+rz(-1.0*5.07865952845335) q[1];
+ry(2.00367210595874/2) q[0];
 """
-    )
+    qasm_out = convert_to_supported_qasm(qasm_in)
+    assert strings_equal(qasm_out, expected_out)
+
+
+def test_convert_qasm_three_qubit_gate():
+    """Test converting qasm string that uses three qubit gate"""
+
+    qasm_in = """
+OPENQASM 2.0;
+include "qelib1.inc";
+gate ryy(param0) q0,q1,q2 { rx(pi/2) q0; rx(pi/2) q1; cx q0,q2; rz(param0) q1; cx q0,q1; rx(-pi/2) q2; rx(-pi/2) q1; }
+qreg q[3];
+ryy(2.0425171585294746) q[1],q[0],q[2];
+"""
+    expected_out = """
+OPENQASM 2.0;
+include "qelib1.inc";
+qreg q[3];
+rx(pi/2) q[1];
+rx(pi/2) q[0];
+cx q[1],q[2];
+rz(2.0425171585294746) q[0];
+cx q[1],q[0];
+rx(-pi/2) q[2];
+rx(-pi/2) q[0];
+"""
+    qasm_out = convert_to_supported_qasm(qasm_in)
+    assert strings_equal(qasm_out, expected_out)
+
+
+def test_convert_qasm_non_param_gate_def():
+    """Test converting qasm string from non-parameterized gate def"""
+
+    qasm_in = """
+OPENQASM 2.0;
+include "qelib1.inc";
+gate ecr q0,q1 { rzx(pi/4) q0,q1; x q0; rzx(-pi/4) q0,q1; }
+qreg q[2];
+ecr q[0],q[1];
+"""
+    expected_out = """
+OPENQASM 2.0;
+include "qelib1.inc";
+qreg q[2];
+rzx(pi/4) q[0],q[1];
+x q[0];
+rzx(-pi/4) q[0],q[1];
+"""
+    qasm_out = convert_to_supported_qasm(qasm_in)
+    assert strings_equal(qasm_out, expected_out)
 
 
-@pytest.mark.skip("Conversion test for when update to qiskit>=0.43.0")
 def test_convert_qasm_recursive_gate_def():
     """Test converting qasm string from gate defined in terms of another gate"""
-    assert (
-        convert_to_supported_qasm(
-            """
+
+    qasm_in = """
 OPENQASM 2.0;
 include "qelib1.inc";
 gate rzx(param0) q0,q1 { h q1; cx q0,q1; rz(param0) q1; cx q0,q1; h q1; }
 gate ecr q0,q1 { rzx(pi/4) q0,q1; x q0; rzx(-pi/4) q0,q1; }
 qreg q[2];
 ecr q[0],q[1];
 """
-        )
-        == """
+    expected_out = """
 OPENQASM 2.0;
 include "qelib1.inc";
 qreg q[2];
 h q[1];
 cx q[0],q[1];
 rz(pi/4) q[1];
 cx q[0],q[1];
@@ -230,8 +290,9 @@
 x q[0];
 h q[1];
 cx q[0],q[1];
 rz(-pi/4) q[1];
 cx q[0],q[1];
 h q[1];
 """
-    )
+    qasm_out = convert_to_supported_qasm(qasm_in)
+    assert strings_equal(qasm_out, expected_out)
```

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/__init__.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/conversions.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/_gate_archive.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/tests/_gate_archive.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_conversions_qiskit.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/tests/test_conversions_qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_from_qiskit.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/tests/test_from_qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_to_qiskit.py` & `qbraid-0.4.1/qbraid/transpiler/cirq_qiskit/tests/test_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/code/__init__.py` & `qbraid-0.4.1/qbraid/transpiler/code/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/code/qasm_to_braket.py` & `qbraid-0.4.1/qbraid/transpiler/code/qasm_to_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/code/tests/test_qasm_to_braket.py` & `qbraid-0.4.1/qbraid/transpiler/code/tests/test_qasm_to_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/conversions.py` & `qbraid-0.4.1/qbraid/transpiler/conversions.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,20 @@
 Module containing functions for converting to/from Cirq's circuit representation.
 
 """
 from typing import TYPE_CHECKING, Tuple
 
 from cirq import Circuit
 from cirq.contrib.qasm_import import circuit_from_qasm
-from cirq.contrib.qasm_import.exception import QasmException
 
 from qbraid.exceptions import PackageValueError, ProgramTypeError
 from qbraid.transpiler.cirq_braket import from_braket, to_braket
 from qbraid.transpiler.cirq_pyquil import from_pyquil, to_pyquil
 from qbraid.transpiler.cirq_pytket import from_pytket, to_pytket
 from qbraid.transpiler.cirq_qasm import from_qasm, to_qasm
-from qbraid.transpiler.cirq_qasm.qasm_parser import QasmParser
 from qbraid.transpiler.cirq_qiskit import from_qiskit, to_qiskit
 from qbraid.transpiler.exceptions import CircuitConversionError
 
 if TYPE_CHECKING:
     import qbraid
 
 
@@ -45,18 +43,18 @@
 
     Returns:
         A Tuple containing the Cirq circuit equivalent to input circuit and the
             input quantum program type.
     """
     if isinstance(program, str):
         try:
-            QasmParser().parse(program)
-            package = "qasm"
-        except QasmException as err:
-            raise CircuitConversionError("Qbraid only support qasm string.") from err
+            from_qasm(program)
+            package = "qasm2"
+        except Exception as err:
+            raise CircuitConversionError("Invalid OpenQASM 2.0 program.") from err
     else:
         try:
             package = program.__module__
         except AttributeError as err:
             raise ProgramTypeError(program) from err
 
     try:
@@ -68,16 +66,19 @@
 
         if "braket" in package:
             return from_braket(program), "braket"
 
         if "pytket" in package:
             return from_pytket(program), "pytket"
 
-        if "qasm" in package:
-            return from_qasm(program), "qasm"
+        if "qasm2" in package:
+            return from_qasm(program), "qasm2"
+
+        if "qasm3" in package:
+            raise NotImplementedError
 
         if isinstance(program, Circuit):
             return program, "cirq"
 
     except Exception as err:
         raise CircuitConversionError(
             "Quantum program could not be converted to a Cirq circuit."
@@ -109,17 +110,20 @@
 
         if frontend == "braket":
             return to_braket(circuit)
 
         if frontend == "pytket":
             return to_pytket(circuit)
 
-        if frontend == "qasm":
+        if frontend == "qasm2":
             return to_qasm(circuit)
 
+        if frontend == "qasm3":
+            raise NotImplementedError
+
         if frontend == "cirq":
             return circuit
 
     except Exception as err:
         raise CircuitConversionError(
             f"Cirq Circuit could not be converted to a " f"quantum program of type {frontend}."
         ) from err
```

### Comparing `qbraid-0.4.0/qbraid/transpiler/custom_gates.py` & `qbraid-0.4.1/qbraid/transpiler/custom_gates.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/exceptions.py` & `qbraid-0.4.1/qbraid/transpiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/tests/test_conversions.py` & `qbraid-0.4.1/qbraid/transpiler/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/tests/test_transpiler.py` & `qbraid-0.4.1/qbraid/transpiler/tests/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/wrappers/abc_qprogram.py` & `qbraid-0.4.1/qbraid/transpiler/wrappers/abc_qprogram.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/wrappers/braket_circuit.py` & `qbraid-0.4.1/qbraid/transpiler/wrappers/pytket_circuit.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module defining BraketCircuitWrapper Class
+Module defining PytketCircuitWrapper Class
 
 """
-from braket.circuits.circuit import Circuit as BKCircuit
+from pytket.circuit import Circuit as TKCircuit
 
 from qbraid.transpiler.wrappers.abc_qprogram import QuantumProgramWrapper
 
 
-class BraketCircuitWrapper(QuantumProgramWrapper):
-    """Wrapper class for Amazon Braket ``Circuit`` objects."""
+class PytketCircuitWrapper(QuantumProgramWrapper):
+    """Wrapper class for Pytket ``Circuit`` objects."""
 
-    def __init__(self, circuit: BKCircuit):
-        """Create a BraketCircuitWrapper
+    def __init__(self, circuit: TKCircuit):
+        """Create a PytketCircuitWrapper
 
         Args:
             circuit: the circuit object to be wrapped
 
         """
         super().__init__(circuit)
 
         self._qubits = circuit.qubits
-        self._num_qubits = len(self.qubits)
-        self._depth = circuit.depth
-        self._package = "braket"
+        self._num_qubits = circuit.n_qubits
+        self._num_clbits = circuit.n_bits
+        self._depth = circuit.depth()
+        self._package = "pytket"
         self._program_type = "Circuit"
```

### Comparing `qbraid-0.4.0/qbraid/transpiler/wrappers/cirq_circuit.py` & `qbraid-0.4.1/qbraid/transpiler/wrappers/cirq_circuit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/wrappers/pyquil_program.py` & `qbraid-0.4.1/qbraid/transpiler/wrappers/pyquil_program.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/qbraid/transpiler/wrappers/pytket_circuit.py` & `qbraid-0.4.1/qbraid/transpiler/wrappers/qiskit_circuit.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module defining PytketCircuitWrapper Class
+Module defining QiskitCircuitWrapper Class
 
 """
-from pytket.circuit import Circuit as TKCircuit
+from cirq import Circuit
 
 from qbraid.transpiler.wrappers.abc_qprogram import QuantumProgramWrapper
 
 
-class PytketCircuitWrapper(QuantumProgramWrapper):
-    """Wrapper class for Pytket ``Circuit`` objects."""
+class QiskitCircuitWrapper(QuantumProgramWrapper):
+    """Wrapper class for Qiskit ``Circuit`` objects"""
 
-    def __init__(self, circuit: TKCircuit):
-        """Create a PytketCircuitWrapper
-
-        Args:
-            circuit: the circuit object to be wrapped
+    def __init__(self, circuit: Circuit):
+        """Create a QiskitCircuitWrapper
 
+        Args
+            circuit: the qiskit ``Circuit`` object to be wrapped
         """
         super().__init__(circuit)
 
         self._qubits = circuit.qubits
-        self._num_qubits = circuit.n_qubits
-        self._num_clbits = circuit.n_bits
+        self._params = circuit.parameters
+        self._num_qubits = circuit.num_qubits
+        self._num_clbits = circuit.num_clbits
         self._depth = circuit.depth()
-        self._package = "pytket"
-        self._program_type = "Circuit"
+        self._package = "qiskit"
+        self._program_type = "QuantumCircuit"
```

### Comparing `qbraid-0.4.0/qbraid/transpiler/wrappers/qasm_str.py` & `qbraid-0.4.1/qbraid/transpiler/wrappers/qasm_str.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,15 @@
 # pylint: disable=invalid-name
 
 
 """
 Module defining Qasm2CircuitWrapper Class
 
 """
-
-from cirq.circuits import Circuit
-
-from qbraid.interface.qbraid_qasm.tools import qasm_num_qubits, qasm_qubits
-from qbraid.transpiler.cirq_qasm.qasm_conversions import from_qasm
+from qbraid.interface.qbraid_qasm.tools import qasm_depth, qasm_num_qubits, qasm_qubits
 from qbraid.transpiler.wrappers.abc_qprogram import QuantumProgramWrapper
 
 
 class QasmCircuitWrapper(QuantumProgramWrapper):
     """Wrapper class for Cirq ``Circuit`` objects."""
 
     def __init__(self, qasm_str: str):
@@ -34,10 +30,10 @@
 
         """
         # coverage: ignore
         super().__init__(qasm_str)
 
         self._qubits = qasm_qubits(qasm_str)
         self._num_qubits = qasm_num_qubits(qasm_str)
-        self._depth = len(Circuit(from_qasm(qasm_str).all_operations()))
-        self._package = "openqasm"
+        self._depth = qasm_depth(qasm_str)
+        self._package = "qasm2"
         self._program_type = "str"
```

### Comparing `qbraid-0.4.0/qbraid/wrappers.py` & `qbraid-0.4.1/qbraid/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,19 @@
     Raises:
         :class:`~qbraid.QbraidError`: If the input circuit is not a supported quantum program.
 
     """
     if isinstance(program, str):
         try:
             QasmParser().parse(program)
-            package = "qasm"
+            package = "qasm2"
         except QasmException as err:
-            raise QbraidError("Qbraid currently only support qasm string.") from err
+            raise QbraidError(
+                "Input of type string must represent a valid OpenQASM 2 program."
+            ) from err
     else:
         try:
             package = program.__module__.split(".")[0]
         except AttributeError as err:
             raise QbraidError(
                 f"Error applying circuit wrapper to quantum program \
                 of type {type(program)}"
```

### Comparing `qbraid-0.4.0/qbraid.egg-info/PKG-INFO` & `qbraid-0.4.1/qbraid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Home-page: https://github.com/qBraid/qBraid/
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
-License: Restricted
+License: GPL v3.0
 Keywords: qbraid,quantum
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,14 +24,15 @@
 
 <img width=full alt="qbraid-sdk-header" src="https://user-images.githubusercontent.com/46977852/224456452-605e51f2-193d-4789-863e-e51cdd4b0a54.png">
 
 [![CI](https://github.com/qBraid/qBraid/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/qBraid/qBraid/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/qBraid/qBraid/branch/main/graph/badge.svg?token=1UTM0XZB7A)](https://codecov.io/gh/qBraid/qBraid)
 [![Documentation Status](https://readthedocs.com/projects/qbraid-qbraid/badge/?version=latest)](https://docs.qbraid.com/en/latest/?badge=latest)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid.svg?color=blue)](https://pypi.org/project/qbraid/)
+[![License](https://img.shields.io/github/license/qBraid/qbraid.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The qBraid-SDK is a Python toolkit for cross-framework abstraction,
 transpilation, and execution of quantum programs.
 
 [<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git)
 
@@ -44,15 +45,15 @@
   circuit-building package, and **execute** on any backend that interfaces with
   a supported frontend.
 - Benchmark, compare, interpret results. Built-in **compatible** post-processing
   enables comparing results between runs and **across backends**.
 
 ## Installation & Setup
 
-<img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/669bd6f3-bbef-428c-9b59-b421c940262e">
+<img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/c82d61b4-2518-4c7e-8f48-05106afa708e">
 
 For the best experience, install the qBraid-SDK environment on
 [lab.qbraid.com](https://lab.qbraid.com). Login (or
 [create an account](https://account.qbraid.com)) and follow the steps to
 [install an environment](https://docs.qbraid.com/en/latest/lab/environments.html#install-environment).
 
 Using the SDK on qBraid Lab means direct, pre-configured access to all
@@ -92,15 +93,15 @@
 ### Transpiler
 
 Construct a quantum program of any supported program type,
 
 ```python
 >>> from qbraid import QPROGRAM_LIBS
 >>> QPROGRAM_LIBS
-['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm']
+['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm2']
 ```
 
 and use the `circuit_wrapper()` to convert to any other supported program type:
 
 ```python
 >>> from qbraid import circuit_wrapper
 >>> from qbraid.interface import random_circuit
@@ -164,16 +165,15 @@
 >>> aws_result.measurement_counts()
 {'00': 483, '01': 14, '10': 486, '11': 17}
 >>> ibm_result.measurement_counts()
 {'00': 496, '01': 12, '10': 479, '11': 13}
 ```
 
 ## Local account setup
-<img mg align="right" width="350" alt="api_key" src="https://github.com/qBraid/qBraid/assets/32727721/d087c404-e9c7-4a0b-b2a5-a58f2e483cce">
-
+<img mg align="right" width="350" alt="api_key" src="https://github.com/qBraid/qBraid/assets/46977852/86235d04-4b12-40e0-befe-1eeacaac9104">
 
 To use the qBraid-SDK locally (outside of qBraid Lab), you must add your account
 credentials:
 
 1. Create a qBraid account or log in to your existing account by visiting
    [account.qbraid.com](https://account.qbraid.com/v2)
 2. Copy your API Key token from the left side of
@@ -239,16 +239,18 @@
 
 - Interested in contributing code, or making a PR? See
   [CONTRIBUTING.md](CONTRIBUTING.md)
 - For feature requests and bug reports:
   [Submit an issue](https://github.com/qBraid/qBraid/issues)
 - For discussions, and specific questions about the qBraid SDK, qBraid Lab, or
   other topics, [join our discord community](https://discord.gg/gwBebaBZZX)
-- For questions that are more suited for a forum, use the `qbraid` tag on
-  [Stack Exchange](https://quantumcomputing.stackexchange.com/)
+- For questions that are more suited for a forum, post to
+  [Quantum Computing Stack Exchange](https://quantumcomputing.stackexchange.com/)
+  with the [`qbraid`](https://quantumcomputing.stackexchange.com/questions/tagged/qbraid) tag.
+  
 - Want your open-source project featured as its own runtime environment on
   qBraid Lab? Fill out our
   [New Environment Request Form](https://forms.gle/a4v7Kdn7G7bs9jYD8)
 
 ## License
 
 [GNU General Public License v3.0](LICENSE)
```

### Comparing `qbraid-0.4.0/qbraid.egg-info/SOURCES.txt` & `qbraid-0.4.1/qbraid.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+ecosystem.json
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 docs/conf.py
@@ -118,27 +119,29 @@
 qbraid/api/session.py
 qbraid/api/tests/test_api_config.py
 qbraid/api/tests/test_api_thirdparty.py
 qbraid/devices/__init__.py
 qbraid/devices/device.py
 qbraid/devices/enums.py
 qbraid/devices/exceptions.py
+qbraid/devices/ionq.py
 qbraid/devices/job.py
 qbraid/devices/result.py
 qbraid/devices/status_maps.py
 qbraid/devices/aws/__init__.py
 qbraid/devices/aws/device.py
 qbraid/devices/aws/job.py
 qbraid/devices/aws/result.py
 qbraid/devices/ibm/__init__.py
 qbraid/devices/ibm/device.py
 qbraid/devices/ibm/job.py
 qbraid/devices/ibm/provider.py
 qbraid/devices/ibm/result.py
 qbraid/devices/ibm/tests/test_ibm_provider.py
+qbraid/devices/tests/test_braket_ionq.py
 qbraid/devices/tests/test_devices.py
 qbraid/devices/tests/test_enums.py
 qbraid/devices/tests/test_results.py
 qbraid/interface/__init__.py
 qbraid/interface/calculate_unitary.py
 qbraid/interface/convert_to_contiguous.py
 qbraid/interface/draw.py
@@ -154,17 +157,19 @@
 qbraid/interface/qbraid_pyquil/__init__.py
 qbraid/interface/qbraid_pyquil/programs.py
 qbraid/interface/qbraid_pyquil/tools.py
 qbraid/interface/qbraid_pytket/__init__.py
 qbraid/interface/qbraid_pytket/circuits.py
 qbraid/interface/qbraid_pytket/tools.py
 qbraid/interface/qbraid_qasm/__init__.py
+qbraid/interface/qbraid_qasm/circuit_drawer.py
 qbraid/interface/qbraid_qasm/circuits.py
 qbraid/interface/qbraid_qasm/tools.py
-qbraid/interface/qbraid_qasm/test/test_qasm_utils.py
+qbraid/interface/qbraid_qasm/tests/test_circuit_drawer.py
+qbraid/interface/qbraid_qasm/tests/test_qasm_utils.py
 qbraid/interface/qbraid_qiskit/__init__.py
 qbraid/interface/qbraid_qiskit/circuits.py
 qbraid/interface/qbraid_qiskit/tools.py
 qbraid/interface/tests/test_calculate_unitary.py
 qbraid/interface/tests/test_convert_to_contiguous.py
 qbraid/interface/tests/test_programs.py
 qbraid/tests/test_top_level.py
@@ -190,28 +195,34 @@
 qbraid/transpiler/cirq_pytket/tests/test_conversions_pytket.py
 qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py
 qbraid/transpiler/cirq_pytket/tests/test_to_pytket.py
 qbraid/transpiler/cirq_qasm/__init__.py
 qbraid/transpiler/cirq_qasm/qasm_conversions.py
 qbraid/transpiler/cirq_qasm/qasm_parser.py
 qbraid/transpiler/cirq_qasm/qasm_preprocess.py
+qbraid/transpiler/cirq_qasm/qelib1_defs.py
 qbraid/transpiler/cirq_qasm/tests/_gate_archive.py
 qbraid/transpiler/cirq_qasm/tests/test_qasm_parser.py
 qbraid/transpiler/cirq_qasm/tests/test_qasm_preprocess.py
 qbraid/transpiler/cirq_qiskit/__init__.py
 qbraid/transpiler/cirq_qiskit/conversions.py
 qbraid/transpiler/cirq_qiskit/tests/_gate_archive.py
 qbraid/transpiler/cirq_qiskit/tests/test_conversions_qiskit.py
 qbraid/transpiler/cirq_qiskit/tests/test_from_qiskit.py
 qbraid/transpiler/cirq_qiskit/tests/test_to_qiskit.py
 qbraid/transpiler/code/__init__.py
 qbraid/transpiler/code/qasm_to_braket.py
 qbraid/transpiler/code/tests/test_qasm_to_braket.py
 qbraid/transpiler/tests/test_conversions.py
 qbraid/transpiler/tests/test_transpiler.py
+qbraid/transpiler/tests/coverage/test_coverage_from_braket.py
+qbraid/transpiler/tests/coverage/test_coverage_from_cirq.py
+qbraid/transpiler/tests/coverage/test_coverage_from_pyquil.py
+qbraid/transpiler/tests/coverage/test_coverage_from_pytket.py
+qbraid/transpiler/tests/coverage/test_coverage_from_qiskit.py
 qbraid/transpiler/wrappers/__init__.py
 qbraid/transpiler/wrappers/abc_qprogram.py
 qbraid/transpiler/wrappers/braket_circuit.py
 qbraid/transpiler/wrappers/cirq_circuit.py
 qbraid/transpiler/wrappers/pyquil_program.py
 qbraid/transpiler/wrappers/pytket_circuit.py
 qbraid/transpiler/wrappers/qasm_str.py
```

### Comparing `qbraid-0.4.0/setup.cfg` & `qbraid-0.4.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qbraid
-license = Restricted
+license = GPL v3.0
 author = qBraid Development Team
 author_email = contact@qbraid.com
 description = A Python toolkit for cross-framework abstraction of quantum programs.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = qbraid, quantum
 url = https://github.com/qBraid/qBraid/
@@ -19,43 +19,45 @@
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 packages = find:
 python_requires = >=3.9
 install_requires = 
-	amazon-braket-sdk~=1.38.1
-	cirq~=1.1.0
-	numpy>=1.17,<1.24
-	pyquil~=3.4.1
-	pytket<1.13.2
-	qiskit<0.43.0
-	qiskit-ibm-provider<0.5.3
-	requests~=2.30.0
+	amazon-braket-sdk~=1.42.1
+	cirq~=1.2.0.dev20230524233104
+	numpy>=1.17
+	pyquil>=3.5.4,<3.6.0
+	pytket~=1.16.0
+	pytket-braket~=0.27.0
+	qiskit~=0.43.1
+	qiskit-ibm-provider~=0.6.1
+	requests~=2.31.0
 	ipython
 
 [options.extras_require]
 test = 
 	sympy
 	pytest
 	coverage
+	qiskit-qasm3-import
 docs = 
 	sphinx
 	sphinx-autodoc-typehints
 	sphinx-rtd-theme
 	docutils<0.17
 
 [options.entry_points]
 qbraid.transpiler = 
 	braket = qbraid.transpiler:BraketCircuitWrapper
 	cirq = qbraid.transpiler:CirqCircuitWrapper
 	pyquil = qbraid.transpiler:PyQuilProgramWrapper
 	qiskit = qbraid.transpiler:QiskitCircuitWrapper
 	pytket = qbraid.transpiler:PytketCircuitWrapper
-	qasm = qbraid.transpiler:QasmCircuitWrapper
+	qasm2 = qbraid.transpiler:QasmCircuitWrapper
 qbraid.devices = 
 	aws.device = qbraid.devices.aws:AwsDeviceWrapper
 	aws.job = qbraid.devices.aws:AwsQuantumTaskWrapper
 	ibm.device = qbraid.devices.ibm:IBMBackendWrapper
 	ibm.job = qbraid.devices.ibm:IBMJobWrapper
 
 [egg_info]
```

### Comparing `qbraid-0.4.0/setup.py` & `qbraid-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/tools/verify_headers.py` & `qbraid-0.4.1/tools/verify_headers.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.4.0/tox.ini` & `qbraid-0.4.1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 passenv =
     JUPYTERHUB_USER
     REFRESH
     QBRAID_API_KEY
     AWS_ACCESS_KEY_ID
     AWS_SECRET_ACCESS_KEY
     QISKIT_IBM_TOKEN
+    QBRAID_RUN_REMOTE_TESTS
 
 [testenv:unit-tests]
 description = Run pytests and generate coverage report.
 extras = 
     test
 commands =
     coverage run -m pytest -x \
                            qbraid/api \
                            qbraid/interface \
                            qbraid/transpiler \
                            qbraid/devices \
-                           qbraid/tests \ 
+                           qbraid/tests \
                            -W ignore::DeprecationWarning \
                            -W ignore::PendingDeprecationWarning \
                            -W ignore::urllib3.exceptions.InsecureRequestWarning
     coverage combine
     coverage report --omit=qbraid/transpiler/*/_gate_archive.py,qbraid/transpiler/custom_gates.py
     coverage html
     coverage xml
```

