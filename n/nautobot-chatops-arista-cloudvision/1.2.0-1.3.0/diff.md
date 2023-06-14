# Comparing `tmp/nautobot-chatops-arista-cloudvision-1.2.0.tar.gz` & `tmp/nautobot_chatops_arista_cloudvision-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot-chatops-arista-cloudvision-1.2.0.tar", max compression
+gzip compressed data, was "nautobot_chatops_arista_cloudvision-1.3.0.tar", max compression
```

## Comparing `nautobot-chatops-arista-cloudvision-1.2.0.tar` & `nautobot_chatops_arista_cloudvision-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11017 2022-08-31 22:09:06.474676 nautobot-chatops-arista-cloudvision-1.2.0/README.md
--rw-r--r--   0        0        0     1048 2022-08-31 22:09:06.474676 nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/__init__.py
--rw-r--r--   0        0        0     2889 2022-08-31 22:09:06.474676 nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/cvpgrpcutils.py
--rw-r--r--   0        0        0    15260 2022-08-31 22:09:06.474676 nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/static/nautobot_cloudvision/cloudvision_logo.png
--rw-r--r--   0        0        0       65 2022-08-31 22:09:06.474676 nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/tests/__init__.py
--rw-r--r--   0        0        0     1022 2022-08-31 22:09:06.474676 nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/tests/test_api.py
--rw-r--r--   0        0        0      630 2022-08-31 22:09:06.474676 nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/tests/test_basic.py
--rw-r--r--   0        0        0    19721 2022-08-31 22:09:06.474676 nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/utils.py
--rw-r--r--   0        0        0    20134 2022-08-31 22:09:06.474676 nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/worker.py
--rw-r--r--   0        0        0     2638 2022-08-31 22:09:19.290686 nautobot-chatops-arista-cloudvision-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    12515 1970-01-01 00:00:00.000000 nautobot-chatops-arista-cloudvision-1.2.0/setup.py
--rw-r--r--   0        0        0    12117 1970-01-01 00:00:00.000000 nautobot-chatops-arista-cloudvision-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11017 2023-06-14 22:47:46.058622 nautobot_chatops_arista_cloudvision-1.3.0/README.md
+-rw-r--r--   0        0        0     1048 2023-06-14 22:47:46.058622 nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/__init__.py
+-rw-r--r--   0        0        0     2928 2023-06-14 22:47:46.058622 nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/cvpgrpcutils.py
+-rw-r--r--   0        0        0    15260 2023-06-14 22:47:46.058622 nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/static/nautobot_cloudvision/cloudvision_logo.png
+-rw-r--r--   0        0        0       65 2023-06-14 22:47:46.062622 nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2023-06-14 22:47:46.062622 nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/tests/test_api.py
+-rw-r--r--   0        0        0      630 2023-06-14 22:47:46.062622 nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/tests/test_basic.py
+-rw-r--r--   0        0        0    19730 2023-06-14 22:47:46.062622 nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/utils.py
+-rw-r--r--   0        0        0    20133 2023-06-14 22:47:46.062622 nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/worker.py
+-rw-r--r--   0        0        0     2589 2023-06-14 22:47:58.659028 nautobot_chatops_arista_cloudvision-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12089 1970-01-01 00:00:00.000000 nautobot_chatops_arista_cloudvision-1.3.0/PKG-INFO
```

### Comparing `nautobot-chatops-arista-cloudvision-1.2.0/README.md` & `nautobot_chatops_arista_cloudvision-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/__init__.py` & `nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/cvpgrpcutils.py` & `nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/cvpgrpcutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,17 @@
             channel_creds = grpc.ssl_channel_credentials(cert)
             response = requests.post(
                 f"https://{cvp_host}/cvpservice/login/authenticate.do", auth=(username, password), verify=False  # nosec
             )
         # Otherwise, the server is expected to have a valid certificate signed by a well-known CA.
         else:
             channel_creds = grpc.ssl_channel_credentials()
