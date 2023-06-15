# Comparing `tmp/kombu-5.3.0rc2.tar.gz` & `tmp/kombu-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kombu-5.3.0rc2.tar", last modified: Wed May 31 05:06:15 2023, max compression
+gzip compressed data, was "kombu-5.3.1.tar", last modified: Thu Jun 15 13:15:32 2023, max compression
```

## Comparing `kombu-5.3.0rc2.tar` & `kombu-5.3.1.tar`

### file list

```diff
@@ -1,346 +1,346 @@
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.304806 kombu-5.3.0rc2/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5599 2022-10-19 13:47:58.000000 kombu-5.3.0rc2/AUTHORS
--rw-rw-r--   0 asif      (1000) asif      (1000)      436 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/FAQ
--rw-rw-r--   0 asif      (1000) asif      (1000)      387 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/INSTALL
--rw-rw-r--   0 asif      (1000) asif      (1000)     1664 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/LICENSE
--rw-rw-r--   0 asif      (1000) asif      (1000)      515 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/MANIFEST.in
--rw-rw-r--   0 asif      (1000) asif      (1000)     1613 2023-05-31 05:06:15.304806 kombu-5.3.0rc2/PKG-INFO
--rw-rw-r--   0 asif      (1000) asif      (1000)    13225 2023-05-31 05:03:21.000000 kombu-5.3.0rc2/README.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      980 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/THANKS
--rw-rw-r--   0 asif      (1000) asif      (1000)       82 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/TODO
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.196804 kombu-5.3.0rc2/docs/
--rw-rw-r--   0 asif      (1000) asif      (1000)     8009 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/Makefile
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.196804 kombu-5.3.0rc2/docs/_ext/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/_ext/.keep
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.196804 kombu-5.3.0rc2/docs/_static/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/_static/.keep
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.196804 kombu-5.3.0rc2/docs/_templates/
--rw-rw-r--   0 asif      (1000) asif      (1000)     3082 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/_templates/sidebardonations.html
--rw-rw-r--   0 asif      (1000) asif      (1000)       30 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/changelog.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      938 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/docs/conf.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       20 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/faq.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.200805 kombu-5.3.0rc2/docs/images/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5393 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/images/favicon.ico
--rw-rw-r--   0 asif      (1000) asif      (1000)   115481 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/images/kombu.jpg
--rw-rw-r--   0 asif      (1000) asif      (1000)    24746 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/images/kombusmall.jpg
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.200805 kombu-5.3.0rc2/docs/includes/
--rw-rw-r--   0 asif      (1000) asif      (1000)      453 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/includes/installation.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)    10599 2023-05-31 05:01:54.000000 kombu-5.3.0rc2/docs/includes/introduction.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      726 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/includes/resources.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      216 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/introduction.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     7476 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/make.bat
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.224805 kombu-5.3.0rc2/docs/reference/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2078 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      301 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.abstract.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      354 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.aws.connection.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      315 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.aws.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      353 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.aws.sqs.connection.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      340 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.aws.sqs.message.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      332 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.aws.sqs.queue.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      327 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.aws.sqs.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      324 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.debug.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      347 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.http.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      338 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.http.curl.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      312 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.http.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      317 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.hub.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      320 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.semaphore.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.asynchronous.timer.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      296 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.clocks.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.common.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      745 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.compat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      513 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.compression.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      884 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.connection.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      461 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.exceptions.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.log.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      266 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.matcher.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      280 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.message.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      275 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.mixins.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2335 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.pidbox.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.pools.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      287 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.resource.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6031 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1118 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/docs/reference/kombu.serialization.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2045 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.simple.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      446 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.SLMQ.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2736 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.SQS.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      533 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.azureservicebus.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      557 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.azurestoragequeues.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1883 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      605 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.confluentkafka.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      459 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.consul.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      451 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.etcd.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      493 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.filesystem.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      741 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.librabbitmq.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      466 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.memory.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      465 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.mongodb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      715 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.pyamqp.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      535 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.pyro.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      664 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.qpid.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      576 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.redis.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      543 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1152 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.sqlalchemy.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      772 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.virtual.exchange.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2271 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.virtual.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      484 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.transport.zookeeper.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      315 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.amq_manager.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      313 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.collections.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.compat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      296 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.debug.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.div.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      311 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.encoding.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      302 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.eventio.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      318 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.functional.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      309 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.imports.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.json.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.limits.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      308 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.objects.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.scheduling.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      289 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.text.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.time.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.url.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/reference/kombu.utils.uuid.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.224805 kombu-5.3.0rc2/docs/templates/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1262 2023-03-09 08:07:52.000000 kombu-5.3.0rc2/docs/templates/readme.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.228805 kombu-5.3.0rc2/docs/userguide/
--rw-rw-r--   0 asif      (1000) asif      (1000)     7046 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/userguide/connections.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     7298 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/userguide/consumers.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1047 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/userguide/examples.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6726 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/userguide/failover.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      232 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/userguide/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     3247 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/userguide/introduction.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5458 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/userguide/pools.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     3635 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/docs/userguide/producers.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6997 2023-03-09 08:07:52.000000 kombu-5.3.0rc2/docs/userguide/serialization.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     3929 2022-03-06 04:55:41.000000 kombu-5.3.0rc2/docs/userguide/simple.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.232805 kombu-5.3.0rc2/examples/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1550 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/complete_receive.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1174 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/complete_send.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.232805 kombu-5.3.0rc2/examples/experimental/
--rw-rw-r--   0 asif      (1000) asif      (1000)      746 2023-05-24 14:33:33.000000 kombu-5.3.0rc2/examples/experimental/async_consume.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      321 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/hello_consumer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      349 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/hello_publisher.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      755 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/memory_transport.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.232805 kombu-5.3.0rc2/examples/rpc-tut6/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1447 2023-05-24 14:33:33.000000 kombu-5.3.0rc2/examples/rpc-tut6/rpc_client.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1332 2023-05-24 14:21:55.000000 kombu-5.3.0rc2/examples/rpc-tut6/rpc_server.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1225 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/simple_eventlet_receive.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1181 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/simple_eventlet_send.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      938 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/simple_receive.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1001 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/simple_send.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.232805 kombu-5.3.0rc2/examples/simple_task_queue/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/examples/simple_task_queue/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      994 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/simple_task_queue/client.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      323 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/simple_task_queue/queues.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       92 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/simple_task_queue/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1276 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/examples/simple_task_queue/worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.240805 kombu-5.3.0rc2/kombu/
--rw-rw-r--   0 asif      (1000) asif      (1000)     3902 2023-05-31 05:01:00.000000 kombu-5.3.0rc2/kombu/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4426 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/abstract.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.244805 kombu-5.3.0rc2/kombu/asynchronous/
--rw-rw-r--   0 asif      (1000) asif      (1000)      237 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/asynchronous/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.244805 kombu-5.3.0rc2/kombu/asynchronous/aws/
--rw-rw-r--   0 asif      (1000) asif      (1000)      475 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/asynchronous/aws/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8538 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/asynchronous/aws/connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      522 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/asynchronous/aws/ext.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.244805 kombu-5.3.0rc2/kombu/asynchronous/aws/sqs/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/kombu/asynchronous/aws/sqs/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6808 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/asynchronous/aws/sqs/connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      131 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/asynchronous/aws/sqs/ext.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      892 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/asynchronous/aws/sqs/message.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4402 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/asynchronous/aws/sqs/queue.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1773 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/asynchronous/debug.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.248805 kombu-5.3.0rc2/kombu/asynchronous/http/
--rw-rw-r--   0 asif      (1000) asif      (1000)      863 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/asynchronous/http/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9592 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/asynchronous/http/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9752 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/kombu/asynchronous/http/curl.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11946 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/asynchronous/hub.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3521 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/asynchronous/semaphore.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6940 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/asynchronous/timer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4825 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/clocks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13529 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/common.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6752 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/compat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2984 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/compression.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    40843 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    33036 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/entity.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2838 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/kombu/exceptions.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4066 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/log.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4269 2022-06-29 07:05:26.000000 kombu-5.3.0rc2/kombu/matcher.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8151 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/message.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    24260 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/messaging.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9701 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/mixins.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    14789 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/pidbox.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3975 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/pools.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7735 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/resource.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    15430 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/serialization.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5302 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/simple.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.256805 kombu-5.3.0rc2/kombu/transport/
--rw-rw-r--   0 asif      (1000) asif      (1000)     6215 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/transport/SLMQ.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    34140 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/transport/SQS.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3342 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/transport/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    15985 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/transport/azureservicebus.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8894 2023-03-09 08:07:52.000000 kombu-5.3.0rc2/kombu/transport/azurestoragequeues.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7687 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/transport/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12106 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/kombu/transport/confluentkafka.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9424 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/transport/consul.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8644 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/transport/etcd.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10416 2022-10-19 13:47:58.000000 kombu-5.3.0rc2/kombu/transport/filesystem.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6022 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/transport/librabbitmq.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2404 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/transport/memory.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    15041 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/transport/mongodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7752 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/transport/pyamqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5844 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/transport/pyro.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    71681 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/transport/qpid.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    48481 2023-05-31 04:56:03.000000 kombu-5.3.0rc2/kombu/transport/redis.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.256805 kombu-5.3.0rc2/kombu/transport/sqlalchemy/
--rw-rw-r--   0 asif      (1000) asif      (1000)     7448 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/transport/sqlalchemy/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2302 2023-03-09 08:07:52.000000 kombu-5.3.0rc2/kombu/transport/sqlalchemy/models.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.256805 kombu-5.3.0rc2/kombu/transport/virtual/
--rw-rw-r--   0 asif      (1000) asif      (1000)      476 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/transport/virtual/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    34231 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/transport/virtual/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4894 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/transport/virtual/exchange.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6339 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/transport/zookeeper.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.260805 kombu-5.3.0rc2/kombu/utils/
--rw-rw-r--   0 asif      (1000) asif      (1000)      698 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/utils/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      716 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/utils/amq_manager.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      942 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/utils/collections.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3444 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/utils/compat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1673 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/utils/debug.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      908 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/utils/div.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2297 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/utils/encoding.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10159 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/utils/eventio.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10699 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/utils/functional.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2089 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/utils/imports.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3609 2023-03-09 08:07:52.000000 kombu-5.3.0rc2/kombu/utils/json.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2551 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/utils/limits.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1743 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/utils/objects.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2928 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/utils/scheduling.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2200 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/utils/text.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      272 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/utils/time.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3804 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/kombu/utils/url.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      327 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/kombu/utils/uuid.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.240805 kombu-5.3.0rc2/kombu.egg-info/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1613 2023-05-31 05:06:14.000000 kombu-5.3.0rc2/kombu.egg-info/PKG-INFO
--rw-rw-r--   0 asif      (1000) asif      (1000)     9284 2023-05-31 05:06:14.000000 kombu-5.3.0rc2/kombu.egg-info/SOURCES.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        1 2023-05-31 05:06:14.000000 kombu-5.3.0rc2/kombu.egg-info/dependency_links.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      641 2023-05-31 05:06:14.000000 kombu-5.3.0rc2/kombu.egg-info/requires.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        6 2023-05-31 05:06:14.000000 kombu-5.3.0rc2/kombu.egg-info/top_level.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.264805 kombu-5.3.0rc2/requirements/
--rw-rw-r--   0 asif      (1000) asif      (1000)      115 2023-05-31 04:56:03.000000 kombu-5.3.0rc2/requirements/default.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       93 2023-03-09 08:07:52.000000 kombu-5.3.0rc2/requirements/dev.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      243 2023-05-31 04:56:03.000000 kombu-5.3.0rc2/requirements/docs.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.268805 kombu-5.3.0rc2/requirements/extras/
--rw-rw-r--   0 asif      (1000) asif      (1000)       25 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/requirements/extras/azureservicebus.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       51 2023-03-20 10:18:51.000000 kombu-5.3.0rc2/requirements/extras/azurestoragequeues.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      111 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/requirements/extras/brotli.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       23 2023-05-24 14:21:55.000000 kombu-5.3.0rc2/requirements/extras/confluentkafka.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/requirements/extras/consul.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/requirements/extras/couchdb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/requirements/extras/etcd.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-11-08 00:17:43.000000 kombu-5.3.0rc2/requirements/extras/librabbitmq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      135 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/requirements/extras/lzma.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/requirements/extras/mongodb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        8 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/requirements/extras/msgpack.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        6 2023-05-24 14:21:55.000000 kombu-5.3.0rc2/requirements/extras/pyro.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       35 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/requirements/extras/qpid.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2023-05-31 04:56:03.000000 kombu-5.3.0rc2/requirements/extras/redis.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/requirements/extras/slmq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       24 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/requirements/extras/sqlalchemy.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       87 2023-05-31 04:56:03.000000 kombu-5.3.0rc2/requirements/extras/sqs.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/requirements/extras/yaml.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/requirements/extras/zookeeper.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/requirements/extras/zstd.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      158 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/requirements/funtest.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      116 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/requirements/pkgutils.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      487 2023-05-31 04:56:03.000000 kombu-5.3.0rc2/requirements/test-ci.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       59 2023-05-31 04:56:03.000000 kombu-5.3.0rc2/requirements/test.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     1172 2023-05-31 05:06:15.304806 kombu-5.3.0rc2/setup.cfg
--rw-rw-r--   0 asif      (1000) asif      (1000)     3837 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/setup.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.268805 kombu-5.3.0rc2/t/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/t/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.268805 kombu-5.3.0rc2/t/integration/
--rw-rw-r--   0 asif      (1000) asif      (1000)      120 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/integration/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17367 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/t/integration/common.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1464 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/t/integration/test_kafka.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3675 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/t/integration/test_mongodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1970 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/integration/test_py_amqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4996 2023-05-31 04:56:03.000000 kombu-5.3.0rc2/t/integration/test_redis.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6008 2022-10-19 13:47:58.000000 kombu-5.3.0rc2/t/mocks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      283 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/skip.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.276805 kombu-5.3.0rc2/t/unit/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/t/unit/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.276805 kombu-5.3.0rc2/t/unit/asynchronous/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/t/unit/asynchronous/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.276805 kombu-5.3.0rc2/t/unit/asynchronous/aws/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/t/unit/asynchronous/aws/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      199 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/asynchronous/aws/case.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.280805 kombu-5.3.0rc2/t/unit/asynchronous/aws/sqs/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/t/unit/asynchronous/aws/sqs/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11941 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/asynchronous/aws/sqs/test_connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7140 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/asynchronous/aws/sqs/test_queue.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      318 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/asynchronous/aws/test_aws.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9277 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/asynchronous/aws/test_connection.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.280805 kombu-5.3.0rc2/t/unit/asynchronous/http/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/t/unit/asynchronous/http/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5728 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/asynchronous/http/test_curl.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4221 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/asynchronous/http/test_http.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17161 2022-10-19 13:47:58.000000 kombu-5.3.0rc2/t/unit/asynchronous/test_hub.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1141 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/asynchronous/test_semaphore.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4247 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/asynchronous/test_timer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9493 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/conftest.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2359 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/t/unit/test_clocks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17580 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_common.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11181 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_compat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2858 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_compression.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    32824 2023-03-09 08:07:52.000000 kombu-5.3.0rc2/t/unit/test_connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13693 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/t/unit/test_entity.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      229 2022-06-19 07:31:49.000000 kombu-5.3.0rc2/t/unit/test_exceptions.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4796 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_log.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1133 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_matcher.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1285 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_message.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    24481 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_messaging.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7875 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_mixins.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12543 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_pidbox.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7238 2022-10-19 13:47:58.000000 kombu-5.3.0rc2/t/unit/test_pools.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11162 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_serialization.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6704 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/test_simple.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.296806 kombu-5.3.0rc2/t/unit/transport/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/t/unit/transport/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    35038 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/t/unit/transport/test_SQS.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13586 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/t/unit/transport/test_azureservicebus.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3455 2023-03-09 08:07:52.000000 kombu-5.3.0rc2/t/unit/transport/test_azurestoragequeues.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5617 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/transport/test_base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2674 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/transport/test_consul.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2197 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/transport/test_etcd.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10594 2022-10-19 13:47:58.000000 kombu-5.3.0rc2/t/unit/transport/test_filesystem.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4891 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/transport/test_librabbitmq.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5643 2022-10-19 13:47:58.000000 kombu-5.3.0rc2/t/unit/transport/test_memory.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    19028 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/t/unit/transport/test_mongodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7008 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/transport/test_pyamqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2892 2022-10-19 13:47:58.000000 kombu-5.3.0rc2/t/unit/transport/test_pyro.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    71045 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/transport/test_qpid.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    60297 2022-08-01 07:19:26.000000 kombu-5.3.0rc2/t/unit/transport/test_redis.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1538 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/transport/test_sqlalchemy.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1014 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/transport/test_transport.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1057 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/transport/test_zookeeper.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.300806 kombu-5.3.0rc2/t/unit/transport/virtual/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/t/unit/transport/virtual/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    21252 2022-10-19 13:47:58.000000 kombu-5.3.0rc2/t/unit/transport/virtual/test_base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5530 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/transport/virtual/test_exchange.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 05:06:15.304806 kombu-5.3.0rc2/t/unit/utils/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.0rc2/t/unit/utils/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1281 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_amq_manager.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2806 2023-03-20 10:18:52.000000 kombu-5.3.0rc2/t/unit/utils/test_compat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1630 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_debug.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1132 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_div.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2962 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_encoding.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8800 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_functional.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      967 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_imports.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2894 2023-05-18 06:10:21.000000 kombu-5.3.0rc2/t/unit/utils/test_json.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1064 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_objects.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2769 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_scheduling.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      459 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_time.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2964 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_url.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      609 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_utils.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      289 2022-04-17 07:07:11.000000 kombu-5.3.0rc2/t/unit/utils/test_uuid.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.097790 kombu-5.3.1/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5599 2022-10-19 13:47:58.000000 kombu-5.3.1/AUTHORS
+-rw-rw-r--   0 asif      (1000) asif      (1000)      436 2021-09-07 04:22:35.000000 kombu-5.3.1/FAQ
+-rw-rw-r--   0 asif      (1000) asif      (1000)      387 2021-09-07 04:22:35.000000 kombu-5.3.1/INSTALL
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1664 2021-09-07 04:22:35.000000 kombu-5.3.1/LICENSE
+-rw-rw-r--   0 asif      (1000) asif      (1000)      515 2021-09-07 04:22:35.000000 kombu-5.3.1/MANIFEST.in
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1610 2023-06-15 13:15:32.097790 kombu-5.3.1/PKG-INFO
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13222 2023-06-15 13:13:28.000000 kombu-5.3.1/README.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      980 2021-09-07 04:22:35.000000 kombu-5.3.1/THANKS
+-rw-rw-r--   0 asif      (1000) asif      (1000)       82 2021-09-07 04:22:35.000000 kombu-5.3.1/TODO
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:31.997787 kombu-5.3.1/docs/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8009 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/Makefile
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:31.997787 kombu-5.3.1/docs/_ext/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/_ext/.keep
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:31.997787 kombu-5.3.1/docs/_static/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/_static/.keep
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.001787 kombu-5.3.1/docs/_templates/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3082 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/_templates/sidebardonations.html
+-rw-rw-r--   0 asif      (1000) asif      (1000)       30 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/changelog.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      938 2022-04-17 07:07:11.000000 kombu-5.3.1/docs/conf.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       20 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/faq.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.001787 kombu-5.3.1/docs/images/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5393 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/images/favicon.ico
+-rw-rw-r--   0 asif      (1000) asif      (1000)   115481 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/images/kombu.jpg
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24746 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/images/kombusmall.jpg
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.001787 kombu-5.3.1/docs/includes/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      453 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/includes/installation.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10596 2023-06-15 13:13:15.000000 kombu-5.3.1/docs/includes/introduction.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      726 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/includes/resources.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      216 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/introduction.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7476 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/make.bat
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.025788 kombu-5.3.1/docs/reference/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2078 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      301 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.abstract.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      354 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.aws.connection.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      315 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.aws.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      353 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.aws.sqs.connection.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      340 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.aws.sqs.message.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      332 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.aws.sqs.queue.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      327 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.aws.sqs.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      324 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.debug.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      347 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.http.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      338 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.http.curl.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      312 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.http.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      317 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.hub.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      320 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.semaphore.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.asynchronous.timer.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      296 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.clocks.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.common.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      745 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.compat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      513 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.compression.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      884 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.connection.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      461 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.exceptions.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.log.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      266 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.matcher.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      280 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.message.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      275 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.mixins.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2335 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.pidbox.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.pools.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      287 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.resource.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6031 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1118 2022-04-17 07:07:11.000000 kombu-5.3.1/docs/reference/kombu.serialization.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2045 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.simple.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      446 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.SLMQ.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2736 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.SQS.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      533 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.azureservicebus.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      557 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.azurestoragequeues.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1883 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      605 2022-06-19 07:31:49.000000 kombu-5.3.1/docs/reference/kombu.transport.confluentkafka.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      459 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.consul.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      451 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.etcd.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      493 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.filesystem.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      741 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.librabbitmq.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      466 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.memory.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      465 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.mongodb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      715 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.pyamqp.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      535 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.pyro.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      664 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.qpid.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      576 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.redis.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      543 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1152 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.sqlalchemy.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      772 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.virtual.exchange.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2271 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.virtual.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      484 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.transport.zookeeper.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      315 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.amq_manager.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      313 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.collections.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.compat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      296 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.debug.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.div.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      311 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.encoding.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      302 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.eventio.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      318 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.functional.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      309 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.imports.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.json.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.limits.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      308 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.objects.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.scheduling.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      289 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.text.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.time.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.url.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/reference/kombu.utils.uuid.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.029788 kombu-5.3.1/docs/templates/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1262 2023-03-09 08:07:52.000000 kombu-5.3.1/docs/templates/readme.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.029788 kombu-5.3.1/docs/userguide/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7046 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/userguide/connections.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7298 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/userguide/consumers.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1047 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/userguide/examples.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6726 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/userguide/failover.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      232 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/userguide/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3247 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/userguide/introduction.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5458 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/userguide/pools.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3635 2021-09-07 04:22:35.000000 kombu-5.3.1/docs/userguide/producers.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6997 2023-03-09 08:07:52.000000 kombu-5.3.1/docs/userguide/serialization.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3929 2022-03-06 04:55:41.000000 kombu-5.3.1/docs/userguide/simple.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.033788 kombu-5.3.1/examples/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1550 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/complete_receive.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1174 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/complete_send.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.033788 kombu-5.3.1/examples/experimental/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      746 2023-05-24 14:33:33.000000 kombu-5.3.1/examples/experimental/async_consume.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      321 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/hello_consumer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      349 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/hello_publisher.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      755 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/memory_transport.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.037788 kombu-5.3.1/examples/rpc-tut6/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1447 2023-05-24 14:33:33.000000 kombu-5.3.1/examples/rpc-tut6/rpc_client.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1332 2023-05-24 14:21:55.000000 kombu-5.3.1/examples/rpc-tut6/rpc_server.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1225 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/simple_eventlet_receive.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1181 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/simple_eventlet_send.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      938 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/simple_receive.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1001 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/simple_send.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.037788 kombu-5.3.1/examples/simple_task_queue/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/examples/simple_task_queue/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      994 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/simple_task_queue/client.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      323 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/simple_task_queue/queues.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       92 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/simple_task_queue/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1276 2022-04-17 07:07:11.000000 kombu-5.3.1/examples/simple_task_queue/worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.045789 kombu-5.3.1/kombu/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3899 2023-06-15 13:12:37.000000 kombu-5.3.1/kombu/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4426 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/abstract.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.045789 kombu-5.3.1/kombu/asynchronous/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      237 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/asynchronous/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.045789 kombu-5.3.1/kombu/asynchronous/aws/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      475 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/asynchronous/aws/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8538 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/asynchronous/aws/connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      522 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/asynchronous/aws/ext.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.049789 kombu-5.3.1/kombu/asynchronous/aws/sqs/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/kombu/asynchronous/aws/sqs/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6808 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/asynchronous/aws/sqs/connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      131 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/asynchronous/aws/sqs/ext.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      892 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/asynchronous/aws/sqs/message.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4402 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/asynchronous/aws/sqs/queue.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1773 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/asynchronous/debug.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.049789 kombu-5.3.1/kombu/asynchronous/http/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      863 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/asynchronous/http/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9592 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/asynchronous/http/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9752 2022-06-19 07:31:49.000000 kombu-5.3.1/kombu/asynchronous/http/curl.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11946 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/asynchronous/hub.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3521 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/asynchronous/semaphore.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6940 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/asynchronous/timer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4825 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/clocks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13529 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/common.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6752 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/compat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2984 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/compression.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    40843 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    33036 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/entity.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2838 2022-06-19 07:31:49.000000 kombu-5.3.1/kombu/exceptions.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4066 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/log.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4269 2022-06-29 07:05:26.000000 kombu-5.3.1/kombu/matcher.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8151 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/message.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24260 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/messaging.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9701 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/mixins.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14789 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/pidbox.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3975 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/pools.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7735 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/resource.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15430 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/serialization.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5302 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/simple.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.057789 kombu-5.3.1/kombu/transport/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6215 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/transport/SLMQ.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    34140 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/transport/SQS.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3342 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/transport/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15985 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/transport/azureservicebus.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8894 2023-03-09 08:07:52.000000 kombu-5.3.1/kombu/transport/azurestoragequeues.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7687 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/transport/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12106 2022-06-19 07:31:49.000000 kombu-5.3.1/kombu/transport/confluentkafka.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9424 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/transport/consul.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8644 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/transport/etcd.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10416 2022-10-19 13:47:58.000000 kombu-5.3.1/kombu/transport/filesystem.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6022 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/transport/librabbitmq.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2404 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/transport/memory.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15041 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/transport/mongodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7752 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/transport/pyamqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5844 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/transport/pyro.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    71681 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/transport/qpid.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    48481 2023-05-31 04:56:03.000000 kombu-5.3.1/kombu/transport/redis.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.057789 kombu-5.3.1/kombu/transport/sqlalchemy/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7448 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/transport/sqlalchemy/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2302 2023-03-09 08:07:52.000000 kombu-5.3.1/kombu/transport/sqlalchemy/models.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.057789 kombu-5.3.1/kombu/transport/virtual/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      476 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/transport/virtual/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    34231 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/transport/virtual/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4894 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/transport/virtual/exchange.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6339 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/transport/zookeeper.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.065789 kombu-5.3.1/kombu/utils/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      698 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/utils/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      716 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/utils/amq_manager.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      942 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/utils/collections.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3444 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/utils/compat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1673 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/utils/debug.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      908 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/utils/div.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2297 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/utils/encoding.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10159 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/utils/eventio.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10699 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/utils/functional.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2089 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/utils/imports.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3587 2023-06-15 12:59:17.000000 kombu-5.3.1/kombu/utils/json.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2551 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/utils/limits.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1743 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/utils/objects.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2928 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/utils/scheduling.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2200 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/utils/text.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      272 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/utils/time.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3804 2022-04-17 07:07:11.000000 kombu-5.3.1/kombu/utils/url.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      327 2023-05-18 06:10:21.000000 kombu-5.3.1/kombu/utils/uuid.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.045789 kombu-5.3.1/kombu.egg-info/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1610 2023-06-15 13:15:31.000000 kombu-5.3.1/kombu.egg-info/PKG-INFO
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9284 2023-06-15 13:15:31.000000 kombu-5.3.1/kombu.egg-info/SOURCES.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        1 2023-06-15 13:15:31.000000 kombu-5.3.1/kombu.egg-info/dependency_links.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      767 2023-06-15 13:15:31.000000 kombu-5.3.1/kombu.egg-info/requires.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        6 2023-06-15 13:15:31.000000 kombu-5.3.1/kombu.egg-info/top_level.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.065789 kombu-5.3.1/requirements/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      123 2023-06-03 06:17:58.000000 kombu-5.3.1/requirements/default.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       93 2023-03-09 08:07:52.000000 kombu-5.3.1/requirements/dev.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      243 2023-05-31 04:56:03.000000 kombu-5.3.1/requirements/docs.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.069789 kombu-5.3.1/requirements/extras/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       25 2023-05-18 06:10:21.000000 kombu-5.3.1/requirements/extras/azureservicebus.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       51 2023-03-20 10:18:51.000000 kombu-5.3.1/requirements/extras/azurestoragequeues.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      111 2023-05-18 06:10:21.000000 kombu-5.3.1/requirements/extras/brotli.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       23 2023-05-24 14:21:55.000000 kombu-5.3.1/requirements/extras/confluentkafka.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.1/requirements/extras/consul.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.1/requirements/extras/couchdb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-09-07 04:22:35.000000 kombu-5.3.1/requirements/extras/etcd.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       44 2023-06-15 12:59:17.000000 kombu-5.3.1/requirements/extras/librabbitmq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       99 2023-06-03 06:17:58.000000 kombu-5.3.1/requirements/extras/lzma.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-19 07:31:49.000000 kombu-5.3.1/requirements/extras/mongodb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        8 2021-09-07 04:22:35.000000 kombu-5.3.1/requirements/extras/msgpack.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        6 2023-05-24 14:21:55.000000 kombu-5.3.1/requirements/extras/pyro.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       35 2021-09-07 04:22:35.000000 kombu-5.3.1/requirements/extras/qpid.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2023-05-31 04:56:03.000000 kombu-5.3.1/requirements/extras/redis.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-09-07 04:22:35.000000 kombu-5.3.1/requirements/extras/slmq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       24 2023-05-18 06:10:21.000000 kombu-5.3.1/requirements/extras/sqlalchemy.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      121 2023-06-15 12:59:17.000000 kombu-5.3.1/requirements/extras/sqs.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-09-07 04:22:35.000000 kombu-5.3.1/requirements/extras/yaml.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2022-06-19 07:31:49.000000 kombu-5.3.1/requirements/extras/zookeeper.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-09-07 04:22:35.000000 kombu-5.3.1/requirements/extras/zstd.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      158 2021-09-07 04:22:35.000000 kombu-5.3.1/requirements/funtest.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      116 2023-05-18 06:10:21.000000 kombu-5.3.1/requirements/pkgutils.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      533 2023-06-15 12:59:17.000000 kombu-5.3.1/requirements/test-ci.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       59 2023-05-31 04:56:03.000000 kombu-5.3.1/requirements/test.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1172 2023-06-15 13:15:32.101790 kombu-5.3.1/setup.cfg
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3837 2023-05-18 06:10:21.000000 kombu-5.3.1/setup.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.069789 kombu-5.3.1/t/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/t/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.073789 kombu-5.3.1/t/integration/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      120 2022-04-17 07:07:11.000000 kombu-5.3.1/t/integration/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17367 2022-06-19 07:31:49.000000 kombu-5.3.1/t/integration/common.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1464 2022-06-19 07:31:49.000000 kombu-5.3.1/t/integration/test_kafka.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3675 2022-06-19 07:31:49.000000 kombu-5.3.1/t/integration/test_mongodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1970 2022-04-17 07:07:11.000000 kombu-5.3.1/t/integration/test_py_amqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4996 2023-05-31 04:56:03.000000 kombu-5.3.1/t/integration/test_redis.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6008 2022-10-19 13:47:58.000000 kombu-5.3.1/t/mocks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      283 2022-04-17 07:07:11.000000 kombu-5.3.1/t/skip.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.081790 kombu-5.3.1/t/unit/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/t/unit/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.081790 kombu-5.3.1/t/unit/asynchronous/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/t/unit/asynchronous/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.081790 kombu-5.3.1/t/unit/asynchronous/aws/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/t/unit/asynchronous/aws/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      199 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/asynchronous/aws/case.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.085790 kombu-5.3.1/t/unit/asynchronous/aws/sqs/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/t/unit/asynchronous/aws/sqs/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11941 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/asynchronous/aws/sqs/test_connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7140 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/asynchronous/aws/sqs/test_queue.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      318 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/asynchronous/aws/test_aws.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9277 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/asynchronous/aws/test_connection.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.085790 kombu-5.3.1/t/unit/asynchronous/http/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/t/unit/asynchronous/http/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5728 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/asynchronous/http/test_curl.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4221 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/asynchronous/http/test_http.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17161 2022-10-19 13:47:58.000000 kombu-5.3.1/t/unit/asynchronous/test_hub.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1141 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/asynchronous/test_semaphore.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4247 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/asynchronous/test_timer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9493 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/conftest.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2359 2022-06-19 07:31:49.000000 kombu-5.3.1/t/unit/test_clocks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17580 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_common.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11181 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_compat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2858 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_compression.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    32824 2023-03-09 08:07:52.000000 kombu-5.3.1/t/unit/test_connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13693 2022-06-19 07:31:49.000000 kombu-5.3.1/t/unit/test_entity.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      229 2022-06-19 07:31:49.000000 kombu-5.3.1/t/unit/test_exceptions.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4796 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_log.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1133 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_matcher.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1285 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_message.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24481 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_messaging.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7875 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_mixins.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12543 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_pidbox.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7238 2022-10-19 13:47:58.000000 kombu-5.3.1/t/unit/test_pools.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11162 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_serialization.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6704 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/test_simple.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.093790 kombu-5.3.1/t/unit/transport/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/t/unit/transport/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    35038 2023-05-18 06:10:21.000000 kombu-5.3.1/t/unit/transport/test_SQS.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13586 2023-05-18 06:10:21.000000 kombu-5.3.1/t/unit/transport/test_azureservicebus.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3455 2023-03-09 08:07:52.000000 kombu-5.3.1/t/unit/transport/test_azurestoragequeues.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5617 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/transport/test_base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2674 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/transport/test_consul.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2197 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/transport/test_etcd.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10594 2022-10-19 13:47:58.000000 kombu-5.3.1/t/unit/transport/test_filesystem.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4891 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/transport/test_librabbitmq.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5643 2022-10-19 13:47:58.000000 kombu-5.3.1/t/unit/transport/test_memory.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    19028 2023-05-18 06:10:21.000000 kombu-5.3.1/t/unit/transport/test_mongodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7008 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/transport/test_pyamqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2892 2022-10-19 13:47:58.000000 kombu-5.3.1/t/unit/transport/test_pyro.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    71045 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/transport/test_qpid.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    60297 2022-08-01 07:19:26.000000 kombu-5.3.1/t/unit/transport/test_redis.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1538 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/transport/test_sqlalchemy.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1014 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/transport/test_transport.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1057 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/transport/test_zookeeper.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.093790 kombu-5.3.1/t/unit/transport/virtual/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/t/unit/transport/virtual/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    21252 2022-10-19 13:47:58.000000 kombu-5.3.1/t/unit/transport/virtual/test_base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5530 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/transport/virtual/test_exchange.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-15 13:15:32.097790 kombu-5.3.1/t/unit/utils/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-09-07 04:22:35.000000 kombu-5.3.1/t/unit/utils/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1281 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_amq_manager.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2806 2023-03-20 10:18:52.000000 kombu-5.3.1/t/unit/utils/test_compat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1630 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_debug.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1132 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_div.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2962 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_encoding.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8800 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_functional.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      967 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_imports.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3235 2023-06-15 12:59:17.000000 kombu-5.3.1/t/unit/utils/test_json.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1064 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_objects.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2769 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_scheduling.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      459 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_time.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2964 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_url.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      609 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_utils.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      289 2022-04-17 07:07:11.000000 kombu-5.3.1/t/unit/utils/test_uuid.py
```

### Comparing `kombu-5.3.0rc2/AUTHORS` & `kombu-5.3.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/LICENSE` & `kombu-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/MANIFEST.in` & `kombu-5.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/PKG-INFO` & `kombu-5.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kombu
-Version: 5.3.0rc2
+Version: 5.3.1
 Summary: Messaging library for Python.
 Home-page: https://kombu.readthedocs.io
 Author: Ask Solem
 Author-email: auvipy@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/celery/kombu
 Keywords: messaging message amqp rabbitmq redis actor producer consumer
