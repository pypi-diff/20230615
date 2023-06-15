# Comparing `tmp/pystmark-0.5.1.tar.gz` & `tmp/pystmark-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystmark-0.5.1.tar", last modified: Tue Mar 30 15:57:28 2021, max compression
+gzip compressed data, was "pystmark-0.5.3.tar", last modified: Thu Jun 15 16:57:34 2023, max compression
```

## Comparing `pystmark-0.5.1.tar` & `pystmark-0.5.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2021-03-30 15:57:28.000000 pystmark-0.5.1/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2021-03-30 15:57:28.000000 pystmark-0.5.1/pystmark.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)     5126 2021-03-30 15:57:28.000000 pystmark-0.5.1/pystmark.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      359 2021-03-30 15:57:28.000000 pystmark-0.5.1/pystmark.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)       16 2021-03-30 15:57:28.000000 pystmark-0.5.1/pystmark.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       24 2021-03-30 15:57:28.000000 pystmark-0.5.1/pystmark.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2021-03-30 15:57:28.000000 pystmark-0.5.1/pystmark.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)     5126 2021-03-30 15:57:28.000000 pystmark-0.5.1/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      186 2021-03-19 15:02:25.000000 pystmark-0.5.1/AUTHORS.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2021-03-30 15:57:28.000000 pystmark-0.5.1/tests/
--rw-r--r--   0 steve      (501) staff       (20)      121 2019-09-26 07:43:02.000000 pystmark-0.5.1/tests/requirements.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2021-03-30 15:57:28.000000 pystmark-0.5.1/tests/integration/
--rw-r--r--   0 steve      (501) staff       (20)        0 2019-09-26 07:43:02.000000 pystmark-0.5.1/tests/integration/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     1485 2019-09-26 07:43:02.000000 pystmark-0.5.1/tests/integration/test_pystmark.py
--rw-r--r--   0 steve      (501) staff       (20)        0 2019-09-26 07:43:02.000000 pystmark-0.5.1/tests/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)    47316 2021-03-30 15:56:21.000000 pystmark-0.5.1/tests/test_pystmark.py
--rw-r--r--   0 steve      (501) staff       (20)       48 2019-09-26 07:43:02.000000 pystmark-0.5.1/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)     3205 2021-03-30 15:56:21.000000 pystmark-0.5.1/README.md
--rwxr-xr-x   0 steve      (501) staff       (20)     4691 2019-09-26 09:30:00.000000 pystmark-0.5.1/setup.py
--rw-r--r--   0 steve      (501) staff       (20)    59561 2021-03-30 15:56:21.000000 pystmark-0.5.1/pystmark.py
--rw-r--r--   0 steve      (501) staff       (20)       38 2021-03-30 15:57:28.000000 pystmark-0.5.1/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)       65 2021-03-30 15:55:43.000000 pystmark-0.5.1/_pystmark_meta.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-15 16:57:34.004375 pystmark-0.5.3/
+-rw-r--r--   0 steve      (501) staff       (20)      186 2021-03-19 15:02:25.000000 pystmark-0.5.3/AUTHORS.md
+-rw-r--r--   0 steve      (501) staff       (20)     1082 2019-09-26 07:43:02.000000 pystmark-0.5.3/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       48 2019-09-26 07:43:02.000000 pystmark-0.5.3/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)     4134 2023-06-15 16:57:34.004119 pystmark-0.5.3/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     3035 2023-06-15 16:49:05.000000 pystmark-0.5.3/README.md
+-rw-r--r--   0 steve      (501) staff       (20)       65 2023-06-15 16:56:29.000000 pystmark-0.5.3/_pystmark_meta.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-15 16:57:34.002374 pystmark-0.5.3/pystmark.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)     4134 2023-06-15 16:57:33.000000 pystmark-0.5.3/pystmark.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      367 2023-06-15 16:57:33.000000 pystmark-0.5.3/pystmark.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-06-15 16:57:33.000000 pystmark-0.5.3/pystmark.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       16 2023-06-15 16:57:33.000000 pystmark-0.5.3/pystmark.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       24 2023-06-15 16:57:33.000000 pystmark-0.5.3/pystmark.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)    59635 2023-06-15 16:49:05.000000 pystmark-0.5.3/pystmark.py
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-06-15 16:57:34.004451 pystmark-0.5.3/setup.cfg
+-rwxr-xr-x   0 steve      (501) staff       (20)     4691 2023-06-15 16:48:01.000000 pystmark-0.5.3/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-15 16:57:34.003171 pystmark-0.5.3/tests/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2019-09-26 07:43:02.000000 pystmark-0.5.3/tests/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-15 16:57:34.003754 pystmark-0.5.3/tests/integration/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2019-09-26 07:43:02.000000 pystmark-0.5.3/tests/integration/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     1485 2019-09-26 07:43:02.000000 pystmark-0.5.3/tests/integration/test_pystmark.py
+-rw-r--r--   0 steve      (501) staff       (20)      121 2019-09-26 07:43:02.000000 pystmark-0.5.3/tests/requirements.txt
+-rw-r--r--   0 steve      (501) staff       (20)    47316 2021-03-30 15:56:21.000000 pystmark-0.5.3/tests/test_pystmark.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pystmark-0.5.1/pystmark.egg-info/PKG-INFO` & `pystmark-0.5.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,15 @@
 Metadata-Version: 2.1
 Name: pystmark
