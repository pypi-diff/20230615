# Comparing `tmp/ansible_rulebook-0.9.4.tar.gz` & `tmp/ansible_rulebook-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_rulebook-0.9.4.tar", last modified: Tue Oct 18 14:33:50 2022, max compression
+gzip compressed data, was "ansible_rulebook-1.0.0.tar", last modified: Thu Jun 15 17:08:23 2023, max compression
```

## Comparing `ansible_rulebook-0.9.4.tar` & `ansible_rulebook-1.0.0.tar`

### file list

```diff
@@ -1,254 +1,402 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.894245 ansible_rulebook-0.9.4/
--rw-r--r--   0 ben        (501) staff       (20)     5536 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/CONTRIBUTING.rst
--rw-r--r--   0 ben        (501) staff       (20)       89 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/HISTORY.rst
--rw-r--r--   0 ben        (501) staff       (20)    11358 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)      295 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/MANIFEST.in
--rw-r--r--   0 ben        (501) staff       (20)     6207 2022-10-18 14:33:50.894403 ansible_rulebook-0.9.4/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     5418 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/README.rst
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.690923 ansible_rulebook-0.9.4/ansible_rulebook/
--rw-r--r--   0 ben        (501) staff       (20)       83 2022-10-18 14:32:48.000000 ansible_rulebook-0.9.4/ansible_rulebook/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)       46 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/__main__.py
--rw-r--r--   0 ben        (501) staff       (20)       63 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/ansible_events.py
--rw-r--r--   0 ben        (501) staff       (20)     4567 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/app.py
--rw-r--r--   0 ben        (501) staff       (20)    16870 2022-10-18 14:18:43.000000 ansible_rulebook-0.9.4/ansible_rulebook/builtin.py
--rw-r--r--   0 ben        (501) staff       (20)     3967 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/cli.py
--rw-r--r--   0 ben        (501) staff       (20)     2696 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/collection.py
--rw-r--r--   0 ben        (501) staff       (20)     3524 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/condition_parser.py
--rw-r--r--   0 ben        (501) staff       (20)      689 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/condition_types.py
--rw-r--r--   0 ben        (501) staff       (20)      124 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/conf.py
--rw-r--r--   0 ben        (501) staff       (20)     3783 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/durability.py
--rw-r--r--   0 ben        (501) staff       (20)    12574 2022-10-18 14:19:08.000000 ansible_rulebook-0.9.4/ansible_rulebook/engine.py
--rw-r--r--   0 ben        (501) staff       (20)      156 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/exception.py
--rw-r--r--   0 ben        (501) staff       (20)      668 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/inventory.py
--rw-r--r--   0 ben        (501) staff       (20)     8641 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/json_generator.py
--rw-r--r--   0 ben        (501) staff       (20)      960 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/key.py
--rw-r--r--   0 ben        (501) staff       (20)       70 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/messages.py
--rw-r--r--   0 ben        (501) staff       (20)     9368 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.4/ansible_rulebook/rule_generator.py
--rw-r--r--   0 ben        (501) staff       (20)     1449 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.4/ansible_rulebook/rule_types.py
--rw-r--r--   0 ben        (501) staff       (20)     3740 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/rules_parser.py
--rw-r--r--   0 ben        (501) staff       (20)     3142 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/util.py
--rw-r--r--   0 ben        (501) staff       (20)     3555 2022-10-15 18:36:10.000000 ansible_rulebook-0.9.4/ansible_rulebook/websocket.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.695021 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     6207 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     7492 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       63 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2022-10-11 23:07:19.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/not-zip-safe
--rw-r--r--   0 ben        (501) staff       (20)      110 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       17 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/top_level.txt
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.716221 ansible_rulebook-0.9.4/docs/
--rw-r--r--   0 ben        (501) staff       (20)      617 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/docs/Makefile
--rw-r--r--   0 ben        (501) staff       (20)      590 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/docs/actions.rst
--rw-r--r--   0 ben        (501) staff       (20)       28 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/authors.rst
--rw-r--r--   0 ben        (501) staff       (20)       39 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/collections.rst
--rw-r--r--   0 ben        (501) staff       (20)     1202 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/conditions.rst
--rwxr-xr-x   0 ben        (501) staff       (20)     4898 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/docs/conf.py
--rw-r--r--   0 ben        (501) staff       (20)       33 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/contributing.rst
--rw-r--r--   0 ben        (501) staff       (20)       42 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/environments.rst
--rw-r--r--   0 ben        (501) staff       (20)      342 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/filters.rst
--rw-r--r--   0 ben        (501) staff       (20)       28 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/history.rst
--rw-r--r--   0 ben        (501) staff       (20)      564 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/host_limit.rst
--rw-r--r--   0 ben        (501) staff       (20)      403 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/docs/index.rst
--rw-r--r--   0 ben        (501) staff       (20)     1113 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/docs/installation.rst
--rw-r--r--   0 ben        (501) staff       (20)      778 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/docs/make.bat
--rw-r--r--   0 ben        (501) staff       (20)     1582 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/multi_events.rst
--rw-r--r--   0 ben        (501) staff       (20)      801 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/multi_sources.rst
--rw-r--r--   0 ben        (501) staff       (20)       27 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/readme.rst
--rw-r--r--   0 ben        (501) staff       (20)    19540 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/docs/rules.rst
--rw-r--r--   0 ben        (501) staff       (20)       24 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/runner.rst
--rw-r--r--   0 ben        (501) staff       (20)     4406 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/docs/sources.rst
--rw-r--r--   0 ben        (501) staff       (20)     2344 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/docs/usage.rst
--rw-r--r--   0 ben        (501) staff       (20)      277 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/pyproject.toml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.717654 ansible_rulebook-0.9.4/schema/
--rw-r--r--   0 ben        (501) staff       (20)     5868 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/schema/ruleset_schema.json
--rw-r--r--   0 ben        (501) staff       (20)     1507 2022-10-18 14:33:50.895105 ansible_rulebook-0.9.4/setup.cfg
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.733298 ansible_rulebook-0.9.4/tests/
--rw-r--r--   0 ben        (501) staff       (20)       46 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/tests/__init__.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.793491 ansible_rulebook-0.9.4/tests/asts/
--rw-r--r--   0 ben        (501) staff       (20)      516 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/01_noop.yml
--rw-r--r--   0 ben        (501) staff       (20)      510 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/02_debug.yml
--rw-r--r--   0 ben        (501) staff       (20)      522 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/03_print_event.yml
--rw-r--r--   0 ben        (501) staff       (20)      888 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/04_set_fact.yml
--rw-r--r--   0 ben        (501) staff       (20)      890 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/05_post_event.yml
--rw-r--r--   0 ben        (501) staff       (20)     1183 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/06_retract_fact.yml
--rw-r--r--   0 ben        (501) staff       (20)      772 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/07_and.yml
--rw-r--r--   0 ben        (501) staff       (20)      770 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/08_or.yml
--rw-r--r--   0 ben        (501) staff       (20)      522 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/09_gt.yml
--rw-r--r--   0 ben        (501) staff       (20)      516 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/10_lt.yml
--rw-r--r--   0 ben        (501) staff       (20)      537 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/11_le.yml
--rw-r--r--   0 ben        (501) staff       (20)      543 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/12_ge.yml
--rw-r--r--   0 ben        (501) staff       (20)      662 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/13_add.yml
--rw-r--r--   0 ben        (501) staff       (20)      670 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/14_sub.yml
--rw-r--r--   0 ben        (501) staff       (20)      683 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/15_multiple_events_all.yml
--rw-r--r--   0 ben        (501) staff       (20)      683 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/16_multiple_events_any.yml
--rw-r--r--   0 ben        (501) staff       (20)      783 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/17_multiple_sources_any.yml
--rw-r--r--   0 ben        (501) staff       (20)      787 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/18_multiple_sources_all.yml
--rw-r--r--   0 ben        (501) staff       (20)      802 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/19_is_defined.yml
--rw-r--r--   0 ben        (501) staff       (20)     1100 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/20_is_not_defined.yml
--rw-r--r--   0 ben        (501) staff       (20)      561 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/21_run_playbook.yml
--rw-r--r--   0 ben        (501) staff       (20)      565 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/23_nested_data.yml
--rw-r--r--   0 ben        (501) staff       (20)      563 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/24_max_attributes.yml
--rw-r--r--   0 ben        (501) staff       (20)      604 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/25_max_attributes_nested.yml
--rw-r--r--   0 ben        (501) staff       (20)      643 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/26_print_events.yml
--rw-r--r--   0 ben        (501) staff       (20)     1066 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/27_var_root.yml
--rw-r--r--   0 ben        (501) staff       (20)      769 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/28_right_side_condition_template.yml
--rw-r--r--   0 ben        (501) staff       (20)      621 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/29_run_module.yml
--rw-r--r--   0 ben        (501) staff       (20)      619 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/30_run_module_missing.yml
--rw-r--r--   0 ben        (501) staff       (20)      626 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/31_run_module_missing_args.yml
--rw-r--r--   0 ben        (501) staff       (20)      641 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/32_run_module_fail.yml
--rw-r--r--   0 ben        (501) staff       (20)      649 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/33_run_playbook_retry.yml
--rw-r--r--   0 ben        (501) staff       (20)      625 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/34_run_playbook_retries.yml
--rw-r--r--   0 ben        (501) staff       (20)     1521 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/35_multiple_rulesets_1_fired.yml
--rw-r--r--   0 ben        (501) staff       (20)     1537 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/36_multiple_rulesets_both_fired.yml
--rw-r--r--   0 ben        (501) staff       (20)     1090 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/37_hosts_facts.yml
--rw-r--r--   0 ben        (501) staff       (20)      534 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/38_shutdown.yml
--rw-r--r--   0 ben        (501) staff       (20)     2984 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/rules.yml
--rw-r--r--   0 ben        (501) staff       (20)      708 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_assignment.yml
--rw-r--r--   0 ben        (501) staff       (20)      707 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_assignment2.yml
--rw-r--r--   0 ben        (501) staff       (20)      923 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions.yml
--rw-r--r--   0 ben        (501) staff       (20)      924 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions2.yml
--rw-r--r--   0 ben        (501) staff       (20)     1440 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions3.yml
--rw-r--r--   0 ben        (501) staff       (20)     1601 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_time.yml
--rw-r--r--   0 ben        (501) staff       (20)     2380 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_timestamp.yml
--rw-r--r--   0 ben        (501) staff       (20)      915 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_vars.yml
--rw-r--r--   0 ben        (501) staff       (20)      579 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_without_assignment.yml
--rw-r--r--   0 ben        (501) staff       (20)     1634 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_filters.yml
--rw-r--r--   0 ben        (501) staff       (20)     1958 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_host_rules.yml
--rw-r--r--   0 ben        (501) staff       (20)     1950 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_rules.yml
--rw-r--r--   0 ben        (501) staff       (20)     2017 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts.yml
--rw-r--r--   0 ben        (501) staff       (20)      529 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts2.yml
--rw-r--r--   0 ben        (501) staff       (20)      529 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts3.yml
--rw-r--r--   0 ben        (501) staff       (20)     1286 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_set_facts.yml
--rw-r--r--   0 ben        (501) staff       (20)     1548 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_simple.yml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.796087 ansible_rulebook-0.9.4/tests/event_filters/
--rw-r--r--   0 ben        (501) staff       (20)     1027 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/event_filters/dashes_to_underscores.py
--rw-r--r--   0 ben        (501) staff       (20)     1376 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/event_filters/json_filter.py
--rw-r--r--   0 ben        (501) staff       (20)      103 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/event_filters/noop.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.832444 ansible_rulebook-0.9.4/tests/examples/
--rw-r--r--   0 ben        (501) staff       (20)      182 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/01_noop.yml
--rw-r--r--   0 ben        (501) staff       (20)      176 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/02_debug.yml
--rw-r--r--   0 ben        (501) staff       (20)      188 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/03_print_event.yml
--rw-r--r--   0 ben        (501) staff       (20)      324 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/04_set_fact.yml
--rw-r--r--   0 ben        (501) staff       (20)      326 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/05_post_event.yml
--rw-r--r--   0 ben        (501) staff       (20)      458 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/06_retract_fact.yml
--rw-r--r--   0 ben        (501) staff       (20)      210 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/07_and.yml
--rw-r--r--   0 ben        (501) staff       (20)      208 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/08_or.yml
--rw-r--r--   0 ben        (501) staff       (20)      165 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/09_gt.yml
--rw-r--r--   0 ben        (501) staff       (20)      162 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/10_lt.yml
--rw-r--r--   0 ben        (501) staff       (20)      175 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/11_le.yml
--rw-r--r--   0 ben        (501) staff       (20)      178 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/12_ge.yml
--rw-r--r--   0 ben        (501) staff       (20)      203 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/13_add.yml
--rw-r--r--   0 ben        (501) staff       (20)      208 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/14_sub.yml
--rw-r--r--   0 ben        (501) staff       (20)      259 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/15_multiple_events_all.yml
--rw-r--r--   0 ben        (501) staff       (20)      259 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/16_multiple_events_any.yml
--rw-r--r--   0 ben        (501) staff       (20)      258 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/17_multiple_sources_any.yml
--rw-r--r--   0 ben        (501) staff       (20)      262 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/18_multiple_sources_all.yml
--rw-r--r--   0 ben        (501) staff       (20)      291 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/19_is_defined.yml
--rw-r--r--   0 ben        (501) staff       (20)      431 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/20_is_not_defined.yml
--rw-r--r--   0 ben        (501) staff       (20)      216 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/21_run_playbook.yml
--rw-r--r--   0 ben        (501) staff       (20)      249 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/22_run_playbook.yml
--rw-r--r--   0 ben        (501) staff       (20)      222 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/23_nested_data.yml
--rw-r--r--   0 ben        (501) staff       (20)      220 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/24_max_attributes.yml
--rw-r--r--   0 ben        (501) staff       (20)      261 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/25_max_attributes_nested.yml
--rw-r--r--   0 ben        (501) staff       (20)      240 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/26_print_events.yml
--rw-r--r--   0 ben        (501) staff       (20)      423 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/27_var_root.yml
--rw-r--r--   0 ben        (501) staff       (20)      349 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/28_right_side_condition_template.yml
--rw-r--r--   0 ben        (501) staff       (20)      270 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/29_run_module.yml
--rw-r--r--   0 ben        (501) staff       (20)      268 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/30_run_module_missing.yml
--rw-r--r--   0 ben        (501) staff       (20)      275 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/31_run_module_missing_args.yml
--rw-r--r--   0 ben        (501) staff       (20)      278 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/32_run_module_fail.yml
--rw-r--r--   0 ben        (501) staff       (20)      288 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/33_run_playbook_retry.yml
--rw-r--r--   0 ben        (501) staff       (20)      268 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/34_run_playbook_retries.yml
--rw-r--r--   0 ben        (501) staff       (20)      575 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/35_multiple_rulesets_1_fired.yml
--rw-r--r--   0 ben        (501) staff       (20)      591 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/36_multiple_rulesets_both_fired.yml
--rw-r--r--   0 ben        (501) staff       (20)      402 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/37_hosts_facts.yml
--rw-r--r--   0 ben        (501) staff       (20)      206 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/38_shutdown.yml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.668601 ansible_rulebook-0.9.4/tests/examples/replays/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.841111 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/
--rw-r--r--   0 ben        (501) staff       (20)       73 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/00.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/01.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/02.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/03.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/04.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/05.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/06.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/07.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/08.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/09.json
--rwxr-xr-x   0 ben        (501) staff       (20)      245 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/generate_data.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.842636 ansible_rulebook-0.9.4/tests/examples/replays/24_max_attributes/
--rw-r--r--   0 ben        (501) staff       (20)     5032 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/24_max_attributes/00.json
--rwxr-xr-x   0 ben        (501) staff       (20)      310 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/24_max_attributes/generate_data.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.844143 ansible_rulebook-0.9.4/tests/examples/replays/25_max_attributes_nested/
--rw-r--r--   0 ben        (501) staff       (20)     3791 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/25_max_attributes_nested/00.json
--rwxr-xr-x   0 ben        (501) staff       (20)      519 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/25_max_attributes_nested/generate_data.py
--rwxr-xr-x   0 ben        (501) staff       (20)     1108 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/generate_asts.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.851946 ansible_rulebook-0.9.4/tests/playbooks/
--rw-r--r--   0 ben        (501) staff       (20)      616 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/check_facts_playbook.yml
--rw-r--r--   0 ben        (501) staff       (20)      302 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/compare_value.yml
--rw-r--r--   0 ben        (501) staff       (20)      825 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/fail_and_succeed.yml
--rw-r--r--   0 ben        (501) staff       (20)      221 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/hello.yml
--rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/hello_events.yml
--rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/hello_world_set_fact.yml
--rw-r--r--   0 ben        (501) staff       (20)       62 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/inventory.yml
--rw-r--r--   0 ben        (501) staff       (20)      111 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/inventory1.yml
--rw-r--r--   0 ben        (501) staff       (20)      362 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/validate_args_playbook.yml
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/vars.yml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.879335 ansible_rulebook-0.9.4/tests/rules/
--rw-r--r--   0 ben        (501) staff       (20)     1410 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/rules.yml
--rw-r--r--   0 ben        (501) staff       (20)      267 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_assignment.yml
--rw-r--r--   0 ben        (501) staff       (20)      266 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_assignment2.yml
--rw-r--r--   0 ben        (501) staff       (20)      307 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_multiple_conditions.yml
--rw-r--r--   0 ben        (501) staff       (20)      308 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_multiple_conditions2.yml
--rw-r--r--   0 ben        (501) staff       (20)      475 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_multiple_conditions3.yml
--rw-r--r--   0 ben        (501) staff       (20)      741 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_time.yml
--rw-r--r--   0 ben        (501) staff       (20)     1070 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_timestamp.yml
--rw-r--r--   0 ben        (501) staff       (20)      281 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_vars.yml
--rw-r--r--   0 ben        (501) staff       (20)      244 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_without_assignment.yml
--rw-r--r--   0 ben        (501) staff       (20)      286 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_duplicate_rule_names.yml
--rw-r--r--   0 ben        (501) staff       (20)      199 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_empty_rule_names.yml
--rw-r--r--   0 ben        (501) staff       (20)      618 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_filters.yml
--rw-r--r--   0 ben        (501) staff       (20)      754 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_host_rules.yml
--rw-r--r--   0 ben        (501) staff       (20)     1463 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_kafka.yml
--rw-r--r--   0 ben        (501) staff       (20)      189 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_missing_rule_names.yml
--rw-r--r--   0 ben        (501) staff       (20)      337 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/test_multiple_sources.yml
--rw-r--r--   0 ben        (501) staff       (20)      746 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_rules.yml
--rw-r--r--   0 ben        (501) staff       (20)      461 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/test_rules_expanded_conditions.yml
--rw-r--r--   0 ben        (501) staff       (20)      813 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_rules_multiple_hosts.yml
--rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_rules_multiple_hosts2.yml
--rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_rules_multiple_hosts3.yml
--rw-r--r--   0 ben        (501) staff       (20)      244 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/test_rules_playbooks.yml
--rw-r--r--   0 ben        (501) staff       (20)      688 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_set_facts.yml
--rw-r--r--   0 ben        (501) staff       (20)      587 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_simple.yml
--rw-r--r--   0 ben        (501) staff       (20)      985 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_states.yml
--rw-r--r--   0 ben        (501) staff       (20)      944 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/webserver_down.yml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.891722 ansible_rulebook-0.9.4/tests/sources/
--rw-r--r--   0 ben        (501) staff       (20)        0 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     2025 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/file.py
--rw-r--r--   0 ben        (501) staff       (20)      375 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/hosts.py
--rw-r--r--   0 ben        (501) staff       (20)      555 2022-10-18 14:13:25.000000 ansible_rulebook-0.9.4/tests/sources/infrange.py
--rw-r--r--   0 ben        (501) staff       (20)     2253 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/log_scraper.py
--rwxr-xr-x   0 ben        (501) staff       (20)      500 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/nested.py
--rw-r--r--   0 ben        (501) staff       (20)      622 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/ping.py
--rw-r--r--   0 ben        (501) staff       (20)     1607 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/process_check.py
--rw-r--r--   0 ben        (501) staff       (20)      413 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/range.py
--rw-r--r--   0 ben        (501) staff       (20)      426 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/range2.py
--rwxr-xr-x   0 ben        (501) staff       (20)      990 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replay.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.893830 ansible_rulebook-0.9.4/tests/sources/replays/
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replays/01.json
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replays/02.json
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replays/03.json
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replays/04.json
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replays/05.json
--rw-r--r--   0 ben        (501) staff       (20)      636 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/sources/template.py
--rw-r--r--   0 ben        (501) staff       (20)      303 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/tick.py
--rwxr-xr-x   0 ben        (501) staff       (20)      436 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/timestamp.py
--rw-r--r--   0 ben        (501) staff       (20)     1320 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/url_check.py
--rw-r--r--   0 ben        (501) staff       (20)      532 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/tests/test_ansible_events.py
--rw-r--r--   0 ben        (501) staff       (20)     6677 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/test_ast.py
--rw-r--r--   0 ben        (501) staff       (20)      619 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/test_collection.py
--rw-r--r--   0 ben        (501) staff       (20)     6916 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.4/tests/test_conditions.py
--rw-r--r--   0 ben        (501) staff       (20)    15703 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/test_engine.py
--rw-r--r--   0 ben        (501) staff       (20)    28166 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/test_examples.py
--rwxr-xr-x   0 ben        (501) staff       (20)     7849 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.4/tests/test_rules.py
--rw-r--r--   0 ben        (501) staff       (20)      576 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/test_simple.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.819764 ansible_rulebook-1.0.0/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    11358 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/LICENSE
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      312 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/MANIFEST.in
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4111 2023-06-15 17:08:23.819847 ansible_rulebook-1.0.0/PKG-INFO
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     3353 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/README.rst
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.772208 ansible_rulebook-1.0.0/ansible_rulebook/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      671 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/__init__.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      634 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/__main__.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     8413 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/app.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    26665 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/builtin.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     7948 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/cli.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4671 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/collection.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1075 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/common.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     8165 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/condition_parser.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2659 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/condition_types.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      796 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/conf.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     9754 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/engine.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.773332 ansible_rulebook-1.0.0/ansible_rulebook/event_filter/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/event_filter/__init__.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1346 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/event_filter/insert_meta_info.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2228 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/exception.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     6285 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/job_template_runner.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    11925 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/json_generator.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      827 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/messages.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     3173 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/rule_generator.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    17737 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/rule_set_runner.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2418 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/rule_types.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     6558 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/rules_parser.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.773465 ansible_rulebook-1.0.0/ansible_rulebook/schema/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    20517 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/schema/ruleset_schema.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     7223 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/util.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1428 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/validators.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4908 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/websocket.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.773098 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4111 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/PKG-INFO
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    12566 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/SOURCES.txt
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)        1 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/dependency_links.txt
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       63 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/entry_points.txt
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)        1 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/not-zip-safe
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      104 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/requires.txt
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       17 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/top_level.txt
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.776357 ansible_rulebook-1.0.0/docs/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      617 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/Makefile
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    11365 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/actions.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2647 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/collections.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    33663 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/conditions.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     5955 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/conf.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2033 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/contributing.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4272 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/decision_environment.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     3560 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/development_environment.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2033 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/events_and_facts.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2700 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/filters.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     7006 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/getting_started.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      625 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/host_limit.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      495 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/index.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2437 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/installation.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     5447 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/introduction.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      778 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/make.bat
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2278 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/multi_events.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4137 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/rulebooks.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2397 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/rules.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       41 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/runner.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     5714 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/sources.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4380 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/usage.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4865 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/variables.rst
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      277 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/pyproject.toml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1487 2023-06-15 17:08:23.820286 ansible_rulebook-1.0.0/setup.cfg
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.778280 ansible_rulebook-1.0.0/tests/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      634 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/__init__.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.785858 ansible_rulebook-1.0.0/tests/asts/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      516 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/01_noop.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      510 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/02_debug.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      522 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/03_print_event.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      888 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/04_set_fact.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      890 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/05_post_event.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1183 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/06_retract_fact.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      772 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/07_and.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      770 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/08_or.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      522 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/09_gt.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      516 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/10_lt.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      537 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/11_le.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      543 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/12_ge.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      662 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/13_add.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      670 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/14_sub.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      683 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/15_multiple_events_all.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      683 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/16_multiple_events_any.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      783 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/17_multiple_sources_any.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      787 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/18_multiple_sources_all.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1076 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/19_is_defined.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1100 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/20_is_not_defined.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      561 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/21_run_playbook.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      565 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/23_nested_data.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      563 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/24_max_attributes.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      604 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/25_max_attributes_nested.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      643 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/26_print_events.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1066 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/27_var_root.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      769 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/28_right_side_condition_template.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      621 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/29_run_module.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      619 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/30_run_module_missing.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      626 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/31_run_module_missing_args.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      641 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/32_run_module_fail.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      649 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/33_run_playbook_retry.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      625 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/34_run_playbook_retries.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1521 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/35_multiple_rulesets_1_fired.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1537 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/36_multiple_rulesets_both_fired.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1090 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/37_hosts_facts.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      534 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/38_shutdown.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2990 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      694 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_assignment.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      693 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_assignment2.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      924 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      925 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions2.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1441 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions3.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1605 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_time.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2385 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_timestamp.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      916 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_vars.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      580 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_without_assignment.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1638 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_filters.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1963 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_host_rules.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1955 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_rules.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2022 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      530 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts2.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      530 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts3.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1338 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_set_facts.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1552 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_simple.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.786147 ansible_rulebook-1.0.0/tests/cassettes/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    28619 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/cassettes/test_job_template.yaml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    10489 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/cassettes/test_job_template_not_exist.yaml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2754 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/conftest.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.786819 ansible_rulebook-1.0.0/tests/data/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       37 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/data/bad_source.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      137 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/data/not_asyncio.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      727 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/data/rulebook.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    47616 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/data/test.tar
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       68 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/data/test_vars.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.788152 ansible_rulebook-1.0.0/tests/e2e/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      878 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/README.md
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/__init__.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.788291 ansible_rulebook-1.0.0/tests/e2e/config/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      246 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/config/default.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      564 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/conftest.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.766501 ansible_rulebook-1.0.0/tests/e2e/files/
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.788913 ansible_rulebook-1.0.0/tests/e2e/files/extra_vars/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      826 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/extra_vars/operator_variables.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      162 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/extra_vars/test_variables_extra_vars.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.789258 ansible_rulebook-1.0.0/tests/e2e/files/inventories/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       35 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/inventories/default_inventory.ini
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       61 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/inventories/default_inventory.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.790032 ansible_rulebook-1.0.0/tests/e2e/files/playbooks/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      404 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/playbooks/long_running.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      344 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/playbooks/print_event.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      240 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/playbooks/print_rule_name.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1522 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/playbooks/run_playbook_test_playbook.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.790783 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.791409 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4727 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_actions_sanity.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2451 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_run_playbook.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1611 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_shutdown_graceful.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1050 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_shutdown_now.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      288 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/hello_events_with_var.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      253 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/malformed_rulebook.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.792607 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     6274 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_logical_operators.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     6060 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_membership_operators.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     6216 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_relational_operators.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     3476 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_select_operator.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     7702 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_selectattr_operator.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2545 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_string_match.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2583 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_string_search_regex.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2623 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_string_search_search.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1394 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/test_disabled_rules.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      270 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/test_process_sigint.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      955 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/test_process_source_end.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.792760 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/variables/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2070 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/variables/test_variables_sanity.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.792922 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/websockets/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      283 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/websockets/test_websocket_range.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      522 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/settings.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    10871 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/test_actions.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    20067 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/test_operators.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     5843 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/test_runtime.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2271 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/test_variables.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     3595 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/test_websocket.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.766978 ansible_rulebook-1.0.0/tests/e2e/utils/
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.793811 ansible_rulebook-1.0.0/tests/e2e/utils/awx/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      164 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/ansible.cfg
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      602 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/create-cluster.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      637 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/install-awx.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      437 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/kind-config.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      855 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/readme.md
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       27 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/requirements.txt
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.767128 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.767376 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.794029 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/defaults/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      226 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/defaults/main.yaml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.794236 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/tasks/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1204 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/tasks/main.yaml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.794632 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/templates/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      162 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/templates/admin-password-secret.yml.j2
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      264 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/templates/awx.yaml.j2
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.794816 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/templates/kustomization/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      464 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/templates/kustomization/kustomization.yaml.j2
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     3917 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.795509 ansible_rulebook-1.0.0/tests/event_filter/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1615 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/event_filter/dashes_to_underscores.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1964 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/event_filter/json_filter.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      691 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/event_filter/noop.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1385 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/event_filter/test_insert_meta_info.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.806738 ansible_rulebook-1.0.0/tests/examples/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      182 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/01_noop.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      176 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/02_debug.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      188 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/03_print_event.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      324 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/04_set_fact.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      326 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/05_post_event.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      458 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/06_retract_fact.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      210 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/07_and.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      208 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/08_or.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      165 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/09_gt.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      162 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/10_lt.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      175 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/11_le.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      178 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/12_ge.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      203 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/13_add.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      208 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/14_sub.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      259 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/15_multiple_events_all.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      259 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/16_multiple_events_any.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      258 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/17_multiple_sources_any.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      262 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/18_multiple_sources_all.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      402 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/19_is_defined.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      431 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/20_is_not_defined.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      216 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/21_run_playbook.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      249 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/22_run_playbook.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      222 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/23_nested_data.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      220 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/24_max_attributes.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      261 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/25_max_attributes_nested.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      240 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/26_print_events.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      894 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/27_var_root.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      205 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/28_right_side_condition_template.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      270 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/29_run_module.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      268 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/30_run_module_missing.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      275 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/31_run_module_missing_args.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      278 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/32_run_module_fail.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      359 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/33_run_playbook_retry.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      339 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/34_run_playbook_retries.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      575 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/35_multiple_rulesets_1_fired.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      766 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/36_multiple_rulesets_both_fired.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      402 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/37_hosts_facts.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      299 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/38_shutdown.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      206 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/39_is_defined.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      183 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/40_in.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      193 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/41_not_in.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      268 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/42_contains.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      276 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/43_not_contains.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      201 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/44_in_and.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      199 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/45_in_or.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      376 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/46_job_template.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      311 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/47_generic_plugin.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      206 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/48_echo.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      445 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/49_float.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      660 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/50_negation.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1375 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/51_vars_namespace.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      648 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/52_once_within.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      659 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/53_once_within_multiple_hosts.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      542 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/54_time_window.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      622 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/55_not_all.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      798 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/56_once_after.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1890 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/57_once_after_multi.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1453 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/58_string_search.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      444 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/59_multiple_actions.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      713 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/60_json_filter.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      608 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/61_select_1.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      903 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/62_select_2.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      938 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/63_selectattr_1.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      589 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/64_selectattr_2.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      413 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/65_selectattr_3.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      881 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/66_sleepy_playbook.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      835 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/67_shutdown_now.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      347 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/68_disabled_rule.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      729 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/69_enhanced_debug.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      724 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/70_null.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1101 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/72_set_fact_with_type.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      874 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/73_mix_and_match_list.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      231 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/74_self_referential.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      538 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/75_all_conditions.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      736 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/76_all_conditions.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      485 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/77_default_events_ttl.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      592 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/78_complete_retract_fact.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.768066 ansible_rulebook-1.0.0/tests/examples/replays/
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.808154 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/00.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/01.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/02.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/03.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/04.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/05.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/06.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/07.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/08.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/09.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      833 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/generate_data.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.808418 ansible_rulebook-1.0.0/tests/examples/replays/24_max_attributes/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     5032 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/24_max_attributes/00.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      898 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/24_max_attributes/generate_data.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.808689 ansible_rulebook-1.0.0/tests/examples/replays/25_max_attributes_nested/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     3791 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/25_max_attributes_nested/00.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1107 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/25_max_attributes_nested/generate_data.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.810142 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/00.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/01.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/02.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/03.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/04.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/05.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/06.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/07.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/08.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/09.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      833 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/generate_data.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1696 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/generate_asts.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.811576 ansible_rulebook-1.0.0/tests/playbooks/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      618 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/check_facts_playbook.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      370 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/compare_value.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      829 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/fail_and_succeed.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      400 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/hello.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      309 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/hello_events.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      290 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/hello_world_set_fact.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      129 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/inventory.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      114 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/inventory1.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      260 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/sleeper.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      704 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/validate_args_playbook.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)       13 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/vars.yml
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.816281 ansible_rulebook-1.0.0/tests/rules/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      300 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rule_names_with_substitution.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1410 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      252 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_assignment.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      251 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_assignment2.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      307 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_multiple_conditions.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      308 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_multiple_conditions2.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      475 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_multiple_conditions3.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      741 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_time.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1070 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_timestamp.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      281 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_vars.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      244 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_without_assignment.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      203 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_blank_rule_name.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      171 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_blank_ruleset_name.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      282 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_combine_hosts.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      329 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_combine_hosts_module.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      286 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_duplicate_rule_names.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      348 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_duplicate_ruleset_names.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      199 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_empty_rule_names.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      618 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_filters.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      754 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_host_rules.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1463 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_kafka.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      189 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_missing_rule_names.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      159 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_missing_ruleset_name.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      337 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_multiple_sources.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      746 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      461 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules_expanded_conditions.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      813 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules_multiple_hosts.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      195 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules_multiple_hosts2.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      195 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules_multiple_hosts3.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      244 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules_playbooks.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      728 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_set_facts.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      587 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_simple.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      985 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_states.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      944 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/webserver_down.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      275 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/run_examples.sh
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.818607 ansible_rulebook-1.0.0/tests/sources/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/__init__.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2613 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/file.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4945 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/generic.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      963 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/hosts.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1613 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/infrange.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2841 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/log_scraper.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1258 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/nested.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1210 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/ping.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2195 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/process_check.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1245 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/range.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1014 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/range2.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1578 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replay.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.819318 ansible_rulebook-1.0.0/tests/sources/replays/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)        9 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replays/01.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)        9 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replays/02.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)        9 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replays/03.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)        9 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replays/04.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)        9 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replays/05.json
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1224 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/template.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      891 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/tick.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1024 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/timestamp.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1908 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/url_check.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1120 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_ansible_events.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     5887 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_app.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    18000 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_ast.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     2206 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_collection.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     3038 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_controller.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    15993 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_engine.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)    66166 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_examples.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     8114 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_rules.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)      576 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_simple.yml
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     4931 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_websocket.py
+drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.819627 ansible_rulebook-1.0.0/tests/unit/
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     3055 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/unit/test_cli.py
+-rw-r--r--   0 madhukanoor   (501) wheel        (0)     1147 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/unit/test_util.py
```

### Comparing `ansible_rulebook-0.9.4/LICENSE` & `ansible_rulebook-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/PKG-INFO` & `ansible_rulebook-1.0.0/docs/getting_started.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,46 @@
-Metadata-Version: 2.1
-Name: ansible_rulebook
-Version: 0.9.4
-Summary: Event driven automation for Ansible
-Home-page: https://github.com/ansible/ansible-rulebook
-License: Apache-2.0
-Keywords: ansible_rulebook
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst; charset=UTF-8
-License-File: LICENSE
-
-================
-ansible-rulebook
-================
-
-
-.. image:: https://img.shields.io/pypi/v/ansible_rulebook.svg
-        :target: https://pypi.python.org/pypi/ansible_rulebook
-
-.. image:: https://img.shields.io/travis/ansible/ansible_rulebook.svg
-        :target: https://travis-ci.com/ansible/ansible_rulebook
-
-.. image:: https://readthedocs.org/projects/ansible-rulebook/badge/?version=latest
-        :target: https://ansible-rulebook.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-* Free software: Apache Software License 2.0
-* Documentation: https://ansible-rulebook.readthedocs.io.
-
-
-Event driven automation for Ansible.
-
-
-The real world is full of events that change the state of our software and systems.
-Our automation needs to be able to react to those events. Introducing *ansible-rulebook*; a command
-line tool that allows you to recognize events that you care about and react accordingly
-by running a playbook or other actions.
-
-============
-Installation
-============
-
-Head over to the `Installation`_ page for details on how to install *ansible-rulebook*. Once installed,
-continue with the **Getting started** section below to begin writing your first rulesets.
-
-.. _Installation: docs/installation.rst
-
 ===============
 Getting started
 ===============
 