```

### Comparing `kombu-5.3.0rc2/README.rst` & `kombu-5.3.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ========================================
  kombu - Messaging library for Python
 ========================================
 
 |build-status| |coverage| |license| |wheel| |pyversion| |pyimp| |downloads|
 
-:Version: 5.3.0rc2
+:Version: 5.3.1
 :Documentation: https://kombu.readthedocs.io/
 :Download: https://pypi.org/project/kombu/
 :Source: https://github.com/celery/kombu/
 :Keywords: messaging, amqp, rabbitmq, redis, mongodb, python, queue
 
 About
 =====
```

### Comparing `kombu-5.3.0rc2/THANKS` & `kombu-5.3.1/THANKS`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/Makefile` & `kombu-5.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/_templates/sidebardonations.html` & `kombu-5.3.1/docs/_templates/sidebardonations.html`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/conf.py` & `kombu-5.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/images/favicon.ico` & `kombu-5.3.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/images/kombu.jpg` & `kombu-5.3.1/docs/images/kombu.jpg`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/images/kombusmall.jpg` & `kombu-5.3.1/docs/images/kombusmall.jpg`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/includes/introduction.txt` & `kombu-5.3.1/docs/includes/introduction.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:Version: 5.3.0rc2
+:Version: 5.3.1
 :Web: https://kombu.readthedocs.io/
 :Download: https://pypi.org/project/kombu/
 :Source: https://github.com/celery/kombu/
 :Keywords: messaging, amqp, rabbitmq, redis, mongodb, python, queue
 
 About
 =====