-Version: 0.5.1
+Version: 0.5.3
 Summary: A Python library for the Postmark API (http://developer.postmarkapp.com/).
 Home-page: https://github.com/xsleonard/pystmark
 Author: Steve Leonard
 Author-email: sleonard76@gmail.com
 License: MIT
-Description: # pystmark
-        
-        [![PyPI version](https://badge.fury.io/py/pystmark.png)](http://badge.fury.io/py/pystmark)
-        [![Build Status](https://travis-ci.org/xsleonard/pystmark.png)](https://travis-ci.org/xsleonard/pystmark)
-        [![Coverage Status](https://coveralls.io/repos/xsleonard/pystmark/badge.png)](https://coveralls.io/r/xsleonard/pystmark)
-        
-        
-        [Postmark API](http://developer.postmarkapp.com/) library for python 2.7, 3.6 and pypy.
-        Built on top of the [requests](http://docs.python-requests.org/en/latest/) library.
-        
-        ## Web Framework Integration
-        
-        * [Flask-Pystmark](https://github.com/xsleonard/flask-pystmark)
-        
-        ## Documentation
-        
-        The full Sphinx-compiled documentation is available here: [https://readthedocs.org/docs/pystmark/en/latest/](https://readthedocs.org/docs/pystmark/en/latest/)
-        
-        ## Example Usage
-        
-        ```python
-        import pystmark
-        
-        API_KEY = 'my_api_key'
-        SENDER = 'me@example.com'
-        
-        # Send a single message
-        message = pystmark.Message(
-            sender=SENDER, to='you@example.com', subject='Hi', text='A message', tag='greeting'
-        )
-        response = pystmark.send(message, api_key=API_KEY)
-        
-        # Send a template message
-        t_model = {
-            'product_name': 'Awesome Product',
-            'name': 'Customer Name',
-            'action_url': 'http://www.example.com/confirmation/aj3s5dopf98sdf',
-            'sender_name': 'Product Team',
-            'product_address_line1': 'Dover',
-            'product_address_line2': 'DE 19012',
-        }
-        
-        message = pystmark.Message(
-            sender=SENDER,
-            to='you@example.com',
-            template_id=11111,
-            template_model=t_model,
-            tag='welcome',
-        )
-        
-        response = pystmark.send_with_template(message, api_key=API_KEY)
-        
-        # Send multiple messages (via Postmark's batch send API)
-        recipients = ['you{0}@example.com'.format(i) for i in xrange(20)]
-        messages = [
-            pystmark.Message(
-                sender=SENDER,
-                to=to,
-                subject='Hi',
-                text='A message',
-                tag='greeting',
-                message_stream='broadcasts',
-            )
-            for to in recipients
-        ]
-        
-        response = pystmark.send_batch(messages, api_key=API_KEY)
-        
-        # Send multiple messages with templates
-        recipients = ['you{0}@example.com'.format(i) for i in xrange(20)]
-        messages = [
-            pystmark.Message(
-                sender=SENDER,
-                to=to,
-                template_id=11111,
-                template_model=t_model,
-                tag='greeting',
-                message_stream='broadcasts',
-            )
-            for to in recipients
-        ]
-        
-        response = pystmark.send_batch_with_templates(messages, api_key=API_KEY)
-        
-        # Check API response error
-        try:
-            response.raise_for_status()
-        except pystmark.UnauthorizedError:
-            print 'Use your real API key'
-        ```
-        
-        ## Contribution
-        
-        1. Fork this repo
-        2. Make your changes and write a test for them
-        3. Add yourself to the [AUTHORS.md](./AUTHORS.md) file and submit a pull request
-        
-        Please run the tests with `./setup.py test --with-integration`, with at least python2.7,
-        before you make a pull request. Requirements for running the tests are in `tests/requirements.txt`.
-        The other versions will be handled by [travis-ci](https://travis-ci.org/).
-        
-        The pep8 tests may fail if using pypy due to [this bug](https://bugs.pypy.org/issue1207),
-        so that test is disabled if pypy is detected.
-        
-        ## Copyright and License
-        
-        pystmark is licensed under the MIT license. See the [LICENSE](./LICENSE) file for full details.
-        
 Keywords: postmark postmarkapp email
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -127,7 +19,127 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Email
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
+# pystmark
+
+[![PyPI version](https://badge.fury.io/py/pystmark.png)](http://badge.fury.io/py/pystmark)
+[![Build Status](https://travis-ci.org/xsleonard/pystmark.png)](https://travis-ci.org/xsleonard/pystmark)
+[![Coverage Status](https://coveralls.io/repos/xsleonard/pystmark/badge.png)](https://coveralls.io/r/xsleonard/pystmark)
+
+
+[Postmark API](http://developer.postmarkapp.com/) library for python 2.7, 3.6 and pypy.
+Built on top of the [requests](http://docs.python-requests.org/en/latest/) library.
+
+## Web Framework Integration
+
+* [Flask-Pystmark](https://github.com/xsleonard/flask-pystmark)
+
+## Documentation
+
+The full Sphinx-compiled documentation is available here: [https://readthedocs.org/docs/pystmark/en/latest/](https://readthedocs.org/docs/pystmark/en/latest/)
+
+## Example Usage
+
+```python
+from pystmark import (
+    Message,
+    send,
+    send_with_template,
+    send_batch,
+    send_batch_with_templates,
+    UnauthorizedError
+)
+
+API_KEY = 'my_api_key'
+SENDER = 'me@example.com'
+
+# Send a single message
+message = Message(
+    sender=SENDER,
+    to='you@example.com',
+    subject='Hi',
+    text='A message',
+    tag='greeting'
+)
+
+response = send(message, api_key=API_KEY)
+
+# Send a template message
+model = {
+    'user_name': 'John Smith',
+    'company': {
+      'name': 'ACME'
+    }
+
+message = Message(
+    sender=SENDER,
+    to='you@example.com',
+    template_id=11111,
+    template_model=model,
+    tag='welcome',
+)
+
+response = send_with_template(message, api_key=API_KEY)
+
+# Send multiple messages
+messages = [
+    Message(
+        sender=SENDER,
+        to='you@example.com',
+        subject='Hi',
+        text='A message',
+        tag='greeting',
+        message_stream='broadcasts',
+    )
+]
+
+response = send_batch(messages, api_key=API_KEY)
+
+# Send multiple messages with templates
+messages = [
+    Message(
+        sender=SENDER,
+        to='you@example.com',
+        template_id=11111,
+        template_model=model,
+        tag='greeting',
+        message_stream='broadcasts',
+    )
+]
+
+response = send_batch_with_templates(messages, api_key=API_KEY)
+
+# Check API response error
+try:
+    response.raise_for_status()
+except UnauthorizedError:
+    print 'Use your real API key'
+
+# Check for errors in each message when sending batch emails:
+for m in response.messages:
+    if m.error_code > 0:
+        print m.message
+```
+
+## Contribution
+
+1. Fork this repo
+2. Make your changes and write a test for them
+3. Add yourself to the [AUTHORS.md](./AUTHORS.md) file and submit a pull request
+
+Please run the tests with `./setup.py test --with-integration`, with at least python2.7,
+before you make a pull request. Requirements for running the tests are in `tests/requirements.txt`.
+The other versions will be handled by [travis-ci](https://travis-ci.org/).
+
+The pep8 tests may fail if using pypy due to [this bug](https://bugs.pypy.org/issue1207),
+so that test is disabled if pypy is detected.
+
+## Copyright and License
+
+pystmark is licensed under the MIT license. See the [LICENSE](./LICENSE) file for full details.
```

### Comparing `pystmark-0.5.1/PKG-INFO` & `pystmark-0.5.3/pystmark.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,15 @@
 Metadata-Version: 2.1
 Name: pystmark
-Version: 0.5.1
+Version: 0.5.3
 Summary: A Python library for the Postmark API (http://developer.postmarkapp.com/).
 Home-page: https://github.com/xsleonard/pystmark
 Author: Steve Leonard
 Author-email: sleonard76@gmail.com
 License: MIT
-Description: # pystmark
-        
-        [![PyPI version](https://badge.fury.io/py/pystmark.png)](http://badge.fury.io/py/pystmark)
-        [![Build Status](https://travis-ci.org/xsleonard/pystmark.png)](https://travis-ci.org/xsleonard/pystmark)
-        [![Coverage Status](https://coveralls.io/repos/xsleonard/pystmark/badge.png)](https://coveralls.io/r/xsleonard/pystmark)
-        
-        
-        [Postmark API](http://developer.postmarkapp.com/) library for python 2.7, 3.6 and pypy.
-        Built on top of the [requests](http://docs.python-requests.org/en/latest/) library.
-        
-        ## Web Framework Integration
-        
-        * [Flask-Pystmark](https://github.com/xsleonard/flask-pystmark)
-        
-        ## Documentation
-        
-        The full Sphinx-compiled documentation is available here: [https://readthedocs.org/docs/pystmark/en/latest/](https://readthedocs.org/docs/pystmark/en/latest/)
-        
-        ## Example Usage
-        
-        ```python
-        import pystmark
-        
-        API_KEY = 'my_api_key'
-        SENDER = 'me@example.com'
-        
-        # Send a single message
-        message = pystmark.Message(
-            sender=SENDER, to='you@example.com', subject='Hi', text='A message', tag='greeting'
-        )
-        response = pystmark.send(message, api_key=API_KEY)
-        
-        # Send a template message
-        t_model = {
-            'product_name': 'Awesome Product',
-            'name': 'Customer Name',
-            'action_url': 'http://www.example.com/confirmation/aj3s5dopf98sdf',
-            'sender_name': 'Product Team',
-            'product_address_line1': 'Dover',
-            'product_address_line2': 'DE 19012',
-        }
-        
-        message = pystmark.Message(
-            sender=SENDER,
-            to='you@example.com',
-            template_id=11111,
-            template_model=t_model,
-            tag='welcome',
-        )
-        
-        response = pystmark.send_with_template(message, api_key=API_KEY)
-        
-        # Send multiple messages (via Postmark's batch send API)
-        recipients = ['you{0}@example.com'.format(i) for i in xrange(20)]
-        messages = [
-            pystmark.Message(
-                sender=SENDER,
-                to=to,
-                subject='Hi',
-                text='A message',
-                tag='greeting',
-                message_stream='broadcasts',
-            )
-            for to in recipients
-        ]
-        
-        response = pystmark.send_batch(messages, api_key=API_KEY)
-        
-        # Send multiple messages with templates
-        recipients = ['you{0}@example.com'.format(i) for i in xrange(20)]
-        messages = [
-            pystmark.Message(
-                sender=SENDER,
-                to=to,
-                template_id=11111,
-                template_model=t_model,
-                tag='greeting',
-                message_stream='broadcasts',
-            )
-            for to in recipients
-        ]
-        
-        response = pystmark.send_batch_with_templates(messages, api_key=API_KEY)
-        
-        # Check API response error
-        try:
-            response.raise_for_status()
-        except pystmark.UnauthorizedError:
-            print 'Use your real API key'
-        ```
-        
-        ## Contribution
-        
-        1. Fork this repo
-        2. Make your changes and write a test for them
-        3. Add yourself to the [AUTHORS.md](./AUTHORS.md) file and submit a pull request
-        
-        Please run the tests with `./setup.py test --with-integration`, with at least python2.7,
-        before you make a pull request. Requirements for running the tests are in `tests/requirements.txt`.
-        The other versions will be handled by [travis-ci](https://travis-ci.org/).
-        
-        The pep8 tests may fail if using pypy due to [this bug](https://bugs.pypy.org/issue1207),
-        so that test is disabled if pypy is detected.
-        
-        ## Copyright and License
-        
-        pystmark is licensed under the MIT license. See the [LICENSE](./LICENSE) file for full details.
-        
 Keywords: postmark postmarkapp email
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -127,7 +19,127 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Email
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
+# pystmark
+
+[![PyPI version](https://badge.fury.io/py/pystmark.png)](http://badge.fury.io/py/pystmark)
+[![Build Status](https://travis-ci.org/xsleonard/pystmark.png)](https://travis-ci.org/xsleonard/pystmark)
+[![Coverage Status](https://coveralls.io/repos/xsleonard/pystmark/badge.png)](https://coveralls.io/r/xsleonard/pystmark)
+
+
+[Postmark API](http://developer.postmarkapp.com/) library for python 2.7, 3.6 and pypy.
+Built on top of the [requests](http://docs.python-requests.org/en/latest/) library.
+
+## Web Framework Integration
+
+* [Flask-Pystmark](https://github.com/xsleonard/flask-pystmark)
+
+## Documentation
+
+The full Sphinx-compiled documentation is available here: [https://readthedocs.org/docs/pystmark/en/latest/](https://readthedocs.org/docs/pystmark/en/latest/)
+
+## Example Usage
+
+```python
+from pystmark import (
+    Message,
+    send,
+    send_with_template,
+    send_batch,
+    send_batch_with_templates,
+    UnauthorizedError
+)
+
+API_KEY = 'my_api_key'
+SENDER = 'me@example.com'
+
+# Send a single message
+message = Message(
+    sender=SENDER,
+    to='you@example.com',
+    subject='Hi',
+    text='A message',
+    tag='greeting'
+)
+
+response = send(message, api_key=API_KEY)
+
+# Send a template message
+model = {
+    'user_name': 'John Smith',
+    'company': {
+      'name': 'ACME'
+    }
+
+message = Message(
+    sender=SENDER,
+    to='you@example.com',
+    template_id=11111,
+    template_model=model,
+    tag='welcome',
+)
+
+response = send_with_template(message, api_key=API_KEY)
+
+# Send multiple messages
+messages = [
+    Message(
+        sender=SENDER,
+        to='you@example.com',
+        subject='Hi',
+        text='A message',
+        tag='greeting',
+        message_stream='broadcasts',
+    )
+]
+
+response = send_batch(messages, api_key=API_KEY)
+
+# Send multiple messages with templates
+messages = [
+    Message(
+        sender=SENDER,
+        to='you@example.com',
+        template_id=11111,
+        template_model=model,
+        tag='greeting',
+        message_stream='broadcasts',
+    )
+]
+
+response = send_batch_with_templates(messages, api_key=API_KEY)
+
+# Check API response error
+try:
+    response.raise_for_status()
+except UnauthorizedError:
+    print 'Use your real API key'
+
+# Check for errors in each message when sending batch emails:
+for m in response.messages:
+    if m.error_code > 0:
+        print m.message
+```
+
+## Contribution
+
+1. Fork this repo
+2. Make your changes and write a test for them
+3. Add yourself to the [AUTHORS.md](./AUTHORS.md) file and submit a pull request
+
+Please run the tests with `./setup.py test --with-integration`, with at least python2.7,
+before you make a pull request. Requirements for running the tests are in `tests/requirements.txt`.
+The other versions will be handled by [travis-ci](https://travis-ci.org/).
+
+The pep8 tests may fail if using pypy due to [this bug](https://bugs.pypy.org/issue1207),
+so that test is disabled if pypy is detected.
+
+## Copyright and License
+
+pystmark is licensed under the MIT license. See the [LICENSE](./LICENSE) file for full details.
```

### Comparing `pystmark-0.5.1/tests/integration/test_pystmark.py` & `pystmark-0.5.3/tests/integration/test_pystmark.py`

 * *Files identical despite different names*

### Comparing `pystmark-0.5.1/tests/test_pystmark.py` & `pystmark-0.5.3/tests/test_pystmark.py`

 * *Files identical despite different names*

### Comparing `pystmark-0.5.1/README.md` & `pystmark-0.5.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,82 +15,92 @@
 ## Documentation
 
 The full Sphinx-compiled documentation is available here: [https://readthedocs.org/docs/pystmark/en/latest/](https://readthedocs.org/docs/pystmark/en/latest/)
 
 ## Example Usage
 
 ```python
-import pystmark
+from pystmark import (
+    Message,
+    send,
+    send_with_template,
+    send_batch,
+    send_batch_with_templates,
+    UnauthorizedError
+)
 
 API_KEY = 'my_api_key'
 SENDER = 'me@example.com'
 
 # Send a single message
-message = pystmark.Message(
-    sender=SENDER, to='you@example.com', subject='Hi', text='A message', tag='greeting'
+message = Message(
+    sender=SENDER,
+    to='you@example.com',
+    subject='Hi',
+    text='A message',
+    tag='greeting'
 )
-response = pystmark.send(message, api_key=API_KEY)
+
+response = send(message, api_key=API_KEY)
 
 # Send a template message
-t_model = {
-    'product_name': 'Awesome Product',
-    'name': 'Customer Name',
-    'action_url': 'http://www.example.com/confirmation/aj3s5dopf98sdf',
-    'sender_name': 'Product Team',
-    'product_address_line1': 'Dover',
-    'product_address_line2': 'DE 19012',
-}
+model = {
+    'user_name': 'John Smith',
+    'company': {
+      'name': 'ACME'
+    }
 
-message = pystmark.Message(
+message = Message(
     sender=SENDER,
     to='you@example.com',
     template_id=11111,
-    template_model=t_model,
+    template_model=model,
     tag='welcome',
 )
 
-response = pystmark.send_with_template(message, api_key=API_KEY)
+response = send_with_template(message, api_key=API_KEY)
 
-# Send multiple messages (via Postmark's batch send API)
-recipients = ['you{0}@example.com'.format(i) for i in xrange(20)]
+# Send multiple messages
 messages = [
-    pystmark.Message(
+    Message(
         sender=SENDER,
-        to=to,
+        to='you@example.com',
         subject='Hi',
         text='A message',
         tag='greeting',
         message_stream='broadcasts',
     )
-    for to in recipients
 ]
 
-response = pystmark.send_batch(messages, api_key=API_KEY)
+response = send_batch(messages, api_key=API_KEY)
 
 # Send multiple messages with templates
-recipients = ['you{0}@example.com'.format(i) for i in xrange(20)]
 messages = [
-    pystmark.Message(
+    Message(
         sender=SENDER,
-        to=to,
+        to='you@example.com',
         template_id=11111,
-        template_model=t_model,
+        template_model=model,
         tag='greeting',
         message_stream='broadcasts',
     )
-    for to in recipients
 ]
 
-response = pystmark.send_batch_with_templates(messages, api_key=API_KEY)
+response = send_batch_with_templates(messages, api_key=API_KEY)
 
 # Check API response error
 try:
     response.raise_for_status()
-except pystmark.UnauthorizedError:
+except UnauthorizedError:
     print 'Use your real API key'
+
+# Check for errors in each message when sending batch emails:
+for m in response.messages:
+    if m.error_code > 0:
+        print m.message
 ```
 
 ## Contribution
 
 1. Fork this repo
 2. Make your changes and write a test for them
 3. Add yourself to the [AUTHORS.md](./AUTHORS.md) file and submit a pull request
```

### Comparing `pystmark-0.5.1/setup.py` & `pystmark-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,23 +107,23 @@
       url='https://github.com/xsleonard/pystmark',
       platforms='any',
       py_modules=['pystmark', '_pystmark_meta'],
       install_requires=['requests>=1.2.0'],
       cmdclass=dict(test=Test),
       license='MIT',
       keywords='postmark postmarkapp email',
-      classifiers=(
+      classifiers=[
           'Development Status :: 4 - Beta',
           'Intended Audience :: Developers',
           'Programming Language :: Python',
           'Programming Language :: Python :: 2.6',
           'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.2',
           'Programming Language :: Python :: 3.3',
           'Programming Language :: Python :: Implementation :: PyPy',
           'License :: OSI Approved :: MIT License',
           'Operating System :: OS Independent',
           'Topic :: Internet :: WWW/HTTP',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Communications :: Email',
-      ))
+      ])
```

### Comparing `pystmark-0.5.1/pystmark.py` & `pystmark-0.5.3/pystmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,18 @@
         Support for bounce and inbound hooks? These should be mostly handled
         in a framework specific manner but there might be some common utilities
         to provide.
         Optionally verify attachment size <=10MB
         Wrapper class for Message attachments and headers?
 """
 
-from collections import Mapping
+try:
+    from collections.abc import Mapping
+except ImportError:
+    from collections import Mapping
 from base64 import b64encode
 import requests
 import mimetypes
 import os.path
 import sys
 
 from _pystmark_meta import __title__, __version__, __license__
@@ -148,15 +151,15 @@
     :type message: A list of `dict` or :class:`Message`
     :param api_key: Your Postmark API key. Required, if `test` is not `True`.
     :param secure: Use the https scheme for the Postmark API.
         Defaults to `True`
     :param test: Use the Postmark Test API. Defaults to `False`.
     :param request_args: Keyword arguments to pass to
         :func:`requests.request`.
-    :rtype: :class:`SendResponse`
+    :rtype: :class:`BatchSendResponse`
     """
     return _default_pyst_batch_template_sender.send(messages=messages,
                                                     api_key=api_key,
                                                     secure=secure,
                                                     test=test,
                                                     **request_args)
```