-**Important:** Running *ansible-rulebook* requires setting the *JAVA_HOME* environment variable. On Fedora-like systems, this will be::
+If ansible-rulebook is not already installed, please follow the `installation guide <installation.html>`_ to install it.
 
-    $ export JAVA_HOME=/usr/lib/jvm/java-17-openjdk
+Now let's get started with a simple hello world example to familiarize ourselves with the concepts:
 
-Let's get started with a simple hello world example to familiarize ourselves with the concepts::
+.. code-block:: yaml
 
     ---
     - name: Hello Events
       hosts: localhost
       sources:
         - ansible.eda.range:
             limit: 5
       rules:
         - name: Say Hello
           condition: event.i == 1
           action:
             run_playbook:
               name: ansible.eda.hello
-    ...
+
 
 
 Events come from a **event source** and then are checked against **rules** to determine if an **action** should
 be taken.  If the **condition** of a rule matches the event it will run the action for that rule.
 
 In this example the event source is the Python range function.  It produces events that count from
 :code:`i=0` to :code:`i=<limit>`.
 
 When :code:`i` is equal to 1 the condition for the the :code:`Say Hello` rule matches and it runs a playbook.
 
 
 Normally events would come from monitoring and alerting systems or other software. The following
-is a more complete example that accepts alerts from Alertmanager::
+is a more complete example that accepts alerts from Alertmanager:
+
+.. code-block:: yaml
+
 
     ---
     - name: Automatic Remediation of a webserver
       hosts: all
       sources:
         - name: listen for alerts
           ansible.eda.alertmanager:
@@ -104,92 +52,138 @@
           action:
             run_playbook:
               name: ansible.eda.start_app
     ...
 
 
 This example sets up a webhook to receive events from alertmanager and then matches events
-where the `fastapi` job alert has a staus of `firing`.  This runs a playbook that will
+where the `fastapi` job alert has a status of `firing`.  This runs a playbook that will
 remediate the issue.
 
 
+Let's build an example rulebook that will trigger an action from a
+webhook. We will be looking for a specific payload from the webhook, and
+if that condition is met from the webhook event, then ansible-rulebook
+will trigger the desired action. Below is our example rulebook:
 
-Features
---------
+.. code-block:: yaml
 
-* Connect to event streams and handle events in near real time.
-* Conditionally launch playbooks based on rules that match events in event streams.
-* Store facts about the world from data in events
-* Limit the hosts where playbooks run based on event data
-* Run smaller jobs that run more quickly by limiting the hosts where playbooks run based on event data
+   ---
+   - name: Listen for events on a webhook
+     hosts: all
 
+     ## Define our source for events
 
+     sources:
+       - ansible.eda.webhook:
+           host: 0.0.0.0
+           port: 5000
 
-Examples
---------
+     ## Define the conditions we are looking for
 
-Rules are organized into rulesets using a syntax that is similar to ansible-playbooks::
+     rules:
+       - name: Say Hello
+         condition: event.payload.message == "Ansible is super cool"
 
-    ---
-    - name: Hello Events
-      hosts: localhost
-      sources:
-        - ansible.eda.range:
-            limit: 5
-      rules:
-        - name: Say Hello
-          condition: event.i == 1
-          action:
-            run_playbook:
-              name: ansible.eda.hello
-    ...
+     ## Define the action we should take should the condition be met
 
-Each ruleset defines: a set of hosts to pass to the playbook, a set of event sources,
-and a set of rules.   The set of hosts is the normal hosts pattern from ansible playbooks.
-The event sources are a new type of plugin that subscribe to events from event streams.
-The rules have conditions that match values in the events and actions that can run playbooks,
-assert facts, retract facts, and print information to the console.
+         action:
+           run_playbook:
+             name: say-what.yml
 
+The playbook ``say-what.yml``:
 
-Let's look closer at the event source::
+.. code-block:: yaml
 
-        - ansible.eda.range:
-            limit: 5
+   - hosts: localhost
+     connection: local
+     tasks:
+       - debug:
+           msg: "Thank you, my friend!"
 
-This section of YAML defines that an event source plugin from the ansible.eda should
-be loaded and given the arguments: limit=5.  This source will generate a range of numbers
-from zero to 4 and then exit.
+If we look at this example, we can see the structure of the rulebook.
+Our sources, rules and actions are defined. We are using the webhook
+source plugin from our ansible.eda collection, and we are looking for a
+message payload from our webhook that contains “Ansible is super cool”.
+Once this condition has been met, our defined action will trigger which
+in this case is to trigger a playbook.
 
-The rules YAML structure looks like the following::
+One important thing to take note of ansible-rulebook is that it is not
+like ansible-playbook which runs a playbook and once the playbook has
+been completed it will exit. With ansible-rulebook, it will continue to
+run waiting for events and matching those events, it will only exit upon
+a shutdown action or if there is an issue with the event source itself,
+for example if a website you are watching with the url-check plugin
+stops working.
 
-        - name: Say Hello
-          condition: event.i == 1
-          action:
-            run_playbook:
-              name: ansible.eda.hello
+With our rulebook built, we will simply tell ansible-rulebook to use it
+as a ruleset and wait for events:
+
+.. code-block:: shell
+
+   root@ansible-rulebook:/root# ansible-rulebook --rulebook webhook-example.yml -i inventory.yml --verbose
+
+   INFO:ansible_events:Starting sources
+   INFO:ansible_events:Starting sources
+   INFO:ansible_events:Starting rules
+   INFO:root:run_ruleset
+   INFO:root:{'all': [{'m': {'payload.message': 'Ansible is super cool!'}}], 'run': <function make_fn.<locals>.fn at 0x7ff962418040>}
+   INFO:root:Waiting for event
+   INFO:root:load source
+   INFO:root:load source filters
+   INFO:root:Calling main in ansible.eda.webhook
+
+Now, ansible-rulebook is ready and it's waiting for an event to match.
+If a webhook is triggered but the payload does not match our condition
+in our rule, we can see it in the ansible-rulebook verbose output:
+
+.. code-block:: shell
+
+   …
+   INFO:root:Calling main in ansible.eda.webhook
+   INFO:aiohttp.access:127.0.0.1 [14/Oct/2022:09:49:32 +0000] "POST /endpoint HTTP/1.1" 200 158 "-" "curl/7.61.1"
+   INFO:root:Waiting for event
+
+But once our payload matches what we are looking for, that's when the
+magic happens, so we will simulate a webhook with the correct payload:
+
+.. code-block:: shell
+
+   curl -H 'Content-Type: application/json' -d "{\"message\": \"Ansible is super cool\"}" 127.0.0.1:5000/endpoint
 
 
-This block of YAML defines a rule with name "Say Hello", a condition that matches
-when an event has an value "i" that is equal to 1, and an action that runs a playbook
-inside the collection ansible.eda.
+   INFO:root:Calling main in ansible.eda.webhook
+   INFO:aiohttp.access:127.0.0.1 [14/Oct/2022:09:50:28 +0000] "POST /endpoint HTTP/1.1" 200 158 "-" "curl/7.61.1"
+   INFO:root:calling Say Hello
+   INFO:root:call_action run_playbook
+   INFO:root:substitute_variables [{'name': 'say-what.yml'}] [{'event': {'payload': {'message': 'Ansible is super cool'}, 'meta': {'endpoint': 'endpoint', 'headers': {'Host': '127.0.0.1:5000', 'User-Agent': 'curl/7.61.1', 'Accept': '*/*', 'Content-Type': 'application/json', 'Content-Length': '36'}}}, 'fact': {'payload': {'message': 'Ansible is super cool'}, 'meta': {'endpoint': 'endpoint', 'headers': {'Host': '127.0.0.1:5000', 'User-Agent': 'curl/7.61.1', 'Accept': '*/*', 'Content-Type': 'application/json', 'Content-Length': '36'}}}}]
+   INFO:root:action args: {'name': 'say-what.yml'}
+   INFO:root:running Ansible playbook: say-what.yml
+   INFO:root:Calling Ansible runner
 
-For more information on usage and examples, please refer to the `Usage`_ guide.
+   PLAY [say thanks] **************************************************************
 
-.. _Usage: docs/usage.rst
+   TASK [debug] *******************************************************************
+   ok: [localhost] => {
+       "msg": "Thank you, my friend!"
+   }
 
+   PLAY RECAP *********************************************************************
+   localhost                  : ok=1    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
 
-Credits
--------
+   INFO:root:Waiting for event
 
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+We can see from the output above, that the condition was met from the
+webhook and ansible-rulebook then triggered our action which was to
+run_playbook. The playbook we defined is then triggered and once it
+completes we can see we revert back to “Waiting for event”.
 
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+Event-Driven Ansible opens up the possibilities of faster resolution and
+greater automated observation of our environments. It has the
+possibility of simplifying the lives of many technical and
+sleep-deprived engineers.
 
-=======
-History
-=======
 
-0.1.0 (2022-02-16)
-------------------
+Extras
+------
 
-* First release on PyPI.
+Video: `Writing Rulebooks <https://www.youtube.com/watch?v=PtevBKX1SYI>`__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ansible_rulebook-0.9.4/README.rst` & `ansible_rulebook-1.0.0/docs/introduction.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,167 +1,134 @@
-================
-ansible-rulebook
-================
+Introduction
+====================
 
+What is Event-Driven Ansible?
+-----------------------------
 
-.. image:: https://img.shields.io/pypi/v/ansible_rulebook.svg
-        :target: https://pypi.python.org/pypi/ansible_rulebook
+Event-Driven Ansible is a new way to enhance and expand automation. It
+improves IT speed and agility, while enabling consistency and
+resilience. The Event-Driven Ansible technology was developed by Red Hat
+and is available as a developer preview. Community input is essential.
+Since we are building a solution to best meet your needs, we're
+providing an opportunity for you to advocate for those needs.
 
-.. image:: https://img.shields.io/travis/ansible/ansible_rulebook.svg
-        :target: https://travis-ci.com/ansible/ansible_rulebook
+Event-Driven Ansible is designed for simplicity and flexibility. By
+writing an Ansible Rulebook (similar to Ansible Playbooks, but more
+oriented to “if-then” scenarios) and allowing Event-Driven Ansible to
+subscribe to an event listening source, your teams can more quickly and
+easily automate a variety of tasks across the organization. EDA is
+providing a way of codifying operational logic.
 
-.. image:: https://readthedocs.org/projects/ansible-rulebook/badge/?version=latest
-        :target: https://ansible-rulebook.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
+Why Event-Driven?
+-----------------
 
-* Free software: Apache Software License 2.0
-* Documentation: https://ansible-rulebook.readthedocs.io.
+Automation allows us to give our systems and technology speed and
+agility while minimizing human error. However, when it comes to trouble
+tickets and issues, we are often left to traditional and often manual
+methods of troubleshooting and information gathering. We inherently slow
+things down and interrupt our businesses. We have to gather information,
+try our common troubleshooting steps, confirm with different teams.
 
+One application of Event-Driven Ansible is to codify this operation
+knowledge in order to remediate technology issues near real-time, or at
+least trigger troubleshooting and information collection in an attempt
+to find the root cause of an outage while your support teams handle
+other issues.
 
-Event driven automation for Ansible.
+Event-Driven Ansible has the potential to change the way we respond to
+issues and illuminates many new automation possibilities.
 
+It opens up the possibilities of faster resolution and greater automated
+observation of our environments.
 
-The real world is full of events that change the state of our software and systems.
-Our automation needs to be able to react to those events. Introducing *ansible-rulebook*; a command
-line tool that allows you to recognize events that you care about and react accordingly
-by running a playbook or other actions.
 
-============
-Installation
-============
+Why Rulebooks?
+--------------
 
-Head over to the `Installation`_ page for details on how to install *ansible-rulebook*. Once installed,
-continue with the **Getting started** section below to begin writing your first rulesets.
+Event-Driven Ansible contains a decision framework that was built using
+Drools. We need a rulebook to tell the system what events to flag and
+how to respond to them. These rulebooks are also created in YAML and are
+used like traditional Ansible Playbooks, so this makes it easier to
+understand and build the rulebooks we need. One key difference between
+playbooks and rulebooks is the If-this-then-that coding that is needed
+in a rulebook to make an event driven automation approach work.
 