```

### Comparing `kombu-5.3.0rc2/docs/includes/resources.txt` & `kombu-5.3.1/docs/includes/resources.txt`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/make.bat` & `kombu-5.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/index.rst` & `kombu-5.3.1/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.compat.rst` & `kombu-5.3.1/docs/reference/kombu.compat.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.compression.rst` & `kombu-5.3.1/docs/reference/kombu.compression.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.connection.rst` & `kombu-5.3.1/docs/reference/kombu.connection.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.pidbox.rst` & `kombu-5.3.1/docs/reference/kombu.pidbox.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.rst` & `kombu-5.3.1/docs/reference/kombu.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.serialization.rst` & `kombu-5.3.1/docs/reference/kombu.serialization.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.simple.rst` & `kombu-5.3.1/docs/reference/kombu.simple.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.SQS.rst` & `kombu-5.3.1/docs/reference/kombu.transport.SQS.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.azureservicebus.rst` & `kombu-5.3.1/docs/reference/kombu.transport.azureservicebus.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.azurestoragequeues.rst` & `kombu-5.3.1/docs/reference/kombu.transport.azurestoragequeues.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.base.rst` & `kombu-5.3.1/docs/reference/kombu.transport.base.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.confluentkafka.rst` & `kombu-5.3.1/docs/reference/kombu.transport.confluentkafka.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.librabbitmq.rst` & `kombu-5.3.1/docs/reference/kombu.transport.librabbitmq.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.pyamqp.rst` & `kombu-5.3.1/docs/reference/kombu.transport.pyamqp.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.pyro.rst` & `kombu-5.3.1/docs/reference/kombu.transport.pyro.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.qpid.rst` & `kombu-5.3.1/docs/reference/kombu.transport.qpid.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.redis.rst` & `kombu-5.3.1/docs/reference/kombu.transport.redis.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.rst` & `kombu-5.3.1/docs/reference/kombu.transport.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.sqlalchemy.rst` & `kombu-5.3.1/docs/reference/kombu.transport.sqlalchemy.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.virtual.exchange.rst` & `kombu-5.3.1/docs/reference/kombu.transport.virtual.exchange.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/reference/kombu.transport.virtual.rst` & `kombu-5.3.1/docs/reference/kombu.transport.virtual.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/templates/readme.txt` & `kombu-5.3.1/docs/templates/readme.txt`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/userguide/connections.rst` & `kombu-5.3.1/docs/userguide/connections.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/userguide/consumers.rst` & `kombu-5.3.1/docs/userguide/consumers.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/userguide/examples.rst` & `kombu-5.3.1/docs/userguide/examples.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/userguide/failover.rst` & `kombu-5.3.1/docs/userguide/failover.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/userguide/introduction.rst` & `kombu-5.3.1/docs/userguide/introduction.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/userguide/pools.rst` & `kombu-5.3.1/docs/userguide/pools.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/userguide/producers.rst` & `kombu-5.3.1/docs/userguide/producers.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/userguide/serialization.rst` & `kombu-5.3.1/docs/userguide/serialization.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/docs/userguide/simple.rst` & `kombu-5.3.1/docs/userguide/simple.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/complete_receive.py` & `kombu-5.3.1/examples/complete_receive.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/complete_send.py` & `kombu-5.3.1/examples/complete_send.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/experimental/async_consume.py` & `kombu-5.3.1/examples/experimental/async_consume.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/memory_transport.py` & `kombu-5.3.1/examples/memory_transport.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/rpc-tut6/rpc_client.py` & `kombu-5.3.1/examples/rpc-tut6/rpc_client.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/rpc-tut6/rpc_server.py` & `kombu-5.3.1/examples/rpc-tut6/rpc_server.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/simple_eventlet_receive.py` & `kombu-5.3.1/examples/simple_eventlet_receive.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/simple_eventlet_send.py` & `kombu-5.3.1/examples/simple_eventlet_send.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/simple_receive.py` & `kombu-5.3.1/examples/simple_receive.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/simple_send.py` & `kombu-5.3.1/examples/simple_send.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/simple_task_queue/client.py` & `kombu-5.3.1/examples/simple_task_queue/client.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/examples/simple_task_queue/worker.py` & `kombu-5.3.1/examples/simple_task_queue/worker.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/__init__.py` & `kombu-5.3.1/kombu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 import re
 import sys
 from collections import namedtuple
 from typing import Any, cast
 