-            response = requests.post(f"https://{cvp_host}/cvpservice/login/authenticate.do", auth=(username, password))
+            response = requests.post(
+                f"https://{cvp_host}/cvpservice/login/authenticate.do", auth=(username, password)
+            )  # nosec
         call_creds = grpc.access_token_call_credentials(response.json()["sessionId"])
     # Set up credentials for CVaaS using supplied token.
     else:
         if CVAAS_ADDR is None:
             cvp_url = "www.arista.io:443"
         else:
             cvp_url = CVAAS_ADDR
```

### Comparing `nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/static/nautobot_cloudvision/cloudvision_logo.png` & `nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/static/nautobot_cloudvision/cloudvision_logo.png`

 * *Files identical despite different names*

### Comparing `nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/tests/test_api.py` & `nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/tests/test_basic.py` & `nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/utils.py` & `nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,15 +538,15 @@
         request = requests.post(
             f"https://{CVP_HOST}/cvpservice/login/authenticate.do",
             auth=(CVP_USERNAME, CVP_PASSWORD),
             verify=False,  # nosec
         )
     else:
         request = requests.post(
-            f"https://{CVP_HOST}/cvpservice/login/authenticate.do", auth=(CVP_USERNAME, CVP_PASSWORD)
+            f"https://{CVP_HOST}/cvpservice/login/authenticate.do", auth=(CVP_USERNAME, CVP_PASSWORD)  # nosec
         )
 
     with open("token.txt", "w") as tokenfile:  # pylint: disable=unspecified-encoding
         tokenfile.write(request.json()["sessionId"])
 
     with open("cvp.crt", "w") as cert_file:  # pylint: disable=unspecified-encoding
         cert_file.write(ssl.get_server_certificate((CVP_HOST, 8443)))
```

### Comparing `nautobot-chatops-arista-cloudvision-1.2.0/nautobot_chatops_arista_cloudvision/worker.py` & `nautobot_chatops_arista_cloudvision-1.3.0/nautobot_chatops_arista_cloudvision/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         f"Standby {dispatcher.user_mention()}, I'm getting the devices from the container {container_name}.",
         ephemeral=True,
     )
 
     devices = get_cloudvision_container_devices(container_name)
 
     if devices:
-
         dispatcher.send_blocks(
             dispatcher.command_response_header(
                 "cloudvision",
                 "get-devices-in-container",
                 [("Container Name", container_name)],
                 "information",
                 cloudvision_logo(dispatcher),
```

### Comparing `nautobot-chatops-arista-cloudvision-1.2.0/pyproject.toml` & `nautobot_chatops_arista_cloudvision-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-chatops-arista-cloudvision"
-version = "v1.2.0"
+version = "v1.3.0"
 description = "Nautobot Chatops Arista Cloudvision Integration"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-chatops-arista-cloudvision"
 repository = "https://github.com/nautobot/nautobot-plugin-chatops-arista-cloudvision"
 keywords = ["nautobot", "nautobot-plugin"]
@@ -17,21 +17,20 @@
 ]
 
 [tool.poetry.plugins."nautobot.workers"]
 "cloudvision" = "nautobot_chatops_arista_cloudvision.worker:cloudvision_chatbot"
 
 [tool.poetry.dependencies]
 # Used for local development
-nautobot = { version = "*", optional = true }
-python = "^3.7"
+nautobot = "^1.5.9"
+python = "^3.8"
 protobuf = "^3.17"
 cvprac = "^1.0.6"
 cloudvision = "^1.1"
 nautobot-chatops = "^1.5.0"
-certifi = "^2021.5.30"
 
 [tool.poetry.dev-dependencies]
 bandit = "*"
 black = "*"
 coverage = "*"
 django-debug-toolbar = "*"
 flake8 = "*"
```

### Comparing `nautobot-chatops-arista-cloudvision-1.2.0/setup.py` & `nautobot_chatops_arista_cloudvision-1.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,229 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['nautobot_chatops_arista_cloudvision',
- 'nautobot_chatops_arista_cloudvision.tests']
-
-package_data = \
-{'': ['*'],
- 'nautobot_chatops_arista_cloudvision': ['static/nautobot_cloudvision/*']}
-
-install_requires = \
-['certifi>=2021.5.30,<2022.0.0',
- 'cloudvision>=1.1,<2.0',
- 'cvprac>=1.0.6,<2.0.0',
- 'nautobot-chatops>=1.5.0,<2.0.0',
- 'protobuf>=3.17,<4.0']
-
-extras_require = \
-{'nautobot': ['nautobot']}
-
-entry_points = \
-{'nautobot.workers': ['cloudvision = '
-                      'nautobot_chatops_arista_cloudvision.worker:cloudvision_chatbot']}
-
-setup_kwargs = {
-    'name': 'nautobot-chatops-arista-cloudvision',
-    'version': '1.2.0',
-    'description': 'Nautobot Chatops Arista Cloudvision Integration',
-    'long_description': '# Arista CloudVision ChatOps\n\nUsing the [Nautobot ChatOps](https://github.com/nautobot/nautobot-plugin-chatops/) base framework, this app adds the ability to gather tag data, device configuration, devices in a specific container, task logs, configlets, device\'s common vulnerabilities and exposures, and device events from Arista\'s CloudVision using Slack, Webex Team, MS Teams, and Mattermost.\n\n## Screenshots\n\n![cloudvision_get_active_events](https://user-images.githubusercontent.com/38091261/128059429-4e4dc269-2113-411b-9721-9ef281a361c5.PNG)\n\n![cloudvision_get_configlet](https://user-images.githubusercontent.com/38091261/128059458-d6395d63-6909-4219-9dcb-dff1801cbda2.PNG)\n\n![cloudvision_get_device_cve](https://user-images.githubusercontent.com/38091261/128059481-2ff60896-81e4-46ae-992b-7d179403fe8f.PNG)\n\n## Installation\n\nThe extension is available as a Python package in PyPI and can be installed with pip\n\n```shell\npip install nautobot-chatops-arista-cloudvision\n```\n\nYou must first update the Nautobot configuration file with a new entry in the `PLUGINS_CONFIG` dictionary.\n\n```python\nPLUGINS_CONFIG = {\n    \'nautobot_chatops\': {\n        \'enable_slack\': True,\n        \'slack_api_token\': os.environ.get("SLACK_API_TOKEN"),\n        \'slack_signing_secret\': os.environ.get("SLACK_SIGNING_SECRET")\n    },\n    \'nautobot_chatops_arista_cloudvision\' : {\n        \'cvaas_token\': os.environ.get("CVAAS_TOKEN"),\n        \'cvp_username\': os.environ.get("CVP_USERNAME"),\n        \'cvp_password\': os.environ.get("CVP_PASSWORD"),\n        \'cvp_host\': os.environ.get("CVP_HOST"),\n        \'cvp_insecure\': os.environ.get("CVP_INSECURE"),\n        \'on_prem\': os.environ.get("ON_PREM")\n    }\n}\n```\n\nAfter that, you must update environment variables depending on if you are using a CVaaS (CloudVision as a Service) or CloudVision on-premise. To update environment variables in Nautobot check out our blog post [here](http://blog.networktocode.com/post/creating-custom-chat-commands-using-nautobot-chatops/)\n\nFor CVAAS the following environment variables must be set.\n\n- `CVAAS_TOKEN`: Token generated from CVAAS service account. Documentation for that process can be found [here](https://www.arista.com/assets/data/pdf/qsg/qsg-books/QS_CloudVision_as_a_Service.pdf) in section 1.7\n- `CVAAS_URL`: This is the url of your CloudVision-as-a-Service. When setting this make sure to include `www`. When not set, this defaults to `www.arista.io`\n\nFor on premise instance of CloudVision, these environment variables must be set.\n\n- `CVP_USERNAME`: The username that will be used to authenticate to CloudVision.\n- `CVP_PASSWORD`: The password for the configured username.\n- `CVP_HOST`: The IP or hostname of the on premise CloudVision appliance.\n- `CVP_INSECURE`: If this is set to `True`, the appliance cert will be downloaded and automatically trusted. Otherwise, the appliance is expected to have a valid certificate.\n- `ON_PREM`: By default this is set to False, this must be changed to `True` if using an on-prem instance of CloudVision.\n\nOnce you have updated your environment file, restart both nautobot and nautobot-worker\n\n```\n$ sudo systemctl daemon-reload\n$ sudo systemctl restart nautobot nautobot-worker\n```\n## Usage\n\n### Command setup\n\nAdd a slash command to Slack called `/cloudvision`.\nSee the [nautobot-chatops installation guide](https://github.com/nautobot/nautobot-plugin-chatops/blob/develop/docs/chat_setup.md) for instructions on adding a slash command to your Slack channel.\n\nThe following commands are available:\n\n- `get-devices-in-container [container-name]`: Retrieves all the devices assigned to the specificied container.\n- `get-configlet [configlet-name]`: Get the configuration of the specified configlet.\n- `get-device-configuration [device-name]`: Get the configuration of the specified device.\n- `get-task-logs [task-id]`: Get the logs of the specified task.\n- `get-applied-configlets [filter-type] [filter-value]`: Get applied configlets to either a specified container or device.\n- `get-active-events [filter-type] [filter-value] [start-time] [end-time]`: Get active events in a given time frame. Filter-type can be filtered by device, type or severity. Filter-value is dynamically created based on the filter-type. Start-time accepts ISO time format as well as relative time inputs. Examples of that are  `-2w`, `-2d`, `-2h` which will go back two weeks, two days and two hours, respectively.\n- `get-tags [device-name]`: Get system or user tags assigned to a device.\n- `get-device-cve [device-name]`: Gets all the CVEs of the specified device. Can also specifiy the `all` parameter to get a count of CVE account for each device.\n\n## Contributing\n\nPull requests are welcomed and automatically built and tested against multiple version of Python and multiple version of Nautobot through TravisCI.\n\nThe project is packaged with a light development environment based on `docker-compose` to help with the local development of the project and to run the tests within TravisCI.\n\nThe project is following Network to Code software development guideline and is leveraging:\n\n- Black, Pylint, Bandit and pydocstyle for Python linting and formatting.\n- Django unit test to ensure the plugin is working properly.\n\n### Development Environment\n\n> A slack workspace is needed to test in a development environment.\n\nThe development environment can be used in 2 ways. First, with a local poetry environment if you wish to develop outside of Docker. Second, inside of a docker container.\n\n#### Invoke tasks\n\nThe [PyInvoke](http://www.pyinvoke.org/) library is used to provide some helper commands based on the environment.  There are a few configuration parameters which can be passed to PyInvoke to override the default configuration:\n\n* `nautobot_ver`: the version of Nautobot to use as a base for any built docker containers (default: 1.2.0)\n* `project_name`: the default docker compose project name (default: nautobot_chatops_arista_cloudvision)\n* `python_ver`: the version of Python to use as a base for any built docker containers (default: 3.8)\n* `local`: a boolean flag indicating if invoke tasks should be run on the host or inside the docker containers (default: False, commands will be run in docker containers)\n* `compose_dir`: the full path to a directory containing the project compose files\n* `compose_files`: a list of compose files applied in order (see [Multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files) for more information)\n\nUsing PyInvoke these configuration options can be overridden using [several methods](http://docs.pyinvoke.org/en/stable/concepts/configuration.html).  Perhaps the simplest is simply setting an environment variable `INVOKE_NAUTOBOT-CHATOPS-EXTENSION-ARISTA_VARIABLE_NAME` where `VARIABLE_NAME` is the variable you are trying to override.  The only exception is `compose_files`, because it is a list it must be overridden in a yaml file.  There is an example `invoke.yml` in this directory which can be used as a starting point.\n\n#### Local Poetry Development Environment\n\n1. Copy `development/creds.example.env` to `development/creds.env` (This file will be ignored by git and docker)\n2. Uncomment the `POSTGRES_HOST`, `REDIS_HOST`, and `NAUTOBOT_ROOT` variables in `development/creds.env`\n3. Create an invoke.yml with the following contents at the root of the repo:\n\n```shell\n---\nnautobot_chatops_arista_cloudvision:\n  local: true\n  compose_files:\n    - "docker-compose.requirements.yml"\n```\n\n3. Run the following commands:\n\n```shell\npoetry shell\npoetry install --extras nautobot\nexport $(cat development/dev.env | xargs)\nexport $(cat development/creds.env | xargs)\ninvoke start && sleep 5\nnautobot-server migrate\n```\n\n> If you want to develop on the latest develop branch of Nautobot, run the following command: ``poetry add git+https://github.com/nautobot/nautobot@develop``. After the ``@`` symbol must match either a branch or a tag.\n\n4. You can now run nautobot-server commands as you would from the [Nautobot documentation](https://nautobot.readthedocs.io/en/latest/) for example to start the development server:\n\n```shell\nnautobot-server runserver 0.0.0.0:8080 --insecure\n```\n\nNautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).\n\n#### Docker Development Environment\n\nThis project is managed by [Python Poetry](https://python-poetry.org/) and has a few requirements to setup your development environment:\n\n1. Install Poetry, see the [Poetry Documentation](https://python-poetry.org/docs/#installation) for your operating system.\n2. Install Docker, see the [Docker documentation](https://docs.docker.com/get-docker/) for your operating system.\n\nOnce you have Poetry and Docker installed you can run the following commands to install all other development dependencies in an isolated python virtual environment:\n\n```shell\npoetry shell\npoetry install\ninvoke start\n```\n\nNautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).\n\n### CLI Helper Commands\n\nThe project is coming with a CLI helper based on [invoke](http://www.pyinvoke.org/) to help setup the development environment. The commands are listed below in 3 categories `dev environment`, `utility` and `testing`.\n\nEach command can be executed with `invoke <command>`. Environment variables `INVOKE_NAUTOBOT_CHATOPS_PLUGIN_CLOUDVISION_PYTHON_VER` and `INVOKE_NAUTOBOT_CHATOPS_PLUGIN_CLOUDVISION_NAUTOBOT_VER` may be specified to override the default versions. Each command also has its own help `invoke <command> --help`\n\n#### Docker dev environment\n\n```no-highlight\n  build            Build all docker images.\n  debug            Start Nautobot and its dependencies in debug mode.\n  destroy          Destroy all containers and volumes.\n  restart          Restart Nautobot and its dependencies.\n  start            Start Nautobot and its dependencies in detached mode.\n  stop             Stop Nautobot and its dependencies.\n```\n\n#### Utility\n\n```no-highlight\n  cli              Launch a bash shell inside the running Nautobot container.\n  create-user      Create a new user in django (default: admin), will prompt for password.\n  makemigrations   Run Make Migration in Django.\n  nbshell          Launch a nbshell session.\n```\n\n#### Testing\n\n```no-highlight\n  bandit           Run bandit to validate basic static code security analysis.\n  black            Run black to check that Python files adhere to its style standards.\n  flake8           This will run flake8 for the specified name and Python version.\n  pydocstyle       Run pydocstyle to validate docstring formatting adheres to NTC defined standards.\n  pylint           Run pylint code analysis.\n  tests            Run all tests for this plugin.\n  unittest         Run Django unit tests for the plugin.\n```\n\n## Questions\n\nFor any questions or comments, please check the [FAQ](FAQ.md) first and feel free to swing by the [Network to Code slack channel](https://networktocode.slack.com/) (channel #networktocode).\nSign up [here](http://slack.networktocode.com/)\n',
-    'author': 'Network to Code, LLC',
-    'author_email': 'info@networktocode.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nautobot/nautobot-plugin-chatops-arista-cloudvision',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+Metadata-Version: 2.1
+Name: nautobot-chatops-arista-cloudvision
+Version: 1.3.0
+Summary: Nautobot Chatops Arista Cloudvision Integration
+Home-page: https://github.com/nautobot/nautobot-plugin-chatops-arista-cloudvision
+License: Apache-2.0
+Keywords: nautobot,nautobot-plugin
+Author: Network to Code, LLC
+Author-email: info@networktocode.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: nautobot
+Requires-Dist: cloudvision (>=1.1,<2.0)
+Requires-Dist: cvprac (>=1.0.6,<2.0.0)
+Requires-Dist: nautobot (>=1.5.9,<2.0.0) ; extra == "nautobot"
+Requires-Dist: nautobot-chatops (>=1.5.0,<2.0.0)
+Requires-Dist: protobuf (>=3.17,<4.0)
+Project-URL: Repository, https://github.com/nautobot/nautobot-plugin-chatops-arista-cloudvision
+Description-Content-Type: text/markdown
+
+# Arista CloudVision ChatOps
+
+Using the [Nautobot ChatOps](https://github.com/nautobot/nautobot-plugin-chatops/) base framework, this app adds the ability to gather tag data, device configuration, devices in a specific container, task logs, configlets, device's common vulnerabilities and exposures, and device events from Arista's CloudVision using Slack, Webex Team, MS Teams, and Mattermost.
+
+## Screenshots
+
+![cloudvision_get_active_events](https://user-images.githubusercontent.com/38091261/128059429-4e4dc269-2113-411b-9721-9ef281a361c5.PNG)
+
+![cloudvision_get_configlet](https://user-images.githubusercontent.com/38091261/128059458-d6395d63-6909-4219-9dcb-dff1801cbda2.PNG)
+
+![cloudvision_get_device_cve](https://user-images.githubusercontent.com/38091261/128059481-2ff60896-81e4-46ae-992b-7d179403fe8f.PNG)
+
+## Installation
+
+The extension is available as a Python package in PyPI and can be installed with pip
+
+```shell
+pip install nautobot-chatops-arista-cloudvision
+```
+
+You must first update the Nautobot configuration file with a new entry in the `PLUGINS_CONFIG` dictionary.
+
+```python
+PLUGINS_CONFIG = {
+    'nautobot_chatops': {
+        'enable_slack': True,
+        'slack_api_token': os.environ.get("SLACK_API_TOKEN"),
+        'slack_signing_secret': os.environ.get("SLACK_SIGNING_SECRET")
+    },
+    'nautobot_chatops_arista_cloudvision' : {
+        'cvaas_token': os.environ.get("CVAAS_TOKEN"),
+        'cvp_username': os.environ.get("CVP_USERNAME"),
+        'cvp_password': os.environ.get("CVP_PASSWORD"),
+        'cvp_host': os.environ.get("CVP_HOST"),
+        'cvp_insecure': os.environ.get("CVP_INSECURE"),
+        'on_prem': os.environ.get("ON_PREM")
+    }
 }
+```
+
+After that, you must update environment variables depending on if you are using a CVaaS (CloudVision as a Service) or CloudVision on-premise. To update environment variables in Nautobot check out our blog post [here](http://blog.networktocode.com/post/creating-custom-chat-commands-using-nautobot-chatops/)
+
+For CVAAS the following environment variables must be set.
+
+- `CVAAS_TOKEN`: Token generated from CVAAS service account. Documentation for that process can be found [here](https://www.arista.com/assets/data/pdf/qsg/qsg-books/QS_CloudVision_as_a_Service.pdf) in section 1.7
+- `CVAAS_URL`: This is the url of your CloudVision-as-a-Service. When setting this make sure to include `www`. When not set, this defaults to `www.arista.io`
+
+For on premise instance of CloudVision, these environment variables must be set.
+
+- `CVP_USERNAME`: The username that will be used to authenticate to CloudVision.
+- `CVP_PASSWORD`: The password for the configured username.
+- `CVP_HOST`: The IP or hostname of the on premise CloudVision appliance.
+- `CVP_INSECURE`: If this is set to `True`, the appliance cert will be downloaded and automatically trusted. Otherwise, the appliance is expected to have a valid certificate.
+- `ON_PREM`: By default this is set to False, this must be changed to `True` if using an on-prem instance of CloudVision.
+
+Once you have updated your environment file, restart both nautobot and nautobot-worker
+
+```
+$ sudo systemctl daemon-reload
+$ sudo systemctl restart nautobot nautobot-worker
+```
+## Usage
+
+### Command setup
+
+Add a slash command to Slack called `/cloudvision`.
+See the [nautobot-chatops installation guide](https://github.com/nautobot/nautobot-plugin-chatops/blob/develop/docs/chat_setup.md) for instructions on adding a slash command to your Slack channel.
+
+The following commands are available:
+
+- `get-devices-in-container [container-name]`: Retrieves all the devices assigned to the specificied container.
+- `get-configlet [configlet-name]`: Get the configuration of the specified configlet.
+- `get-device-configuration [device-name]`: Get the configuration of the specified device.
+- `get-task-logs [task-id]`: Get the logs of the specified task.
+- `get-applied-configlets [filter-type] [filter-value]`: Get applied configlets to either a specified container or device.
+- `get-active-events [filter-type] [filter-value] [start-time] [end-time]`: Get active events in a given time frame. Filter-type can be filtered by device, type or severity. Filter-value is dynamically created based on the filter-type. Start-time accepts ISO time format as well as relative time inputs. Examples of that are  `-2w`, `-2d`, `-2h` which will go back two weeks, two days and two hours, respectively.
+- `get-tags [device-name]`: Get system or user tags assigned to a device.
+- `get-device-cve [device-name]`: Gets all the CVEs of the specified device. Can also specifiy the `all` parameter to get a count of CVE account for each device.
+
+## Contributing
+
+Pull requests are welcomed and automatically built and tested against multiple version of Python and multiple version of Nautobot through TravisCI.
+
+The project is packaged with a light development environment based on `docker-compose` to help with the local development of the project and to run the tests within TravisCI.
+
+The project is following Network to Code software development guideline and is leveraging:
+
+- Black, Pylint, Bandit and pydocstyle for Python linting and formatting.
+- Django unit test to ensure the plugin is working properly.
+
+### Development Environment
+
+> A slack workspace is needed to test in a development environment.
+
+The development environment can be used in 2 ways. First, with a local poetry environment if you wish to develop outside of Docker. Second, inside of a docker container.
+
+#### Invoke tasks
+
+The [PyInvoke](http://www.pyinvoke.org/) library is used to provide some helper commands based on the environment.  There are a few configuration parameters which can be passed to PyInvoke to override the default configuration:
+
+* `nautobot_ver`: the version of Nautobot to use as a base for any built docker containers (default: 1.2.0)
+* `project_name`: the default docker compose project name (default: nautobot_chatops_arista_cloudvision)
+* `python_ver`: the version of Python to use as a base for any built docker containers (default: 3.8)
+* `local`: a boolean flag indicating if invoke tasks should be run on the host or inside the docker containers (default: False, commands will be run in docker containers)
+* `compose_dir`: the full path to a directory containing the project compose files
+* `compose_files`: a list of compose files applied in order (see [Multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files) for more information)
+
+Using PyInvoke these configuration options can be overridden using [several methods](http://docs.pyinvoke.org/en/stable/concepts/configuration.html).  Perhaps the simplest is simply setting an environment variable `INVOKE_NAUTOBOT-CHATOPS-EXTENSION-ARISTA_VARIABLE_NAME` where `VARIABLE_NAME` is the variable you are trying to override.  The only exception is `compose_files`, because it is a list it must be overridden in a yaml file.  There is an example `invoke.yml` in this directory which can be used as a starting point.
+
+#### Local Poetry Development Environment
+
+1. Copy `development/creds.example.env` to `development/creds.env` (This file will be ignored by git and docker)
+2. Uncomment the `POSTGRES_HOST`, `REDIS_HOST`, and `NAUTOBOT_ROOT` variables in `development/creds.env`
+3. Create an invoke.yml with the following contents at the root of the repo:
+
+```shell
+---
+nautobot_chatops_arista_cloudvision:
+  local: true
+  compose_files:
+    - "docker-compose.requirements.yml"
+```
+
+3. Run the following commands:
+
+```shell
+poetry shell
+poetry install --extras nautobot
+export $(cat development/dev.env | xargs)
+export $(cat development/creds.env | xargs)
+invoke start && sleep 5
+nautobot-server migrate
+```
+
+> If you want to develop on the latest develop branch of Nautobot, run the following command: ``poetry add git+https://github.com/nautobot/nautobot@develop``. After the ``@`` symbol must match either a branch or a tag.
+
+4. You can now run nautobot-server commands as you would from the [Nautobot documentation](https://nautobot.readthedocs.io/en/latest/) for example to start the development server:
+
+```shell
+nautobot-server runserver 0.0.0.0:8080 --insecure
+```
+
+Nautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).
+
+#### Docker Development Environment
+
+This project is managed by [Python Poetry](https://python-poetry.org/) and has a few requirements to setup your development environment:
+
+1. Install Poetry, see the [Poetry Documentation](https://python-poetry.org/docs/#installation) for your operating system.
+2. Install Docker, see the [Docker documentation](https://docs.docker.com/get-docker/) for your operating system.
+
+Once you have Poetry and Docker installed you can run the following commands to install all other development dependencies in an isolated python virtual environment:
+
+```shell
+poetry shell
+poetry install
+invoke start
+```
+
+Nautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).
+
+### CLI Helper Commands
+
+The project is coming with a CLI helper based on [invoke](http://www.pyinvoke.org/) to help setup the development environment. The commands are listed below in 3 categories `dev environment`, `utility` and `testing`.
+
+Each command can be executed with `invoke <command>`. Environment variables `INVOKE_NAUTOBOT_CHATOPS_PLUGIN_CLOUDVISION_PYTHON_VER` and `INVOKE_NAUTOBOT_CHATOPS_PLUGIN_CLOUDVISION_NAUTOBOT_VER` may be specified to override the default versions. Each command also has its own help `invoke <command> --help`
+
+#### Docker dev environment
+
+```no-highlight
+  build            Build all docker images.
+  debug            Start Nautobot and its dependencies in debug mode.
+  destroy          Destroy all containers and volumes.
+  restart          Restart Nautobot and its dependencies.
+  start            Start Nautobot and its dependencies in detached mode.
+  stop             Stop Nautobot and its dependencies.
+```
+
+#### Utility
+
+```no-highlight
+  cli              Launch a bash shell inside the running Nautobot container.
+  create-user      Create a new user in django (default: admin), will prompt for password.
+  makemigrations   Run Make Migration in Django.
+  nbshell          Launch a nbshell session.
+```
+
+#### Testing
+
+```no-highlight
+  bandit           Run bandit to validate basic static code security analysis.
+  black            Run black to check that Python files adhere to its style standards.
+  flake8           This will run flake8 for the specified name and Python version.
+  pydocstyle       Run pydocstyle to validate docstring formatting adheres to NTC defined standards.
+  pylint           Run pylint code analysis.
+  tests            Run all tests for this plugin.
+  unittest         Run Django unit tests for the plugin.
+```
+
+## Questions
 
+For any questions or comments, please check the [FAQ](FAQ.md) first and feel free to swing by the [Network to Code slack channel](https://networktocode.slack.com/) (channel #networktocode).
+Sign up [here](http://slack.networktocode.com/)
 
-setup(**setup_kwargs)
```

