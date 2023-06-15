# Comparing `tmp/gigalixir-1.5.1.tar.gz` & `tmp/gigalixir-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigalixir-1.5.1.tar", last modified: Mon Jun 12 14:23:45 2023, max compression
+gzip compressed data, was "gigalixir-1.6.0.tar", last modified: Thu Jun 15 17:44:15 2023, max compression
```

## Comparing `gigalixir-1.5.1.tar` & `gigalixir-1.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/
--rw-rw-r--   0 tim       (1001) tim       (1001)     1081 2022-12-06 04:22:54.000000 gigalixir-1.5.1/LICENSE
--rw-rw-r--   0 tim       (1001) tim       (1001)      269 2023-06-12 14:23:45.311078 gigalixir-1.5.1/PKG-INFO
--rw-rw-r--   0 tim       (1001) tim       (1001)     1470 2022-12-06 04:22:54.000000 gigalixir-1.5.1/README.md
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/gigalixir/
--rw-rw-r--   0 tim       (1001) tim       (1001)    40314 2023-06-12 14:17:21.000000 gigalixir-1.5.1/gigalixir/__init__.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      229 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/api_exception.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      858 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/api_key.py
--rw-rw-r--   0 tim       (1001) tim       (1001)    10135 2022-09-09 11:05:48.000000 gigalixir-1.5.1/gigalixir/app.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      538 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/app_activity.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      391 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/auth.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1560 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/canary.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1966 2023-06-12 13:26:20.000000 gigalixir-1.5.1/gigalixir/config.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     4082 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/database.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1633 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/domain.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1336 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/free_database.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      601 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/git.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      446 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/invoice.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1262 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/log_drain.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     2653 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/mfa.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     3084 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/netrc.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     7045 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/observer.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/gigalixir/openers/
--rw-rw-r--   0 tim       (1001) tim       (1001)        0 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/openers/__init__.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      207 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/openers/darwin.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      214 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/openers/linux.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      210 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/openers/windows.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1172 2022-01-18 14:21:12.000000 gigalixir-1.5.1/gigalixir/payment_method.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1274 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/permission.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      347 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/presenter.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      538 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/release.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/gigalixir/routers/
--rw-rw-r--   0 tim       (1001) tim       (1001)        0 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/routers/__init__.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1551 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/routers/darwin.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      902 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/routers/linux.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      618 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/routers/windows.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1490 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/shell.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1234 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/ssh_key.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      801 2022-08-20 15:11:07.000000 gigalixir-1.5.1/gigalixir/usage.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     7549 2023-03-16 02:46:36.000000 gigalixir-1.5.1/gigalixir/user.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/gigalixir.egg-info/
--rw-rw-r--   0 tim       (1001) tim       (1001)      269 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1001) tim       (1001)     1019 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)        1 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)       63 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)      187 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/requires.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)       10 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/top_level.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)       63 2023-06-12 14:23:45.311078 gigalixir-1.5.1/setup.cfg
--rw-rw-r--   0 tim       (1001) tim       (1001)      959 2023-06-12 14:17:49.000000 gigalixir-1.5.1/setup.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/test/
--rw-rw-r--   0 tim       (1001) tim       (1001)    36261 2022-01-27 06:29:24.000000 gigalixir-1.5.1/test/test_gigalixir.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-15 17:44:15.832167 gigalixir-1.6.0/
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1081 2022-12-06 04:22:54.000000 gigalixir-1.6.0/LICENSE
+-rw-rw-r--   0 tim       (1001) tim       (1001)      269 2023-06-15 17:44:15.832167 gigalixir-1.6.0/PKG-INFO
+-rw-rw-r--   0 tim       (1001) tim       (1001)      420 2023-06-15 17:42:00.000000 gigalixir-1.6.0/README.md
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-15 17:44:15.828167 gigalixir-1.6.0/gigalixir/
+-rw-rw-r--   0 tim       (1001) tim       (1001)    38398 2023-06-15 17:30:39.000000 gigalixir-1.6.0/gigalixir/__init__.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      229 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/api_exception.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      858 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/api_key.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)    10135 2022-09-09 11:05:48.000000 gigalixir-1.6.0/gigalixir/app.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      538 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/app_activity.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      391 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/auth.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1560 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/canary.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1966 2023-06-12 13:26:20.000000 gigalixir-1.6.0/gigalixir/config.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     4082 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/database.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1633 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/domain.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      555 2023-06-13 05:24:59.000000 gigalixir-1.6.0/gigalixir/free_database.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      601 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/git.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      446 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/invoice.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1262 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/log_drain.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     2653 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/mfa.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     3084 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/netrc.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     7045 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/observer.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-15 17:44:15.828167 gigalixir-1.6.0/gigalixir/openers/
+-rw-rw-r--   0 tim       (1001) tim       (1001)        0 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/openers/__init__.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      207 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/openers/darwin.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      214 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/openers/linux.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      210 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/openers/windows.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1172 2022-01-18 14:21:12.000000 gigalixir-1.6.0/gigalixir/payment_method.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1274 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/permission.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      347 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/presenter.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      538 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/release.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-15 17:44:15.832167 gigalixir-1.6.0/gigalixir/routers/
+-rw-rw-r--   0 tim       (1001) tim       (1001)        0 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/routers/__init__.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1551 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/routers/darwin.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      902 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/routers/linux.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      618 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/routers/windows.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1490 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/shell.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1234 2022-01-04 16:13:56.000000 gigalixir-1.6.0/gigalixir/ssh_key.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      801 2022-08-20 15:11:07.000000 gigalixir-1.6.0/gigalixir/usage.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     7549 2023-03-16 02:46:36.000000 gigalixir-1.6.0/gigalixir/user.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-15 17:44:15.828167 gigalixir-1.6.0/gigalixir.egg-info/
+-rw-rw-r--   0 tim       (1001) tim       (1001)      269 2023-06-15 17:44:15.000000 gigalixir-1.6.0/gigalixir.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1019 2023-06-15 17:44:15.000000 gigalixir-1.6.0/gigalixir.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)        1 2023-06-15 17:44:15.000000 gigalixir-1.6.0/gigalixir.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)       63 2023-06-15 17:44:15.000000 gigalixir-1.6.0/gigalixir.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)      187 2023-06-15 17:44:15.000000 gigalixir-1.6.0/gigalixir.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)       10 2023-06-15 17:44:15.000000 gigalixir-1.6.0/gigalixir.egg-info/top_level.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)       63 2023-06-15 17:44:15.832167 gigalixir-1.6.0/setup.cfg
+-rw-rw-r--   0 tim       (1001) tim       (1001)      959 2023-06-15 17:31:56.000000 gigalixir-1.6.0/setup.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-15 17:44:15.832167 gigalixir-1.6.0/test/
+-rw-rw-r--   0 tim       (1001) tim       (1001)    36261 2022-01-27 06:29:24.000000 gigalixir-1.6.0/test/test_gigalixir.py
```

### Comparing `gigalixir-1.5.1/LICENSE` & `gigalixir-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/__init__.py` & `gigalixir-1.6.0/gigalixir/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,14 @@
 class AliasedGroup(click.Group):
     def get_command(self, ctx, cmd_name):
         rv = click.Group.get_command(self, ctx, cmd_name)
         if rv is not None:
             return rv
         aliases = {
             "configs": "config",
-            "set_config": "deprecated:set_config",
             "databases": "pg",
             "scale_database": "pg:scale",
             "delete_database": "pg:destroy",
             "status": "ps",
             "scale": "ps:scale",
             "rollback": "releases:rollback",
             "remote_console": "ps:remote_console",
@@ -165,17 +164,14 @@
             "delete_ssh_key": "account:ssh_keys:remove",
             "add_domain": "domains:add",
             "send_email_confirmation_token": "account:confirmation:resend",
             "send_reset_password_token": "account:password:reset",
             "delete_app": "apps:destroy",
             "delete_permission": "access:remove",
             "permissions": "access",
-            "delete_free_database": "deprecated:delete_free_database",
-            "free_databases": "deprecated:free_databases",
-            "create_free_database": "deprecated:create_free_database",
             "delete_domain": "domains:remove",
             "delete_config": "config:unset",
             "add_permission": "access:add",
             "create_database": "pg:create",
             "set_git_remote": "git:remote",
             "invoices": "account:invoices",
             "current_period_usage": "account:usage",
@@ -293,15 +289,15 @@
     Current app status.
     """
     gigalixir_app.status(ctx.obj['host'], app_name)
 
 @cli.command(name='pg:scale')
 @click.option('-a', '--app_name', envvar="GIGALIXIR_APP")
 @click.option('-d', '--database_id', required=True)
-@click.option('-s', '--size', type=float, default=0.6, help='Size of the database can be 0.6, 1.7, 4, 8, 16, 32, 48, 64, or 128.')
+@click.option('-s', '--size', type=float, default=0.6, help='Size of the database can be 0.6, 1.7, 4, 8, 16, 32, 48, 64, or 96.')
 @click.pass_context
 @report_errors
 @detect_app_name
 def scale_database(ctx, app_name, database_id, size):
     """
     Scale database. Find the database id by running `gigalixir pg`
     """
@@ -805,27 +801,14 @@
 def databases(ctx, app_name):
     """
     Get databases for your app.
     """
     gigalixir_database.get(ctx.obj['host'], app_name)
 
 # @get.command()
-# deprecated. pg/databases above lists free and standard.
-@cli.command(name='deprecated:free_databases')
-@click.option('-a', '--app_name', envvar="GIGALIXIR_APP")
-@click.pass_context
-@report_errors
-@detect_app_name
-def free_databases(ctx, app_name):
-    """
-    Get free databases for your app.
-    """
-    gigalixir_free_database.get(ctx.obj['host'], app_name)
-
-# @get.command()
 @cli.command()
 @click.option('-a', '--app_name', envvar="GIGALIXIR_APP")
 @click.pass_context
 @report_errors
 @detect_app_name
 def domains(ctx, app_name):
     """
@@ -911,33 +894,14 @@
     logging.getLogger("gigalixir-cli").info("WARNING: Deleting your database will destroy all your data and backups.")
     logging.getLogger("gigalixir-cli").info("WARNING: This can not be undone.")
     logging.getLogger("gigalixir-cli").info("WARNING: Please make sure you backup your data first.")
     if yes or click.confirm('Do you want to delete your database and all backups?'):
         gigalixir_database.delete(ctx.obj['host'], app_name, database_id)
 
 # @delete.command()
-# is this command still needed? i think delete_database/pg:destroy above can delete free databases?
-@cli.command(name='deprecated:delete_free_database')
-@click.option('-a', '--app_name', envvar="GIGALIXIR_APP")
-@click.option('-y', '--yes', is_flag=True)
-@click.option('-d', '--database_id', required=True)
-@click.pass_context
-@report_errors
-@detect_app_name
-def delete_free_database(ctx, app_name, yes, database_id):
-    """
-    Delete free database. Find the database id by running `gigalixir pg`
-    """
-    logging.getLogger("gigalixir-cli").info("WARNING: Deleting your database will destroy all your data.")
-    logging.getLogger("gigalixir-cli").info("WARNING: This can not be undone.")
-    logging.getLogger("gigalixir-cli").info("WARNING: Please make sure you backup your data first.")
-    if yes or click.confirm('Do you want to delete your database?'):
-        gigalixir_free_database.delete(ctx.obj['host'], app_name, database_id)
-
-# @delete.command()
 @cli.command(name='domains:remove')
 @click.option('-a', '--app_name', envvar="GIGALIXIR_APP")
 @click.argument('fully_qualified_domain_name')
 @click.pass_context
 @report_errors
 @detect_app_name
 def delete_domain(ctx, app_name, fully_qualified_domain_name):
@@ -982,15 +946,15 @@
     """
     Connect to the database using psql
     """
     gigalixir_database.psql(ctx.obj['host'], app_name)
 
 @cli.command(name='pg:create')
 @click.option('-a', '--app_name', envvar="GIGALIXIR_APP")
-@click.option('-s', '--size', type=float, default=0.6, help='Size of the database can be 0.6, 1.7, 4, 8, 16, 32, 64, or 128.')
+@click.option('-s', '--size', type=float, default=0.6, help='Size of the database can be 0.6, 1.7, 4, 8, 16, 32, 48, 64, or 96.')
 @click.option('-c', '--cloud')
 @click.option('-r', '--region')
 @click.option('-f', '--free', is_flag=True)
 @click.option('-y', '--yes', is_flag=True)
 @click.pass_context
 @report_errors
 @detect_app_name
@@ -1003,25 +967,14 @@
             raise Exception("Sorry, free tier databases only run on gcp in us-central1. Try creating a standard database instead.")
         else:
             if yes or click.confirm("A word of caution: Free tier databases are not suitable for production and migrating from a free db to a standard db is not trivial. Do you wish to continue?"):
                 gigalixir_free_database.create(ctx.obj['host'], app_name)
     else:
         gigalixir_database.create(ctx.obj['host'], app_name, size, cloud, region)
 
-@cli.command(name='deprecated:create_free_database')
-@click.option('-a', '--app_name', envvar="GIGALIXIR_APP")
-@click.pass_context
-@report_errors
-@detect_app_name
-def create_free_database(ctx, app_name):
-    """
-    Create a new free database for app.
-    """
-    gigalixir_free_database.create(ctx.obj['host'], app_name)
-
 # @create.command()
 @cli.command(name='git:remote')
 @click.argument('app_name')
 @click.pass_context
 @report_errors
 def set_git_remote(ctx, app_name):
     """
```

### Comparing `gigalixir-1.5.1/gigalixir/api_key.py` & `gigalixir-1.6.0/gigalixir/api_key.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/app.py` & `gigalixir-1.6.0/gigalixir/app.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/app_activity.py` & `gigalixir-1.6.0/gigalixir/app_activity.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/canary.py` & `gigalixir-1.6.0/gigalixir/canary.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/config.py` & `gigalixir-1.6.0/gigalixir/config.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/database.py` & `gigalixir-1.6.0/gigalixir/database.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/domain.py` & `gigalixir-1.6.0/gigalixir/domain.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/free_database.py` & `gigalixir-1.6.0/gigalixir/permission.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import requests
-import logging
 from . import auth
 from . import presenter
 import urllib
 import json
 import click
 from six.moves.urllib.parse import quote
 
 def get(host, app_name):
-    r = requests.get('%s/api/apps/%s/free_databases' % (host, quote(app_name.encode('utf-8'))), headers = {
+    r = requests.get('%s/api/apps/%s/permissions' % (host, quote(app_name.encode('utf-8'))), headers = {
         'Content-Type': 'application/json',
     })
     if r.status_code != 200:
         if r.status_code == 401:
             raise auth.AuthException()
         raise Exception(r.text)
     else:
         data = json.loads(r.text)["data"]
         presenter.echo_json(data)
 
-def create(host, app_name):
-    r = requests.post('%s/api/apps/%s/free_databases' % (host, quote(app_name.encode('utf-8'))), headers = {
+def create(host, app_name, email):
+    r = requests.post('%s/api/apps/%s/permissions' % (host, quote(app_name.encode('utf-8'))), headers = {
         'Content-Type': 'application/json',
-    }, json = {})
+    }, json = {
+        "email": email,
+    })
     if r.status_code != 201:
         if r.status_code == 401:
             raise auth.AuthException()
         raise Exception(r.text)
-    data = json.loads(r.text)["data"]
-    presenter.echo_json(data)
 
-def delete(host, app_name, database_id):
-    r = requests.delete('%s/api/apps/%s/free_databases/%s' % (host, quote(app_name.encode('utf-8')), quote(database_id.encode('utf-8'))), headers = {
+def delete(host, app_name, email):
+    r = requests.delete('%s/api/apps/%s/permissions' % (host, quote(app_name.encode('utf-8'))), headers = {
         'Content-Type': 'application/json',
+    }, json = {
+        "email": email,
     })
     if r.status_code != 200:
         if r.status_code == 401:
             raise auth.AuthException()
         raise Exception(r.text)
-
```

### Comparing `gigalixir-1.5.1/gigalixir/git.py` & `gigalixir-1.6.0/gigalixir/git.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/log_drain.py` & `gigalixir-1.6.0/gigalixir/log_drain.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/mfa.py` & `gigalixir-1.6.0/gigalixir/mfa.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/netrc.py` & `gigalixir-1.6.0/gigalixir/netrc.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/observer.py` & `gigalixir-1.6.0/gigalixir/observer.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/payment_method.py` & `gigalixir-1.6.0/gigalixir/payment_method.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/permission.py` & `gigalixir-1.6.0/gigalixir/usage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,31 @@
 import requests
 from . import auth
 from . import presenter
 import urllib
 import json
 import click
-from six.moves.urllib.parse import quote
 
-def get(host, app_name):
-    r = requests.get('%s/api/apps/%s/permissions' % (host, quote(app_name.encode('utf-8'))), headers = {
+def get(host):
+    r = requests.get('%s/api/usage' % (host), headers = {
         'Content-Type': 'application/json',
     })
     if r.status_code != 200:
         if r.status_code == 401:
             raise auth.AuthException()
         raise Exception(r.text)
     else:
         data = json.loads(r.text)["data"]
         presenter.echo_json(data)
 
-def create(host, app_name, email):
-    r = requests.post('%s/api/apps/%s/permissions' % (host, quote(app_name.encode('utf-8'))), headers = {
+def run_rate(host):
+    r = requests.get('%s/api/usage/run_rate' % (host), headers = {
         'Content-Type': 'application/json',
-    }, json = {
-        "email": email,
-    })
-    if r.status_code != 201:
-        if r.status_code == 401:
-            raise auth.AuthException()
-        raise Exception(r.text)
-
-def delete(host, app_name, email):
-    r = requests.delete('%s/api/apps/%s/permissions' % (host, quote(app_name.encode('utf-8'))), headers = {
-        'Content-Type': 'application/json',
-    }, json = {
-        "email": email,
     })
     if r.status_code != 200:
         if r.status_code == 401:
             raise auth.AuthException()
         raise Exception(r.text)
+    else:
+        data = json.loads(r.text)["data"]
+        presenter.echo_json(data)
+
```

### Comparing `gigalixir-1.5.1/gigalixir/release.py` & `gigalixir-1.6.0/gigalixir/release.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/routers/darwin.py` & `gigalixir-1.6.0/gigalixir/routers/darwin.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/routers/linux.py` & `gigalixir-1.6.0/gigalixir/routers/linux.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/routers/windows.py` & `gigalixir-1.6.0/gigalixir/routers/windows.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/shell.py` & `gigalixir-1.6.0/gigalixir/shell.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/ssh_key.py` & `gigalixir-1.6.0/gigalixir/ssh_key.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir/user.py` & `gigalixir-1.6.0/gigalixir/user.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/gigalixir.egg-info/SOURCES.txt` & `gigalixir-1.6.0/gigalixir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gigalixir-1.5.1/setup.py` & `gigalixir-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gigalixir',
     url='https://github.com/gigalixir/gigalixir-cli',
     author='Tim Day',
     author_email='tim@gigalixir.com',
-    version='1.5.1',
+    version='1.6.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'click>=8.1',
         'requests>=2.28',
         'stripe>=4.1',
         'rollbar>=0.16',
```

### Comparing `gigalixir-1.5.1/test/test_gigalixir.py` & `gigalixir-1.6.0/test/test_gigalixir.py`

 * *Files identical despite different names*