-__version__ = '5.3.0rc2'
+__version__ = '5.3.1'
 __author__ = 'Ask Solem'
 __contact__ = 'auvipy@gmail.com'
 __homepage__ = 'https://kombu.readthedocs.io'
 __docformat__ = 'restructuredtext en'
 
 # -eof meta-
```

### Comparing `kombu-5.3.0rc2/kombu/abstract.py` & `kombu-5.3.1/kombu/abstract.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/aws/connection.py` & `kombu-5.3.1/kombu/asynchronous/aws/connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/aws/ext.py` & `kombu-5.3.1/kombu/asynchronous/aws/ext.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/aws/sqs/connection.py` & `kombu-5.3.1/kombu/asynchronous/aws/sqs/connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/aws/sqs/message.py` & `kombu-5.3.1/kombu/asynchronous/aws/sqs/message.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/aws/sqs/queue.py` & `kombu-5.3.1/kombu/asynchronous/aws/sqs/queue.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/debug.py` & `kombu-5.3.1/kombu/asynchronous/debug.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/http/__init__.py` & `kombu-5.3.1/kombu/asynchronous/http/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/http/base.py` & `kombu-5.3.1/kombu/asynchronous/http/base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/http/curl.py` & `kombu-5.3.1/kombu/asynchronous/http/curl.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/hub.py` & `kombu-5.3.1/kombu/asynchronous/hub.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/semaphore.py` & `kombu-5.3.1/kombu/asynchronous/semaphore.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/asynchronous/timer.py` & `kombu-5.3.1/kombu/asynchronous/timer.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/clocks.py` & `kombu-5.3.1/kombu/clocks.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/common.py` & `kombu-5.3.1/kombu/common.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/compat.py` & `kombu-5.3.1/kombu/compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/compression.py` & `kombu-5.3.1/kombu/compression.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/connection.py` & `kombu-5.3.1/kombu/connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/entity.py` & `kombu-5.3.1/kombu/entity.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/exceptions.py` & `kombu-5.3.1/kombu/exceptions.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/log.py` & `kombu-5.3.1/kombu/log.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/matcher.py` & `kombu-5.3.1/kombu/matcher.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/message.py` & `kombu-5.3.1/kombu/message.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/messaging.py` & `kombu-5.3.1/kombu/messaging.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/mixins.py` & `kombu-5.3.1/kombu/mixins.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/pidbox.py` & `kombu-5.3.1/kombu/pidbox.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/pools.py` & `kombu-5.3.1/kombu/pools.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/resource.py` & `kombu-5.3.1/kombu/resource.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/serialization.py` & `kombu-5.3.1/kombu/serialization.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/simple.py` & `kombu-5.3.1/kombu/simple.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/SLMQ.py` & `kombu-5.3.1/kombu/transport/SLMQ.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/SQS.py` & `kombu-5.3.1/kombu/transport/SQS.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/__init__.py` & `kombu-5.3.1/kombu/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/azureservicebus.py` & `kombu-5.3.1/kombu/transport/azureservicebus.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/azurestoragequeues.py` & `kombu-5.3.1/kombu/transport/azurestoragequeues.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/base.py` & `kombu-5.3.1/kombu/transport/base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/confluentkafka.py` & `kombu-5.3.1/kombu/transport/confluentkafka.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/consul.py` & `kombu-5.3.1/kombu/transport/consul.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/etcd.py` & `kombu-5.3.1/kombu/transport/etcd.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/filesystem.py` & `kombu-5.3.1/kombu/transport/filesystem.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/librabbitmq.py` & `kombu-5.3.1/kombu/transport/librabbitmq.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/memory.py` & `kombu-5.3.1/kombu/transport/memory.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/mongodb.py` & `kombu-5.3.1/kombu/transport/mongodb.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/pyamqp.py` & `kombu-5.3.1/kombu/transport/pyamqp.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/pyro.py` & `kombu-5.3.1/kombu/transport/pyro.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/qpid.py` & `kombu-5.3.1/kombu/transport/qpid.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/redis.py` & `kombu-5.3.1/kombu/transport/redis.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/sqlalchemy/__init__.py` & `kombu-5.3.1/kombu/transport/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/sqlalchemy/models.py` & `kombu-5.3.1/kombu/transport/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/virtual/base.py` & `kombu-5.3.1/kombu/transport/virtual/base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/virtual/exchange.py` & `kombu-5.3.1/kombu/transport/virtual/exchange.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/transport/zookeeper.py` & `kombu-5.3.1/kombu/transport/zookeeper.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/__init__.py` & `kombu-5.3.1/kombu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/amq_manager.py` & `kombu-5.3.1/kombu/utils/amq_manager.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/collections.py` & `kombu-5.3.1/kombu/utils/collections.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/compat.py` & `kombu-5.3.1/kombu/utils/compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/debug.py` & `kombu-5.3.1/kombu/utils/debug.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/div.py` & `kombu-5.3.1/kombu/utils/div.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/encoding.py` & `kombu-5.3.1/kombu/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/eventio.py` & `kombu-5.3.1/kombu/utils/eventio.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/functional.py` & `kombu-5.3.1/kombu/utils/functional.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/imports.py` & `kombu-5.3.1/kombu/utils/imports.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/json.py` & `kombu-5.3.1/kombu/utils/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,10 +119,10 @@
     lambda o: datetime.fromisoformat(o).date(),
 )
 register_type(time, "time", lambda o: o.isoformat(), time.fromisoformat)
 register_type(Decimal, "decimal", str, Decimal)
 register_type(
     uuid.UUID,
     "uuid",
-    lambda o: {"hex": o.hex, "version": o.version},
+    lambda o: {"hex": o.hex},
     lambda o: uuid.UUID(**o),
 )