-.. _Installation: docs/installation.rst
 
-===============
-Getting started
-===============
-
-**Important:** Running *ansible-rulebook* requires setting the *JAVA_HOME* environment variable. On Fedora-like systems, this will be::
-
-    $ export JAVA_HOME=/usr/lib/jvm/java-17-openjdk
-
-Let's get started with a simple hello world example to familiarize ourselves with the concepts::
-
-    ---
-    - name: Hello Events
-      hosts: localhost
-      sources:
-        - ansible.eda.range:
-            limit: 5
-      rules:
-        - name: Say Hello
-          condition: event.i == 1
-          action:
-            run_playbook:
-              name: ansible.eda.hello
-    ...
-
-
-Events come from a **event source** and then are checked against **rules** to determine if an **action** should
-be taken.  If the **condition** of a rule matches the event it will run the action for that rule.
-
-In this example the event source is the Python range function.  It produces events that count from
-:code:`i=0` to :code:`i=<limit>`.
-
-When :code:`i` is equal to 1 the condition for the the :code:`Say Hello` rule matches and it runs a playbook.
-
-
-Normally events would come from monitoring and alerting systems or other software. The following
-is a more complete example that accepts alerts from Alertmanager::
+**A rulebook is comprised of three main components:**
 
-    ---
-    - name: Automatic Remediation of a webserver
-      hosts: all
-      sources:
-        - name: listen for alerts
-          ansible.eda.alertmanager:
-            host: 0.0.0.0
-            port: 8000
-      rules:
-        - name: restart web server
-          condition: event.alert.labels.job == "fastapi" and event.alert.status == "firing"
-          action:
-            run_playbook:
-              name: ansible.eda.start_app
-    ...
+-  **Sources** define which event source we will use. These sources come
+   from source plugins which have been built to accommodate common use
+   cases. With time, more and more sources will be available. There are
+   some source plugins that are available already, including: webhooks,
+   Kafka, Azure service bus, file changes, and alertmanager.
 
+-  **Rules** define conditionals we will try to match from the event
+   source. Should the condition be met, then we can trigger an action.
 
-This example sets up a webhook to receive events from alertmanager and then matches events
-where the `fastapi` job alert has a staus of `firing`.  This runs a playbook that will
-remediate the issue.
+-  **Actions** trigger what you need to happen should a condition be
+   met. Some of the current actions are: run_playbook, run_module,
+   set_fact, post_event, debug.
 
+So to summarize:
 
+**Events are processed by a rules engine**
 
-Features
---------
+-  Rules trigger based on conditions and actions can be carried out by
+   the rules engine
+-  Rules are organized into Ansible Rulebooks
+-  Ansible rules can apply to events occurring on specific hosts or
+   groups
 
-* Connect to event streams and handle events in near real time.
-* Conditionally launch playbooks based on rules that match events in event streams.
-* Store facts about the world from data in events
-* Limit the hosts where playbooks run based on event data
-* Run smaller jobs that run more quickly by limiting the hosts where playbooks run based on event data
+**Conditional management of actions to events**
 
+-  Simple YAML structure for logical conditions
+-  Events can trigger different types of actions:
+-  Run Ansible Playbooks
+-  Run Modules directly
+-  Post new events to the event handler
 
+**YAML-like format familiarity**
 
-Examples
---------
+-  Current Ansible users quickly learn and use Rulebook writing
 
-Rules are organized into rulesets using a syntax that is similar to ansible-playbooks::
 
-    ---
-    - name: Hello Events
-      hosts: localhost
-      sources:
-        - ansible.eda.range:
-            limit: 5
-      rules:
-        - name: Say Hello
-          condition: event.i == 1
-          action:
-            run_playbook:
-              name: ansible.eda.hello
-    ...
-
-Each ruleset defines: a set of hosts to pass to the playbook, a set of event sources,
-and a set of rules.   The set of hosts is the normal hosts pattern from ansible playbooks.
-The event sources are a new type of plugin that subscribe to events from event streams.
-The rules have conditions that match values in the events and actions that can run playbooks,
-assert facts, retract facts, and print information to the console.
-
-
-Let's look closer at the event source::
-
-        - ansible.eda.range:
-            limit: 5
-
-This section of YAML defines that an event source plugin from the ansible.eda should
-be loaded and given the arguments: limit=5.  This source will generate a range of numbers
-from zero to 4 and then exit.
-
-The rules YAML structure looks like the following::
-
-        - name: Say Hello
-          condition: event.i == 1
-          action:
-            run_playbook:
-              name: ansible.eda.hello
-
-
-This block of YAML defines a rule with name "Say Hello", a condition that matches
-when an event has an value "i" that is equal to 1, and an action that runs a playbook
-inside the collection ansible.eda.
-
-For more information on usage and examples, please refer to the `Usage`_ guide.
+Getting started
+---------------
+See `Getting Started <getting_started.html>`_
 
-.. _Usage: docs/usage.rst
 
+Other Resources
+---------------
 
-Credits
--------
+Whether you are beginning your automation journey or a seasoned veteran,
+there are a variety of resources to enhance your automation knowledge:
+
+-  `Self-paced lab
+   exercises <https://www.redhat.com/en/engage/redhat-ansible-automation-202108061218>`__
+   - We have interactive, in-browser exercises to help you get started
+   with Event-Driven Ansible and ansible-rulebook.
+-  `Event-Driven Ansible web page <https://ansible.com/event-driven>`__
+-  `Introducing Event-Driven Ansible
+   blog <https://www.ansible.com/blog/introducing-event-driven-ansible>`__
+-  `Why Event-Driven
+   Matters <https://www.ansible.com/blog/why-event-driven-matters>`__ -
+   Have a look at another blog about why Event-Driven Ansible matters.
+-  `Event-Driven Rulebooks <https://youtu.be/PtevBKX1SYI>`__ - Watch
+   another example of Event-Driven Ansible on our YouTube channel.
+-  `EDA and Gitops <https://youtu.be/Bb51DftLbPE>`__ - Watch another
+   example of Event-Driven Ansible, but with GitOps, on our YouTube
+   channel.
+-  Learn more about Event-Driven Ansible at our office hours `December
+   14,
+   2022 <https://www.redhat.com/en/events/webinar/event-driven-ansible-office-hours-december>`__.
+-  `Ansible Rulebook
+   CLI <https://github.com/ansible/ansible-rulebook>`__
+
+Office Hours
+------------
+
+Join us for Office Hours on the Event-Driven Ansible developer preview
+on December 14th at 11AM ET. Get some tips and techniques, ask questions
+and share your feedback! Learn from the community. See you there.
+https://www.ansible.com/resources/webinars-training/event-driven-ansible-office-hours-dec
 
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ansible_rulebook-0.9.4/ansible_rulebook/builtin.py` & `ansible_rulebook-1.0.0/ansible_rulebook/rule_set_runner.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,659 +1,487 @@
+#  Copyright 2022 Red Hat, Inc.
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
 import asyncio
-import concurrent.futures
-import glob
-import json
+import gc
 import logging
-import os
-import shutil
-import sys
-import tempfile
 import uuid
-from asyncio.exceptions import CancelledError
-from datetime import datetime
-from functools import partial
-from pprint import pprint
-from typing import Callable, Dict, List, Optional, Union
-
-import ansible_runner
-import dpath.util
-import janus
-import yaml
-
-if os.environ.get("RULES_ENGINE", "drools") == "drools":
-    from drools import ruleset as lang
-else:
-    from durable import lang
-
-from .collection import find_playbook, has_playbook, split_collection_name
-from .conf import settings
-from .exception import ShutdownException
-from .util import get_horizontal_rule
-
-logger = logging.getLogger(__name__)
-
-tar = shutil.which("tar")
-
-
-async def none(
-    event_log,
-    inventory: Dict,
-    hosts: List,
-    variables: Dict,
-    facts: Dict,
-    project_data_file: str,
-    source_ruleset_name: str,
-    source_rule_name: str,
-    ruleset: str,
-):
-    await event_log.put(
-        dict(
-            type="Action",
-            action="noop",
-            ruleset=source_ruleset_name,
-            rule=source_rule_name,
-            activation_id=settings.identifier,
-            run_at=str(datetime.utcnow()),
-        )
-    )
-
-
-async def debug(event_log, **kwargs):
-    print(get_horizontal_rule("="))
-    print("kwargs:")
-    pprint(kwargs)
-    print(get_horizontal_rule("="))
-    sys.stdout.flush()
-    await event_log.put(
-        dict(
-            type="Action",
-            action="debug",
-            playbook_name=kwargs.get("name"),
-            ruleset=kwargs.get("source_ruleset_name"),
-            rule=kwargs.get("source_rule_name"),
-            activation_id=settings.identifier,
-            run_at=str(datetime.utcnow()),
-        )
-    )
-
-
-async def print_event(
-    event_log,
-    inventory: Dict,
-    hosts: List,
-    variables: Dict,
-    facts: Dict,
-    project_data_file: str,
-    source_ruleset_name: str,
-    source_rule_name: str,
-    ruleset: str,
-    name: Optional[str] = None,
-    var_root: Union[str, Dict, None] = None,
-    pretty: Optional[str] = None,
-):
-    print_fn: Callable = print
-    if pretty:
-        print_fn = pprint
-
-    if var_root:
-        update_variables(variables, var_root)
-
-    var_name = "event"
-    if "events" in variables:
-        var_name = "events"
-
-    print_fn(variables[var_name])
-    sys.stdout.flush()
-    await event_log.put(
-        dict(
-            type="Action",
-            action="print_event",
-            activation_id=settings.identifier,
-            ruleset=source_ruleset_name,
-            rule=source_rule_name,
-            playbook_name=name,
-            run_at=str(datetime.utcnow()),
-        )
-    )
-
-
-async def set_fact(
-    event_log,
-    inventory: Dict,
-    hosts: List,
-    variables: Dict,
-    facts: Dict,
-    project_data_file: str,
-    source_ruleset_name: str,
-    source_rule_name: str,
-    ruleset: str,
-    fact: Dict,
-    name: Optional[str] = None,
-):
-    logger.debug("set_fact %s %s", ruleset, fact)
-    lang.assert_fact(ruleset, fact)
-    await event_log.put(
-        dict(
-            type="Action",
-            action="set_fact",
-            activation_id=settings.identifier,
-            ruleset=source_ruleset_name,
-            rule=source_rule_name,
-            playbook_name=name,
-            run_at=str(datetime.utcnow()),
-        )
-    )
-
-
-async def retract_fact(
-    event_log,
-    inventory: Dict,
-    hosts: List,
-    variables: Dict,
-    facts: Dict,
-    project_data_file: str,
-    source_ruleset_name: str,
-    source_rule_name: str,
-    ruleset: str,
-    fact: Dict,
-    name: Optional[str] = None,
-):
-    lang.retract_fact(ruleset, fact)
-    await event_log.put(
-        dict(
-            type="Action",
-            action="retract_fact",
-            ruleset=source_ruleset_name,
-            rule=source_rule_name,
-            activation_id=settings.identifier,
-            playbook_name=name,
-            run_at=str(datetime.utcnow()),
-        )
-    )
+from pprint import PrettyPrinter, pformat
+from types import MappingProxyType
+from typing import Dict, List, Optional, Union, cast
+
+import dpath
+from drools import ruleset as lang
+from drools.exceptions import (
+    MessageNotHandledException,
+    MessageObservedException,
+)
 
+from ansible_rulebook.builtin import actions as builtin_actions
+from ansible_rulebook.conf import settings
+from ansible_rulebook.exception import (
+    ShutdownException,
+    UnsupportedActionException,
+)
+from ansible_rulebook.messages import Shutdown
+from ansible_rulebook.rule_types import (
+    Action,
+    ActionContext,
+    EngineRuleSetQueuePlan,
+    ExecutionStrategy,
+)
+from ansible_rulebook.rules_parser import parse_hosts
+from ansible_rulebook.util import (
+    run_at,
+    send_session_stats,
+    substitute_variables,
+)
 
-async def post_event(
-    event_log,
-    inventory: Dict,
-    hosts: List,
-    variables: Dict,
-    facts: Dict,
-    project_data_file: str,
-    source_ruleset_name: str,
-    source_rule_name: str,
-    ruleset: str,
-    event: Dict,
-):
-    lang.post(ruleset, event)
-
-    await event_log.put(
-        dict(
-            type="Action",
-            action="post_event",
-            ruleset=source_ruleset_name,
-            rule=source_rule_name,
-            activation_id=settings.identifier,
-            run_at=str(datetime.utcnow()),
-        )
-    )
+logger = logging.getLogger(__name__)
 
 
-async def run_playbook(
-    event_log,
-    inventory: Dict,
-    hosts: List,
-    variables: Dict,
-    facts: Dict,
-    project_data_file: str,
-    source_ruleset_name: str,
-    source_rule_name: str,
-    ruleset: str,
-    name: str,
-    set_facts: Optional[bool] = None,
-    post_events: Optional[bool] = None,
-    verbosity: int = 0,
-    var_root: Union[str, Dict, None] = None,
-    copy_files: Optional[bool] = False,
-    json_mode: Optional[bool] = False,
-    retries: Optional[int] = 0,
-    retry: Optional[bool] = False,
-    delay: Optional[int] = 0,
-    **kwargs,
-):
-
-    logger.info("running Ansible playbook: %s", name)
-    temp, playbook_name = await pre_process_runner(
-        event_log,
-        inventory,
+class RuleSetRunner:
+    def __init__(
+        self,
+        event_log: asyncio.Queue,
+        ruleset_queue_plan: EngineRuleSetQueuePlan,
+        hosts_facts,
         variables,
-        facts,
-        name,
-        "run_playbook",
-        var_root,
-        copy_files,
-        True,
-        project_data_file,
-        **kwargs,
-    )
-
-    job_id = str(uuid.uuid4())
-
-    logger.info(f"ruleset: {source_ruleset_name}, rule: {source_rule_name}")
-    await event_log.put(
-        dict(
-            type="Job",
-            job_id=job_id,
-            ansible_rulebook_id=settings.identifier,
-            name=playbook_name,
-            ruleset=source_ruleset_name,
-            rule=source_rule_name,
-            hosts=",".join(hosts),
-            action="run_playbook",
-        )
-    )
-
-    logger.info("Calling Ansible runner")
+        rule_set,
+        project_data_file: Optional[str] = None,
+        parsed_args=None,
+        broadcast_method=None,
+    ):
+        self.action_loop_task = None
+        self.event_log = event_log
+        self.ruleset_queue_plan = ruleset_queue_plan
+        self.name = ruleset_queue_plan.ruleset.name
+        self.rule_set = rule_set
+        self.hosts_facts = hosts_facts
+        self.variables = variables
+        self.project_data_file = project_data_file
+        self.parsed_args = parsed_args
+        self.shutdown = None
+        self.active_actions = set()
+        self.broadcast_method = broadcast_method
+        self.event_counter = 0
 