```

### Comparing `kombu-5.3.0rc2/kombu/utils/limits.py` & `kombu-5.3.1/kombu/utils/limits.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/objects.py` & `kombu-5.3.1/kombu/utils/objects.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/scheduling.py` & `kombu-5.3.1/kombu/utils/scheduling.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/text.py` & `kombu-5.3.1/kombu/utils/text.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu/utils/url.py` & `kombu-5.3.1/kombu/utils/url.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu.egg-info/PKG-INFO` & `kombu-5.3.1/kombu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kombu
-Version: 5.3.0rc2
+Version: 5.3.1
 Summary: Messaging library for Python.
 Home-page: https://kombu.readthedocs.io
 Author: Ask Solem
 Author-email: auvipy@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/celery/kombu
 Keywords: messaging message amqp rabbitmq redis actor producer consumer
```

### Comparing `kombu-5.3.0rc2/kombu.egg-info/SOURCES.txt` & `kombu-5.3.1/kombu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/kombu.egg-info/requires.txt` & `kombu-5.3.1/kombu.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 amqp<6.0.0,>=5.1.1
 vine
 
 [:python_version < "3.10"]
 typing_extensions
 
 [:python_version < "3.9"]
-backports.zoneinfo>=0.2.1
+backports.zoneinfo[tzdata]>=0.2.1
 
 [azureservicebus]
 azure-servicebus>=7.10.0
 
 [azurestoragequeues]
 azure-identity>=1.12.0
 azure-storage-queue>=12.6.0
@@ -17,14 +17,16 @@
 [confluentkafka]
 confluent-kafka==2.1.1
 
 [consul]
 python-consul2
 
 [librabbitmq]
+
+[librabbitmq:python_version < "3.11"]
 librabbitmq>=2.0.0
 
 [mongodb]
 pymongo>=4.1.1
 
 [msgpack]
 msgpack
@@ -43,15 +45,17 @@
 softlayer_messaging>=1.0.3
 
 [sqlalchemy]
 sqlalchemy<2.1,>=1.4.48
 
 [sqs]
 boto3>=1.26.143
-pycurl==7.43.0.5
 urllib3>=1.26.16
 
+[sqs:sys_platform != "win32" and platform_python_implementation == "CPython"]
+pycurl>=7.43.0.5
+
 [yaml]
 PyYAML>=3.10
 
 [zookeeper]
 kazoo>=2.8.0
```

### Comparing `kombu-5.3.0rc2/setup.cfg` & `kombu-5.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/setup.py` & `kombu-5.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/integration/common.py` & `kombu-5.3.1/t/integration/common.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/integration/test_kafka.py` & `kombu-5.3.1/t/integration/test_kafka.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/integration/test_mongodb.py` & `kombu-5.3.1/t/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/integration/test_py_amqp.py` & `kombu-5.3.1/t/integration/test_py_amqp.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/integration/test_redis.py` & `kombu-5.3.1/t/integration/test_redis.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/mocks.py` & `kombu-5.3.1/t/mocks.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/asynchronous/aws/sqs/test_connection.py` & `kombu-5.3.1/t/unit/asynchronous/aws/sqs/test_connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/asynchronous/aws/sqs/test_queue.py` & `kombu-5.3.1/t/unit/asynchronous/aws/sqs/test_queue.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/asynchronous/aws/test_connection.py` & `kombu-5.3.1/t/unit/asynchronous/aws/test_connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/asynchronous/http/test_curl.py` & `kombu-5.3.1/t/unit/asynchronous/http/test_curl.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/asynchronous/http/test_http.py` & `kombu-5.3.1/t/unit/asynchronous/http/test_http.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/asynchronous/test_hub.py` & `kombu-5.3.1/t/unit/asynchronous/test_hub.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/asynchronous/test_semaphore.py` & `kombu-5.3.1/t/unit/asynchronous/test_semaphore.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/asynchronous/test_timer.py` & `kombu-5.3.1/t/unit/asynchronous/test_timer.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/conftest.py` & `kombu-5.3.1/t/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_clocks.py` & `kombu-5.3.1/t/unit/test_clocks.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_common.py` & `kombu-5.3.1/t/unit/test_common.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_compat.py` & `kombu-5.3.1/t/unit/test_compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_compression.py` & `kombu-5.3.1/t/unit/test_compression.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_connection.py` & `kombu-5.3.1/t/unit/test_connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_entity.py` & `kombu-5.3.1/t/unit/test_entity.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_log.py` & `kombu-5.3.1/t/unit/test_log.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_matcher.py` & `kombu-5.3.1/t/unit/test_matcher.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_message.py` & `kombu-5.3.1/t/unit/test_message.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_messaging.py` & `kombu-5.3.1/t/unit/test_messaging.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_mixins.py` & `kombu-5.3.1/t/unit/test_mixins.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_pidbox.py` & `kombu-5.3.1/t/unit/test_pidbox.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_pools.py` & `kombu-5.3.1/t/unit/test_pools.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_serialization.py` & `kombu-5.3.1/t/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/test_simple.py` & `kombu-5.3.1/t/unit/test_simple.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_SQS.py` & `kombu-5.3.1/t/unit/transport/test_SQS.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_azureservicebus.py` & `kombu-5.3.1/t/unit/transport/test_azureservicebus.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_azurestoragequeues.py` & `kombu-5.3.1/t/unit/transport/test_azurestoragequeues.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_base.py` & `kombu-5.3.1/t/unit/transport/test_base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_consul.py` & `kombu-5.3.1/t/unit/transport/test_consul.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_etcd.py` & `kombu-5.3.1/t/unit/transport/test_etcd.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_filesystem.py` & `kombu-5.3.1/t/unit/transport/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_librabbitmq.py` & `kombu-5.3.1/t/unit/transport/test_librabbitmq.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_memory.py` & `kombu-5.3.1/t/unit/transport/test_memory.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_mongodb.py` & `kombu-5.3.1/t/unit/transport/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_pyamqp.py` & `kombu-5.3.1/t/unit/transport/test_pyamqp.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_pyro.py` & `kombu-5.3.1/t/unit/transport/test_pyro.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_qpid.py` & `kombu-5.3.1/t/unit/transport/test_qpid.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_redis.py` & `kombu-5.3.1/t/unit/transport/test_redis.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_sqlalchemy.py` & `kombu-5.3.1/t/unit/transport/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_transport.py` & `kombu-5.3.1/t/unit/transport/test_transport.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/test_zookeeper.py` & `kombu-5.3.1/t/unit/transport/test_zookeeper.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/virtual/test_base.py` & `kombu-5.3.1/t/unit/transport/virtual/test_base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/transport/virtual/test_exchange.py` & `kombu-5.3.1/t/unit/transport/virtual/test_exchange.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_amq_manager.py` & `kombu-5.3.1/t/unit/utils/test_amq_manager.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_compat.py` & `kombu-5.3.1/t/unit/utils/test_compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_debug.py` & `kombu-5.3.1/t/unit/utils/test_debug.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_div.py` & `kombu-5.3.1/t/unit/utils/test_div.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_encoding.py` & `kombu-5.3.1/t/unit/utils/test_encoding.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_functional.py` & `kombu-5.3.1/t/unit/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_imports.py` & `kombu-5.3.1/t/unit/utils/test_imports.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_json.py` & `kombu-5.3.1/t/unit/utils/test_json.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 if sys.version_info >= (3, 9):
     from zoneinfo import ZoneInfo
 else:
     from backports.zoneinfo import ZoneInfo
 
 
 class Custom:
-
     def __init__(self, data):
         self.data = data
 
     def __json__(self):
         return self.data
 
 
@@ -67,14 +66,19 @@
 
     def test_UUID(self):
         constructors = [
             uuid.uuid1,
             lambda: uuid.uuid3(uuid.NAMESPACE_URL, "https://example.org"),
             uuid.uuid4,
             lambda: uuid.uuid5(uuid.NAMESPACE_URL, "https://example.org"),
+            # The uuids below correspond to v6, v7 and v8 respectively and were
+            # generated using the package uuid6.
+            lambda: uuid.UUID("1ee0b1e6-dd55-63d2-867f-88cb9205458f"),
+            lambda: uuid.UUID("0188bcbb-8475-7605-a094-fe41c58df798"),
+            lambda: uuid.UUID("0188bcbb-8cb2-8bf7-b3b5-fd1faa0431bd"),
         ]
         for constructor in constructors:
             id = constructor()
             loaded_value = loads(dumps({'u': id}))
             assert loaded_value == {'u': id}
             assert loaded_value["u"].version == id.version
```

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_objects.py` & `kombu-5.3.1/t/unit/utils/test_objects.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_scheduling.py` & `kombu-5.3.1/t/unit/utils/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_url.py` & `kombu-5.3.1/t/unit/utils/test_url.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.0rc2/t/unit/utils/test_utils.py` & `kombu-5.3.1/t/unit/utils/test_utils.py`

 * *Files identical despite different names*