-    if retry:
-        retries = max(retries, 1)
-    for i in range(retries + 1):
-        if i > 0:
-            if delay > 0:
-                await asyncio.sleep(delay)
-            logger.info(
-                "Previous run_playbook failed. Retry %d of %d", i, retries
+    async def run_ruleset(self):
+        tasks = []
+        try:
+            prime_facts(self.name, self.hosts_facts)
+            task_name = (
+                f"action_plan_task:: {self.ruleset_queue_plan.ruleset.name}"
+            )
+            self.action_loop_task = asyncio.create_task(
+                self._drain_actionplan_queue(), name=task_name
+            )
+            tasks.append(self.action_loop_task)
+            task_name = (
+                f"source_reader_task:: {self.ruleset_queue_plan.ruleset.name}"
             )
+            self.source_loop_task = asyncio.create_task(
+                self._drain_source_queue(), name=task_name
+            )
+            tasks.append(self.source_loop_task)
+            await asyncio.wait([self.action_loop_task])
+        except asyncio.CancelledError:
+            logger.debug("Cancelled error caught in run_ruleset")
+            for task in tasks:
+                if not task.done():
+                    logger.debug("Cancelling (2) task %s", task.get_name())
+                    task.cancel()
 
-        run_at = str(datetime.utcnow())
-        await call_runner(
-            event_log,
-            job_id,
-            temp,
-            dict(playbook=playbook_name),
-            hosts,
-            verbosity,
-            json_mode,
-        )
-        if get_status(temp) != "failed":
-            break
+        try:
+            await asyncio.gather(*tasks, return_exceptions=True)
+        except asyncio.CancelledError:
+            raise
+
+    async def _cleanup(self):
+        logger.info("Cleaning up ruleset %s", self.name)
+        if not self.source_loop_task.done():
+            self.source_loop_task.cancel()
+
+        if (
+            self.active_actions
+            and self.shutdown
+            and self.shutdown.kind == "graceful"
+        ):
+            logger.info("Waiting for active actions to end")
+            await asyncio.wait(
+                self.active_actions,
+                return_when=asyncio.FIRST_EXCEPTION,
+                timeout=self.shutdown.delay,
+            )
 
-    return await post_process_runner(
-        event_log,
-        temp,
-        ruleset,
-        settings.identifier,
-        name,
-        "run_playbook",
-        job_id,
-        run_at,
-        set_facts,
-        post_events,
-    )
-
-
-async def run_module(
-    event_log,
-    inventory: Dict,
-    hosts: List,
-    variables: Dict,
-    facts: Dict,
-    project_data_file: str,
-    source_ruleset_name: str,
-    source_rule_name: str,
-    ruleset: str,
-    name: str,
-    set_facts: Optional[bool] = None,
-    post_events: Optional[bool] = None,
-    verbosity: int = 0,
-    var_root: Union[str, Dict, None] = None,
-    copy_files: Optional[bool] = False,
-    json_mode: Optional[bool] = False,
-    module_args: Union[Dict, None] = None,
-    retries: Optional[int] = 0,
-    retry: Optional[bool] = False,
-    delay: Optional[int] = 0,
-    **kwargs,
-):
-
-    temp, module_name = await pre_process_runner(
-        event_log,
-        inventory,
-        variables,
-        facts,
-        name,
-        "run_module",
-        var_root,
-        copy_files,
-        False,
-        project_data_file,
-        **kwargs,
-    )
-    job_id = str(uuid.uuid4())
-
-    await event_log.put(
-        dict(
-            type="Job",
-            job_id=job_id,
-            ansible_rulebook_id=settings.identifier,
-            name=module_name,
-            ruleset=source_ruleset_name,
-            rule=source_rule_name,
-            hosts=",".join(hosts),
-            action="run_module",
+        for task in self.active_actions:
+            logger.debug("Cancelling active task %s", task.get_name())
+            task.cancel()
+        if self.shutdown:
+            await self.event_log.put(
+                dict(
+                    type="Shutdown",
+                    message=self.shutdown.message,
+                    delay=self.shutdown.delay,
+                    source_plugin=self.shutdown.source_plugin,
+                    kind=self.shutdown.kind,
+                )
+            )
+        stats = lang.end_session(self.name)
+        if self.parsed_args and self.parsed_args.heartbeat > 0:
+            await send_session_stats(self.event_log, stats)
+        logger.info(pformat(stats))
+
+    async def _handle_shutdown(self):
+        logger.info(
+            "Ruleset: %s, received shutdown: %s",
+            self.name,
+            str(self.shutdown),
         )
-    )
-
-    logger.info("Calling Ansible runner")
-    module_args_str = ""
-    if module_args:
-        for k, v in module_args.items():
-            if len(module_args_str) > 0:
-                module_args_str += " "
-            module_args_str += f'{k}="{v}"'
-
-    if retry:
-        retries = max(retries, 1)
-    for i in range(retries + 1):
-        if i > 0:
-            if delay > 0:
-                await asyncio.sleep(delay)
+        if self.shutdown.kind == "now":
             logger.info(
-                "Previous run_module failed. Retry %d of %d", i, retries
+                "ruleset: %s has issued an immediate shutdown", self.name
             )
-        run_at = str(datetime.utcnow())
-        await call_runner(
-            event_log,
-            job_id,
-            temp,
-            dict(
-                module=module_name,
-                host_pattern=",".join(hosts),
-                module_args=module_args_str,
-            ),
-            hosts,
-            verbosity,
-            json_mode,
-        )
-        if get_status(temp) != "failed":
-            break
+            self.action_loop_task.cancel()
+        elif (
+            self.ruleset_queue_plan.plan.queue.empty()
+            and not self.active_actions
+        ):
+            logger.info("ruleset: %s shutdown no pending work", self.name)
+            self.action_loop_task.cancel()
+        else:
+            logger.info(
+                "ruleset: %s waiting %f for shutdown",
+                self.name,
+                self.shutdown.delay,
+            )
+            await asyncio.sleep(self.shutdown.delay)
+            if not self.action_loop_task.done():
+                self.action_loop_task.cancel()
+
+        return
 
-    return await post_process_runner(
-        event_log,
-        temp,
-        ruleset,
-        settings.identifier,
-        name,
-        "run_module",
-        job_id,
-        run_at,
-        set_facts,
-        post_events,
-    )
-
-
-async def call_runner(
-    event_log,
-    job_id: str,
-    private_data_dir: str,
-    runner_args: Dict,
-    hosts: List,
-    verbosity: int = 0,
-    json_mode: Optional[bool] = False,
-):
-
-    host_limit = ",".join(hosts)
-
-    loop = asyncio.get_running_loop()
-
-    queue = janus.Queue()
-
-    # The event_callback is called from the ansible-runner thread
-    # It needs a thread-safe synchronous queue.
-    # Janus provides a sync queue connected to an async queue
-    # Here we push the event into the sync side of janus
-    def event_callback(event, *args, **kwargs):
-        event["job_id"] = job_id
-        event["ansible_rulebook_id"] = settings.identifier
-        queue.sync_q.put(dict(type="AnsibleEvent", event=event))
-
-    # Here we read the async side and push it into the event queue
-    # which is also async.
-    # We do this until cancelled at the end of the ansible runner call.
-    # We might need to drain the queue here before ending.
-    async def read_queue():
+    async def _drain_source_queue(self):
+        logger.info("Waiting for events, ruleset: %s", self.name)
         try:
             while True:
-                val = await queue.async_q.get()
-                event_data = val.get("event", {})
-                val["run_at"] = event_data.get("created")
-                await event_log.put(val)
-        except CancelledError:
-            pass
-
-    tasks = []
+                data = await self.ruleset_queue_plan.source_queue.get()
+                if self.parsed_args and self.parsed_args.print_events:
+                    PrettyPrinter(indent=4).pprint(data)
 
-    tasks.append(asyncio.create_task(read_queue()))
+                logger.debug(
+                    "Ruleset: %s, received event: %s ", self.name, str(data)
+                )
+                if isinstance(data, Shutdown):
+                    self.shutdown = data
+                    return await self._handle_shutdown()
+
+                if not data:
+                    # TODO: is it really necessary to add such event
+                    # to event_log?
+                    await self.event_log.put(dict(type="EmptyEvent"))
+                    continue
+
+                try:
+                    logger.debug(
+                        "Posting data to ruleset %s => %s",
+                        self.name,
+                        str(data),
+                    )
+                    lang.post(self.name, data)
+                except MessageObservedException:
+                    logger.debug("MessageObservedException: %s", data)
+                except MessageNotHandledException:
+                    logger.debug("MessageNotHandledException: %s", data)
+                except BaseException as e:
+                    logger.error(e)
+                finally:
+                    logger.debug(lang.get_pending_events(self.name))
+                    if (
+                        settings.gc_after
+                        and self.event_counter > settings.gc_after
+                    ):
+                        self.event_counter = 0
+                        gc.collect()
+                    else:
+                        self.event_counter += 1
+                    while self.ruleset_queue_plan.plan.queue.qsize() > 10:
+                        await asyncio.sleep(0)
+        except asyncio.CancelledError:
+            logger.debug("Source Task Cancelled for ruleset %s", self.name)
+            raise
+
+    def _handle_action_completion(self, task):
+        self.active_actions.discard(task)
+        logger.info(
+            "Task %s finished, active actions %d",
+            task.get_name(),
+            len(self.active_actions),
+        )
+        if (
+            self.ruleset_queue_plan.plan.queue.empty()
+            and self.shutdown
+            and len(self.active_actions) == 0
+        ):
+            logger.info("All actions done")
+            if not self.action_loop_task.done():
+                self.action_loop_task.cancel()
 
-    with concurrent.futures.ThreadPoolExecutor(max_workers=1) as task_pool:
-        await loop.run_in_executor(
-            task_pool,
-            partial(
-                ansible_runner.run,
-                private_data_dir=private_data_dir,
-                limit=host_limit,
-                verbosity=verbosity,
-                event_handler=event_callback,
-                json_mode=json_mode,
-                **runner_args,
+    async def _drain_actionplan_queue(self):
+        logger.info("Waiting for actions on events from %s", self.name)
+        try:
+            while True:
+                queue_item = await self.ruleset_queue_plan.plan.queue.get()
+                rule_run_at = run_at()
+                action_item = cast(ActionContext, queue_item)
+                if len(action_item.actions) > 1:
+                    task = asyncio.create_task(
+                        self._run_multiple_actions(action_item, rule_run_at)
+                    )
+                    self.active_actions.add(task)
+                    task.add_done_callback(self._handle_action_completion)
+                else:
+                    task = self._run_action(
+                        action_item.actions[0], action_item, rule_run_at
+                    )
+
+                if (
+                    self.rule_set.execution_strategy
+                    == ExecutionStrategy.SEQUENTIAL
+                ):
+                    await task
+        except asyncio.CancelledError:
+            logger.debug(
+                "Action Plan Task Cancelled for ruleset %s", self.name
+            )
+            raise
+        except BaseException as e:
+            logger.error(e)
+            raise
+        finally:
+            await self._cleanup()
+
+    async def _run_multiple_actions(
+        self, action_item: ActionContext, rule_run_at: str
+    ) -> None:
+        for action in action_item.actions:
+            await self._run_action(action, action_item, rule_run_at)
+
+    def _run_action(
+        self, action: Action, action_item: ActionContext, rule_run_at: str
+    ) -> asyncio.Task:
+        task_name = (
+            f"action::{action.action}::"
+            f"{self.ruleset_queue_plan.ruleset.name}::"
+            f"{action_item.rule}"
+        )
+        logger.debug("Creating action task %s", task_name)
+        task = asyncio.create_task(
+            self._call_action(
+                action_item.ruleset,
+                action_item.ruleset_uuid,
+                action_item.rule,
+                action_item.rule_uuid,
+                rule_run_at,
+                action.action,
+                MappingProxyType(action.action_args),
+                action_item.variables,
+                action_item.inventory,
+                action_item.hosts,
+                action_item.rule_engine_results,
             ),
+            name=task_name,
         )
-
-    # Cancel the queue reading task
-    for task in tasks:
-        task.cancel()
-    await asyncio.gather(*tasks)
-
-
-async def untar_project(output_dir, project_data_file):
-
-    cmd = [tar, "zxvf", project_data_file]
-    proc = await asyncio.create_subprocess_exec(
-        *cmd,
-        cwd=output_dir,
-        stdout=asyncio.subprocess.PIPE,
-        stderr=asyncio.subprocess.PIPE,
-    )
-
-    stdout, stderr = await proc.communicate()
-
-    if stdout:
-        logger.debug(stdout.decode())
-    if stderr:
-        logger.debug(stderr.decode())
-
-
-async def pre_process_runner(
-    event_log,
-    inventory: Dict,
-    variables: Dict,
-    facts: Dict,
-    name: str,
-    action: str,
-    var_root: Union[str, Dict, None] = None,
-    copy_files: Optional[bool] = False,
-    check_files: Optional[bool] = True,
-    project_data_file: Optional[str] = None,
-    **kwargs,
-):
-
-    private_data_dir = tempfile.mkdtemp(prefix=action)
-    logger.debug("private data dir %s", private_data_dir)
-    logger.debug("variables %s", variables)
-    logger.debug("facts %s", facts)
-
-    variables["facts"] = facts
-    for k, v in kwargs.items():
-        variables[k] = v
-
-    if var_root:
-        update_variables(variables, var_root)
-
-    env_dir = os.path.join(private_data_dir, "env")
-    inventory_dir = os.path.join(private_data_dir, "inventory")
-    project_dir = os.path.join(private_data_dir, "project")
-
-    playbook_name = name
-
-    os.mkdir(env_dir)
-    with open(os.path.join(env_dir, "extravars"), "w") as f:
-        f.write(yaml.dump(variables))
-    os.mkdir(inventory_dir)
-    with open(os.path.join(inventory_dir, "hosts"), "w") as f:
-        f.write(yaml.dump(inventory))
-    os.mkdir(project_dir)
-
-    logger.debug("project_data_file: %s", project_data_file)
-    if project_data_file:
-        if os.path.exists(project_data_file):
-            await untar_project(project_dir, project_data_file)
-            return (private_data_dir, playbook_name)
-
-    if check_files:
-        if os.path.exists(name):
-            playbook_name = os.path.basename(name)
-            shutil.copy(name, os.path.join(project_dir, playbook_name))
-            if copy_files:
-                shutil.copytree(
-                    os.path.dirname(os.path.abspath(name)),
-                    project_dir,
-                    dirs_exist_ok=True,
+        self.active_actions.add(task)
+        task.add_done_callback(self._handle_action_completion)
+        return task
+
+    async def _call_action(
+        self,
+        ruleset: str,
+        ruleset_uuid: str,
+        rule: str,
+        rule_uuid: str,
+        rule_run_at: str,
+        action: str,
+        immutable_action_args: MappingProxyType,
+        variables: Dict,
+        inventory: str,
+        hosts: List,
+        rules_engine_result,
+    ) -> None:
+        logger.info("call_action %s", action)
+        action_args = immutable_action_args.copy()
+
+        error = None
+        if action in builtin_actions:
+            try:
+                if action == "run_job_template":
+                    limit = dpath.get(
+                        action_args,
+                        "job_args.limit",
+                        separator=".",
+                        default=None,
+                    )
+                    if isinstance(limit, list):
+                        hosts = limit
+                    elif isinstance(limit, str):
+                        hosts = [limit]
+                elif action == "shutdown":
+                    if self.parsed_args and "delay" not in action_args:
+                        action_args["delay"] = self.parsed_args.shutdown_delay
+
+                single_match = None
+                keys = list(rules_engine_result.data.keys())
+                if len(keys) == 0:
+                    single_match = {}
+                elif len(keys) == 1 and keys[0] == "m":
+                    single_match = rules_engine_result.data[keys[0]]
+                else:
+                    multi_match = rules_engine_result.data
+                variables_copy = variables.copy()
+                if single_match is not None:
+                    variables_copy["event"] = single_match
+                    event = single_match
+                    if "meta" in event:
+                        if "hosts" in event["meta"]:
+                            hosts = parse_hosts(event["meta"]["hosts"])
+                else:
+                    variables_copy["events"] = multi_match
+                    new_hosts = []
+                    for event in variables_copy["events"].values():
+                        if "meta" in event:
+                            if "hosts" in event["meta"]:
+                                new_hosts.extend(
+                                    parse_hosts(event["meta"]["hosts"])
+                                )
+                    if new_hosts:
+                        hosts = new_hosts
+
+                if "var_root" in action_args:
+                    var_root = action_args.pop("var_root")
+                    logger.info(
+                        "Update variables [%s] with new root [%s]",
+                        variables_copy,
+                        var_root,
+                    )
+                    _update_variables(variables_copy, var_root)
+
+                logger.info(
+                    "substitute_variables [%s] [%s]",
+                    action_args,
+                    variables_copy,
                 )
-        elif has_playbook(*split_collection_name(name)):
-            playbook_name = name
-            shutil.copy(
-                find_playbook(*split_collection_name(name)),
-                os.path.join(project_dir, name),
-            )
+                action_args = {
+                    k: substitute_variables(v, variables_copy)
+                    for k, v in action_args.items()
+                }
+                logger.info("action args: %s", action_args)
+
+                if "ruleset" not in action_args:
+                    action_args["ruleset"] = ruleset
+
+                await builtin_actions[action](
+                    event_log=self.event_log,
+                    inventory=inventory,
+                    hosts=hosts,
+                    variables=variables_copy,
+                    project_data_file=self.project_data_file,
+                    source_ruleset_name=ruleset,
+                    source_ruleset_uuid=ruleset_uuid,
+                    source_rule_name=rule,
+                    source_rule_uuid=rule_uuid,
+                    rule_run_at=rule_run_at,
+                    **action_args,
+                )
+            except KeyError as e:
+                logger.error(
+                    "KeyError %s with variables %s",
+                    str(e),
+                    pformat(variables_copy),
+                )
+                error = e
+            except MessageNotHandledException as e:
+                logger.error(
+                    "Message cannot be handled: %s err %s", action_args, str(e)
+                )
+                error = e
+            except MessageObservedException as e:
+                logger.info("MessageObservedException: %s", action_args)
+                error = e
+            except ShutdownException as e:
+                if self.shutdown:
+                    logger.info(
+                        "A shutdown is already in progress, ignoring this one"
+                    )
+                else:
+                    await self.broadcast_method(e.shutdown)
+            except asyncio.CancelledError:
+                logger.debug("Action task caught Cancelled error")
+                raise
+            except Exception as e:
+                logger.error("Error calling action %s, err %s", action, str(e))
+                error = e
+            except BaseException as e:
+                logger.error(e)
+                raise
         else:
-            logger.error(
-                "Could not find a playbook for %s from %s", name, os.getcwd()
+            logger.error("Action %s not supported", action)
+            error = UnsupportedActionException(
+                f"Action {action} not supported"
             )
 
-    return (private_data_dir, playbook_name)
-
-
-async def post_process_runner(
-    event_log,
-    private_data_dir: str,
-    ruleset: str,
-    activation_id: str,
-    name: str,
-    action: str,
-    job_id: str,
-    run_at: str,
-    set_facts: Optional[bool] = None,
-    post_events: Optional[bool] = None,
-):
-
-    for rc_file in glob.glob(
-        os.path.join(private_data_dir, "artifacts", "*", "rc")
-    ):
-        with open(rc_file, "r") as f:
-            rc = int(f.read())
-
-    status = get_status(private_data_dir)
-
-    result = dict(
-        type="Action",
-        action=action,
-        activation_id=activation_id,
-        playbook_name=name,
-        job_id=job_id,
-        ruleset=ruleset,
-        rc=rc,
-        status=status,
-        run_at=run_at,
-    )
-    await event_log.put(result)
-
-    if set_facts or post_events:
-        logger.debug("set_facts")
-        for host_facts in glob.glob(
-            os.path.join(private_data_dir, "artifacts", "*", "fact_cache", "*")
-        ):
-            with open(host_facts) as f:
-                fact = json.loads(f.read())
-            logger.debug("fact %s", fact)
-            if set_facts:
-                lang.assert_fact(ruleset, fact)
-            if post_events:
-                lang.post(ruleset, fact)
-
-    return result
-
-
-async def shutdown(
-    event_log,
-    inventory: Dict,
-    hosts: List,
-    variables: Dict,
-    facts: Dict,
-    project_data_file: str,
-    source_ruleset_name: str,
-    source_rule_name: str,
-    ruleset: str,
-):
-    await event_log.put(
-        dict(
-            type="Action",
-            action="shutdown",
-            activation_id=settings.identifier,
-            ruleset=source_ruleset_name,
-            rule=source_rule_name,
-            run_at=str(datetime.utcnow()),
-        )
-    )
-    raise ShutdownException()
+        if error:
+            await self.event_log.put(
+                dict(
+                    type="Action",
+                    action=action,
+                    action_uuid=str(uuid.uuid4()),
+                    activation_id=settings.identifier,
+                    playbook_name=action_args.get("name"),
+                    status="failed",
+                    run_at=run_at(),
+                    reason=dict(error=str(error)),
+                    rule=rule,
+                    ruleset=ruleset,
+                    rule_uuid=rule_uuid,
+                    ruleset_uuid=ruleset_uuid,
+                )
+            )
 
 
-actions: Dict[str, Callable] = dict(
-    none=none,
-    debug=debug,
-    print_event=print_event,
-    set_fact=set_fact,
-    retract_fact=retract_fact,
-    post_event=post_event,
-    run_playbook=run_playbook,
-    run_module=run_module,
-    shutdown=shutdown,
-)
+def prime_facts(name: str, hosts_facts: List[Dict]):
+    for data in hosts_facts:
+        try:
+            lang.assert_fact(name, data)
+        except MessageNotHandledException:
+            pass
 
 
-def update_variables(variables: Dict, var_root: Union[str, Dict]):
+def _update_variables(variables: Dict, var_root: Union[str, Dict]):
     var_roots = {var_root: var_root} if isinstance(var_root, str) else var_root
     if "event" in variables:
         for key, _new_key in var_roots.items():
-            new_value = dpath.util.get(
+            new_value = dpath.get(
                 variables["event"], key, separator=".", default=None
             )
             if new_value:
                 variables["event"] = new_value
                 break
     elif "events" in variables:
         for _k, v in variables["events"].items():
             for old_key, new_key in var_roots.items():
-                new_value = dpath.util.get(
-                    v, old_key, separator=".", default=None
-                )
+                new_value = dpath.get(v, old_key, separator=".", default=None)
                 if new_value:
                     variables["events"][new_key] = new_value
                     break
-
-
-def get_status(private_data_dir: str):
-    status_files = glob.glob(
-        os.path.join(private_data_dir, "artifacts", "*", "status")
-    )
-    status_files.sort(key=os.path.getmtime, reverse=True)
-    with open(status_files[0], "r") as f:
-        status = f.read()
-    return status
```

### Comparing `ansible_rulebook-0.9.4/ansible_rulebook.egg-info/PKG-INFO` & `ansible_rulebook-1.0.0/docs/sources.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,195 +1,175 @@
-Metadata-Version: 2.1
-Name: ansible-rulebook
-Version: 0.9.4
-Summary: Event driven automation for Ansible
-Home-page: https://github.com/ansible/ansible-rulebook
-License: Apache-2.0
-Keywords: ansible_rulebook
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst; charset=UTF-8
-License-File: LICENSE
+.. _event-source-plugins:
 
-================
-ansible-rulebook
-================
+====================
+Event Source Plugins
+====================
 
+Events come from event sources. Event driven automation supports many event
+sources using a plugin system. Event source plugins can be stored locally but
+are preferably distributed via collections.
 
-.. image:: https://img.shields.io/pypi/v/ansible_rulebook.svg
-        :target: https://pypi.python.org/pypi/ansible_rulebook
+`Ansible.eda <https://github.com/ansible/event-driven-ansible>`_
+is the collection that includes our initial set of event source plugins.
+These include:
 
-.. image:: https://img.shields.io/travis/ansible/ansible_rulebook.svg
-        :target: https://travis-ci.com/ansible/ansible_rulebook
+..
+    TODO: Add extended documentation for plugins in the collection and link to it here.
 
-.. image:: https://readthedocs.org/projects/ansible-rulebook/badge/?version=latest
-        :target: https://ansible-rulebook.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
+* alertmanager
+    Receive events via a webhook from alertmanager
 
-* Free software: Apache Software License 2.0
-* Documentation: https://ansible-rulebook.readthedocs.io.
+* azure_service_bus
+    Receive events from an Azure service
 
+* kafka
+    Receive events via a kafka topic
 
-Event driven automation for Ansible.
+* url_check
+    Poll a set of URLs and send events with their statuses
 
+* watchdog
+    Watch file system and send events when a file status changes
 
-The real world is full of events that change the state of our software and systems.
-Our automation needs to be able to react to those events. Introducing *ansible-rulebook*; a command
-line tool that allows you to recognize events that you care about and react accordingly
-by running a playbook or other actions.
+* webhook
+    Provide a webhook and receive events from it
 
-============
-Installation
-============
+* tick
+    Generate events with an increasing index i that never ends
+    Mainly used for development and testing
 
-Head over to the `Installation`_ page for details on how to install *ansible-rulebook*. Once installed,
-continue with the **Getting started** section below to begin writing your first rulesets.
+* file
+    Load facts from YAML files initially and reload when any file changes
+    Mainly used for development and testing
 
-.. _Installation: docs/installation.rst
+* range
+    Generate events with an increasing index i within a range
+    Mainly used for development and testing
 
-===============
-Getting started
-===============
 
-**Important:** Running *ansible-rulebook* requires setting the *JAVA_HOME* environment variable. On Fedora-like systems, this will be::
+How to Develop a Custom Plugin
+------------------------------
+You can build your own event source plugin in python. A plugin is a single
+python file. You can start with this example:
 
-    $ export JAVA_HOME=/usr/lib/jvm/java-17-openjdk
+Plugin template
+^^^^^^^^^^^^^^^
 
-Let's get started with a simple hello world example to familiarize ourselves with the concepts::
+.. code-block:: python
 
-    ---
-    - name: Hello Events
-      hosts: localhost
-      sources:
-        - ansible.eda.range:
-            limit: 5
-      rules:
-        - name: Say Hello
-          condition: event.i == 1
-          action:
-            run_playbook:
-              name: ansible.eda.hello
-    ...
+  """
+  template.py
 
+  An ansible-rulebook event source plugin template.
 
-Events come from a **event source** and then are checked against **rules** to determine if an **action** should
-be taken.  If the **condition** of a rule matches the event it will run the action for that rule.
+  Arguments:
+    - delay: seconds to wait between events
 
-In this example the event source is the Python range function.  It produces events that count from
-:code:`i=0` to :code:`i=<limit>`.
+  Examples:
+    sources:
+      - template:
+          delay: 1
 
-When :code:`i` is equal to 1 the condition for the the :code:`Say Hello` rule matches and it runs a playbook.
+  """
+  import asyncio
+  from typing import Any, Dict
 
 
-Normally events would come from monitoring and alerting systems or other software. The following
-is a more complete example that accepts alerts from Alertmanager::
+  async def main(queue: asyncio.Queue, args: Dict[str, Any]):
+      delay = args.get("delay", 0)
 
-    ---
-    - name: Automatic Remediation of a webserver
-      hosts: all
-      sources:
-        - name: listen for alerts
-          ansible.eda.alertmanager:
-            host: 0.0.0.0
-            port: 8000
-      rules:
-        - name: restart web server
-          condition: event.alert.labels.job == "fastapi" and event.alert.status == "firing"
-          action:
-            run_playbook:
-              name: ansible.eda.start_app
-    ...
+      while True:
+          await queue.put(dict(template=dict(msg="hello world")))
+          await asyncio.sleep(delay)
 
 
-This example sets up a webhook to receive events from alertmanager and then matches events
-where the `fastapi` job alert has a staus of `firing`.  This runs a playbook that will
-remediate the issue.
+  if __name__ == "__main__":
 
+      class MockQueue:
+          async def put(self, event):
+              print(event)
 
+      mock_arguments = dict()
+      asyncio.run(main(MockQueue(), mock_arguments))
 
-Features
---------
 
-* Connect to event streams and handle events in near real time.
-* Conditionally launch playbooks based on rules that match events in event streams.
-* Store facts about the world from data in events
-* Limit the hosts where playbooks run based on event data
-* Run smaller jobs that run more quickly by limiting the hosts where playbooks run based on event data
+Plugin entrypoint
+^^^^^^^^^^^^^^^^^
+The plugin python file must contain an entrypoint function exactly like the
+following:
 
+.. code-block:: python
 
+  async def main(queue: asyncio.Queue, args: Dict[str, Any]):
 
-Examples
---------
+It is an async function. The first argument is an asyncio queue that will be
+consumed by ansible-rulebook CLI. The rest arguments are custom defined. They
+must match the arguments in the source section of the rulebook. For example
+the template plugin expects a single argument ``delay``. In the rulebook the
+source section looks like:
 
-Rules are organized into rulesets using a syntax that is similar to ansible-playbooks::
+.. code-block:: yaml
 
-    ---
-    - name: Hello Events
-      hosts: localhost
-      sources:
-        - ansible.eda.range:
-            limit: 5
-      rules:
-        - name: Say Hello
-          condition: event.i == 1
-          action:
-            run_playbook:
-              name: ansible.eda.hello
-    ...
+  - name: example
+    hosts: all
+    sources:
+      - template:
+          delay: 5
 
-Each ruleset defines: a set of hosts to pass to the playbook, a set of event sources,
-and a set of rules.   The set of hosts is the normal hosts pattern from ansible playbooks.
-The event sources are a new type of plugin that subscribe to events from event streams.
-The rules have conditions that match values in the events and actions that can run playbooks,
-assert facts, retract facts, and print information to the console.
+Each source must contain a key which is the name of the plugin. Its nested keys
+must match argument names expected by the main function. The name of the plugin
+is the python filename. If the plugin is from a collection then the plugin name
+is a FQCN which is the collection name concatenating with the python filename
+with a period delimit, for example ``ansible.eda.range``.
 
+In the main function you can implement code that connects to an external source
+of events, retrieves events and puts them onto the provided asyncio queue. The
+event data put on the queue must be a dictionary. You can insert the ``meta``
+key that points to another dictionary that holds a list of hosts. These hosts
+will limit where the ansible playbook can run. A simple example looks like
+``{"i": 2, "meta": {hosts: "localhost"}}``. ``hosts`` can be a comma delimited
+string or a list of host names.
 
-Let's look closer at the event source::
+As the plugin have full access to an unbounded queue that is consumed by ansible-rulebbok
+we carefully recommend to use always the method ``asyncio.Queue.put`` to put events as it's a non-blocking call.
+To give free cpu cycles to the event loop to process the events, we recommend to use ``asyncio.sleep(0)``
+inmediately after the ``put`` method.
 
-        - ansible.eda.range:
-            limit: 5
+.. note::
+    ansible-rulebook is intended to be a long running process and react to events over the time.
+    If the ``main`` function of **any of the sources** exits then the ansible-rulebook process will be terminated.
+    Usually you may want to implement a loop that keeps running and waits for events endlessly.
 
-This section of YAML defines that an event source plugin from the ansible.eda should
-be loaded and given the arguments: limit=5.  This source will generate a range of numbers
-from zero to 4 and then exit.
+.. note::
+    The rulebook can contain it's own logic to finish the process through the ``shutdown`` action.
+    If your plugin needs to perform some cleanup before the process is terminated, you must catch the ``asyncio.CancelledError`` exception.
 
-The rules YAML structure looks like the following::
 
-        - name: Say Hello
-          condition: event.i == 1
-          action:
-            run_playbook:
-              name: ansible.eda.hello
+Distributing plugins
+^^^^^^^^^^^^^^^^^^^^
 
+For local tests the plugin source file can be saved under a folder specified by
+the ``-S`` argument in the ansible-rulebook CLI. The recommended method for
+distributing and installing the plugin is through a collection. In this case
+the plugin source file should be placed under ``plugins/event_source`` folder
+and referred to by FQCN. The following rulebook example illustrates how to
+refer to the range plugin provided by ``ansible.eda`` collection:
 
-This block of YAML defines a rule with name "Say Hello", a condition that matches
-when an event has an value "i" that is equal to 1, and an action that runs a playbook
-inside the collection ansible.eda.
+.. code-block:: yaml
 
-For more information on usage and examples, please refer to the `Usage`_ guide.
+  - name: example2
+    hosts: localhost
+    sources:
+      - name: range
+        ansible.eda.range:
+          limit: 5
 
-.. _Usage: docs/usage.rst
+Any dependent packages needed by the custom plugin should be installed in the
+ansible-rulebook CLI env regardless the plugin is local or from a collection.
 
+Document plugins
+^^^^^^^^^^^^^^^^
 
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-
-=======
-History
-=======
-
-0.1.0 (2022-02-16)
-------------------
-
-* First release on PyPI.
+It is strongly recommended that you add comments at the top of the source file.
+Please describe the purpose of the event source plugin. List all required or
+optional arguments. Also add an example how to configure the plugin in a
+rulebook.
```

### Comparing `ansible_rulebook-0.9.4/docs/Makefile` & `ansible_rulebook-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/docs/conf.py` & `ansible_rulebook-1.0.0/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 #!/usr/bin/env python
+
+#  Copyright 2022 Red Hat, Inc.
 #
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
 # ansible_rulebook documentation build configuration file, created by
 # sphinx-quickstart on Fri Jun  9 13:47:02 2017.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
@@ -15,44 +29,49 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
+
+sys.path.insert(0, os.path.abspath(".."))
 
 import ansible_rulebook
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = [
+    'sphinx.ext.autodoc',
+    'sphinx.ext.viewcode',
+    'sphinx_ansible_theme',
+]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'ansible-rulebook'
-copyright = "2022, Ben Thomasson"
-author = "Ben Thomasson"
+project = "ansible-rulebook"
+copyright = f"2022-{datetime.datetime.today().year}, Red Hat, Inc"
+author = "Red Hat, Inc"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = ansible_rulebook.__version__
@@ -60,103 +79,121 @@
 release = ansible_rulebook.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = 'en'
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = 'sphinx_ansible_theme'
+html_title = "Ansible Rulebook Documentation"
+
+html_theme_options = {
+    'display_version': False,
+    'titles_only': False,
+    'documentation_home_url': 'https://ansible-rulebook.readthedocs.io/en/latest/',
+}
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+# html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'ansible_rulebookdoc'
+htmlhelp_basename = "ansible_rulebookdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'ansible_rulebook.tex',
-     'ansible-rulebook Documentation',
-     'Ben Thomasson', 'manual'),
+    (
+        master_doc,
+        "ansible_rulebook.tex",
+        "ansible-rulebook Documentation",
+        "Red Hat Ansible",
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'ansible_rulebook',
-     'ansible-rulebook Documentation',
-     [author], 1)
+    (
+        master_doc,
+        "ansible_rulebook",
+        "ansible-rulebook Documentation",
+        [author],
+        1,
+    )
 ]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'ansible_rulebook',
-     'ansible-rulebook Documentation',
-     author,
-     'ansible_rulebook',
-     'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "ansible_rulebook",
+        "ansible-rulebook Documentation",
+        author,
+        "ansible_rulebook",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 
+# Extra options
 
+# Text by default
+highlight_language = "text"
```

### Comparing `ansible_rulebook-0.9.4/docs/host_limit.rst` & `ansible_rulebook-1.0.0/docs/host_limit.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-========================
+==============
 Limiting hosts
-========================
+==============
 
 You can limit hosts to run a playbook through configuring the meta data in an event's data.
 The limiting hosts must be a subset of the hosts (inventory) selected in the rules file.
 
-Event data example::
+Event data example:
+
+.. code-block:: json
 
     {
         "i": 0,
         "meta": {"hosts": "localhost"}
     }
 
 The value for "hosts" can be a comma delimited string of multiple host names, but typically
 it is a single host. This is useful to restrict a remedy playbook to run only on the problematical host
-that emits a monitored event.
+that emits a monitored event. Be sure that the source plugin already sends this metadata.
```

### Comparing `ansible_rulebook-0.9.4/docs/make.bat` & `ansible_rulebook-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/setup.cfg` & `ansible_rulebook-1.0.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-[bumpversion]
-current_version = 0.9.4
-commit = True
-tag = True
-
 [metadata]
 name = ansible_rulebook
-version = 0.9.4
+version = 1.0.0
 description = Event driven automation for Ansible
 url = https://github.com/ansible/ansible-rulebook
 license = Apache-2.0
 keywords = ansible_rulebook
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	asyncio
-	durable_rules
+	aiohttp
 	pyparsing >= 3.0
 	jsonschema
 	jinja2
-	redis
-	dpath
+	dpath >= 2.1.4
 	janus
 	ansible-runner
 	websockets
-	drools_jpy
+	drools_jpy == 0.3.4
 
 [options.packages.find]
 include = 
 	ansible_rulebook
 	ansible_rulebook.*
 
 [options.entry_points]
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/01_noop.yml` & `ansible_rulebook-1.0.0/tests/asts/01_noop.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/03_print_event.yml` & `ansible_rulebook-1.0.0/tests/asts/03_print_event.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/04_set_fact.yml` & `ansible_rulebook-1.0.0/tests/asts/04_set_fact.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/05_post_event.yml` & `ansible_rulebook-1.0.0/tests/asts/05_post_event.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/06_retract_fact.yml` & `ansible_rulebook-1.0.0/tests/asts/06_retract_fact.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/07_and.yml` & `ansible_rulebook-1.0.0/tests/asts/07_and.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/08_or.yml` & `ansible_rulebook-1.0.0/tests/asts/08_or.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/09_gt.yml` & `ansible_rulebook-1.0.0/tests/asts/09_gt.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/10_lt.yml` & `ansible_rulebook-1.0.0/tests/asts/10_lt.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/11_le.yml` & `ansible_rulebook-1.0.0/tests/asts/11_le.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/12_ge.yml` & `ansible_rulebook-1.0.0/tests/asts/12_ge.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/13_add.yml` & `ansible_rulebook-1.0.0/tests/asts/13_add.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/14_sub.yml` & `ansible_rulebook-1.0.0/tests/asts/14_sub.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/15_multiple_events_all.yml` & `ansible_rulebook-1.0.0/tests/asts/15_multiple_events_all.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/16_multiple_events_any.yml` & `ansible_rulebook-1.0.0/tests/asts/16_multiple_events_any.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/17_multiple_sources_any.yml` & `ansible_rulebook-1.0.0/tests/asts/17_multiple_sources_any.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/18_multiple_sources_all.yml` & `ansible_rulebook-1.0.0/tests/asts/18_multiple_sources_all.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/19_is_defined.yml` & `ansible_rulebook-1.0.0/tests/asts/33_run_playbook_retry.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 - RuleSet:
     hosts:
     - all
-    name: 19 is defined
+    name: 33 run playbook and retry after an interval
     rules:
     - Rule:
         action:
           Action:
-            action: set_fact
+            action: run_playbook
             action_args:
-              fact:
-                msg: hello
+              delay: 1
+              name: playbooks/fail_and_succeed.yml
+              retry: true
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
                 Integer: 1
         enabled: true
         name: r1
-    - Rule:
-        action:
-          Action:
-            action: debug
-            action_args: {}
-        condition:
-          AllCondition:
-          - IsDefinedExpression:
-              Event: msg
-        enabled: true
-        name: r2
     sources:
     - EventSource:
         name: range
         source_args:
           limit: 5
         source_filters: []
         source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/20_is_not_defined.yml` & `ansible_rulebook-1.0.0/tests/asts/20_is_not_defined.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/21_run_playbook.yml` & `ansible_rulebook-1.0.0/tests/asts/21_run_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/23_nested_data.yml` & `ansible_rulebook-1.0.0/tests/asts/23_nested_data.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/24_max_attributes.yml` & `ansible_rulebook-1.0.0/tests/asts/24_max_attributes.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/25_max_attributes_nested.yml` & `ansible_rulebook-1.0.0/tests/asts/25_max_attributes_nested.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/26_print_events.yml` & `ansible_rulebook-1.0.0/tests/asts/26_print_events.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/27_var_root.yml` & `ansible_rulebook-1.0.0/tests/asts/27_var_root.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/28_right_side_condition_template.yml` & `ansible_rulebook-1.0.0/tests/asts/28_right_side_condition_template.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/29_run_module.yml` & `ansible_rulebook-1.0.0/tests/asts/29_run_module.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/30_run_module_missing.yml` & `ansible_rulebook-1.0.0/tests/asts/30_run_module_missing.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/31_run_module_missing_args.yml` & `ansible_rulebook-1.0.0/tests/asts/31_run_module_missing_args.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/32_run_module_fail.yml` & `ansible_rulebook-1.0.0/tests/asts/32_run_module_fail.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/33_run_playbook_retry.yml` & `ansible_rulebook-1.0.0/tests/asts/test_set_facts.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,54 @@
 - RuleSet:
     hosts:
     - all
-    name: 33 run playbook and retry after an interval
+    name: Test Assert Fact of different data types
     rules:
     - Rule:
-        action:
-          Action:
-            action: run_playbook
+        actions:
+        - Action:
+            action: set_fact
             action_args:
-              delay: 1
-              name: playbooks/fail_and_succeed.yml
-              retry: true
+              fact:
+                alpha: 1
+                beta:
+                  location: "{{ Naboo }}"
+                  name: R2D2
+                msg: hello world
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
                 Integer: 1
         enabled: true
         name: r1
+    - Rule:
+        actions:
+        - Action:
+            action: run_playbook
+            action_args:
+              copy_files: true
+              name: playbooks/validate_args_playbook.yml
+              extra_vars:
+                my_vars:
+                  event.alpha: 1
+                  event.beta.location: "{{ Naboo }}"
+                  event.beta.name: R2D2
+                  event.msg: hello world
+        condition:
+          AllCondition:
+          - EqualsExpression:
+              lhs:
+                Event: msg
+              rhs:
+                String: hello world
+        enabled: true
+        name: r2
     sources:
     - EventSource:
         name: range
         source_args:
           limit: 5
         source_filters: []
         source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/34_run_playbook_retries.yml` & `ansible_rulebook-1.0.0/tests/asts/34_run_playbook_retries.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/35_multiple_rulesets_1_fired.yml` & `ansible_rulebook-1.0.0/tests/asts/35_multiple_rulesets_1_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/36_multiple_rulesets_both_fired.yml` & `ansible_rulebook-1.0.0/tests/asts/36_multiple_rulesets_both_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/37_hosts_facts.yml` & `ansible_rulebook-1.0.0/tests/asts/37_hosts_facts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/38_shutdown.yml` & `ansible_rulebook-1.0.0/tests/asts/38_shutdown.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/asts/rules.yml` & `ansible_rulebook-1.0.0/tests/asts/rules.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 - RuleSet:
     hosts:
     - localhost
     name: Demo rules
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: slack
             action_args:
               color: good
               msg: 'Deployment success at {{event.payload.eventTime}}: {{management_url}}{{event.payload.applicationId}}'
               token: '{{token}}'
         condition:
           AllCondition:
@@ -17,16 +17,16 @@
               lhs:
                 Event: payload.provisioningState
               rhs:
                 String: Succeeded
         enabled: true
         name: send to slack3
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: slack
             action_args:
               color: warning
               msg: 'Deployment deleted at {{event.payload.eventTime}}: {{management_url}}{{event.payload.applicationId}}'
               token: '{{token}}'
         condition:
           AllCondition:
@@ -34,48 +34,48 @@
               lhs:
                 Event: payload.provisioningState
               rhs:
                 String: Deleted
         enabled: true
         name: send to slack4
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: slack
             action_args:
               msg: '{{event}}'
               token: '{{token}}'
         condition:
           AllCondition:
           - NotEqualsExpression:
               lhs:
                 Event: payload.eventType
               rhs:
                 String: GET
         enabled: true
         name: send to slack5
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: slack
             action_args:
               msg: '{{event}}'
               token: '{{token}}'
         condition:
           AllCondition:
           - NotEqualsExpression:
               lhs:
                 Event: payload.text
               rhs:
                 String: ''
         enabled: true
         name: send to slack6
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: set_fact
             action_args:
               fact:
                 received_greeting: true
               ruleset: Demo rules
         condition:
           AllCondition:
@@ -83,16 +83,16 @@
               lhs:
                 Event: payload.text
               rhs:
                 String: ''
         enabled: true
         name: assert fact
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: log
             action_args: {}
         condition:
           AllCondition:
           - NotEqualsExpression:
               lhs:
                 Event: payload.text
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/rules_with_assignment.yml` & `ansible_rulebook-1.0.0/tests/asts/rules_without_assignment.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 - RuleSet:
     hosts:
     - localhost
-    name: Demo rules with assignment
+    name: Demo rules multiple conditions all
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: debug
             action_args:
-              events_event: '{{events.first}}'
+              event: '{{event}}'
         condition:
           AllCondition:
-          - AssignmentExpression:
+          - EqualsExpression:
               lhs:
-                Events: first
+                Fact: i
               rhs:
-                EqualsExpression:
-                  lhs:
-                    Event: i
-                  rhs:
-                    Integer: 0
+                Integer: 0
         enabled: true
         name: assignment
     sources:
     - EventSource:
         name: range
         source_args:
           limit: 5
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/rules_with_assignment2.yml` & `ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions2.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 - RuleSet:
     hosts:
     - localhost
-    name: Demo rules with assignment2
+    name: Demo rules multiple conditions all
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: debug
-            action_args:
-              events_event: '{{events.first}}'
+            action_args: {}
         condition:
           AllCondition:
           - AssignmentExpression:
               lhs:
-                Facts: first
+                Events: first
               rhs:
                 EqualsExpression:
                   lhs:
-                    Fact: i
+                    Event: i
                   rhs:
                     Integer: 0
+          - AssignmentExpression:
+              lhs:
+                Events: second
+              rhs:
+                EqualsExpression:
+                  lhs:
+                    Event: i
+                  rhs:
+                    Integer: 1
         enabled: true
-        name: assignment
+        name: multiple conditions
     sources:
     - EventSource:
         name: range
         source_args:
           limit: 5
         source_filters: []
         source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions.yml` & `ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 - RuleSet:
     hosts:
     - localhost
     name: Demo rules multiple conditions any
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: debug
             action_args: {}
         condition:
           AnyCondition:
           - AssignmentExpression:
               lhs:
                 Events: event
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions2.yml` & `ansible_rulebook-1.0.0/tests/asts/rules_with_vars.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 - RuleSet:
     hosts:
     - localhost
-    name: Demo rules multiple conditions all
+    name: Rules with vars
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: debug
             action_args: {}
         condition:
           AllCondition:
           - AssignmentExpression:
               lhs:
                 Events: first
@@ -30,10 +30,10 @@
                     Integer: 1
         enabled: true
         name: multiple conditions
     sources:
     - EventSource:
         name: range
         source_args:
-          limit: 5
+          limit: '{{limit}}'
         source_filters: []
         source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions3.yml` & `ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions3.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 - RuleSet:
     hosts:
     - localhost
     name: Demo rules multiple conditions reference assignment
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: debug
             action_args:
               first: '{{events.first}}'
               second: '{{events.second}}'
               third: '{{events.third}}'
         condition:
           AllCondition:
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/rules_with_time.yml` & `ansible_rulebook-1.0.0/tests/asts/rules_with_timestamp.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,91 @@
 - RuleSet:
     hosts:
     - localhost
-    name: Demo rules with time
+    name: Demo rules with timestamp
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: set_fact
             action_args:
               fact:
-                current_time: '{{event.time.tick}}'
+                current_time: '{{event.timestamp.unix_timestamp}}'
         condition:
           AllCondition:
           - IsDefinedExpression:
-              Event: time.tick
+              Event: timestamp.unix_timestamp
         enabled: true
-        name: promote time.tick to current_time fact
+        name: promote timestamp.unix_timestamp to current_time fact
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
+            action: set_fact
+            action_args:
+              fact:
+                initial_time: '{{facts.time.current_time}}'
+        condition:
+          AllCondition:
+          - AssignmentExpression:
+              lhs:
+                Facts: time
+              rhs:
+                IsDefinedExpression:
+                  Fact: current_time
+          - IsNotDefinedExpression:
+              Event: initial_time
+        enabled: true
+        name: set the initial time
+    - Rule:
+        actions:
+        - Action:
             action: retract_fact
             action_args:
               fact:
-                current_time: '{{event.current_time}}'
+                current_time: '{{fact.current_time}}'
         condition:
           AllCondition:
           - IsDefinedExpression:
               Fact: current_time
         enabled: true
         name: retract current_time fact
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: debug
             action_args: {}
         condition:
           AllCondition:
           - IsDefinedExpression:
-              Fact: current_time
+              Fact: initial_time
         enabled: true
-        name: matches current_time fact before it is retracted since facts fire all
-          matching rules
+        name: debug
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: shutdown
             action_args: {}
         condition:
           AllCondition:
+          - AssignmentExpression:
+              lhs:
+                Facts: a
+              rhs:
+                IsDefinedExpression:
+                  Fact: initial_time
           - GreaterThanOrEqualToExpression:
               lhs:
                 Fact: current_time
               rhs:
-                Integer: 5
+                AdditionExpression:
+                  lhs:
+                    Facts: a.initial_time
+                  rhs:
+                    Integer: 5
         enabled: true
-        name: shutdown after 5 ticks
+        name: shutdown
     sources:
     - EventSource:
-        name: tick
+        name: timestamp
         source_args: {}
         source_filters: []
-        source_name: tick
+        source_name: timestamp
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/rules_with_timestamp.yml` & `ansible_rulebook-1.0.0/tests/asts/test_filters.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,91 +1,73 @@
 - RuleSet:
     hosts:
-    - localhost
-    name: Demo rules with timestamp
+    - all
+    name: Test rule filters
     rules:
     - Rule:
-        action:
-          Action:
-            action: set_fact
+        actions:
+        - Action:
+            action: print_event
             action_args:
-              fact:
-                current_time: '{{event.timestamp.unix_timestamp}}'
+              pretty: true
+              var_root: i
         condition:
           AllCondition:
-          - IsDefinedExpression:
-              Event: timestamp.unix_timestamp
+          - EqualsExpression:
+              lhs:
+                Event: i
+              rhs:
+                Integer: 0
         enabled: true
-        name: promote timestamp.unix_timestamp to current_time fact
+        name: r1
     - Rule:
-        action:
-          Action:
-            action: set_fact
-            action_args:
-              fact:
-                initial_time: '{{facts.time.current_time}}'
+        actions:
+        - Action:
+            action: print_event
+            action_args: {}
         condition:
           AllCondition:
-          - AssignmentExpression:
+          - EqualsExpression:
               lhs:
-                Facts: time
+                Event: i
               rhs:
-                IsDefinedExpression:
-                  Fact: current_time
-          - IsNotDefinedExpression:
-              Event: initial_time
+                Integer: 1
         enabled: true
-        name: set the initial time
+        name: r2
     - Rule:
-        action:
-          Action:
-            action: retract_fact
+        actions:
+        - Action:
+            action: run_playbook
             action_args:
-              fact:
-                current_time: '{{fact.current_time}}'
+              name: playbooks/hello_world_set_fact.yml
+              post_events: true
+              var_root: i
         condition:
           AllCondition:
-          - IsDefinedExpression:
-              Fact: current_time
+          - EqualsExpression:
+              lhs:
+                Event: i
+              rhs:
+                Integer: 2
         enabled: true
-        name: retract current_time fact
+        name: r3
     - Rule:
-        action:
-          Action:
-            action: debug
+        actions:
+        - Action:
+            action: print_event
             action_args: {}
         condition:
           AllCondition:
           - IsDefinedExpression:
-              Fact: initial_time
-        enabled: true
-        name: debug
-    - Rule:
-        action:
-          Action:
-            action: shutdown
-            action_args: {}
-        condition:
-          AllCondition:
-          - AssignmentExpression:
-              lhs:
-                Facts: a
-              rhs:
-                IsDefinedExpression:
-                  Fact: initial_time
-          - GreaterThanOrEqualToExpression:
-              lhs:
-                Fact: current_time
-              rhs:
-                AdditionExpression:
-                  lhs:
-                    Facts: a.initial_time
-                  rhs:
-                    Integer: 5
+              Event: msg
         enabled: true
-        name: shutdown
+        name: r4
     sources:
     - EventSource:
-        name: timestamp
-        source_args: {}
-        source_filters: []
-        source_name: timestamp
+        name: range
+        source_args:
+          limit: 5
+        source_filters:
+        - EventSourceFilter:
+            filter_args: null
+            filter_name: noop
+        source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/rules_with_vars.yml` & `ansible_rulebook-1.0.0/tests/asts/rules_with_assignment.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 - RuleSet:
     hosts:
     - localhost
-    name: Rules with vars
+    name: Demo rules with assignment
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: debug
-            action_args: {}
+            action_args:
+              var: events.first
         condition:
           AllCondition:
           - AssignmentExpression:
               lhs:
                 Events: first
               rhs:
                 EqualsExpression:
                   lhs:
                     Event: i
                   rhs:
                     Integer: 0
-          - AssignmentExpression:
-              lhs:
-                Events: second
-              rhs:
-                EqualsExpression:
-                  lhs:
-                    Event: i
-                  rhs:
-                    Integer: 1
         enabled: true
-        name: multiple conditions
+        name: assignment
     sources:
     - EventSource:
         name: range
         source_args:
-          limit: '{{limit}}'
+          limit: 5
         source_filters: []
         source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/rules_without_assignment.yml` & `ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts2.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 - RuleSet:
     hosts:
-    - localhost
-    name: Demo rules multiple conditions all
+    - all
+    name: Test rules multiple hosts 2
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: debug
-            action_args:
-              event: '{{event}}'
+            action_args: {}
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
-                Fact: i
+                Event: i
               rhs:
-                Integer: 0
+                Integer: 1
         enabled: true
-        name: assignment
+        name: r1
     sources:
     - EventSource:
         name: range
         source_args:
           limit: 5
         source_filters: []
         source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/test_filters.yml` & `ansible_rulebook-1.0.0/tests/asts/test_rules.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,89 @@
 - RuleSet:
     hosts:
     - all
-    name: Test rule filters
+    name: Test rules4
     rules:
     - Rule:
-        action:
-          Action:
-            action: print_event
+        actions:
+        - Action:
+            action: set_fact
             action_args:
-              pretty: true
-              var_root: i
+              fact:
+                j: 1
+              ruleset: Test rules4
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
-                Integer: 0
+                Integer: 1
         enabled: true
         name: r1
     - Rule:
-        action:
-          Action:
-            action: print_event
-            action_args: {}
+        actions:
+        - Action:
+            action: run_playbook
+            action_args:
+              name: playbooks/hello_world_set_fact.yml
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
-                Integer: 1
+                Integer: 2
         enabled: true
         name: r2
     - Rule:
-        action:
-          Action:
-            action: run_playbook
+        actions:
+        - Action:
+            action: retract_fact
             action_args:
-              name: playbooks/hello_world_set_fact.yml
-              post_events: true
-              var_root: i
+              fact:
+                j: 3
+              ruleset: Test rules4
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
-                Integer: 2
+                Integer: 3
         enabled: true
         name: r3
     - Rule:
-        action:
-          Action:
-            action: print_event
+        actions:
+        - Action:
+            action: post_event
+            action_args:
+              event:
+                j: 4
+              ruleset: Test rules4
+        condition:
+          AllCondition:
+          - EqualsExpression:
+              lhs:
+                Event: i
+              rhs:
+                Integer: 4
+        enabled: true
+        name: r4
+    - Rule:
+        actions:
+        - Action:
+            action: none
             action_args: {}
         condition:
           AllCondition:
           - IsDefinedExpression:
-              Event: msg
+              Event: j
         enabled: true
-        name: r4
+        name: r5
     sources:
     - EventSource:
         name: range
         source_args:
           limit: 5
-        source_filters:
-        - EventSourceFilter:
-            filter_args: null
-            filter_name: noop
+        source_filters: []
         source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/test_host_rules.yml` & `ansible_rulebook-1.0.0/tests/asts/test_simple.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,70 @@
 - RuleSet:
     hosts:
     - all
-    name: Test host rules
+    name: Test rules simple
     rules:
     - Rule:
-        action:
-          Action:
-            action: set_fact
+        actions:
+        - Action:
+            action: print_event
             action_args:
-              fact:
-                j: 1
-              ruleset: Test host rules
+              pretty: true
+              var_root: i
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
-                Integer: 1
+                Integer: 0
         enabled: true
         name: r1
     - Rule:
-        action:
-          Action:
-            action: run_playbook
-            action_args:
-              name: playbooks/hello_events.yml
+        actions:
+        - Action:
+            action: print_event
+            action_args: {}
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
-                Integer: 2
+                Integer: 1
         enabled: true
         name: r2
     - Rule:
-        action:
-          Action:
-            action: retract_fact
+        actions:
+        - Action:
+            action: run_playbook
             action_args:
-              fact:
-                j: 3
-              ruleset: Test host rules
+              name: playbooks/hello_world_set_fact.yml
+              post_events: true
+              var_root: i
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
-                Integer: 3
+                Integer: 2
         enabled: true
         name: r3
     - Rule:
-        action:
-          Action:
-            action: post_event
-            action_args:
-              event:
-                j: 4
-              ruleset: Test host rules
-        condition:
-          AllCondition:
-          - EqualsExpression:
-              lhs:
-                Event: i
-              rhs:
-                Integer: 4
-        enabled: true
-        name: r4
-    - Rule:
-        action:
-          Action:
-            action: none
+        actions:
+        - Action:
+            action: print_event
             action_args: {}
         condition:
           AllCondition:
           - IsDefinedExpression:
-              Event: j
+              Event: msg
         enabled: true
-        name: r5
+        name: r4
     sources:
     - EventSource:
-        name: hosts
+        name: range
         source_args:
           limit: 5
         source_filters: []
-        source_name: hosts
+        source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/test_rules.yml` & `ansible_rulebook-1.0.0/tests/asts/test_host_rules.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 - RuleSet:
     hosts:
     - all
-    name: Test rules4
+    name: Test host rules
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: set_fact
             action_args:
               fact:
                 j: 1
-              ruleset: Test rules4
+              ruleset: Test host rules
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
                 Integer: 1
         enabled: true
         name: r1
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: run_playbook
             action_args:
-              name: playbooks/hello_world_set_fact.yml
+              name: playbooks/hello_events.yml
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
                 Integer: 2
         enabled: true
         name: r2
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: retract_fact
             action_args:
               fact:
                 j: 3
-              ruleset: Test rules4
+              ruleset: Test host rules
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
                 Integer: 3
         enabled: true
         name: r3
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: post_event
             action_args:
               event:
                 j: 4
-              ruleset: Test rules4
+              ruleset: Test host rules
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
                 Integer: 4
         enabled: true
         name: r4
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: none
             action_args: {}
         condition:
           AllCondition:
           - IsDefinedExpression:
               Event: j
         enabled: true
         name: r5
     sources:
     - EventSource:
-        name: range
+        name: hosts
         source_args:
           limit: 5
         source_filters: []
-        source_name: range
+        source_name: hosts
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts.yml` & `ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 - RuleSet:
     hosts:
     - localhost0, localhost1
     name: Test rules multiple hosts
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: set_fact
             action_args:
               fact:
                 j: 1
               ruleset: Test rules multiple hosts
         condition:
           AllCondition:
@@ -17,31 +17,31 @@
               lhs:
                 Event: i
               rhs:
                 Integer: 1
         enabled: true
         name: r1
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: run_playbook
             action_args:
               name: playbooks/hello_events.yml
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
                 Integer: 2
         enabled: true
         name: r2
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: retract_fact
             action_args:
               fact:
                 j: 3
               ruleset: Test rules multiple hosts
         condition:
           AllCondition:
@@ -49,16 +49,16 @@
               lhs:
                 Event: i
               rhs:
                 Integer: 3
         enabled: true
         name: r3
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: post_event
             action_args:
               event:
                 j: 4
               ruleset: Test rules multiple hosts
         condition:
           AllCondition:
@@ -66,16 +66,16 @@
               lhs:
                 Event: i
               rhs:
                 Integer: 4
         enabled: true
         name: r4
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: none
             action_args: {}
         condition:
           AllCondition:
           - IsDefinedExpression:
               Event: j
         enabled: true
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts2.yml` & `ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts3.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 - RuleSet:
     hosts:
     - all
-    name: Test rules multiple hosts 2
+    name: Test rules multiple hosts 3
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: debug
             action_args: {}
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts3.yml` & `ansible_rulebook-1.0.0/tests/asts/rules_with_assignment2.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 - RuleSet:
     hosts:
-    - all
-    name: Test rules multiple hosts 3
+    - localhost
+    name: Demo rules with assignment2
     rules:
     - Rule:
-        action:
-          Action:
+        actions:
+        - Action:
             action: debug
-            action_args: {}
+            action_args:
+              var: events.first
         condition:
           AllCondition:
-          - EqualsExpression:
+          - AssignmentExpression:
               lhs:
-                Event: i
+                Facts: first
               rhs:
-                Integer: 1
+                EqualsExpression:
+                  lhs:
+                    Fact: i
+                  rhs:
+                    Integer: 0
         enabled: true
-        name: r1
+        name: assignment
     sources:
     - EventSource:
         name: range
         source_args:
           limit: 5
         source_filters: []
         source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/asts/test_simple.yml` & `ansible_rulebook-1.0.0/tests/asts/19_is_defined.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,51 @@
 - RuleSet:
     hosts:
     - all
-    name: Test rules simple
+    name: 19 is defined
     rules:
     - Rule:
         action:
           Action:
-            action: print_event
+            action: set_fact
             action_args:
-              pretty: true
-              var_root: i
+              fact:
+                msg: hello
         condition:
           AllCondition:
           - EqualsExpression:
               lhs:
                 Event: i
               rhs:
-                Integer: 0
+                Integer: 1
         enabled: true
         name: r1
     - Rule:
         action:
           Action:
-            action: print_event
+            action: debug
             action_args: {}
         condition:
           AllCondition:
-          - EqualsExpression:
-              lhs:
-                Event: i
-              rhs:
-                Integer: 1
+          - IsDefinedExpression:
+              Event: msg
         enabled: true
         name: r2
     - Rule:
         action:
           Action:
-            action: run_playbook
-            action_args:
-              name: playbooks/hello_world_set_fact.yml
-              post_events: true
-              var_root: i
-        condition:
-          AllCondition:
-          - EqualsExpression:
-              lhs:
-                Event: i
-              rhs:
-                Integer: 2
-        enabled: true
-        name: r3
-    - Rule:
-        action:
-          Action:
             action: print_event
-            action_args: {}
+            action_args:
+              pretty: true
         condition:
           AllCondition:
           - IsDefinedExpression:
-              Event: msg
+              Event: payload
         enabled: true
-        name: r4
+        name: r3
     sources:
     - EventSource:
         name: range
         source_args:
           limit: 5
         source_filters: []
         source_name: range
```

### Comparing `ansible_rulebook-0.9.4/tests/event_filters/json_filter.py` & `ansible_rulebook-1.0.0/tests/event_filter/json_filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+#  Copyright 2022 Red Hat, Inc.
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
 """
 json_filter.py:   An event filter that filters keys out of events.
 
 Includes override excludes.
 
 This is useful to exclude information from events that is unneeded
 by the rule engine.
```

### Comparing `ansible_rulebook-0.9.4/tests/examples/35_multiple_rulesets_1_fired.yml` & `ansible_rulebook-1.0.0/tests/examples/35_multiple_rulesets_1_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/examples/replays/24_max_attributes/00.json` & `ansible_rulebook-1.0.0/tests/examples/replays/24_max_attributes/00.json`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/examples/replays/25_max_attributes_nested/00.json` & `ansible_rulebook-1.0.0/tests/examples/replays/25_max_attributes_nested/00.json`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/playbooks/check_facts_playbook.yml` & `ansible_rulebook-1.0.0/tests/playbooks/check_facts_playbook.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
   hosts: localhost
   gather_facts: false
   tasks:
     - name: Fail if the value is missing
       ansible.builtin.fail:
         msg: "Failing because hello world fact does not match"
       when: fact.msg != "hello world"
+
     - name: Fail if the alpha is missing
       ansible.builtin.fail:
         msg: "Failing because alpha fact does not match"
       when: fact.alpha != 1
+
     - name: Fail if the beta.location doesn't match
       ansible.builtin.fail:
         msg: "Failing because beta.location fact does not match"
       when: fact.beta.location != "Naboo"
```

### Comparing `ansible_rulebook-0.9.4/tests/rules/rules.yml` & `ansible_rulebook-1.0.0/tests/rules/rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/rules/rules_with_time.yml` & `ansible_rulebook-1.0.0/tests/rules/rules_with_time.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/rules/rules_with_timestamp.yml` & `ansible_rulebook-1.0.0/tests/rules/rules_with_timestamp.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/rules/test_filters.yml` & `ansible_rulebook-1.0.0/tests/rules/test_filters.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/rules/test_host_rules.yml` & `ansible_rulebook-1.0.0/tests/rules/test_host_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/rules/test_kafka.yml` & `ansible_rulebook-1.0.0/tests/rules/test_kafka.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/rules/test_rules.yml` & `ansible_rulebook-1.0.0/tests/rules/test_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/rules/test_rules_multiple_hosts.yml` & `ansible_rulebook-1.0.0/tests/rules/test_rules_multiple_hosts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/rules/test_simple.yml` & `ansible_rulebook-1.0.0/tests/rules/test_simple.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/rules/test_states.yml` & `ansible_rulebook-1.0.0/tests/rules/test_states.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/rules/webserver_down.yml` & `ansible_rulebook-1.0.0/tests/rules/webserver_down.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.4/tests/test_simple.yml` & `ansible_rulebook-1.0.0/tests/test_simple.yml`

 * *Files identical despite different names*

