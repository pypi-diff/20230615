# Comparing `tmp/barman-3.5.0.tar.gz` & `tmp/barman-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barman-3.5.0.tar", last modified: Wed Mar 29 17:06:53 2023, max compression
+gzip compressed data, was "dist/barman-3.6.0.tar", last modified: Thu Jun 15 12:24:44 2023, max compression
```

## Comparing `barman-3.5.0.tar` & `barman-3.6.0.tar`

### file list

```diff
@@ -1,298 +1,306 @@
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/doc/
--rw-r--r--   0     1001      123     3623 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-wal-restore.1
--rw-r--r--   0     1001      123     6559 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-wal-restore.1
--rw-r--r--   0     1001      123     6187 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-backup-list.1
--rw-r--r--   0     1001      123      745 2023-03-29 17:06:23.000000 barman-3.5.0/doc/Dockerfile
--rw-r--r--   0     1001      123     2331 2023-03-29 17:06:23.000000 barman-3.5.0/doc/Makefile
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/doc/barman.5.d/
--rw-r--r--   0     1001      123      388 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-post_archive_retry_script.md
--rw-r--r--   0     1001      123      405 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-backup_compression_format.md
--rw-r--r--   0     1001      123       26 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/80-see-also.md
--rw-r--r--   0     1001      123       59 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/05-name.md
--rw-r--r--   0     1001      123      652 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-recovery_staging_path.md
--rw-r--r--   0     1001      123       63 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-wals_directory.md
--rw-r--r--   0     1001      123      162 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-custom_decompression_filter.md
--rw-r--r--   0     1001      123      144 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-post_archive_script.md
--rw-r--r--   0     1001      123      425 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-pre_wal_delete_retry_script.md
--rw-r--r--   0     1001      123       80 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-pre_backup_script.md
--rw-r--r--   0     1001      123       97 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-pre_wal_delete_script.md
--rw-r--r--   0     1001      123      403 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-pre_backup_retry_script.md
--rw-r--r--   0     1001      123      171 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-slot_name.md
--rw-r--r--   0     1001      123      464 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-archiver.md
--rw-r--r--   0     1001      123     1055 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-primary_conninfo.md
--rw-r--r--   0     1001      123      117 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-parallel_jobs_start_batch_size.md
--rw-r--r--   0     1001      123      129 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-incoming_wals_directory.md
--rw-r--r--   0     1001      123      155 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/95-resources.md
--rw-r--r--   0     1001      123      192 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-basebackup_retry_sleep.md
--rw-r--r--   0     1001      123      328 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-compression.md
--rw-r--r--   0     1001      123       79 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-retention_policy_mode.md
--rw-r--r--   0     1001      123      176 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-bandwidth_limit.md
--rw-r--r--   0     1001      123      229 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/25-configuration-file-syntax.md
--rw-r--r--   0     1001      123      100 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-custom_compression_filter.md
--rw-r--r--   0     1001      123      237 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-streaming_archiver_name.md
--rw-r--r--   0     1001      123      411 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-archiver_batch_size.md
--rw-r--r--   0     1001      123      244 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-backup_compression_workers.md
--rw-r--r--   0     1001      123      250 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-create_slot.md
--rw-r--r--   0     1001      123      220 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-parallel_jobs.md
--rw-r--r--   0     1001      123      366 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-conninfo.md
--rw-r--r--   0     1001      123      413 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-pre_delete_retry_script.md
--rw-r--r--   0     1001      123      379 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-post_wal_delete_retry_script.md
--rw-r--r--   0     1001      123      186 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-snapshot-instance.md
--rw-r--r--   0     1001      123      111 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/00-header.md
--rw-r--r--   0     1001      123      546 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-last_backup_minimum_size.md
--rw-r--r--   0     1001      123      284 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-snapshot-gcp-project.md
--rw-r--r--   0     1001      123      138 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-parallel_jobs_start_batch_period.md
--rw-r--r--   0     1001      123      213 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-errors_directory.md
--rw-r--r--   0     1001      123       91 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-minimum_redundancy.md
--rw-r--r--   0     1001      123      174 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-streaming_conninfo.md
--rw-r--r--   0     1001      123       86 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-backup_directory.md
--rw-r--r--   0     1001      123      472 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-last_backup_maximum_age.md
--rw-r--r--   0     1001      123      367 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-last_wal_maximum_age.md
--rw-r--r--   0     1001      123      365 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-recovery_options.md
--rw-r--r--   0     1001      123       66 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-description.md
--rw-r--r--   0     1001      123      757 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-backup_method.md
--rw-r--r--   0     1001      123      512 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-custom_compression_magic.md
--rw-r--r--   0     1001      123      362 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-post_backup_retry_script.md
--rw-r--r--   0     1001      123      368 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-forward-config-path.md
--rw-r--r--   0     1001      123      183 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-basebackup_retry_times.md
--rw-r--r--   0     1001      123      179 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-check_timeout.md
--rw-r--r--   0     1001      123      130 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-wal_retention_policy.md
--rw-r--r--   0     1001      123      118 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-post_backup_script.md
--rw-r--r--   0     1001      123      202 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-snapshot-disks.md
--rw-r--r--   0     1001      123      252 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-max_incoming_wals_queue.md
--rw-r--r--   0     1001      123      272 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/15-description.md
--rw-r--r--   0     1001      123       10 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/45-options.md
--rw-r--r--   0     1001      123       88 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-ssh_command.md
--rw-r--r--   0     1001      123       56 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-barman_home.md
--rw-r--r--   0     1001      123      210 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/20-configuration-file-locations.md
--rw-r--r--   0     1001      123      463 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-immediate_checkpoint.md
--rw-r--r--   0     1001      123      109 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-pre_archive_script.md
--rw-r--r--   0     1001      123      233 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-path_prefix.md
--rw-r--r--   0     1001      123      651 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-streaming_archiver.md
--rw-r--r--   0     1001      123       80 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-log_level.md
--rw-r--r--   0     1001      123      139 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-post_wal_delete_script.md
--rw-r--r--   0     1001      123      239 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-backup_compression_location.md
--rw-r--r--   0     1001      123      163 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-streaming_wals_directory.md
--rw-r--r--   0     1001      123       52 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-log_file.md
--rw-r--r--   0     1001      123      119 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-post_recovery_script.md
--rw-r--r--   0     1001      123       79 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-basebackups_directory.md
--rw-r--r--   0     1001      123      405 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-pre_recovery_retry_script.md
--rw-r--r--   0     1001      123      212 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-snapshot-provider.md
--rw-r--r--   0     1001      123     1545 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/70-hook-scripts.md
--rw-r--r--   0     1001      123      593 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/90-authors.md
--rw-r--r--   0     1001      123      363 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-post_recovery_retry_script.md
--rw-r--r--   0     1001      123      537 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/30-configuration-file-directory.md
--rw-r--r--   0     1001      123      174 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/99-copying.md
--rw-r--r--   0     1001      123      653 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-retention_policy.md
--rw-r--r--   0     1001      123      487 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-reuse_backup.md
--rw-r--r--   0     1001      123      373 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-post_delete_retry_script.md
--rw-r--r--   0     1001      123       83 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-barman_lock_directory.md
--rw-r--r--   0     1001      123      762 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/75-example.md
--rw-r--r--   0     1001      123      247 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-network_compression.md
--rw-r--r--   0     1001      123      129 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-post_delete_script.md
--rw-r--r--   0     1001      123      224 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-snapshot-zone.md
--rw-r--r--   0     1001      123      992 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-backup_options.md
--rw-r--r--   0     1001      123      267 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-tablespace_bandwidth_limit.md
--rw-r--r--   0     1001      123      440 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-pre_archive_retry_script.md
--rw-r--r--   0     1001      123      441 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-streaming_archiver_batch_size.md
--rw-r--r--   0     1001      123       79 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-pre_recovery_script.md
--rw-r--r--   0     1001      123      172 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-streaming_backup_name.md
--rw-r--r--   0     1001      123       91 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-pre_delete_script.md
--rw-r--r--   0     1001      123      539 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-backup_compression.md
--rw-r--r--   0     1001      123      505 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-active.md
--rw-r--r--   0     1001      123      359 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-primary_ssh_command.md
--rw-r--r--   0     1001      123      275 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5.d/50-backup_compression_level.md
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/doc/build/
--rw-r--r--   0     1001      123     1750 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/Makefile
--rwxr-xr-x   0     1001      123     1417 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/build
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/doc/build/templates/
--rw-r--r--   0     1001      123   102895 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/templates/logo-hires.png
--rw-r--r--   0     1001      123    16668 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/templates/postgres.pdf
--rw-r--r--   0     1001      123    81089 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/templates/logo-horizontal-hires.png
--rw-r--r--   0     1001      123      161 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/templates/default.yaml
--rw-r--r--   0     1001      123     9952 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/templates/Barman.tex
--rw-r--r--   0     1001      123     6346 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/templates/default.latex
--rw-r--r--   0     1001      123     3895 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/templates/edb-enterprisedb-logo.png
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/doc/build/html-templates/
--rw-r--r--   0     1001      123    21298 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/html-templates/docs.css
--rw-r--r--   0     1001      123     3520 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/html-templates/template-cli.html
--rw-r--r--   0     1001      123     1187 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/html-templates/barman.css
--rw-r--r--   0     1001      123     5572 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/html-templates/template.html
--rw-r--r--   0     1001      123     3838 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/html-templates/template-utils.html
--rw-r--r--   0     1001      123   147074 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/html-templates/bootstrap.css
--rw-r--r--   0     1001      123      238 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/html-templates/SOURCES.md
--rw-r--r--   0     1001      123      111 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/html-templates/template.css
--rw-r--r--   0     1001      123     1092 2023-03-29 17:06:23.000000 barman-3.5.0/doc/build/html-templates/override.css
--rw-r--r--   0     1001      123     5827 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-restore.1.md
--rw-r--r--   0     1001      123     8707 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-backup-delete.1
--rw-r--r--   0     1001      123    30618 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.5
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/doc/barman.1.d/
--rw-r--r--   0     1001      123      393 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-check.md
--rw-r--r--   0     1001      123      642 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-sync-info.md
--rw-r--r--   0     1001      123       26 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/80-see-also.md
--rw-r--r--   0     1001      123     5863 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-recover.md
--rw-r--r--   0     1001      123       60 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/05-name.md
--rw-r--r--   0     1001      123      291 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-list-backups.md
--rw-r--r--   0     1001      123     1268 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-keep.md
--rw-r--r--   0     1001      123      270 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-diagnose.md
--rw-r--r--   0     1001      123      596 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/20-options.md
--rw-r--r--   0     1001      123      590 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-check-wal-archive.md
--rw-r--r--   0     1001      123      155 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/95-resources.md
--rw-r--r--   0     1001      123       41 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/10-synopsis.md
--rw-r--r--   0     1001      123      333 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-check-backup.md
--rw-r--r--   0     1001      123      850 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-switch-wal.md
--rw-r--r--   0     1001      123      668 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-receive-wal.md
--rw-r--r--   0     1001      123       74 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-list-servers.md
--rw-r--r--   0     1001      123      701 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-put-wal.md
--rw-r--r--   0     1001      123      111 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/00-header.md
--rw-r--r--   0     1001      123      143 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-delete.md
--rw-r--r--   0     1001      123       55 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/45-commands.md
--rw-r--r--   0     1001      123      295 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-rebuild-xlogdb.md
--rw-r--r--   0     1001      123      266 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-archive-wal.md
--rw-r--r--   0     1001      123     3139 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-backup.md
--rw-r--r--   0     1001      123      347 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/85-bugs.md
--rw-r--r--   0     1001      123      272 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/15-description.md
--rw-r--r--   0     1001      123      788 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-list-files.md
--rw-r--r--   0     1001      123     1420 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-show-backup.md
--rw-r--r--   0     1001      123     1048 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-get-wal.md
--rw-r--r--   0     1001      123      798 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-status.md
--rw-r--r--   0     1001      123      241 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-show-servers.md
--rw-r--r--   0     1001      123      621 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/90-authors.md
--rw-r--r--   0     1001      123       81 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-switch-xlog.md
--rw-r--r--   0     1001      123      444 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/70-backup-id-shortcuts.md
--rw-r--r--   0     1001      123      174 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/99-copying.md
--rw-r--r--   0     1001      123      351 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-sync-wals.md
--rw-r--r--   0     1001      123      279 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-cron.md
--rw-r--r--   0     1001      123      578 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-replication-status.md
--rw-r--r--   0     1001      123      368 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/50-sync-backup.md
--rw-r--r--   0     1001      123       51 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1.d/75-exit-status.md
--rw-r--r--   0     1001      123    26326 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.1
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/doc/images/
--rw-r--r--   0     1001      123   227695 2023-03-29 17:06:23.000000 barman-3.5.0/doc/images/barman-architecture-scenario1b.png
--rw-r--r--   0     1001      123   228769 2023-03-29 17:06:23.000000 barman-3.5.0/doc/images/barman-architecture-scenario2b.png
--rw-r--r--   0     1001      123   179610 2023-03-29 17:06:23.000000 barman-3.5.0/doc/images/barman-architecture-scenario1.png
--rw-r--r--   0     1001      123   201845 2023-03-29 17:06:23.000000 barman-3.5.0/doc/images/barman-architecture-scenario2.png
--rw-r--r--   0     1001      123   157428 2023-03-29 17:06:23.000000 barman-3.5.0/doc/images/barman-architecture-georedundancy.png
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/doc/barman.d/
--rw-r--r--   0     1001      123     1546 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.d/ssh-server.conf-template
--rw-r--r--   0     1001      123      950 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.d/passive-server.conf-template
--rw-r--r--   0     1001      123     1500 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.d/streaming-server.conf-template
--rw-r--r--   0     1001      123    10062 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-backup.1.md
--rw-r--r--   0     1001      123     2241 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-wal-archive.1.md
--rw-r--r--   0     1001      123     6494 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-check-wal-archive.1
--rw-r--r--   0     1001      123    11346 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-wal-archive.1
--rw-r--r--   0     1001      123     2631 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-wal-archive.1
--rw-r--r--   0     1001      123     5293 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-backup-keep.1.md
--rw-r--r--   0     1001      123     4979 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-backup-show.1.md
--rw-r--r--   0     1001      123       47 2023-03-29 17:06:23.000000 barman-3.5.0/doc/.gitignore
--rw-r--r--   0     1001      123     7394 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-restore.1
--rw-r--r--   0     1001      123     8575 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-wal-archive.1.md
--rw-r--r--   0     1001      123     6769 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-backup-keep.1
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/doc/manual/
--rw-r--r--   0     1001      123    47556 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/50-feature-details.en.md
--rw-r--r--   0     1001      123     4181 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/99-references.en.md
--rw-r--r--   0     1001      123     8651 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/16-installation.en.md
--rw-r--r--   0     1001      123      667 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/Makefile
--rw-r--r--   0     1001      123     3564 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/17-configuration.en.md
--rw-r--r--   0     1001      123     1335 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/30-windows-support.en.md
--rw-r--r--   0     1001      123     5034 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/23-wal_streaming.en.md
--rw-r--r--   0     1001      123     2629 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/41-global-commands.en.md
--rw-r--r--   0     1001      123    13511 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/43-backup-commands.en.md
--rw-r--r--   0     1001      123     3665 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/66-about.en.md
--rw-r--r--   0     1001      123    10034 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/55-barman-cli.en.md
--rw-r--r--   0     1001      123      785 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/00-head.en.md
--rw-r--r--   0     1001      123     1001 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/02-before_you_start.en.md
--rw-r--r--   0     1001      123    11250 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/42-server-commands.en.md
--rw-r--r--   0     1001      123     1017 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/26-rsync_backup.en.md
--rw-r--r--   0     1001      123       43 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/.gitignore
--rw-r--r--   0     1001      123     1732 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/65-troubleshooting.en.md
--rw-r--r--   0     1001      123      823 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/20-server_setup.en.md
--rw-r--r--   0     1001      123     5283 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/24-wal_archiving.en.md
--rw-r--r--   0     1001      123    11160 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/10-design.en.md
--rw-r--r--   0     1001      123     2914 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/15-system_requirements.en.md
--rw-r--r--   0     1001      123     5065 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/28-snapshots.en.md
--rw-r--r--   0     1001      123      862 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/22-config_file.en.md
--rw-r--r--   0     1001      123     9313 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/21-preliminary_steps.en.md
--rw-r--r--   0     1001      123     4014 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/01-intro.en.md
--rw-r--r--   0     1001      123     1083 2023-03-29 17:06:23.000000 barman-3.5.0/doc/manual/25-streaming_backup.en.md
--rw-r--r--   0     1001      123     3501 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman.conf
--rw-r--r--   0     1001      123     4868 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-backup-list.1.md
--rw-r--r--   0     1001      123     3067 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-wal-restore.1.md
--rw-r--r--   0     1001      123     6926 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-backup-delete.1.md
--rw-r--r--   0     1001      123    13008 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-backup.1
--rw-r--r--   0     1001      123     5091 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-check-wal-archive.1.md
--rw-r--r--   0     1001      123     5131 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-wal-restore.1.md
--rw-r--r--   0     1001      123     6334 2023-03-29 17:06:23.000000 barman-3.5.0/doc/barman-cloud-backup-show.1
--rw-r--r--   0     1001      123      196 2023-03-29 17:06:23.000000 barman-3.5.0/MANIFEST.in
--rw-r--r--   0     1001      123    35147 2023-03-29 17:06:23.000000 barman-3.5.0/LICENSE
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/scripts/
--rw-r--r--   0     1001      123       98 2023-03-29 17:06:23.000000 barman-3.5.0/scripts/barman.bash_completion
--rw-r--r--   0     1001      123     1447 2023-03-29 17:06:53.000000 barman-3.5.0/PKG-INFO
--rw-r--r--   0     1001      123     2193 2023-03-29 17:06:23.000000 barman-3.5.0/README.rst
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/barman/
--rw-r--r--   0     1001      123     5959 2023-03-29 17:06:23.000000 barman-3.5.0/barman/process.py
--rw-r--r--   0     1001      123   164482 2023-03-29 17:06:23.000000 barman-3.5.0/barman/server.py
--rw-r--r--   0     1001      123    19890 2023-03-29 17:06:23.000000 barman-3.5.0/barman/fs.py
--rw-r--r--   0     1001      123    16411 2023-03-29 17:06:23.000000 barman-3.5.0/barman/xlog.py
--rw-r--r--   0     1001      123    42482 2023-03-29 17:06:23.000000 barman-3.5.0/barman/wal_archiver.py
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/barman/clients/
--rw-r--r--   0     1001      123     6302 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_compression.py
--rwxr-xr-x   0     1001      123    16333 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/walrestore.py
--rw-r--r--   0     1001      123     6705 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_walrestore.py
--rw-r--r--   0     1001      123    12796 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_restore.py
--rw-r--r--   0     1001      123     3147 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_check_wal_archive.py
--rw-r--r--   0     1001      123      724 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/__init__.py
--rwxr-xr-x   0     1001      123    11331 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/walarchive.py
--rw-r--r--   0     1001      123     6660 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_cli.py
--rw-r--r--   0     1001      123     4438 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_backup_list.py
--rwxr-xr-x   0     1001      123    13605 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_backup.py
--rw-r--r--   0     1001      123    14156 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_backup_delete.py
--rw-r--r--   0     1001      123     4344 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_backup_keep.py
--rw-r--r--   0     1001      123     3720 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_backup_show.py
--rwxr-xr-x   0     1001      123    11355 2023-03-29 17:06:23.000000 barman-3.5.0/barman/clients/cloud_walarchive.py
--rw-r--r--   0     1001      123     4343 2023-03-29 17:06:23.000000 barman-3.5.0/barman/diagnose.py
--rw-r--r--   0     1001      123    11374 2023-03-29 17:06:23.000000 barman-3.5.0/barman/lockfile.py
--rw-r--r--   0     1001      123    25604 2023-03-29 17:06:23.000000 barman-3.5.0/barman/utils.py
--rw-r--r--   0     1001      123    12760 2023-03-29 17:06:23.000000 barman-3.5.0/barman/annotations.py
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/barman/cloud_providers/
--rw-r--r--   0     1001      123    28533 2023-03-29 17:06:23.000000 barman-3.5.0/barman/cloud_providers/google_cloud_storage.py
--rw-r--r--   0     1001      123     8973 2023-03-29 17:06:23.000000 barman-3.5.0/barman/cloud_providers/__init__.py
--rw-r--r--   0     1001      123    14428 2023-03-29 17:06:23.000000 barman-3.5.0/barman/cloud_providers/aws_s3.py
--rw-r--r--   0     1001      123    19597 2023-03-29 17:06:23.000000 barman-3.5.0/barman/cloud_providers/azure_blob_storage.py
--rw-r--r--   0     1001      123    40156 2023-03-29 17:06:23.000000 barman-3.5.0/barman/config.py
--rw-r--r--   0     1001      123    88904 2023-03-29 17:06:23.000000 barman-3.5.0/barman/backup_executor.py
--rw-r--r--   0     1001      123    49647 2023-03-29 17:06:23.000000 barman-3.5.0/barman/copy_controller.py
--rw-r--r--   0     1001      123      890 2023-03-29 17:06:23.000000 barman-3.5.0/barman/__init__.py
--rw-r--r--   0     1001      123    63696 2023-03-29 17:06:23.000000 barman-3.5.0/barman/postgres.py
--rw-r--r--   0     1001      123    81394 2023-03-29 17:06:23.000000 barman-3.5.0/barman/recovery_executor.py
--rw-r--r--   0     1001      123     5491 2023-03-29 17:06:23.000000 barman-3.5.0/barman/backup_manifest.py
--rw-r--r--   0     1001      123    77879 2023-03-29 17:06:23.000000 barman-3.5.0/barman/output.py
--rw-r--r--   0     1001      123    45270 2023-03-29 17:06:23.000000 barman-3.5.0/barman/command_wrappers.py
--rw-r--r--   0     1001      123    61294 2023-03-29 17:06:23.000000 barman-3.5.0/barman/backup.py
--rw-r--r--   0     1001      123    68305 2023-03-29 17:06:23.000000 barman-3.5.0/barman/cli.py
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/barman/storage/
--rw-r--r--   0     1001      123     1679 2023-03-29 17:06:23.000000 barman-3.5.0/barman/storage/file_stats.py
--rw-r--r--   0     1001      123      724 2023-03-29 17:06:23.000000 barman-3.5.0/barman/storage/__init__.py
--rw-r--r--   0     1001      123     1799 2023-03-29 17:06:23.000000 barman-3.5.0/barman/storage/file_manager.py
--rw-r--r--   0     1001      123     2397 2023-03-29 17:06:23.000000 barman-3.5.0/barman/storage/local_file_manager.py
--rw-r--r--   0     1001      123    19109 2023-03-29 17:06:23.000000 barman-3.5.0/barman/retention_policies.py
--rw-r--r--   0     1001      123     9554 2023-03-29 17:06:23.000000 barman-3.5.0/barman/exceptions.py
--rw-r--r--   0     1001      123     4215 2023-03-29 17:06:23.000000 barman-3.5.0/barman/postgres_plumbing.py
--rw-r--r--   0     1001      123    33055 2023-03-29 17:06:23.000000 barman-3.5.0/barman/compression.py
--rw-r--r--   0     1001      123      805 2023-03-29 17:06:51.000000 barman-3.5.0/barman/version.py
--rw-r--r--   0     1001      123    28226 2023-03-29 17:06:23.000000 barman-3.5.0/barman/infofile.py
--rw-r--r--   0     1001      123    93358 2023-03-29 17:06:23.000000 barman-3.5.0/barman/cloud.py
--rw-r--r--   0     1001      123    11394 2023-03-29 17:06:23.000000 barman-3.5.0/barman/hooks.py
--rw-r--r--   0     1001      123     2315 2023-03-29 17:06:23.000000 barman-3.5.0/barman/remote_status.py
--rwxr-xr-x   0     1001      123     4864 2023-03-29 17:06:23.000000 barman-3.5.0/setup.py
-drwxr-xr-x   0     1001      123        0 2023-03-29 17:06:53.000000 barman-3.5.0/barman.egg-info/
--rw-r--r--   0     1001      123        1 2023-03-29 17:06:53.000000 barman-3.5.0/barman.egg-info/dependency_links.txt
--rw-r--r--   0     1001      123      729 2023-03-29 17:06:53.000000 barman-3.5.0/barman.egg-info/entry_points.txt
--rw-r--r--   0     1001      123     9338 2023-03-29 17:06:53.000000 barman-3.5.0/barman.egg-info/SOURCES.txt
--rw-r--r--   0     1001      123     1447 2023-03-29 17:06:53.000000 barman-3.5.0/barman.egg-info/PKG-INFO
--rw-r--r--   0     1001      123      205 2023-03-29 17:06:53.000000 barman-3.5.0/barman.egg-info/requires.txt
--rw-r--r--   0     1001      123        7 2023-03-29 17:06:53.000000 barman-3.5.0/barman.egg-info/top_level.txt
--rw-r--r--   0     1001      123      280 2023-03-29 17:06:53.000000 barman-3.5.0/setup.cfg
--rw-r--r--   0     1001      123     1259 2023-03-29 17:06:23.000000 barman-3.5.0/AUTHORS
--rw-r--r--   0     1001      123    54721 2023-03-29 17:06:23.000000 barman-3.5.0/NEWS
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/build/
+-rwxr-xr-x   0     1001      123     1417 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/build
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/build/templates/
+-rw-r--r--   0     1001      123    81089 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/logo-horizontal-hires.png
+-rw-r--r--   0     1001      123     6346 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/default.latex
+-rw-r--r--   0     1001      123      161 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/default.yaml
+-rw-r--r--   0     1001      123    16668 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/postgres.pdf
+-rw-r--r--   0     1001      123     3895 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/edb-enterprisedb-logo.png
+-rw-r--r--   0     1001      123   102895 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/logo-hires.png
+-rw-r--r--   0     1001      123     9952 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/Barman.tex
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/build/html-templates/
+-rw-r--r--   0     1001      123     3838 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/template-utils.html
+-rw-r--r--   0     1001      123     1187 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/barman.css
+-rw-r--r--   0     1001      123    21298 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/docs.css
+-rw-r--r--   0     1001      123      238 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/SOURCES.md
+-rw-r--r--   0     1001      123   147074 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/bootstrap.css
+-rw-r--r--   0     1001      123     5572 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/template.html
+-rw-r--r--   0     1001      123      111 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/template.css
+-rw-r--r--   0     1001      123     3520 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/template-cli.html
+-rw-r--r--   0     1001      123     1092 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/override.css
+-rw-r--r--   0     1001      123     1750 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/Makefile
+-rw-r--r--   0     1001      123     2240 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-wal-archive.1.md
+-rw-r--r--   0     1001      123       47 2023-06-15 12:24:22.000000 barman-3.6.0/doc/.gitignore
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/barman.5.d/
+-rw-r--r--   0     1001      123      537 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/30-configuration-file-directory.md
+-rw-r--r--   0     1001      123      244 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_compression_workers.md
+-rw-r--r--   0     1001      123      405 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_compression_format.md
+-rw-r--r--   0     1001      123       80 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-log_level.md
+-rw-r--r--   0     1001      123      505 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-active.md
+-rw-r--r--   0     1001      123      472 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-last_backup_maximum_age.md
+-rw-r--r--   0     1001      123     1055 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-primary_conninfo.md
+-rw-r--r--   0     1001      123      220 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-parallel_jobs.md
+-rw-r--r--   0     1001      123      210 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/20-configuration-file-locations.md
+-rw-r--r--   0     1001      123      463 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-immediate_checkpoint.md
+-rw-r--r--   0     1001      123      117 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-parallel_jobs_start_batch_size.md
+-rw-r--r--   0     1001      123      222 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-azure_credential.md
+-rw-r--r--   0     1001      123       52 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-log_file.md
+-rw-r--r--   0     1001      123      144 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_archive_script.md
+-rw-r--r--   0     1001      123      440 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_archive_retry_script.md
+-rw-r--r--   0     1001      123      379 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_wal_delete_retry_script.md
+-rw-r--r--   0     1001      123      162 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-custom_decompression_filter.md
+-rw-r--r--   0     1001      123      487 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-reuse_backup.md
+-rw-r--r--   0     1001      123      367 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-last_wal_maximum_age.md
+-rw-r--r--   0     1001      123      179 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-check_timeout.md
+-rw-r--r--   0     1001      123      139 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_wal_delete_script.md
+-rw-r--r--   0     1001      123       79 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_recovery_script.md
+-rw-r--r--   0     1001      123      110 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/00-header.md
+-rw-r--r--   0     1001      123      272 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/15-description.md
+-rw-r--r--   0     1001      123      757 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_method.md
+-rw-r--r--   0     1001      123       97 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_wal_delete_script.md
+-rw-r--r--   0     1001      123       79 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-retention_policy_mode.md
+-rw-r--r--   0     1001      123      174 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/99-copying.md
+-rw-r--r--   0     1001      123      263 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-gcp-zone.md
+-rw-r--r--   0     1001      123      992 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_options.md
+-rw-r--r--   0     1001      123      186 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-snapshot-instance.md
+-rw-r--r--   0     1001      123      275 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_compression_level.md
+-rw-r--r--   0     1001      123       10 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/45-options.md
+-rw-r--r--   0     1001      123      237 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_archiver_name.md
+-rw-r--r--   0     1001      123       88 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-ssh_command.md
+-rw-r--r--   0     1001      123       66 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-description.md
+-rw-r--r--   0     1001      123      411 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-archiver_batch_size.md
+-rw-r--r--   0     1001      123      413 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_delete_retry_script.md
+-rw-r--r--   0     1001      123      172 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_backup_name.md
+-rw-r--r--   0     1001      123       83 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-barman_lock_directory.md
+-rw-r--r--   0     1001      123      464 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-archiver.md
+-rw-r--r--   0     1001      123       63 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-wals_directory.md
+-rw-r--r--   0     1001      123       86 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_directory.md
+-rw-r--r--   0     1001      123      328 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-compression.md
+-rw-r--r--   0     1001      123      109 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_archive_script.md
+-rw-r--r--   0     1001      123      229 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/25-configuration-file-syntax.md
+-rw-r--r--   0     1001      123       59 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/05-name.md
+-rw-r--r--   0     1001      123      212 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-snapshot-provider.md
+-rw-r--r--   0     1001      123      213 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-errors_directory.md
+-rw-r--r--   0     1001      123      365 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-recovery_options.md
+-rw-r--r--   0     1001      123      441 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_archiver_batch_size.md
+-rw-r--r--   0     1001      123      388 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_archive_retry_script.md
+-rw-r--r--   0     1001      123       91 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-minimum_redundancy.md
+-rw-r--r--   0     1001      123      267 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-tablespace_bandwidth_limit.md
+-rw-r--r--   0     1001      123      363 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_recovery_retry_script.md
+-rw-r--r--   0     1001      123      294 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-azure_subscription_id.md
+-rw-r--r--   0     1001      123      539 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_compression.md
+-rw-r--r--   0     1001      123      300 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-azure_resource_group.md
+-rw-r--r--   0     1001      123      129 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_delete_script.md
+-rw-r--r--   0     1001      123      403 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_backup_retry_script.md
+-rw-r--r--   0     1001      123      155 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/95-resources.md
+-rw-r--r--   0     1001      123      129 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-incoming_wals_directory.md
+-rw-r--r--   0     1001      123      405 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_recovery_retry_script.md
+-rw-r--r--   0     1001      123      247 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-network_compression.md
+-rw-r--r--   0     1001      123       79 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-basebackups_directory.md
+-rw-r--r--   0     1001      123      130 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-wal_retention_policy.md
+-rw-r--r--   0     1001      123      762 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/75-example.md
+-rw-r--r--   0     1001      123      593 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/90-authors.md
+-rw-r--r--   0     1001      123      250 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-create_slot.md
+-rw-r--r--   0     1001      123      512 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-custom_compression_magic.md
+-rw-r--r--   0     1001      123      652 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-recovery_staging_path.md
+-rw-r--r--   0     1001      123      252 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-max_incoming_wals_queue.md
+-rw-r--r--   0     1001      123      174 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_conninfo.md
+-rw-r--r--   0     1001      123      362 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_backup_retry_script.md
+-rw-r--r--   0     1001      123      239 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_compression_location.md
+-rw-r--r--   0     1001      123       26 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/80-see-also.md
+-rw-r--r--   0     1001      123      138 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-parallel_jobs_start_batch_period.md
+-rw-r--r--   0     1001      123      176 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-bandwidth_limit.md
+-rw-r--r--   0     1001      123      119 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_recovery_script.md
+-rw-r--r--   0     1001      123       80 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_backup_script.md
+-rw-r--r--   0     1001      123      366 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-conninfo.md
+-rw-r--r--   0     1001      123      233 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-path_prefix.md
+-rw-r--r--   0     1001      123      653 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-retention_policy.md
+-rw-r--r--   0     1001      123      359 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-primary_ssh_command.md
+-rw-r--r--   0     1001      123      118 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_backup_script.md
+-rw-r--r--   0     1001      123      651 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_archiver.md
+-rw-r--r--   0     1001      123       91 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_delete_script.md
+-rw-r--r--   0     1001      123      373 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_delete_retry_script.md
+-rw-r--r--   0     1001      123      546 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-last_backup_minimum_size.md
+-rw-r--r--   0     1001      123      368 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-forward-config-path.md
+-rw-r--r--   0     1001      123      163 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_wals_directory.md
+-rw-r--r--   0     1001      123      192 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-basebackup_retry_sleep.md
+-rw-r--r--   0     1001      123      100 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-custom_compression_filter.md
+-rw-r--r--   0     1001      123      425 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_wal_delete_retry_script.md
+-rw-r--r--   0     1001      123       56 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-barman_home.md
+-rw-r--r--   0     1001      123      202 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-snapshot-disks.md
+-rw-r--r--   0     1001      123     1545 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/70-hook-scripts.md
+-rw-r--r--   0     1001      123      171 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-slot_name.md
+-rw-r--r--   0     1001      123      183 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-basebackup_retry_times.md
+-rw-r--r--   0     1001      123      275 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-gcp-project.md
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/runbooks/
+-rw-r--r--   0     1001      123     9399 2023-06-15 12:24:22.000000 barman-3.6.0/doc/runbooks/snapshot_recovery_azure.md
+-rw-r--r--   0     1001      123    31574 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5
+-rw-r--r--   0     1001      123     5531 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-keep.1.md
+-rw-r--r--   0     1001      123     6536 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-restore.1.md
+-rw-r--r--   0     1001      123     6500 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-list.1
+-rw-r--r--   0     1001      123    11659 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-wal-archive.1
+-rw-r--r--   0     1001      123     5329 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-check-wal-archive.1.md
+-rw-r--r--   0     1001      123     9020 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-delete.1
+-rw-r--r--   0     1001      123     5369 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-wal-restore.1.md
+-rw-r--r--   0     1001      123     5215 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-show.1.md
+-rw-r--r--   0     1001      123    11338 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup.1.md
+-rw-r--r--   0     1001      123     5106 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-list.1.md
+-rw-r--r--   0     1001      123    26819 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1
+-rw-r--r--   0     1001      123     8813 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-wal-archive.1.md
+-rw-r--r--   0     1001      123     8362 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-restore.1
+-rw-r--r--   0     1001      123     6872 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-wal-restore.1
+-rw-r--r--   0     1001      123      706 2023-06-15 12:24:22.000000 barman-3.6.0/doc/Dockerfile
+-rw-r--r--   0     1001      123     3066 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-wal-restore.1.md
+-rw-r--r--   0     1001      123     6645 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-show.1
+-rw-r--r--   0     1001      123     7164 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-delete.1.md
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/barman.d/
+-rw-r--r--   0     1001      123      950 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.d/passive-server.conf-template
+-rw-r--r--   0     1001      123     1546 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.d/ssh-server.conf-template
+-rw-r--r--   0     1001      123     1500 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.d/streaming-server.conf-template
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/barman.1.d/
+-rw-r--r--   0     1001      123      788 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-list-files.md
+-rw-r--r--   0     1001      123      241 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-show-servers.md
+-rw-r--r--   0     1001      123       41 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/10-synopsis.md
+-rw-r--r--   0     1001      123      368 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-sync-backup.md
+-rw-r--r--   0     1001      123       81 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-switch-xlog.md
+-rw-r--r--   0     1001      123      347 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/85-bugs.md
+-rw-r--r--   0     1001      123      110 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/00-header.md
+-rw-r--r--   0     1001      123      272 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/15-description.md
+-rw-r--r--   0     1001      123      174 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/99-copying.md
+-rw-r--r--   0     1001      123       55 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/45-commands.md
+-rw-r--r--   0     1001      123      295 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-rebuild-xlogdb.md
+-rw-r--r--   0     1001      123      850 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-switch-wal.md
+-rw-r--r--   0     1001      123     3139 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-backup.md
+-rw-r--r--   0     1001      123       74 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-list-servers.md
+-rw-r--r--   0     1001      123       98 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-generate-manifest.md
+-rw-r--r--   0     1001      123     1048 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-get-wal.md
+-rw-r--r--   0     1001      123       61 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-verify.md
+-rw-r--r--   0     1001      123     5849 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-recover.md
+-rw-r--r--   0     1001      123      393 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-check.md
+-rw-r--r--   0     1001      123       51 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/75-exit-status.md
+-rw-r--r--   0     1001      123       60 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/05-name.md
+-rw-r--r--   0     1001      123      279 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-cron.md
+-rw-r--r--   0     1001      123      798 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-status.md
+-rw-r--r--   0     1001      123      668 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-receive-wal.md
+-rw-r--r--   0     1001      123      155 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/95-resources.md
+-rw-r--r--   0     1001      123      333 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-check-backup.md
+-rw-r--r--   0     1001      123     1268 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-keep.md
+-rw-r--r--   0     1001      123      270 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-diagnose.md
+-rw-r--r--   0     1001      123      596 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/20-options.md
+-rw-r--r--   0     1001      123      621 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/90-authors.md
+-rw-r--r--   0     1001      123      701 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-put-wal.md
+-rw-r--r--   0     1001      123      642 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-sync-info.md
+-rw-r--r--   0     1001      123       26 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/80-see-also.md
+-rw-r--r--   0     1001      123      291 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-list-backups.md
+-rw-r--r--   0     1001      123      143 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-delete.md
+-rw-r--r--   0     1001      123      578 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-replication-status.md
+-rw-r--r--   0     1001      123      351 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-sync-wals.md
+-rw-r--r--   0     1001      123      590 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-check-wal-archive.md
+-rw-r--r--   0     1001      123      266 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-archive-wal.md
+-rw-r--r--   0     1001      123      265 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-verify-backup.md
+-rw-r--r--   0     1001      123     1420 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-show-backup.md
+-rw-r--r--   0     1001      123      444 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/70-backup-id-shortcuts.md
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/images/
+-rw-r--r--   0     1001      123   228769 2023-06-15 12:24:22.000000 barman-3.6.0/doc/images/barman-architecture-scenario2b.png
+-rw-r--r--   0     1001      123   157428 2023-06-15 12:24:22.000000 barman-3.6.0/doc/images/barman-architecture-georedundancy.png
+-rw-r--r--   0     1001      123   179610 2023-06-15 12:24:22.000000 barman-3.6.0/doc/images/barman-architecture-scenario1.png
+-rw-r--r--   0     1001      123   227695 2023-06-15 12:24:22.000000 barman-3.6.0/doc/images/barman-architecture-scenario1b.png
+-rw-r--r--   0     1001      123   201845 2023-06-15 12:24:22.000000 barman-3.6.0/doc/images/barman-architecture-scenario2.png
+-rw-r--r--   0     1001      123     3622 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-wal-restore.1
+-rw-r--r--   0     1001      123     7082 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-keep.1
+-rw-r--r--   0     1001      123    14779 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup.1
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/manual/
+-rw-r--r--   0     1001      123     5283 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/24-wal_archiving.en.md
+-rw-r--r--   0     1001      123       43 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/.gitignore
+-rw-r--r--   0     1001      123     2914 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/15-system_requirements.en.md
+-rw-r--r--   0     1001      123     4309 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/99-references.en.md
+-rw-r--r--   0     1001      123     1335 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/30-windows-support.en.md
+-rw-r--r--   0     1001      123    49424 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/50-feature-details.en.md
+-rw-r--r--   0     1001      123    13511 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/43-backup-commands.en.md
+-rw-r--r--   0     1001      123     1083 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/25-streaming_backup.en.md
+-rw-r--r--   0     1001      123     2629 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/41-global-commands.en.md
+-rw-r--r--   0     1001      123     5034 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/23-wal_streaming.en.md
+-rw-r--r--   0     1001      123     1017 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/26-rsync_backup.en.md
+-rw-r--r--   0     1001      123     3665 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/66-about.en.md
+-rw-r--r--   0     1001      123    11271 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/42-server-commands.en.md
+-rw-r--r--   0     1001      123      784 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/00-head.en.md
+-rw-r--r--   0     1001      123      823 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/20-server_setup.en.md
+-rw-r--r--   0     1001      123     8659 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/16-installation.en.md
+-rw-r--r--   0     1001      123    10341 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/55-barman-cli.en.md
+-rw-r--r--   0     1001      123     6706 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/28-snapshots.en.md
+-rw-r--r--   0     1001      123      667 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/Makefile
+-rw-r--r--   0     1001      123      862 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/22-config_file.en.md
+-rw-r--r--   0     1001      123     1001 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/02-before_you_start.en.md
+-rw-r--r--   0     1001      123    11160 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/10-design.en.md
+-rw-r--r--   0     1001      123     4014 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/01-intro.en.md
+-rw-r--r--   0     1001      123     9313 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/21-preliminary_steps.en.md
+-rw-r--r--   0     1001      123     1732 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/65-troubleshooting.en.md
+-rw-r--r--   0     1001      123     3564 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/17-configuration.en.md
+-rw-r--r--   0     1001      123     6807 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-check-wal-archive.1
+-rw-r--r--   0     1001      123     2331 2023-06-15 12:24:22.000000 barman-3.6.0/doc/Makefile
+-rw-r--r--   0     1001      123     2630 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-wal-archive.1
+-rw-r--r--   0     1001      123     3501 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.conf
+-rw-r--r--   0     1001      123     2193 2023-06-15 12:24:22.000000 barman-3.6.0/README.rst
+-rw-r--r--   0     1001      123    35147 2023-06-15 12:24:22.000000 barman-3.6.0/LICENSE
+-rw-r--r--   0     1001      123      196 2023-06-15 12:24:22.000000 barman-3.6.0/MANIFEST.in
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/
+-rw-r--r--   0     1001      123        1 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/dependency_links.txt
+-rw-r--r--   0     1001      123      258 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/requires.txt
+-rw-r--r--   0     1001      123        7 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/top_level.txt
+-rw-r--r--   0     1001      123     9589 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/SOURCES.txt
+-rw-r--r--   0     1001      123      729 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/entry_points.txt
+-rw-r--r--   0     1001      123     1479 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/PKG-INFO
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/barman/
+-rw-r--r--   0     1001      123      890 2023-06-15 12:24:22.000000 barman-3.6.0/barman/__init__.py
+-rw-r--r--   0     1001      123   164482 2023-06-15 12:24:22.000000 barman-3.6.0/barman/server.py
+-rw-r--r--   0     1001      123    42482 2023-06-15 12:24:22.000000 barman-3.6.0/barman/wal_archiver.py
+-rw-r--r--   0     1001      123    11394 2023-06-15 12:24:22.000000 barman-3.6.0/barman/hooks.py
+-rw-r--r--   0     1001      123     4343 2023-06-15 12:24:22.000000 barman-3.6.0/barman/diagnose.py
+-rw-r--r--   0     1001      123    69167 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cli.py
+-rw-r--r--   0     1001      123    77879 2023-06-15 12:24:22.000000 barman-3.6.0/barman/output.py
+-rw-r--r--   0     1001      123    19890 2023-06-15 12:24:22.000000 barman-3.6.0/barman/fs.py
+-rw-r--r--   0     1001      123    12760 2023-06-15 12:24:22.000000 barman-3.6.0/barman/annotations.py
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/barman/clients/
+-rw-r--r--   0     1001      123    14774 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_backup_delete.py
+-rw-r--r--   0     1001      123      724 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/__init__.py
+-rwxr-xr-x   0     1001      123    11355 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_walarchive.py
+-rw-r--r--   0     1001      123     6705 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_walrestore.py
+-rw-r--r--   0     1001      123     4344 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_backup_keep.py
+-rw-r--r--   0     1001      123     3720 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_backup_show.py
+-rwxr-xr-x   0     1001      123    16333 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/walrestore.py
+-rw-r--r--   0     1001      123    13672 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_restore.py
+-rw-r--r--   0     1001      123     4438 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_backup_list.py
+-rw-r--r--   0     1001      123     3147 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_check_wal_archive.py
+-rwxr-xr-x   0     1001      123    11331 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/walarchive.py
+-rw-r--r--   0     1001      123     6302 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_compression.py
+-rw-r--r--   0     1001      123     6339 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_cli.py
+-rwxr-xr-x   0     1001      123    14285 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_backup.py
+-rw-r--r--   0     1001      123    19109 2023-06-15 12:24:22.000000 barman-3.6.0/barman/retention_policies.py
+-rw-r--r--   0     1001      123     4215 2023-06-15 12:24:22.000000 barman-3.6.0/barman/postgres_plumbing.py
+-rw-r--r--   0     1001      123     5959 2023-06-15 12:24:22.000000 barman-3.6.0/barman/process.py
+-rw-r--r--   0     1001      123    95393 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cloud.py
+-rw-r--r--   0     1001      123    16411 2023-06-15 12:24:22.000000 barman-3.6.0/barman/xlog.py
+-rw-r--r--   0     1001      123     2315 2023-06-15 12:24:22.000000 barman-3.6.0/barman/remote_status.py
+-rw-r--r--   0     1001      123    45270 2023-06-15 12:24:22.000000 barman-3.6.0/barman/command_wrappers.py
+-rw-r--r--   0     1001      123    49647 2023-06-15 12:24:22.000000 barman-3.6.0/barman/copy_controller.py
+-rw-r--r--   0     1001      123     5491 2023-06-15 12:24:22.000000 barman-3.6.0/barman/backup_manifest.py
+-rw-r--r--   0     1001      123    33055 2023-06-15 12:24:22.000000 barman-3.6.0/barman/compression.py
+-rw-r--r--   0     1001      123     9554 2023-06-15 12:24:22.000000 barman-3.6.0/barman/exceptions.py
+-rw-r--r--   0     1001      123    61344 2023-06-15 12:24:22.000000 barman-3.6.0/barman/backup.py
+-rw-r--r--   0     1001      123    40522 2023-06-15 12:24:22.000000 barman-3.6.0/barman/config.py
+-rw-r--r--   0     1001      123    89029 2023-06-15 12:24:22.000000 barman-3.6.0/barman/backup_executor.py
+-rw-r--r--   0     1001      123    11374 2023-06-15 12:24:22.000000 barman-3.6.0/barman/lockfile.py
+-rw-r--r--   0     1001      123    28226 2023-06-15 12:24:22.000000 barman-3.6.0/barman/infofile.py
+-rw-r--r--   0     1001      123    25604 2023-06-15 12:24:22.000000 barman-3.6.0/barman/utils.py
+-rw-r--r--   0     1001      123    63696 2023-06-15 12:24:22.000000 barman-3.6.0/barman/postgres.py
+-rw-r--r--   0     1001      123    81412 2023-06-15 12:24:22.000000 barman-3.6.0/barman/recovery_executor.py
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/barman/storage/
+-rw-r--r--   0     1001      123      724 2023-06-15 12:24:22.000000 barman-3.6.0/barman/storage/__init__.py
+-rw-r--r--   0     1001      123     1799 2023-06-15 12:24:22.000000 barman-3.6.0/barman/storage/file_manager.py
+-rw-r--r--   0     1001      123     1679 2023-06-15 12:24:22.000000 barman-3.6.0/barman/storage/file_stats.py
+-rw-r--r--   0     1001      123     2397 2023-06-15 12:24:22.000000 barman-3.6.0/barman/storage/local_file_manager.py
+-rw-r--r--   0     1001      123      805 2023-06-15 12:24:43.000000 barman-3.6.0/barman/version.py
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/barman/cloud_providers/
+-rw-r--r--   0     1001      123    12220 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cloud_providers/__init__.py
+-rw-r--r--   0     1001      123    14428 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cloud_providers/aws_s3.py
+-rw-r--r--   0     1001      123    39481 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cloud_providers/azure_blob_storage.py
+-rw-r--r--   0     1001      123    30678 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cloud_providers/google_cloud_storage.py
+-rw-r--r--   0     1001      123    55839 2023-06-15 12:24:22.000000 barman-3.6.0/NEWS
+drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/scripts/
+-rw-r--r--   0     1001      123       98 2023-06-15 12:24:22.000000 barman-3.6.0/scripts/barman.bash_completion
+-rwxr-xr-x   0     1001      123     4933 2023-06-15 12:24:22.000000 barman-3.6.0/setup.py
+-rw-r--r--   0     1001      123      280 2023-06-15 12:24:44.000000 barman-3.6.0/setup.cfg
+-rw-r--r--   0     1001      123     1479 2023-06-15 12:24:44.000000 barman-3.6.0/PKG-INFO
+-rw-r--r--   0     1001      123     1277 2023-06-15 12:24:22.000000 barman-3.6.0/AUTHORS
```

### Comparing `barman-3.5.0/doc/barman-wal-restore.1` & `barman-3.6.0/doc/barman-wal-restore.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-WAL\-RESTORE" "1" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN\-WAL\-RESTORE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
 barman\-wal\-restore \- \[aq]restore_command\[aq] based on Barman\[aq]s
 get\-wal
 .SH SYNOPSIS
 .PP
```

### Comparing `barman-3.5.0/doc/barman-cloud-wal-restore.1` & `barman-3.6.0/doc/barman-cloud-wal-restore.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-WAL\-RESTORE" "1" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN\-CLOUD\-WAL\-RESTORE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-wal\-restore \- Restore PostgreSQL WAL files from the
 Cloud using \f[C]restore_command\f[]
 .SH SYNOPSIS
 .PP
@@ -24,15 +24,15 @@
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-wal\-restore\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-credential\ {azure\-cli,managed\-identity}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name\ wal_name\ wal_dest
 
 This\ script\ can\ be\ used\ as\ a\ `restore_command`\ to\ download\ WAL\ files
 previously\ archived\ with\ barman\-cloud\-wal\-archive\ command.\ Currently\ AWS\ S3,
 Azure\ Blob\ Storage\ and\ Google\ Cloud\ Storage\ are\ supported.
 
 positional\ arguments:
@@ -61,21 +61,23 @@
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
-\ \ \-\-credential\ {azure\-cli,managed\-identity}
+\ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure\ Blob\ Storage.\ If\ omitted
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ then\ the\ credential\ will\ be\ obtained\ from\ the
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment.\ If\ no\ credentials\ can\ be\ found\ in\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used\ for\ authenticating\ with\ all\ other\ Azure
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ services.\ If\ no\ credentials\ can\ be\ found\ in\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ then\ the\ default\ Azure\ authentication\ flow
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ also\ be\ used\ for\ Azure\ Blob\ Storage.
 \f[]
 .fi
 .SH REFERENCES
 .PP
 For Boto:
 .IP \[bu] 2
 https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-cloud-backup-list.1` & `barman-3.6.0/doc/barman-cloud-backup-list.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-BACKUP\-LIST" "1" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN\-CLOUD\-BACKUP\-LIST" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-backup\-list \- List backups stored in the Cloud
 .SH SYNOPSIS
 .PP
 barman\-cloud\-backup\-list [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
@@ -22,15 +22,15 @@
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-backup\-list\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-credential\ {azure\-cli,managed\-identity}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-format\ FORMAT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name
 
 This\ script\ can\ be\ used\ to\ list\ backups\ made\ with\ barman\-cloud\-backup\ command.
 Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and\ Google\ Cloud\ Storage\ are\ supported.
 
 positional\ arguments:
@@ -56,21 +56,23 @@
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
-\ \ \-\-credential\ {azure\-cli,managed\-identity}
+\ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure\ Blob\ Storage.\ If\ omitted
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ then\ the\ credential\ will\ be\ obtained\ from\ the
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment.\ If\ no\ credentials\ can\ be\ found\ in\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used\ for\ authenticating\ with\ all\ other\ Azure
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ services.\ If\ no\ credentials\ can\ be\ found\ in\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ then\ the\ default\ Azure\ authentication\ flow
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ also\ be\ used\ for\ Azure\ Blob\ Storage.
 \f[]
 .fi
 .SH REFERENCES
 .PP
 For Boto:
 .IP \[bu] 2
 https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/Makefile` & `barman-3.6.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/50-recovery_staging_path.md` & `barman-3.6.0/doc/barman.5.d/50-recovery_staging_path.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/50-primary_conninfo.md` & `barman-3.6.0/doc/barman.5.d/50-primary_conninfo.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/50-last_backup_minimum_size.md` & `barman-3.6.0/doc/barman.5.d/50-last_backup_minimum_size.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/50-backup_method.md` & `barman-3.6.0/doc/barman.5.d/50-backup_method.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/50-custom_compression_magic.md` & `barman-3.6.0/doc/barman.5.d/50-custom_compression_magic.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/50-streaming_archiver.md` & `barman-3.6.0/doc/barman.5.d/50-streaming_archiver.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/70-hook-scripts.md` & `barman-3.6.0/doc/barman.5.d/70-hook-scripts.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/90-authors.md` & `barman-3.6.0/doc/barman.5.d/90-authors.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/30-configuration-file-directory.md` & `barman-3.6.0/doc/barman.5.d/30-configuration-file-directory.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/50-retention_policy.md` & `barman-3.6.0/doc/barman.5.d/50-retention_policy.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/75-example.md` & `barman-3.6.0/doc/barman.5.d/75-example.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/50-backup_options.md` & `barman-3.6.0/doc/barman.5.d/50-backup_options.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.5.d/50-backup_compression.md` & `barman-3.6.0/doc/barman.5.d/50-backup_compression.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/Makefile` & `barman-3.6.0/doc/build/Makefile`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/build` & `barman-3.6.0/doc/build/build`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/templates/logo-hires.png` & `barman-3.6.0/doc/build/templates/logo-hires.png`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/templates/postgres.pdf` & `barman-3.6.0/doc/build/templates/postgres.pdf`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/templates/logo-horizontal-hires.png` & `barman-3.6.0/doc/build/templates/logo-horizontal-hires.png`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/templates/Barman.tex` & `barman-3.6.0/doc/build/templates/Barman.tex`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/templates/default.latex` & `barman-3.6.0/doc/build/templates/default.latex`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/templates/edb-enterprisedb-logo.png` & `barman-3.6.0/doc/build/templates/edb-enterprisedb-logo.png`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/html-templates/docs.css` & `barman-3.6.0/doc/build/html-templates/docs.css`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/html-templates/template-cli.html` & `barman-3.6.0/doc/build/html-templates/template-cli.html`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/html-templates/barman.css` & `barman-3.6.0/doc/build/html-templates/barman.css`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/html-templates/template.html` & `barman-3.6.0/doc/build/html-templates/template.html`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/html-templates/template-utils.html` & `barman-3.6.0/doc/build/html-templates/template-utils.html`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/html-templates/bootstrap.css` & `barman-3.6.0/doc/build/html-templates/bootstrap.css`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/build/html-templates/override.css` & `barman-3.6.0/doc/build/html-templates/override.css`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman-cloud-restore.1.md` & `barman-3.6.0/doc/barman-cloud-restore.1.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-RESTORE(1) Barman User manuals | Version 3.5.0
+% BARMAN-CLOUD-RESTORE(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% March 29, 2023
+% June 15, 2023
 
 # NAME
 
 barman-cloud-restore - Restore a PostgreSQL backup from the Cloud
 
 
 # SYNOPSIS
@@ -28,18 +28,20 @@
 
 # Usage
 ```
 usage: barman-cloud-restore [-V] [--help] [-v | -q] [-t]
                             [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
                             [--endpoint-url ENDPOINT_URL] [-P PROFILE]
                             [--read-timeout READ_TIMEOUT]
-                            [--credential {azure-cli,managed-identity}]
+                            [--azure-credential {azure-cli,managed-identity}]
                             [--tablespace NAME:LOCATION]
                             [--snapshot-recovery-instance SNAPSHOT_RECOVERY_INSTANCE]
-                            [--snapshot-recovery-zone SNAPSHOT_RECOVERY_ZONE]
+                            [--snapshot-recovery-zone GCP_ZONE]
+                            [--gcp-zone GCP_ZONE]
+                            [--azure-resource-group AZURE_RESOURCE_GROUP]
                             source_url server_name backup_id recovery_dir
 
 This script can be used to download a backup previously made with barman-
 cloud-backup command.Currently AWS S3, Azure Blob Storage and Google Cloud
 Storage are supported.
 
 positional arguments:
@@ -58,37 +60,46 @@
   --cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}
                         The cloud provider to use as a storage backend
   --tablespace NAME:LOCATION
                         tablespace relocation rule
   --snapshot-recovery-instance SNAPSHOT_RECOVERY_INSTANCE
                         Instance where the disks recovered from the snapshots
                         are attached
-  --snapshot-recovery-zone SNAPSHOT_RECOVERY_ZONE
+  --snapshot-recovery-zone GCP_ZONE
                         Zone containing the instance and disks for the
-                        snapshot recovery
+                        snapshot recovery (deprecated: replaced by --gcp-zone)
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
   -P PROFILE, --profile PROFILE
                         profile name (e.g. INI section in AWS credentials
                         file)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
-  --credential {azure-cli,managed-identity}
+  --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
-                        authenticating with Azure Blob Storage. If omitted
-                        then the credential will be obtained from the
-                        environment. If no credentials can be found in the
+                        authenticating with Azure. If omitted then Azure Blob
+                        Storage credentials will be obtained from the
+                        environment and the default Azure authentication flow
+                        will be used for authenticating with all other Azure
+                        services. If no credentials can be found in the
                         environment then the default Azure authentication flow
-                        will be used
+                        will also be used for Azure Blob Storage.
+  --azure-resource-group AZURE_RESOURCE_GROUP
+                        Resource group containing the instance and disks for
+                        the snapshot recovery
+
+Extra options for google-cloud-storage cloud provider:
+  --gcp-zone GCP_ZONE   Zone containing the instance and disks for the
+                        snapshot recovery
 ```
 # REFERENCES
 
 For Boto:
 
 * https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-cloud-backup-delete.1` & `barman-3.6.0/doc/barman-cloud-backup-delete.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-BACKUP\-DELETE" "1" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN\-CLOUD\-BACKUP\-DELETE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-backup\-delete \- Delete backups stored in the Cloud
 .SH SYNOPSIS
 .PP
 barman\-cloud\-backup\-delete [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
@@ -47,15 +47,15 @@
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-backup\-delete\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-credential\ {azure\-cli,managed\-identity}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ (\-b\ BACKUP_ID\ |\ \-r\ RETENTION_POLICY)
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-dry\-run]\ [\-\-batch\-size\ DELETE_BATCH_SIZE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name
 
 This\ script\ can\ be\ used\ to\ delete\ backups\ made\ with\ barman\-cloud\-backup
 command.\ Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and\ Google\ Cloud\ Storage\ are
 supported.
@@ -97,21 +97,23 @@
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
-\ \ \-\-credential\ {azure\-cli,managed\-identity}
+\ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure\ Blob\ Storage.\ If\ omitted
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ then\ the\ credential\ will\ be\ obtained\ from\ the
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment.\ If\ no\ credentials\ can\ be\ found\ in\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used\ for\ authenticating\ with\ all\ other\ Azure
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ services.\ If\ no\ credentials\ can\ be\ found\ in\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ then\ the\ default\ Azure\ authentication\ flow
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ also\ be\ used\ for\ Azure\ Blob\ Storage.
 \f[]
 .fi
 .SH REFERENCES
 .PP
 For Boto:
 .IP \[bu] 2
 https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman.5` & `barman-3.6.0/doc/barman.5`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN" "5" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN" "5" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
 barman \- Backup and Recovery Manager for PostgreSQL
 .SH DESCRIPTION
 .PP
 Barman is an administration tool for disaster recovery of PostgreSQL
@@ -92,14 +92,45 @@
 would limit itself to maximum \f[C]archiver_batch_size\f[] WAL segments
 per single run.
 Integer.
 Global/Server.
 .RS
 .RE
 .TP
+.B azure_credential
+The credential type (either \f[C]azure\-cli\f[] or
+\f[C]managed\-identity\f[]) to use when authenticating with Azure.
+If this is omitted then the default Azure authentication flow will be
+used.
+Global/Server.
+.RS
+.RE
+.TP
+.B azure_resource_group
+The name of the Azure resource group to which the compute instance and
+disks defined by \f[C]snapshot_instance\f[] and \f[C]snapshot_disks\f[]
+belong.
+Global/Server.
+Required when the \f[C]snapshot\f[] value is specified for
+\f[C]backup_method\f[] and \f[C]snapshot_provider\f[] is set to
+\f[C]azure\f[].
+.RS
+.RE
+.TP
+.B azure_subscription_id
+The ID of the Azure subscription which owns the instance and storage
+volumes defined by \f[C]snapshot_instance\f[] and
+\f[C]snapshot_disks\f[].
+Global/Server.
+Required when the \f[C]snapshot\f[] value is specified for
+\f[C]backup_method\f[] and \f[C]snapshot_provider\f[] is set to
+\f[C]azure\f[].
+.RS
+.RE
+.TP
 .B backup_compression
 The compression to be used during the backup process.
 Only supported when \f[C]backup_method\ =\ postgres\f[].
 Can either be unset or \f[C]gzip\f[],\f[C]lz4\f[] or \f[C]zstd\f[].
 If unset then no compression will be used during the backup.
 Use of this option requires that the CLI application for the specified
 compression algorithm is available on the Barman server (at backup time)
@@ -329,14 +360,34 @@
 Set to true if you are invoking barman with the \f[C]\-c/\-\-config\f[]
 option and your configuration is in the same place on both the passive
 and primary barman servers.
 Defaults to false.
 .RS
 .RE
 .TP
+.B gcp_project
+The ID of the GCP project which owns the instance and storage volumes
+defined by \f[C]snapshot_instance\f[] and \f[C]snapshot_disks\f[].
+Global/Server.
+Required when the \f[C]snapshot\f[] value is specified for
+\f[C]backup_method\f[] and \f[C]snapshot_provider\f[] is set to
+\f[C]gcp\f[].
+.RS
+.RE
+.TP
+.B gcp_zone
+The name of the availability zone where the compute instance and disks
+to be backed up in a snapshot backup are located.
+Server.
+Required when the \f[C]snapshot\f[] value is specified for
+\f[C]backup_method\f[] and \f[C]snapshot_provider\f[] is set to
+\f[C]gcp\f[].
+.RS
+.RE
+.TP
 .B immediate_checkpoint
 This option allows you to control the way PostgreSQL handles checkpoint
 at the start of the backup.
 If set to \f[C]false\f[] (default), the I/O workload for the checkpoint
 will be limited, according to the \f[C]checkpoint_completion_target\f[]
 setting on the PostgreSQL server.
 If set to \f[C]true\f[], an immediate checkpoint will be requested,
@@ -749,24 +800,14 @@
 taken using cloud snapshots.
 Server.
 Required when the \f[C]snapshot\f[] value is specified for
 \f[C]backup_method\f[].
 .RS
 .RE
 .TP
-.B snapshot_gcp_project
-The ID of the GCP project which owns the instance and storage volumes
-defined by \f[C]snapshot_instance\f[] and \f[C]snapshot_disks\f[].
-Global/Server.
-Required when the \f[C]snapshot\f[] value is specified for
-\f[C]backup_method\f[] and \f[C]snapshot_provider\f[] is set to
-\f[C]gcp\f[].
-.RS
-.RE
-.TP
 .B snapshot_instance
 The name of the VM or compute instance where the storage volumes are
 attached.
 Server.
 Required when the \f[C]snapshot\f[] value is specified for
 \f[C]backup_method\f[].
 .RS
@@ -777,23 +818,14 @@
 Global/Server.
 Required when the \f[C]snapshot\f[] value is specified for
 \f[C]backup_method\f[].
 Supported values: \f[C]gcp\f[].
 .RS
 .RE
 .TP
-.B snapshot_zone
-The name of the availability zone where the compute instance and disks
-to be backed up in a snapshot backup are located.
-Server.
-Required when the \f[C]snapshot\f[] value is specified for
-\f[C]backup_method\f[].
-.RS
-.RE
-.TP
 .B ssh_command
 Command used by Barman to login to the Postgres server via ssh.
 Server.
 .RS
 .RE
 .TP
 .B streaming_archiver
```

### Comparing `barman-3.5.0/doc/barman.1.d/50-sync-info.md` & `barman-3.6.0/doc/barman.1.d/50-sync-info.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-recover.md` & `barman-3.6.0/doc/barman.1.d/50-recover.md`

 * *Files 1% similar despite different names*

```diff
@@ -118,11 +118,11 @@
         can be used to write the recovery options to an alternative location.
 
     --snapshot-recovery-instance *INSTANCE_NAME*
     :   Name of the instance where the disks recovered from the snapshots are
         attached. This option is required when recovering backups made with
         `backup_method = snapshot`.
 
-    --snapshot-recovery-zone *ZONE_NAME*
+    --gcp-zone *ZONE_NAME*
     :   Name of the availability zone where the instance and disks for snapshot
         are located. This option is required when recovering backups made with
         `backup_method = snapshot`.
```

### Comparing `barman-3.5.0/doc/barman.1.d/50-keep.md` & `barman-3.6.0/doc/barman.1.d/50-keep.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/20-options.md` & `barman-3.6.0/doc/barman.1.d/20-options.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-check-wal-archive.md` & `barman-3.6.0/doc/barman.1.d/50-check-wal-archive.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-switch-wal.md` & `barman-3.6.0/doc/barman.1.d/50-switch-wal.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-receive-wal.md` & `barman-3.6.0/doc/barman.1.d/50-receive-wal.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-put-wal.md` & `barman-3.6.0/doc/barman.1.d/50-put-wal.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-backup.md` & `barman-3.6.0/doc/barman.1.d/50-backup.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-list-files.md` & `barman-3.6.0/doc/barman.1.d/50-list-files.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-show-backup.md` & `barman-3.6.0/doc/barman.1.d/50-show-backup.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-get-wal.md` & `barman-3.6.0/doc/barman.1.d/50-get-wal.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-status.md` & `barman-3.6.0/doc/barman.1.d/50-status.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/90-authors.md` & `barman-3.6.0/doc/barman.1.d/90-authors.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1.d/50-replication-status.md` & `barman-3.6.0/doc/barman.1.d/50-replication-status.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.1` & `barman-3.6.0/doc/barman.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN" "1" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
 barman \- Backup and Recovery Manager for PostgreSQL
 .SH SYNOPSIS
 .PP
 barman [\f[I]OPTIONS\f[]] \f[I]COMMAND\f[]
@@ -245,14 +245,19 @@
 Collect diagnostic information about the server where barman is
 installed and all the configured servers, including: global
 configuration, SSH version, Python version, \f[C]rsync\f[] version, as
 well as current configuration and status of all servers.
 .RS
 .RE
 .TP
+.B generate\-manifest \f[I]SERVER_NAME\f[] \f[I]BACKUP_ID\f[]
+Generates a backup_manifest file for a backup_id.
+.RS
+.RE
+.TP
 .B get\-wal \f[I][OPTIONS]\f[] \f[I]SERVER_NAME\f[] \f[I]WAL_NAME\f[]
 Retrieve a WAL file from the \f[C]xlog\f[] archive of a given server.
 By default, the requested WAL file, if found, is returned as
 uncompressed content to \f[C]STDOUT\f[].
 The following options allow users to change this behaviour:
 .RS
 .TP
@@ -622,15 +627,15 @@
 Name of the instance where the disks recovered from the snapshots are
 attached.
 This option is required when recovering backups made with
 \f[C]backup_method\ =\ snapshot\f[].
 .RS
 .RE
 .TP
-.B \-\-snapshot\-recovery\-zone \f[I]ZONE_NAME\f[]
+.B \-\-gcp\-zone \f[I]ZONE_NAME\f[]
 Name of the availability zone where the instance and disks for snapshot
 are located.
 This option is required when recovering backups made with
 \f[C]backup_method\ =\ snapshot\f[].
 .RS
 .RE
 .RE
@@ -810,14 +815,27 @@
 Executes a copy of all the archived WAL files that are present on
 \f[C]SERVER_NAME\f[] node.
 This command is available only for passive nodes, and uses the
 \f[C]primary_ssh_command\f[] option to establish a secure connection
 with the primary node.
 .RS
 .RE
+.TP
+.B verify\-backup \f[I]SERVER_NAME\f[] \f[I]BACKUP_ID\f[]
+Executes \f[C]pg_verifybackup\f[] against a backup manifest file
+(available since Postgres 13).
+For rsync backups, it can be used with generate\-manifest command.
+Requires \f[C]pg_verifybackup\f[] installed on the backup server
+.RS
+.RE
+.TP
+.B verify \f[I]SERVER_NAME\f[] \f[I]BACKUP_ID\f[]
+Alias for verify\-backup
+.RS
+.RE
 .SH BACKUP ID SHORTCUTS
 .PP
 Rather than using the timestamp backup ID, you can use any of the
 following shortcuts/aliases to identity a backup for a given server:
 .TP
 .B first
 Oldest available backup for that server, in chronological order.
```

### Comparing `barman-3.5.0/doc/images/barman-architecture-scenario1b.png` & `barman-3.6.0/doc/images/barman-architecture-scenario1b.png`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/images/barman-architecture-scenario2b.png` & `barman-3.6.0/doc/images/barman-architecture-scenario2b.png`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/images/barman-architecture-scenario1.png` & `barman-3.6.0/doc/images/barman-architecture-scenario1.png`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/images/barman-architecture-scenario2.png` & `barman-3.6.0/doc/images/barman-architecture-scenario2.png`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/images/barman-architecture-georedundancy.png` & `barman-3.6.0/doc/images/barman-architecture-georedundancy.png`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.d/ssh-server.conf-template` & `barman-3.6.0/doc/barman.d/ssh-server.conf-template`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.d/passive-server.conf-template` & `barman-3.6.0/doc/barman.d/passive-server.conf-template`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.d/streaming-server.conf-template` & `barman-3.6.0/doc/barman.d/streaming-server.conf-template`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman-cloud-backup.1.md` & `barman-3.6.0/doc/barman-cloud-backup.1.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-BACKUP(1) Barman User manuals | Version 3.5.0
+% BARMAN-CLOUD-BACKUP(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% March 29, 2023
+% June 15, 2023
 
 # NAME
 
 barman-cloud-backup - Backup a PostgreSQL instance and stores it in the Cloud
 
 
 # SYNOPSIS
@@ -40,26 +40,28 @@
 
 # Usage
 ```
 usage: barman-cloud-backup [-V] [--help] [-v | -q] [-t]
                            [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
                            [--endpoint-url ENDPOINT_URL] [-P PROFILE]
                            [--read-timeout READ_TIMEOUT]
-                           [--credential {azure-cli,managed-identity}]
+                           [--azure-credential {azure-cli,managed-identity}]
                            [-z | -j | --snappy] [-h HOST] [-p PORT] [-U USER]
                            [--immediate-checkpoint] [-J JOBS]
                            [-S MAX_ARCHIVE_SIZE] [-d DBNAME] [-n BACKUP_NAME]
                            [--snapshot-instance SNAPSHOT_INSTANCE]
-                           [--snapshot-disk NAME]
-                           [--snapshot-zone SNAPSHOT_ZONE]
-                           [--snapshot-gcp-project SNAPSHOT_GCP_PROJECT]
-                           [--kms-key-name KMS_KEY_NAME]
+                           [--snapshot-disk NAME] [--snapshot-zone GCP_ZONE]
+                           [--snapshot-gcp-project GCP_PROJECT]
+                           [--gcp-project GCP_PROJECT]
+                           [--kms-key-name KMS_KEY_NAME] [--gcp-zone GCP_ZONE]
                            [--tags [TAGS [TAGS ...]]] [-e {AES256,aws:kms}]
                            [--sse-kms-key-id SSE_KMS_KEY_ID]
                            [--encryption-scope ENCRYPTION_SCOPE]
+                           [--azure-subscription-id AZURE_SUBSCRIPTION_ID]
+                           [--azure-resource-group AZURE_RESOURCE_GROUP]
                            destination_url server_name
 
 This script can be used to perform a backup of a local PostgreSQL instance and
 ship the resulting tarball(s) to the Cloud. Currently AWS S3, Azure Blob
 Storage and Google Cloud Storage are supported.
 
 positional arguments:
@@ -99,16 +101,17 @@
                         a name which can be used to reference this backup in
                         commands such as barman-cloud-restore and barman-
                         cloud-backup-delete
   --snapshot-instance SNAPSHOT_INSTANCE
                         Instance where the disks to be backed up as snapshots
                         are attached
   --snapshot-disk NAME  Name of a disk from which snapshots should be taken
-  --snapshot-zone SNAPSHOT_ZONE
+  --snapshot-zone GCP_ZONE
                         Zone of the disks from which snapshots should be taken
+                        (deprecated: replaced by --gcp-zone)
   --tags [TAGS [TAGS ...]]
                         Tags to be added to all uploaded files in cloud
                         storage
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
@@ -126,32 +129,47 @@
   --sse-kms-key-id SSE_KMS_KEY_ID
                         The AWS KMS key ID that should be used for encrypting
                         the uploaded data in S3. Can be specified using the
                         key ID on its own or using the full ARN for the key.
                         Only allowed if `-e/--encryption` is set to `aws:kms`.
 
 Extra options for the azure-blob-storage cloud provider:
-  --credential {azure-cli,managed-identity}
+  --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
-                        authenticating with Azure Blob Storage. If omitted
-                        then the credential will be obtained from the
-                        environment. If no credentials can be found in the
+                        authenticating with Azure. If omitted then Azure Blob
+                        Storage credentials will be obtained from the
+                        environment and the default Azure authentication flow
+                        will be used for authenticating with all other Azure
+                        services. If no credentials can be found in the
                         environment then the default Azure authentication flow
-                        will be used
+                        will also be used for Azure Blob Storage.
   --encryption-scope ENCRYPTION_SCOPE
                         The name of an encryption scope defined in the Azure
                         Blob Storage service which is to be used to encrypt
                         the data in Azure
+  --azure-subscription-id AZURE_SUBSCRIPTION_ID
+                        The ID of the Azure subscription which owns the
+                        instance and storage volumes defined by the
+                        --snapshot-instance and --snapshot-disk arguments.
+  --azure-resource-group AZURE_RESOURCE_GROUP
+                        The name of the Azure resource group to which the
+                        compute instance and disks defined by the --snapshot-
+                        instance and --snapshot-disk arguments belong.
 
 Extra options for google-cloud-storage cloud provider:
-  --snapshot-gcp-project SNAPSHOT_GCP_PROJECT
-                        GCP project under which disk snapshots should be stored
+  --snapshot-gcp-project GCP_PROJECT
+                        GCP project under which disk snapshots should be
+                        stored (deprecated: replaced by --gcp-project)
+  --gcp-project GCP_PROJECT
+                        GCP project under which disk snapshots should be
+                        stored
   --kms-key-name KMS_KEY_NAME
                         The name of the GCP KMS key which should be used for
                         encrypting the uploaded data in GCS.
+  --gcp-zone GCP_ZONE   Zone of the disks from which snapshots should be taken
 ```
 # REFERENCES
 
 For Boto:
 
 * https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-wal-archive.1.md` & `barman-3.6.0/doc/barman-wal-archive.1.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-WAL-ARCHIVE(1) Barman User manuals | Version 3.5.0
+% BARMAN-WAL-ARCHIVE(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% March 29, 2023
+% June 15, 2023
 
 # NAME
 
 barman-wal-archive - `archive_command` based on Barman's put-wal
 
 
 # SYNOPSIS
```

### Comparing `barman-3.5.0/doc/barman-cloud-check-wal-archive.1` & `barman-3.6.0/doc/barman-cloud-check-wal-archive.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-CHECK\-WAL\-ARCHIVE" "1" "March 29, 2023" "Barman User manuals" "Version
-3.5.0"
+.TH "BARMAN\-CLOUD\-CHECK\-WAL\-ARCHIVE" "1" "June 15, 2023" "Barman User manuals" "Version
+3.6.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-check\-wal\-archive \- Check a WAL archive destination
 for a new PostgreSQL cluster
 .SH SYNOPSIS
 .PP
@@ -26,15 +26,15 @@
 .nf
 \f[C]
 usage:\ barman\-cloud\-check\-wal\-archive\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-P\ PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-credential\ {azure\-cli,managed\-identity}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-timeline\ TIMELINE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ destination_url\ server_name
 
 Checks\ that\ the\ WAL\ archive\ on\ the\ specified\ cloud\ storage\ can\ be\ safely\ used
 for\ a\ new\ PostgreSQL\ server.
 
 positional\ arguments:
@@ -61,21 +61,23 @@
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
-\ \ \-\-credential\ {azure\-cli,managed\-identity}
+\ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure\ Blob\ Storage.\ If\ omitted
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ then\ the\ credential\ will\ be\ obtained\ from\ the
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment.\ If\ no\ credentials\ can\ be\ found\ in\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used\ for\ authenticating\ with\ all\ other\ Azure
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ services.\ If\ no\ credentials\ can\ be\ found\ in\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ then\ the\ default\ Azure\ authentication\ flow
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ also\ be\ used\ for\ Azure\ Blob\ Storage.
 \f[]
 .fi
 .SH REFERENCES
 .PP
 For Boto:
 .IP \[bu] 2
 https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-cloud-wal-archive.1` & `barman-3.6.0/doc/barman-cloud-wal-archive.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-WAL\-ARCHIVE" "1" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN\-CLOUD\-WAL\-ARCHIVE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-wal\-archive \- Archive PostgreSQL WAL files in the Cloud
 using \f[C]archive_command\f[]
 .SH SYNOPSIS
 .PP
@@ -29,15 +29,15 @@
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-wal\-archive\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-credential\ {azure\-cli,managed\-identity}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-z\ |\ \-j\ |\ \-\-snappy]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-tags\ [TAGS\ [TAGS\ ...]]]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-history\-tags\ [HISTORY_TAGS\ [HISTORY_TAGS\ ...]]]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-kms\-key\-name\ KMS_KEY_NAME]\ [\-e\ ENCRYPTION]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-sse\-kms\-key\-id\ SSE_KMS_KEY_ID]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-encryption\-scope\ ENCRYPTION_SCOPE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-max\-block\-size\ MAX_BLOCK_SIZE]
@@ -94,21 +94,23 @@
 \ \ \-\-sse\-kms\-key\-id\ SSE_KMS_KEY_ID
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ AWS\ KMS\ key\ ID\ that\ should\ be\ used\ for\ encrypting
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ uploaded\ data\ in\ S3.\ Can\ be\ specified\ using\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ key\ ID\ on\ its\ own\ or\ using\ the\ full\ ARN\ for\ the\ key.
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Only\ allowed\ if\ `\-e/\-\-encryption`\ is\ set\ to\ `aws:kms`.
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
-\ \ \-\-credential\ {azure\-cli,managed\-identity}
+\ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure\ Blob\ Storage.\ If\ omitted
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ then\ the\ credential\ will\ be\ obtained\ from\ the
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment.\ If\ no\ credentials\ can\ be\ found\ in\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used\ for\ authenticating\ with\ all\ other\ Azure
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ services.\ If\ no\ credentials\ can\ be\ found\ in\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ then\ the\ default\ Azure\ authentication\ flow
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ also\ be\ used\ for\ Azure\ Blob\ Storage.
 \ \ \-\-encryption\-scope\ ENCRYPTION_SCOPE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ name\ of\ an\ encryption\ scope\ defined\ in\ the\ Azure
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Blob\ Storage\ service\ which\ is\ to\ be\ used\ to\ encrypt
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ data\ in\ Azure
 \ \ \-\-max\-block\-size\ MAX_BLOCK_SIZE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ chunk\ size\ to\ be\ used\ when\ uploading\ an\ object\ via
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ concurrent\ chunk\ method\ (default:\ 4MB).
```

### Comparing `barman-3.5.0/doc/barman-wal-archive.1` & `barman-3.6.0/doc/barman-wal-archive.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-WAL\-ARCHIVE" "1" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN\-WAL\-ARCHIVE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
 barman\-wal\-archive \- \f[C]archive_command\f[] based on Barman\[aq]s
 put\-wal
 .SH SYNOPSIS
 .PP
```

### Comparing `barman-3.5.0/doc/barman-cloud-backup-keep.1.md` & `barman-3.6.0/doc/barman-cloud-backup-keep.1.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-BACKUP-DELETE(1) Barman User manuals | Version 3.5.0
+% BARMAN-CLOUD-BACKUP-DELETE(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% March 29, 2023
+% June 15, 2023
 
 # NAME
 
 barman-cloud-backup-keep - Flag backups which should be kept forever
 
 
 # SYNOPSIS
@@ -24,15 +24,15 @@
 
 # Usage
 ```
 usage: barman-cloud-backup-keep [-V] [--help] [-v | -q] [-t]
                                 [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
                                 [--endpoint-url ENDPOINT_URL] [-P PROFILE]
                                 [--read-timeout READ_TIMEOUT]
-                                [--credential {azure-cli,managed-identity}]
+                                [--azure-credential {azure-cli,managed-identity}]
                                 (-r | -s | --target {full,standalone})
                                 source_url server_name backup_id
 
 This script can be used to tag backups in cloud storage as archival backups
 such that they will not be deleted. Currently AWS S3, Azure Blob Storage and
 Google Cloud Storage are supported.
 
@@ -65,21 +65,23 @@
                         file)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
-  --credential {azure-cli,managed-identity}
+  --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
-                        authenticating with Azure Blob Storage. If omitted
-                        then the credential will be obtained from the
-                        environment. If no credentials can be found in the
+                        authenticating with Azure. If omitted then Azure Blob
+                        Storage credentials will be obtained from the
+                        environment and the default Azure authentication flow
+                        will be used for authenticating with all other Azure
+                        services. If no credentials can be found in the
                         environment then the default Azure authentication flow
-                        will be used
+                        will also be used for Azure Blob Storage.
 ```
 # REFERENCES
 
 For Boto:
 
 * https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-cloud-backup-show.1.md` & `barman-3.6.0/doc/barman-cloud-backup-show.1.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-BACKUP-SHOW(1) Barman User manuals | Version 3.4.0
+% BARMAN-CLOUD-BACKUP-SHOW(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% January 26, 2023
+% June 15, 2023
 
 # NAME
 
 barman-cloud-backup-show - Show metadata for a backup stored in the Cloud
 
 
 # SYNOPSIS
@@ -24,15 +24,15 @@
 
 # Usage
 ```
 usage: barman-cloud-backup-show [-V] [--help] [-v | -q] [-t]
                                 [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
                                 [--endpoint-url ENDPOINT_URL] [-P PROFILE]
                                 [--read-timeout READ_TIMEOUT]
-                                [--credential {azure-cli,managed-identity}]
+                                [--azure-credential {azure-cli,managed-identity}]
                                 [--format FORMAT]
                                 source_url server_name backup_id
 
 This script can be used to show metadata for backups made with barman-cloud-
 backup command. Currently AWS S3, Azure Blob Storage and Google Cloud Storage
 are supported.
 
@@ -60,21 +60,23 @@
                         file)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
-  --credential {azure-cli,managed-identity}
+  --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
-                        authenticating with Azure Blob Storage. If omitted
-                        then the credential will be obtained from the
-                        environment. If no credentials can be found in the
+                        authenticating with Azure. If omitted then Azure Blob
+                        Storage credentials will be obtained from the
+                        environment and the default Azure authentication flow
+                        will be used for authenticating with all other Azure
+                        services. If no credentials can be found in the
                         environment then the default Azure authentication flow
-                        will be used
+                        will also be used for Azure Blob Storage.
 ```
 # REFERENCES
 
 For Boto:
 
 * https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-cloud-restore.1` & `barman-3.6.0/doc/barman-cloud-backup-keep.1`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,85 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-RESTORE" "1" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN\-CLOUD\-BACKUP\-DELETE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
-barman\-cloud\-restore \- Restore a PostgreSQL backup from the Cloud
+barman\-cloud\-backup\-keep \- Flag backups which should be kept forever
 .SH SYNOPSIS
 .PP
-barman\-cloud\-restore [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
-\f[I]SERVER_NAME\f[] \f[I]BACKUP_ID\f[] \f[I]RECOVERY_DIR\f[]
+barman\-cloud\-backup\-keep [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
+\f[I]SERVER_NAME\f[] \f[I]BACKUP_ID\f[]
 .SH DESCRIPTION
 .PP
-This script can be used to download a backup previously made with
-\f[C]barman\-cloud\-backup\f[] command.
-Currently AWS S3, Azure Blob Storage and Google Cloud Storage are
-supported.
-.PP
-This script can also be used to prepare for recovery from a snapshot
-backup by checking the attached disks were cloned from the correct
-snapshots and downloading the backup label from object storage.
+This script can be used to flag backups previously made with
+\f[C]barman\-cloud\-backup\f[] as archival backups.
+Archival backups are kept forever regardless of any retention policies
+applied.
 .PP
 This script and Barman are administration tools for disaster recovery of
 PostgreSQL servers written in Python and maintained by EnterpriseDB.
 .SH Usage
 .IP
 .nf
 \f[C]
-usage:\ barman\-cloud\-restore\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-credential\ {azure\-cli,managed\-identity}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-tablespace\ NAME:LOCATION]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-recovery\-instance\ SNAPSHOT_RECOVERY_INSTANCE]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-recovery\-zone\ SNAPSHOT_RECOVERY_ZONE]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name\ backup_id\ recovery_dir
+usage:\ barman\-cloud\-backup\-keep\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ (\-r\ |\ \-s\ |\ \-\-target\ {full,standalone})
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name\ backup_id
 
-This\ script\ can\ be\ used\ to\ download\ a\ backup\ previously\ made\ with\ barman\-
-cloud\-backup\ command.Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and\ Google\ Cloud
-Storage\ are\ supported.
+This\ script\ can\ be\ used\ to\ tag\ backups\ in\ cloud\ storage\ as\ archival\ backups
+such\ that\ they\ will\ not\ be\ deleted.\ Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and
+Google\ Cloud\ Storage\ are\ supported.
 
 positional\ arguments:
 \ \ source_url\ \ \ \ \ \ \ \ \ \ \ \ URL\ of\ the\ cloud\ source,\ such\ as\ a\ bucket\ in\ AWS\ S3.
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ For\ example:\ `s3://bucket/path/to/folder`.
 \ \ server_name\ \ \ \ \ \ \ \ \ \ \ the\ name\ of\ the\ server\ as\ configured\ in\ Barman.
-\ \ backup_id\ \ \ \ \ \ \ \ \ \ \ \ \ the\ backup\ ID
-\ \ recovery_dir\ \ \ \ \ \ \ \ \ \ the\ path\ to\ a\ directory\ for\ recovery.
+\ \ backup_id\ \ \ \ \ \ \ \ \ \ \ \ \ the\ backup\ ID\ of\ the\ backup\ to\ be\ kept
 
 optional\ arguments:
 \ \ \-V,\ \-\-version\ \ \ \ \ \ \ \ \ show\ program\[aq]s\ version\ number\ and\ exit
 \ \ \-\-help\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ show\ this\ help\ message\ and\ exit
 \ \ \-v,\ \-\-verbose\ \ \ \ \ \ \ \ \ increase\ output\ verbosity\ (e.g.,\ \-vv\ is\ more\ than\ \-v)
 \ \ \-q,\ \-\-quiet\ \ \ \ \ \ \ \ \ \ \ decrease\ output\ verbosity\ (e.g.,\ \-qq\ is\ less\ than\ \-q)
 \ \ \-t,\ \-\-test\ \ \ \ \ \ \ \ \ \ \ \ Test\ cloud\ connectivity\ and\ exit
 \ \ \-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ cloud\ provider\ to\ use\ as\ a\ storage\ backend
-\ \ \-\-tablespace\ NAME:LOCATION
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ tablespace\ relocation\ rule
-\ \ \-\-snapshot\-recovery\-instance\ SNAPSHOT_RECOVERY_INSTANCE
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Instance\ where\ the\ disks\ recovered\ from\ the\ snapshots
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ are\ attached
-\ \ \-\-snapshot\-recovery\-zone\ SNAPSHOT_RECOVERY_ZONE
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Zone\ containing\ the\ instance\ and\ disks\ for\ the
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ snapshot\ recovery
+\ \ \-r,\ \-\-release\ \ \ \ \ \ \ \ \ If\ specified,\ the\ command\ will\ remove\ the\ keep
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ annotation\ and\ the\ backup\ will\ be\ eligible\ for
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ deletion
+\ \ \-s,\ \-\-status\ \ \ \ \ \ \ \ \ \ Print\ the\ keep\ status\ of\ the\ backup
+\ \ \-\-target\ {full,standalone}
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Specify\ the\ recovery\ target\ for\ this\ backup
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
 \ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
-\ \ \-\-credential\ {azure\-cli,managed\-identity}
+\ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure\ Blob\ Storage.\ If\ omitted
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ then\ the\ credential\ will\ be\ obtained\ from\ the
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment.\ If\ no\ credentials\ can\ be\ found\ in\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used\ for\ authenticating\ with\ all\ other\ Azure
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ services.\ If\ no\ credentials\ can\ be\ found\ in\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ then\ the\ default\ Azure\ authentication\ flow
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ also\ be\ used\ for\ Azure\ Blob\ Storage.
 \f[]
 .fi
 .SH REFERENCES
 .PP
 For Boto:
 .IP \[bu] 2
 https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
@@ -118,26 +111,23 @@
 .IP \[bu] 2
 azure\-storage\-blob
 .IP \[bu] 2
 azure\-identity (optional, if you wish to use DefaultAzureCredential)
 .PP
 If using \f[C]\-\-cloud\-provider=google\-cloud\-storage\f[] *
 google\-cloud\-storage
-.PP
-If using \f[C]\-\-cloud\-provider=google\-cloud\-storage\f[] with
-snapshot backups * grpcio * google\-cloud\-compute
 .SH EXIT STATUS
 .TP
 .B 0
 Success
 .RS
 .RE
 .TP
 .B 1
-The restore was not successful
+The keep command was not successful
 .RS
 .RE
 .TP
 .B 2
 The connection to the cloud provider failed
 .RS
 .RE
```

### Comparing `barman-3.5.0/doc/barman-cloud-wal-archive.1.md` & `barman-3.6.0/doc/barman-cloud-wal-archive.1.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-WAL-ARCHIVE(1) Barman User manuals | Version 3.5.0
+% BARMAN-CLOUD-WAL-ARCHIVE(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% March 29, 2023
+% June 15, 2023
 
 # NAME
 
 barman-cloud-wal-archive - Archive PostgreSQL WAL files in the Cloud using `archive_command`
 
 
 # SYNOPSIS
@@ -29,15 +29,15 @@
 
 # Usage
 ```
 usage: barman-cloud-wal-archive [-V] [--help] [-v | -q] [-t]
                                 [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
                                 [--endpoint-url ENDPOINT_URL] [-P PROFILE]
                                 [--read-timeout READ_TIMEOUT]
-                                [--credential {azure-cli,managed-identity}]
+                                [--azure-credential {azure-cli,managed-identity}]
                                 [-z | -j | --snappy]
                                 [--tags [TAGS [TAGS ...]]]
                                 [--history-tags [HISTORY_TAGS [HISTORY_TAGS ...]]]
                                 [--kms-key-name KMS_KEY_NAME] [-e ENCRYPTION]
                                 [--sse-kms-key-id SSE_KMS_KEY_ID]
                                 [--encryption-scope ENCRYPTION_SCOPE]
                                 [--max-block-size MAX_BLOCK_SIZE]
@@ -94,21 +94,23 @@
   --sse-kms-key-id SSE_KMS_KEY_ID
                         The AWS KMS key ID that should be used for encrypting
                         the uploaded data in S3. Can be specified using the
                         key ID on its own or using the full ARN for the key.
                         Only allowed if `-e/--encryption` is set to `aws:kms`.
 
 Extra options for the azure-blob-storage cloud provider:
-  --credential {azure-cli,managed-identity}
+  --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
-                        authenticating with Azure Blob Storage. If omitted
-                        then the credential will be obtained from the
-                        environment. If no credentials can be found in the
+                        authenticating with Azure. If omitted then Azure Blob
+                        Storage credentials will be obtained from the
+                        environment and the default Azure authentication flow
+                        will be used for authenticating with all other Azure
+                        services. If no credentials can be found in the
                         environment then the default Azure authentication flow
-                        will be used
+                        will also be used for Azure Blob Storage.
   --encryption-scope ENCRYPTION_SCOPE
                         The name of an encryption scope defined in the Azure
                         Blob Storage service which is to be used to encrypt
                         the data in Azure
   --max-block-size MAX_BLOCK_SIZE
                         The chunk size to be used when uploading an object via
                         the concurrent chunk method (default: 4MB).
```

### Comparing `barman-3.5.0/doc/barman-cloud-backup-keep.1` & `barman-3.6.0/doc/barman-cloud-backup-show.1`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,81 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-BACKUP\-DELETE" "1" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN\-CLOUD\-BACKUP\-SHOW" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
-barman\-cloud\-backup\-keep \- Flag backups which should be kept forever
+barman\-cloud\-backup\-show \- Show metadata for a backup stored in the
+Cloud
 .SH SYNOPSIS
 .PP
-barman\-cloud\-backup\-keep [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
+barman\-cloud\-backup\-show [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
 \f[I]SERVER_NAME\f[] \f[I]BACKUP_ID\f[]
 .SH DESCRIPTION
 .PP
-This script can be used to flag backups previously made with
-\f[C]barman\-cloud\-backup\f[] as archival backups.
-Archival backups are kept forever regardless of any retention policies
-applied.
+This script can be used to display metadata for backups previously made
+with the \f[C]barman\-cloud\-backup\f[] command.
+Currently AWS S3, Azure Blob Storage and Google Cloud Storage are
+supported.
 .PP
 This script and Barman are administration tools for disaster recovery of
 PostgreSQL servers written in Python and maintained by EnterpriseDB.
 .SH Usage
 .IP
 .nf
 \f[C]
-usage:\ barman\-cloud\-backup\-keep\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
+usage:\ barman\-cloud\-backup\-show\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-credential\ {azure\-cli,managed\-identity}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ (\-r\ |\ \-s\ |\ \-\-target\ {full,standalone})
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-format\ FORMAT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name\ backup_id
 
-This\ script\ can\ be\ used\ to\ tag\ backups\ in\ cloud\ storage\ as\ archival\ backups
-such\ that\ they\ will\ not\ be\ deleted.\ Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and
-Google\ Cloud\ Storage\ are\ supported.
+This\ script\ can\ be\ used\ to\ show\ metadata\ for\ backups\ made\ with\ barman\-cloud\-
+backup\ command.\ Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and\ Google\ Cloud\ Storage
+are\ supported.
 
 positional\ arguments:
 \ \ source_url\ \ \ \ \ \ \ \ \ \ \ \ URL\ of\ the\ cloud\ source,\ such\ as\ a\ bucket\ in\ AWS\ S3.
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ For\ example:\ `s3://bucket/path/to/folder`.
 \ \ server_name\ \ \ \ \ \ \ \ \ \ \ the\ name\ of\ the\ server\ as\ configured\ in\ Barman.
-\ \ backup_id\ \ \ \ \ \ \ \ \ \ \ \ \ the\ backup\ ID\ of\ the\ backup\ to\ be\ kept
+\ \ backup_id\ \ \ \ \ \ \ \ \ \ \ \ \ the\ backup\ ID
 
 optional\ arguments:
 \ \ \-V,\ \-\-version\ \ \ \ \ \ \ \ \ show\ program\[aq]s\ version\ number\ and\ exit
 \ \ \-\-help\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ show\ this\ help\ message\ and\ exit
 \ \ \-v,\ \-\-verbose\ \ \ \ \ \ \ \ \ increase\ output\ verbosity\ (e.g.,\ \-vv\ is\ more\ than\ \-v)
 \ \ \-q,\ \-\-quiet\ \ \ \ \ \ \ \ \ \ \ decrease\ output\ verbosity\ (e.g.,\ \-qq\ is\ less\ than\ \-q)
 \ \ \-t,\ \-\-test\ \ \ \ \ \ \ \ \ \ \ \ Test\ cloud\ connectivity\ and\ exit
 \ \ \-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ cloud\ provider\ to\ use\ as\ a\ storage\ backend
-\ \ \-r,\ \-\-release\ \ \ \ \ \ \ \ \ If\ specified,\ the\ command\ will\ remove\ the\ keep
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ annotation\ and\ the\ backup\ will\ be\ eligible\ for
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ deletion
-\ \ \-s,\ \-\-status\ \ \ \ \ \ \ \ \ \ Print\ the\ keep\ status\ of\ the\ backup
-\ \ \-\-target\ {full,standalone}
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Specify\ the\ recovery\ target\ for\ this\ backup
+\ \ \-\-format\ FORMAT\ \ \ \ \ \ \ Output\ format\ (console\ or\ json).\ Default\ console.
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
 \ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
-\ \ \-\-credential\ {azure\-cli,managed\-identity}
+\ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure\ Blob\ Storage.\ If\ omitted
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ then\ the\ credential\ will\ be\ obtained\ from\ the
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment.\ If\ no\ credentials\ can\ be\ found\ in\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used\ for\ authenticating\ with\ all\ other\ Azure
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ services.\ If\ no\ credentials\ can\ be\ found\ in\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ then\ the\ default\ Azure\ authentication\ flow
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ also\ be\ used\ for\ Azure\ Blob\ Storage.
 \f[]
 .fi
 .SH REFERENCES
 .PP
 For Boto:
 .IP \[bu] 2
 https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
@@ -107,25 +105,26 @@
 .PP
 If using \f[C]\-\-cloud\-provider=azure\-blob\-storage\f[]:
 .IP \[bu] 2
 azure\-storage\-blob
 .IP \[bu] 2
 azure\-identity (optional, if you wish to use DefaultAzureCredential)
 .PP
-If using \f[C]\-\-cloud\-provider=google\-cloud\-storage\f[] *
+If using \f[C]\-\-cloud\-provider=google\-cloud\-storage\f[]
+.IP \[bu] 2
 google\-cloud\-storage
 .SH EXIT STATUS
 .TP
 .B 0
 Success
 .RS
 .RE
 .TP
 .B 1
-The keep command was not successful
+The show command was not successful
 .RS
 .RE
 .TP
 .B 2
 The connection to the cloud provider failed
 .RS
 .RE
```

### Comparing `barman-3.5.0/doc/manual/50-feature-details.en.md` & `barman-3.6.0/doc/manual/50-feature-details.en.md`

 * *Files 2% similar despite different names*

```diff
@@ -1045,16 +1045,16 @@
 5. The mount point and mount options for each disk are saved in the backup metadata.
 6. Barman stops the backup using the PostgreSQL backup API.
 
 The cloud provider API calls are made on the node where the backup command runs; this will be either the Barman server (when `barman backup` is used) or the PostgreSQL server (when `barman-cloud-backup` is used).
 
 The following pre-flight checks are carried out before each backup and also when `barman check` runs against a server configured for snapshot backups:
 
-- The compute instance specified by `snapshot_instance` exists in the availability zone specified by `snapshot_zone`.
-- The disks specified by `snapshot_disks` exist in the availability zone specified by `snapshot_zone`.
+- The compute instance specified by `snapshot_instance` and any provider-specific arguments exists.
+- The disks specified by `snapshot_disks` exist.
 - The disks specified by `snapshot_disks` are attached to `snapshot_instance`.
 - The disks specified by `snapshot_disks` are mounted on `snapshot_instance`.
 
 ### Recovering from a snapshot backup
 
 Barman will not currently perform a fully automated recovery from snapshot backups.
 This is because recovery from snapshots requires the provision and management of new infrastructure which is something better handled by dedicated infrastructure-as-code solutions such as Terraform.
@@ -1067,43 +1067,56 @@
 Recovery from a snapshot backup consists of the following steps:
 
 1. Provision a new disk for each snapshot taken during the backup.
 2. Provision a compute instance where each disk provisioned in step 1 is attached and mounted according to the backup metadata.
 3. Use the [barman recover](#recover) or [barman-cloud-restore](#barman-cloud-restore-for-snapshots) command to validate and finalize the recovery.
 
 Steps 1 and 2 are best handled by an existing infrastructure-as-code system however it is also possible to carry these steps out manually or using a custom script.
-An example of such a script is [provided with Barman][snapshot-recovery-script] however this script makes various assumptions about the environment in which it runs and should not be considered suitable for production use.
+
+The following resources may be helpful when carrying out these steps:
+
+- An example [recovery script for GCP][snapshot-recovery-script].
+- An example [runbook for Azure][snapshot-recovery-runbook-azure].
+
+The above resources make assumptions about the backup/recovery environment and should not be considered suitable for production use without further customization.
 
 Once the recovery instance is provisioned and disks cloned from the backup snapshots are attached and mounted, run `barman recover` with the following additional arguments:
 
 - `--remote-ssh-command`: The ssh command required to log in to the recovery instance.
 - `--snapshot-recovery-instance`: The name of the recovery instance as required by the cloud provider.
-- `--snapshot-recovery-zone`:  The name of the availability zone in which the recovery instance is located.
+- Any additional arguments specific to the snapshot provider.
 
 For example:
 
 ``` bash
 barman recover SERVER_NAME BACKUP_ID REMOTE_RECOVERY_DIRECTORY \
     --remote-ssh-command 'ssh USER@HOST' \
-    --snapshot-recovery-instance INSTANCE_NAME \
-    --snapshot-recovery-zone ZONE_NAME
+    --snapshot-recovery-instance INSTANCE_NAME
 ```
 
+Barman will automatically detect that the backup is a snapshot backup and check that the attached disks were cloned from the snapshots for that backup.
+Barman will then prepare PostgreSQL for recovery by copying the backup label and WALs into place and setting any required recovery options in the PostgreSQL configuration.
+
+The following additional `barman recover` arguments are available with the `gcp` provider:
+
+- `--gcp-zone`: The name of the availability zone in which the recovery instance is located. If not provided then Barman will use the value of `gcp_zone` set in the server config.
+
+The following additional `barman recover` arguments are available with the `azure` provider:
+
+- `--azure-resource-group`: The resource group to which the recovery instance belongs. If not provided then Barman will use the value of `azure_resource_group` set in the server config.
+
 Note the following `barman recover` arguments / config variables are unavailable when recovering snapshot backups:
 
 | **Command argument**      | **Config variable** .   |
 |:-------------------------:|:-----------------------:|
 | `--bwlimit`               | `bandwidth_limit`       |
 | `--jobs`                  | `parallel_jobs`         |
 | `--recovery-staging-path` | `recovery_staging_path` |
 | `--tablespace`            | N/A                     |
 
-Barman will automatically detect that the backup is a snapshot backup and check that the attached disks were cloned from the snapshots for that backup.
-Barman will then prepare PostgreSQL for recovery by copying the backup label and WALs into place and setting any required recovery options in the PostgreSQL configuration.
-
 ### Backup metadata for snapshot backups
 
 Whether the recovery disks and instance are provisioned via infrastructure-as-code, ad-hoc automation or manually, it will be necessary to query Barman to find the snapshots required for a given backup.
 This can be achieved using [barman show-backup](#show-backup) which will provide details for each snapshot in the backup.
 For example:
 
 ``` bash
@@ -1167,7 +1180,34 @@
     }
   ]
 }
 ...
 ```
 
 For backups taken with `barman-cloud-backup` there is an analogous [barman-cloud-backup-show][pgbarman-barman-cloud-backup-show] command which can be used along with `barman-cloud-backup-list` to query the backup metadata in the cloud object store.
+
+The metadata available in `snapshots_info/provider_info` and `snapshots_info/snapshots/*/provider` varies by cloud provider as explained in the following sections.
+
+#### GCP provider-specific metadata
+
+The following fields are available in `snapshots_info/provider_info`:
+
+- `project`: The GCP project ID of the project which owns the resources involved in backup and recovery.
+
+The following fields are available in `snapshots_info/snapshots/*/provider`:
+
+- `device_name`: The short device name with which the source disk for the snapshot was attached to the backup VM at the time of the backup.
+- `snapshot_name`: The name of the snapshot.
+- `snapshot_project`: The GCP project ID which owns the snapshot.
+
+#### Azure provider-specific metadata
+
+The following fields are available in `snapshots_info/provider_info`:
+
+- `subscription_id`: The Azure subscription ID which owns the resources involved in backup and recovery.
+- `resource_group`: The Azure resource group to which the resources involved in the backup belong.
+
+The following fields are available in `snapshots_info/snapshots/*/provider`:
+
+- `location`: The Azure location of the disk from which the snapshot was taken.
+- `lun`: The LUN identifying the disk from which the snapshot was taken at the time of the backup.
+- `snapshot_name`: The name of the snapshot.
```

### Comparing `barman-3.5.0/doc/manual/99-references.en.md` & `barman-3.6.0/doc/manual/99-references.en.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
   [google-cloud-storage]: https://cloud.google.com/storage/docs/reference/libraries
   [pg_basebackup-documentation]: https://www.postgresql.org/docs/current/app-pgbasebackup.html
   [pg-backup-api]: https://github.com/EnterpriseDB/pg-backup-api
   [config-options]: https://docs.pgbarman.org/barman.5.html#options
   [barman-downloads]: https://pgbarman.org/downloads/
   [python-2-sunset]: https://www.python.org/doc/sunset-python-2/
   [psql]: https://www.postgresql.org/docs/current/app-psql.html
+  [snapshot-recovery-runbook-azure]: https://github.com/EnterpriseDB/barman/blob/master/doc/runbooks/snapshot_recovery_azure.md
   [snapshot-recovery-script]: https://github.com/EnterpriseDB/barman/blob/master/scripts/prepare_snapshot_recovery.py
   [postgres-low-level-base-backup]: https://www.postgresql.org/docs/current/continuous-archiving.html#BACKUP-LOWLEVEL-BASE-BACKUP
   [pgbarman-barman-cloud-backup-show]: https://docs.pgbarman.org/release/latest/barman-cloud-backup-show.1.html
 
   [8]: https://en.wikipedia.org/wiki/Hard_link
   [11]: https://www.pgbarman.org/
   [12]: https://www.pgbarman.org/support/
```

### Comparing `barman-3.5.0/doc/manual/16-installation.en.md` & `barman-3.6.0/doc/manual/16-installation.en.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 
 Then, as `root` simply type:
 
 ``` bash
 yum install barman
 ```
 
-> **NOTE: **
+> **NOTE:**
 > We suggest that you exclude any Barman related packages from getting updated
 > via the PGDG repository. This can be done by adding the following line
 > to any PGDG repository definition that is included in the Barman server inside
 > any `/etc/yum.repos.d/pgdg-*.repo` file:
+
    ```ini
    exclude=barman* python*-barman
    ```
+
 > By doing this, you solely rely on
 > EnterpriseDB's 2ndQuadrant repositories for package management of Barman software.
 
 ## Installation on Debian/Ubuntu using packages
 
 Barman can be installed on Debian and Ubuntu Linux systems using
 packages.
@@ -107,15 +109,15 @@
 ## PostgreSQL client/server binaries
 
 The following Barman features depend on PostgreSQL binaries:
 
 * [Streaming backup](#streaming-backup) with `backup_method = postgres` (requires `pg_basebackup`)
 * [Streaming WAL archiving](#wal-streaming) with `streaming_archiver = on` (requires
   `pg_receivewal` or `pg_receivexlog`)
-* [Verifying backups](#verify) with `barman verify-backup` (requires `pg_verifybackup`)
+* [Verifying backups](#verify-backup) with `barman verify-backup` (requires `pg_verifybackup`)
 
 Depending on the target OS these binaries are installed with either the PostgreSQL client or server packages:
 
 * On RedHat/CentOS and SLES:
   * The `pg_basebackup` and `pg_receivewal`/`pg_receivexlog` binaries are installed with the PostgreSQL client packages.
   * The `pg_verifybackup` binary is installed with the PostgreSQL server packages.
   * All binaries are installed in `/usr/pgsql-${PG_MAJOR_VERSION}/bin`.
```

### Comparing `barman-3.5.0/doc/manual/Makefile` & `barman-3.6.0/doc/manual/Makefile`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/17-configuration.en.md` & `barman-3.6.0/doc/manual/17-configuration.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/30-windows-support.en.md` & `barman-3.6.0/doc/manual/30-windows-support.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/23-wal_streaming.en.md` & `barman-3.6.0/doc/manual/23-wal_streaming.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/41-global-commands.en.md` & `barman-3.6.0/doc/manual/41-global-commands.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/43-backup-commands.en.md` & `barman-3.6.0/doc/manual/43-backup-commands.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/66-about.en.md` & `barman-3.6.0/doc/manual/66-about.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/55-barman-cli.en.md` & `barman-3.6.0/doc/manual/55-barman-cli.en.md`

 * *Files 4% similar despite different names*

```diff
@@ -203,19 +203,24 @@
 
 ### barman-cloud-backup for snapshots
 
 To take a snapshot backup with barman-cloud, use `barman-cloud-backup` with the following additional arguments:
 
 - `--snapshot-disk` (can be used multiple times for multiple disks)
 - `--snapshot-instance`
-- `--snapshot-zone`
 
-If the `--cloud-provider` is `google-cloud-storage` then the following argument is also required:
+If the `--cloud-provider` is `google-cloud-storage` then the following arguments are also required:
 
-- `--snapshot-gcp-project`
+- `--gcp-project`
+- `--gcp-zone`
+
+If the `--cloud-provider` is `azure-blob-storage` then the following arguments are also required:
+
+- `--azure-subscription-id`
+- `--azure-resource-group`
 
 The following options cannot be used with `barman-cloud-backup` when cloud snapshots are requested:
 
 - `--bzip2`, `--gzip` or `--snappy`
 - `--jobs`
 
 Once a backup has been taken it can be managed using the standard barman-cloud commands such as `barman-cloud-backup-delete` and `barman-cloud-backup-keep`.
@@ -226,13 +231,20 @@
 This carries out the same pre-recovery checks as `barman recover` and copies the backup label into place on the recovery instance.
 
 The snapshot metadata required to provision the recovery instance can be queried using `barman-cloud-backup-show`.
 
 Note that, just like when using `barman-cloud-restore` with an object stored backup, the command will not prepare PostgreSQL for the recovery.
 Any PITR options, custom `restore_command` values or WAL files required before PostgreSQL starts must be handled manually or by external tooling.
 
-The following additional arguments must be used with `barman-cloud-restore` when restoring a backup made with cloud snapshots:
+The following additional argument must be used with `barman-cloud-restore` when restoring a backup made with cloud snapshots:
 
 - `--snapshot-recovery-instance`
-- `--snapshot-recovery-zone`
+
+The following additional arguments are required with the `gcp` provider:
+
+- `--gcp-zone`
+
+The following additional arguments are required with the `azure` provider:
+
+- `--azure-resource-group`
 
 The `--tablespace` option cannot be used with `barman-cloud-restore` when restoring a cloud snapshot backup:
```

### Comparing `barman-3.5.0/doc/manual/00-head.en.md` & `barman-3.6.0/doc/manual/00-head.en.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 % Barman Manual
 % EnterpriseDB UK Limited
-% March 29, 2023 (3.5.0)
+% June 15, 2023 (3.6.0)
 
 **Barman** (Backup and Recovery Manager) is an open-source administration tool for disaster recovery of PostgreSQL servers written in Python. It allows your organisation to perform remote backups of multiple servers in business critical environments to reduce risk and help DBAs during the recovery phase.
 
 [Barman][11] is distributed under GNU GPL 3 and maintained by [EnterpriseDB][13], a platinum sponsor of the [PostgreSQL project][31].
 
 > **IMPORTANT:** \newline
 > This manual assumes that you are familiar with theoretical disaster
```

### Comparing `barman-3.5.0/doc/manual/02-before_you_start.en.md` & `barman-3.6.0/doc/manual/02-before_you_start.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/42-server-commands.en.md` & `barman-3.6.0/doc/manual/42-server-commands.en.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,14 @@
 archived before setting the state to `DONE` and proceeding
 with post-backup hook scripts.  If the `--wait-timeout` option is
 provided, Barman will stop waiting for WAL files after the specified
 number of seconds, and the state will remain in `WAITING_FOR_WALS`.The
 `cron` command will continue to check that missing WAL files are
 archived, then label the backup as `DONE`.
 
-
-
 ## `check`
 
 You can check the connection to a given server and the
 configuration coherence with the `check` command:
 
 ``` bash
 barman check <server_name>
@@ -67,26 +65,29 @@
 > The `check` command is probably the most critical feature that
 > Barman implements. We recommend to integrate it with your alerting
 > and monitoring infrastructure. The `--nagios` option allows you
 > to easily create a plugin for Nagios/Icinga.
 
 ## `generate-manifest`
 
-This command is useful when backup is created remotely and pg_basebackup is not 
+This command is useful when backup is created remotely and pg_basebackup is not
 involved and `backup_manifest` file does not exist in backup.
 It will generate `backup_manifest` file from backup_id using backup in barman server.
 If the file already exist, generation command will abort.
 
 Command example:
+
 ```bash
 barman generate-manifest <server_name> <backup_id>
 ```
+
 Either backup_id [backup id shortcuts]{#backup-id-shortcuts} can be used.
 
 This command can also be used as post_backup hook script as follows:
+
 ```bash
 post_backup_script=barman generate-manifest ${BARMAN_SERVER} ${BARMAN_BACKUP_ID}
 ```
 
 ## `get-wal`
 
 Barman allows users to request any _xlog_ file from its WAL archive
@@ -143,15 +144,15 @@
 
 Setting `recovery_options` to `get-wal` for a remote recovery will instead
 generate a `restore_command` using the `barman-wal-restore` script.
 `barman-wal-restore` is a more resilient shell script which manages SSH
 connection errors.
 
 This script has many useful options such as the automatic compression and
-decompression of the WAL files and the *peek* feature, which allows you
+decompression of the WAL files and the _peek_ feature, which allows you
 to retrieve the next WAL files while PostgreSQL is applying one of them. It is
 an excellent way to optimise the bandwidth usage between PostgreSQL and
 Barman.
 
 `barman-wal-restore` is available in the `barman-cli` package.
 
 This is an example of a `restore_command` for a remote recovery:
@@ -288,15 +289,14 @@
 ``` bash
 barman show-servers <server_name>
 ```
 
 > **TIP:** you can request a full configuration report using `all` as
 > the server name.
 
-
 ## `status`
 
 The `status` command shows live information and status of a PostgreSQL
 server or of all servers if you use `all` as server name.
 
 ``` bash
 barman status <server_name>
@@ -320,19 +320,21 @@
 the xlog switch. By default, a 30 seconds timeout is enforced (this
 can be changed with `--archive-timeout`). If no WAL file is received,
 an error is returned.
 
 > **NOTE:** In Barman 2.1 and 2.2 this command was called `switch-xlog`.
 > It has been renamed for naming consistency with PostgreSQL 10 and higher.
 
-## `verify`
+## `verify-backup`
 
-The `verify` command uses backup_manifest file from backup and runs 
+The `verify-backup` command uses backup_manifest file from backup and runs
 `pg_verifybackup` against it.  
+
 ```bash
-barman verify <server_name> <backup_id>
+barman verify-backup <server_name> <backup_id>
 ```
+
 This command will call `pg_verifybackup <path_to_backup_manifest> -n` (available on PG>=13)
 `pg_verifybackup` Must be installed on backup server.
 For rsync backups, it can be used with `generate-manifest` command.
 
 Either backup_id [backup id shortcuts]{#backup-id-shortcuts} can be used.
```

### Comparing `barman-3.5.0/doc/manual/26-rsync_backup.en.md` & `barman-3.6.0/doc/manual/26-rsync_backup.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/65-troubleshooting.en.md` & `barman-3.6.0/doc/manual/65-troubleshooting.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/20-server_setup.en.md` & `barman-3.6.0/doc/manual/20-server_setup.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/24-wal_archiving.en.md` & `barman-3.6.0/doc/manual/24-wal_archiving.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/10-design.en.md` & `barman-3.6.0/doc/manual/10-design.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/15-system_requirements.en.md` & `barman-3.6.0/doc/manual/15-system_requirements.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/28-snapshots.en.md` & `barman-3.6.0/doc/manual/28-snapshots.en.md`

 * *Files 19% similar despite different names*

```diff
@@ -42,49 +42,88 @@
 - `compute.disks.get`
 - `compute.globalOperations.get`
 - `compute.instances.get`
 - `compute.snapshots.create`
 - `compute.snapshots.delete`
 - `compute.snapshots.list`
 
+#### Azure snapshot prerequisites
+
+The azure-mgmt-compute and azure-identity libraries must be available to the Python distribution used by Barman.
+
+These libraries are an optional dependency and are not installed as standard by any of the Barman packages.
+They can be installed as follows using `pip`:
+
+``` bash
+pip3 install azure-mgmt-compute azure-identity
+```
+
+> **NOTE:** The minimum version of Python required by the azure-mgmt-compute
+> library is 3.7. Azure snapshots cannot be used with earlier versions of Python.
+
+The following additional prerequisites apply to snapshot backups on Azure:
+
+- All disks included in the snapshot backup must be managed disks which are attached to the VM instance as data disks.
+- Barman must be able to use a credential obtained either using managed identity or CLI login and this must grant access to Azure with the required set of permissions.
+
+The following permissions are required:
+
+- `Microsoft.Compute/disks/read`
+- `Microsoft.Compute/virtualMachines/read`
+- `Microsoft.Compute/snapshots/read`
+- `Microsoft.Compute/snapshots/write`
+- `Microsoft.Compute/snapshots/delete`
+
 ### Configuration for snapshot backups
 
 To configure Barman for backup via cloud snapshots, set the `backup_method` parameter to `snapshot` and set `snapshot_provider` to a supported cloud provider:
 
 ``` ini
 backup_method = snapshot
 snapshot_provider = gcp
 ```
 
-Currently only Google Cloud Platform (gcp) is supported.
+Currently Google Cloud Platform (`gcp`) and Microsoft Azure (`azure`) are supported.
 
 The following parameters must be set regardless of cloud provider:
 
 ``` ini
 snapshot_instance = INSTANCE_NAME
-snapshot_zone = ZONE
 snapshot_disks = DISK_NAME,DISK2_NAME,...
 ```
 
-Where `snapshot_instance` is set to the name of the VM or compute instance where the storage volumes are attached, `snapshot_zone` is the available zone in which the instance is located and `snapshot_disks` is a comma-separated list of the disks which should be included in the backup.
+Where `snapshot_instance` is set to the name of the VM or compute instance where the storage volumes are attached and `snapshot_disks` is a comma-separated list of the disks which should be included in the backup.
 
 > **IMPORTANT:** You must ensure that `snapshot_disks` includes every disk
 > which stores data required by PostgreSQL. Any data which is not stored
 > on a storage volume listed in `snapshot_disks` will not be included in the
 > backup and therefore will not be available at recovery time.
 
 #### Configuration for Google Cloud Platform snapshots
 
-The following additional parameter must be set when using GCP:
+The following additional parameters must be set when using GCP:
+
+``` ini
+gcp_project = GCP_PROJECT_ID
+gcp_zone = ZONE
+```
+
+`gcp_project` should be set to the ID of the GCP project which owns the instance and storage volumes defined by `snapshot_instance` and `snapshot_disks`. `gcp_zone` should be set to the availability zone in which the instance is located.
+
+#### Configuration for Azure snapshots
+
+The following additional parameters must be set when using Azure:
 
 ``` ini
-snapshot_gcp_project = GCP_PROJECT_ID
+azure_subscription_id = AZURE_SUBSCRIPTION_ID
+azure_resource_group = AZURE_RESOURCE_GROUP
 ```
 
-This should be set to the ID of the GCP project which owns the instance and storage volumes defined by `snapshot_instance` and `snapshot_disks`.
+`azure_subscription_id` should be set to the ID of the Azure subscription ID which owns the instance and storage volumes defined by `snapshot_instance` and `snapshot_disks`.
+`azure_resource_group` should be set to the resource group to which the instance and disks belong.
 
 ### Taking a snapshot backup
 
 Once the configuration options are set and appropriate credentials are available to Barman, backups can be taken using the [barman backup](#backup) command.
 
 Barman will validate the configuration parameters for snapshot backups during the `barman check` command and also when starting a backup.
```

### Comparing `barman-3.5.0/doc/manual/22-config_file.en.md` & `barman-3.6.0/doc/manual/22-config_file.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/21-preliminary_steps.en.md` & `barman-3.6.0/doc/manual/21-preliminary_steps.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/01-intro.en.md` & `barman-3.6.0/doc/manual/01-intro.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/manual/25-streaming_backup.en.md` & `barman-3.6.0/doc/manual/25-streaming_backup.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman.conf` & `barman-3.6.0/doc/barman.conf`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/doc/barman-cloud-backup-list.1.md` & `barman-3.6.0/doc/barman-cloud-backup-list.1.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-BACKUP-LIST(1) Barman User manuals | Version 3.5.0
+% BARMAN-CLOUD-BACKUP-LIST(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% March 29, 2023
+% June 15, 2023
 
 # NAME
 
 barman-cloud-backup-list - List backups stored in the Cloud
 
 
 # SYNOPSIS
@@ -24,15 +24,15 @@
 
 # Usage
 ```
 usage: barman-cloud-backup-list [-V] [--help] [-v | -q] [-t]
                                 [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
                                 [--endpoint-url ENDPOINT_URL] [-P PROFILE]
                                 [--read-timeout READ_TIMEOUT]
-                                [--credential {azure-cli,managed-identity}]
+                                [--azure-credential {azure-cli,managed-identity}]
                                 [--format FORMAT]
                                 source_url server_name
 
 This script can be used to list backups made with barman-cloud-backup command.
 Currently AWS S3, Azure Blob Storage and Google Cloud Storage are supported.
 
 positional arguments:
@@ -58,21 +58,23 @@
                         file)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
-  --credential {azure-cli,managed-identity}
+  --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
-                        authenticating with Azure Blob Storage. If omitted
-                        then the credential will be obtained from the
-                        environment. If no credentials can be found in the
+                        authenticating with Azure. If omitted then Azure Blob
+                        Storage credentials will be obtained from the
+                        environment and the default Azure authentication flow
+                        will be used for authenticating with all other Azure
+                        services. If no credentials can be found in the
                         environment then the default Azure authentication flow
-                        will be used
+                        will also be used for Azure Blob Storage.
 ```
 # REFERENCES
 
 For Boto:
 
 * https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-wal-restore.1.md` & `barman-3.6.0/doc/barman-wal-restore.1.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-WAL-RESTORE(1) Barman User manuals | Version 3.5.0
+% BARMAN-WAL-RESTORE(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% March 29, 2023
+% June 15, 2023
 
 # NAME
 
 barman-wal-restore - 'restore_command' based on Barman's get-wal
 
 
 # SYNOPSIS
```

### Comparing `barman-3.5.0/doc/barman-cloud-backup-delete.1.md` & `barman-3.6.0/doc/barman-cloud-backup-delete.1.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-BACKUP-DELETE(1) Barman User manuals | Version 3.5.0
+% BARMAN-CLOUD-BACKUP-DELETE(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% March 29, 2023
+% June 15, 2023
 
 # NAME
 
 barman-cloud-backup-delete - Delete backups stored in the Cloud
 
 
 # SYNOPSIS
@@ -44,15 +44,15 @@
 
 # Usage
 ```
 usage: barman-cloud-backup-delete [-V] [--help] [-v | -q] [-t]
                                   [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
                                   [--endpoint-url ENDPOINT_URL] [-P PROFILE]
                                   [--read-timeout READ_TIMEOUT]
-                                  [--credential {azure-cli,managed-identity}]
+                                  [--azure-credential {azure-cli,managed-identity}]
                                   (-b BACKUP_ID | -r RETENTION_POLICY)
                                   [--dry-run] [--batch-size DELETE_BATCH_SIZE]
                                   source_url server_name
 
 This script can be used to delete backups made with barman-cloud-backup
 command. Currently AWS S3, Azure Blob Storage and Google Cloud Storage are
 supported.
@@ -94,21 +94,23 @@
                         file)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
-  --credential {azure-cli,managed-identity}
+  --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
-                        authenticating with Azure Blob Storage. If omitted
-                        then the credential will be obtained from the
-                        environment. If no credentials can be found in the
+                        authenticating with Azure. If omitted then Azure Blob
+                        Storage credentials will be obtained from the
+                        environment and the default Azure authentication flow
+                        will be used for authenticating with all other Azure
+                        services. If no credentials can be found in the
                         environment then the default Azure authentication flow
-                        will be used
+                        will also be used for Azure Blob Storage.
 ```
 # REFERENCES
 
 For Boto:
 
 * https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-cloud-backup.1` & `barman-3.6.0/doc/barman-cloud-backup.1`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-BACKUP" "1" "March 29, 2023" "Barman User manuals" "Version 3.5.0"
+.TH "BARMAN\-CLOUD\-BACKUP" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-backup \- Backup a PostgreSQL instance and stores it in
 the Cloud
 .SH SYNOPSIS
 .PP
@@ -43,26 +43,28 @@
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-backup\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-credential\ {azure\-cli,managed\-identity}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-z\ |\ \-j\ |\ \-\-snappy]\ [\-h\ HOST]\ [\-p\ PORT]\ [\-U\ USER]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-immediate\-checkpoint]\ [\-J\ JOBS]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-S\ MAX_ARCHIVE_SIZE]\ [\-d\ DBNAME]\ [\-n\ BACKUP_NAME]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-instance\ SNAPSHOT_INSTANCE]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-disk\ NAME]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-zone\ SNAPSHOT_ZONE]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-gcp\-project\ SNAPSHOT_GCP_PROJECT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-kms\-key\-name\ KMS_KEY_NAME]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-disk\ NAME]\ [\-\-snapshot\-zone\ GCP_ZONE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-gcp\-project\ GCP_PROJECT]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-gcp\-project\ GCP_PROJECT]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-kms\-key\-name\ KMS_KEY_NAME]\ [\-\-gcp\-zone\ GCP_ZONE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-tags\ [TAGS\ [TAGS\ ...]]]\ [\-e\ {AES256,aws:kms}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-sse\-kms\-key\-id\ SSE_KMS_KEY_ID]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-encryption\-scope\ ENCRYPTION_SCOPE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-subscription\-id\ AZURE_SUBSCRIPTION_ID]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-resource\-group\ AZURE_RESOURCE_GROUP]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ destination_url\ server_name
 
 This\ script\ can\ be\ used\ to\ perform\ a\ backup\ of\ a\ local\ PostgreSQL\ instance\ and
 ship\ the\ resulting\ tarball(s)\ to\ the\ Cloud.\ Currently\ AWS\ S3,\ Azure\ Blob
 Storage\ and\ Google\ Cloud\ Storage\ are\ supported.
 
 positional\ arguments:
@@ -102,16 +104,17 @@
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ a\ name\ which\ can\ be\ used\ to\ reference\ this\ backup\ in
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ commands\ such\ as\ barman\-cloud\-restore\ and\ barman\-
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ cloud\-backup\-delete
 \ \ \-\-snapshot\-instance\ SNAPSHOT_INSTANCE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Instance\ where\ the\ disks\ to\ be\ backed\ up\ as\ snapshots
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ are\ attached
 \ \ \-\-snapshot\-disk\ NAME\ \ Name\ of\ a\ disk\ from\ which\ snapshots\ should\ be\ taken
-\ \ \-\-snapshot\-zone\ SNAPSHOT_ZONE
+\ \ \-\-snapshot\-zone\ GCP_ZONE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Zone\ of\ the\ disks\ from\ which\ snapshots\ should\ be\ taken
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ (deprecated:\ replaced\ by\ \-\-gcp\-zone)
 \ \ \-\-tags\ [TAGS\ [TAGS\ ...]]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Tags\ to\ be\ added\ to\ all\ uploaded\ files\ in\ cloud
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ storage
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
@@ -129,32 +132,47 @@
 \ \ \-\-sse\-kms\-key\-id\ SSE_KMS_KEY_ID
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ AWS\ KMS\ key\ ID\ that\ should\ be\ used\ for\ encrypting
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ uploaded\ data\ in\ S3.\ Can\ be\ specified\ using\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ key\ ID\ on\ its\ own\ or\ using\ the\ full\ ARN\ for\ the\ key.
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Only\ allowed\ if\ `\-e/\-\-encryption`\ is\ set\ to\ `aws:kms`.
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
-\ \ \-\-credential\ {azure\-cli,managed\-identity}
+\ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure\ Blob\ Storage.\ If\ omitted
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ then\ the\ credential\ will\ be\ obtained\ from\ the
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment.\ If\ no\ credentials\ can\ be\ found\ in\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used\ for\ authenticating\ with\ all\ other\ Azure
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ services.\ If\ no\ credentials\ can\ be\ found\ in\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ then\ the\ default\ Azure\ authentication\ flow
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ also\ be\ used\ for\ Azure\ Blob\ Storage.
 \ \ \-\-encryption\-scope\ ENCRYPTION_SCOPE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ name\ of\ an\ encryption\ scope\ defined\ in\ the\ Azure
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Blob\ Storage\ service\ which\ is\ to\ be\ used\ to\ encrypt
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ data\ in\ Azure
+\ \ \-\-azure\-subscription\-id\ AZURE_SUBSCRIPTION_ID
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ ID\ of\ the\ Azure\ subscription\ which\ owns\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ instance\ and\ storage\ volumes\ defined\ by\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \-\-snapshot\-instance\ and\ \-\-snapshot\-disk\ arguments.
+\ \ \-\-azure\-resource\-group\ AZURE_RESOURCE_GROUP
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ name\ of\ the\ Azure\ resource\ group\ to\ which\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ compute\ instance\ and\ disks\ defined\ by\ the\ \-\-snapshot\-
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ instance\ and\ \-\-snapshot\-disk\ arguments\ belong.
 
 Extra\ options\ for\ google\-cloud\-storage\ cloud\ provider:
-\ \ \-\-snapshot\-gcp\-project\ SNAPSHOT_GCP_PROJECT
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ GCP\ project\ under\ which\ disk\ snapshots\ should\ be\ stored
+\ \ \-\-snapshot\-gcp\-project\ GCP_PROJECT
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ GCP\ project\ under\ which\ disk\ snapshots\ should\ be
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ stored\ (deprecated:\ replaced\ by\ \-\-gcp\-project)
+\ \ \-\-gcp\-project\ GCP_PROJECT
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ GCP\ project\ under\ which\ disk\ snapshots\ should\ be
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ stored
 \ \ \-\-kms\-key\-name\ KMS_KEY_NAME
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ name\ of\ the\ GCP\ KMS\ key\ which\ should\ be\ used\ for
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ encrypting\ the\ uploaded\ data\ in\ GCS.
+\ \ \-\-gcp\-zone\ GCP_ZONE\ \ \ Zone\ of\ the\ disks\ from\ which\ snapshots\ should\ be\ taken
 \f[]
 .fi
 .SH REFERENCES
 .PP
 For Boto:
 .IP \[bu] 2
 https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-cloud-check-wal-archive.1.md` & `barman-3.6.0/doc/barman-cloud-check-wal-archive.1.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-CHECK-WAL-ARCHIVE(1) Barman User manuals | Version 3.5.0
+% BARMAN-CLOUD-CHECK-WAL-ARCHIVE(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% March 29, 2023
+% June 15, 2023
 
 # NAME
 
 barman-cloud-check-wal-archive - Check a WAL archive destination for a new PostgreSQL cluster
 
 
 # SYNOPSIS
@@ -26,15 +26,15 @@
 # Usage
 ```
 usage: barman-cloud-check-wal-archive [-V] [--help] [-v | -q] [-t]
                                       [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
                                       [--endpoint-url ENDPOINT_URL]
                                       [-P PROFILE]
                                       [--read-timeout READ_TIMEOUT]
-                                      [--credential {azure-cli,managed-identity}]
+                                      [--azure-credential {azure-cli,managed-identity}]
                                       [--timeline TIMELINE]
                                       destination_url server_name
 
 Checks that the WAL archive on the specified cloud storage can be safely used
 for a new PostgreSQL server.
 
 positional arguments:
@@ -61,21 +61,23 @@
                         file)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
-  --credential {azure-cli,managed-identity}
+  --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
-                        authenticating with Azure Blob Storage. If omitted
-                        then the credential will be obtained from the
-                        environment. If no credentials can be found in the
+                        authenticating with Azure. If omitted then Azure Blob
+                        Storage credentials will be obtained from the
+                        environment and the default Azure authentication flow
+                        will be used for authenticating with all other Azure
+                        services. If no credentials can be found in the
                         environment then the default Azure authentication flow
-                        will be used
+                        will also be used for Azure Blob Storage.
 ```
 # REFERENCES
 
 For Boto:
 
 * https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-cloud-wal-restore.1.md` & `barman-3.6.0/doc/barman-cloud-wal-restore.1.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-WAL-RESTORE(1) Barman User manuals | Version 3.5.0
+% BARMAN-CLOUD-WAL-RESTORE(1) Barman User manuals | Version 3.6.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% March 29, 2023
+% June 15, 2023
 
 # NAME
 
 barman-cloud-wal-restore - Restore PostgreSQL WAL files from the Cloud using `restore_command`
 
 
 # SYNOPSIS
@@ -24,15 +24,15 @@
 
 # Usage
 ```
 usage: barman-cloud-wal-restore [-V] [--help] [-v | -q] [-t]
                                 [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
                                 [--endpoint-url ENDPOINT_URL] [-P PROFILE]
                                 [--read-timeout READ_TIMEOUT]
-                                [--credential {azure-cli,managed-identity}]
+                                [--azure-credential {azure-cli,managed-identity}]
                                 source_url server_name wal_name wal_dest
 
 This script can be used as a `restore_command` to download WAL files
 previously archived with barman-cloud-wal-archive command. Currently AWS S3,
 Azure Blob Storage and Google Cloud Storage are supported.
 
 positional arguments:
@@ -61,21 +61,23 @@
                         file)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
-  --credential {azure-cli,managed-identity}
+  --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
-                        authenticating with Azure Blob Storage. If omitted
-                        then the credential will be obtained from the
-                        environment. If no credentials can be found in the
+                        authenticating with Azure. If omitted then Azure Blob
+                        Storage credentials will be obtained from the
+                        environment and the default Azure authentication flow
+                        will be used for authenticating with all other Azure
+                        services. If no credentials can be found in the
                         environment then the default Azure authentication flow
-                        will be used
+                        will also be used for Azure Blob Storage.
 ```
 # REFERENCES
 
 For Boto:
 
 * https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
```

### Comparing `barman-3.5.0/doc/barman-cloud-backup-show.1` & `barman-3.6.0/doc/barman-cloud-restore.1`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,103 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-BACKUP\-SHOW" "1" "January 26, 2023" "Barman User manuals" "Version 3.4.0"
+.TH "BARMAN\-CLOUD\-RESTORE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
 .hy
 .SH NAME
 .PP
-barman\-cloud\-backup\-show \- Show metadata for a backup stored in the
-Cloud
+barman\-cloud\-restore \- Restore a PostgreSQL backup from the Cloud
 .SH SYNOPSIS
 .PP
-barman\-cloud\-backup\-show [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
-\f[I]SERVER_NAME\f[] \f[I]BACKUP_ID\f[]
+barman\-cloud\-restore [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
+\f[I]SERVER_NAME\f[] \f[I]BACKUP_ID\f[] \f[I]RECOVERY_DIR\f[]
 .SH DESCRIPTION
 .PP
-This script can be used to display metadata for backups previously made
-with the \f[C]barman\-cloud\-backup\f[] command.
+This script can be used to download a backup previously made with
+\f[C]barman\-cloud\-backup\f[] command.
 Currently AWS S3, Azure Blob Storage and Google Cloud Storage are
 supported.
 .PP
+This script can also be used to prepare for recovery from a snapshot
+backup by checking the attached disks were cloned from the correct
+snapshots and downloading the backup label from object storage.
+.PP
 This script and Barman are administration tools for disaster recovery of
 PostgreSQL servers written in Python and maintained by EnterpriseDB.
 .SH Usage
 .IP
 .nf
 \f[C]
-usage:\ barman\-cloud\-backup\-show\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-credential\ {azure\-cli,managed\-identity}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-format\ FORMAT]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name\ backup_id
-
-This\ script\ can\ be\ used\ to\ show\ metadata\ for\ backups\ made\ with\ barman\-cloud\-
-backup\ command.\ Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and\ Google\ Cloud\ Storage
-are\ supported.
+usage:\ barman\-cloud\-restore\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-tablespace\ NAME:LOCATION]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-recovery\-instance\ SNAPSHOT_RECOVERY_INSTANCE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-recovery\-zone\ GCP_ZONE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-gcp\-zone\ GCP_ZONE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-resource\-group\ AZURE_RESOURCE_GROUP]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name\ backup_id\ recovery_dir
+
+This\ script\ can\ be\ used\ to\ download\ a\ backup\ previously\ made\ with\ barman\-
+cloud\-backup\ command.Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and\ Google\ Cloud
+Storage\ are\ supported.
 
 positional\ arguments:
 \ \ source_url\ \ \ \ \ \ \ \ \ \ \ \ URL\ of\ the\ cloud\ source,\ such\ as\ a\ bucket\ in\ AWS\ S3.
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ For\ example:\ `s3://bucket/path/to/folder`.
 \ \ server_name\ \ \ \ \ \ \ \ \ \ \ the\ name\ of\ the\ server\ as\ configured\ in\ Barman.
 \ \ backup_id\ \ \ \ \ \ \ \ \ \ \ \ \ the\ backup\ ID
+\ \ recovery_dir\ \ \ \ \ \ \ \ \ \ the\ path\ to\ a\ directory\ for\ recovery.
 
 optional\ arguments:
 \ \ \-V,\ \-\-version\ \ \ \ \ \ \ \ \ show\ program\[aq]s\ version\ number\ and\ exit
 \ \ \-\-help\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ show\ this\ help\ message\ and\ exit
 \ \ \-v,\ \-\-verbose\ \ \ \ \ \ \ \ \ increase\ output\ verbosity\ (e.g.,\ \-vv\ is\ more\ than\ \-v)
 \ \ \-q,\ \-\-quiet\ \ \ \ \ \ \ \ \ \ \ decrease\ output\ verbosity\ (e.g.,\ \-qq\ is\ less\ than\ \-q)
 \ \ \-t,\ \-\-test\ \ \ \ \ \ \ \ \ \ \ \ Test\ cloud\ connectivity\ and\ exit
 \ \ \-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ cloud\ provider\ to\ use\ as\ a\ storage\ backend
-\ \ \-\-format\ FORMAT\ \ \ \ \ \ \ Output\ format\ (console\ or\ json).\ Default\ console.
+\ \ \-\-tablespace\ NAME:LOCATION
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ tablespace\ relocation\ rule
+\ \ \-\-snapshot\-recovery\-instance\ SNAPSHOT_RECOVERY_INSTANCE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Instance\ where\ the\ disks\ recovered\ from\ the\ snapshots
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ are\ attached
+\ \ \-\-snapshot\-recovery\-zone\ GCP_ZONE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Zone\ containing\ the\ instance\ and\ disks\ for\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ snapshot\ recovery\ (deprecated:\ replaced\ by\ \-\-gcp\-zone)
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
 \ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
-\ \ \-\-credential\ {azure\-cli,managed\-identity}
+\ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure\ Blob\ Storage.\ If\ omitted
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ then\ the\ credential\ will\ be\ obtained\ from\ the
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment.\ If\ no\ credentials\ can\ be\ found\ in\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used\ for\ authenticating\ with\ all\ other\ Azure
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ services.\ If\ no\ credentials\ can\ be\ found\ in\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ then\ the\ default\ Azure\ authentication\ flow
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ be\ used
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ will\ also\ be\ used\ for\ Azure\ Blob\ Storage.
+\ \ \-\-azure\-resource\-group\ AZURE_RESOURCE_GROUP
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Resource\ group\ containing\ the\ instance\ and\ disks\ for
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ snapshot\ recovery
+
+Extra\ options\ for\ google\-cloud\-storage\ cloud\ provider:
+\ \ \-\-gcp\-zone\ GCP_ZONE\ \ \ Zone\ containing\ the\ instance\ and\ disks\ for\ the
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ snapshot\ recovery
 \f[]
 .fi
 .SH REFERENCES
 .PP
 For Boto:
 .IP \[bu] 2
 https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html
@@ -103,26 +127,28 @@
 .PP
 If using \f[C]\-\-cloud\-provider=azure\-blob\-storage\f[]:
 .IP \[bu] 2
 azure\-storage\-blob
 .IP \[bu] 2
 azure\-identity (optional, if you wish to use DefaultAzureCredential)
 .PP
-If using \f[C]\-\-cloud\-provider=google\-cloud\-storage\f[]
-.IP \[bu] 2
+If using \f[C]\-\-cloud\-provider=google\-cloud\-storage\f[] *
 google\-cloud\-storage
+.PP
+If using \f[C]\-\-cloud\-provider=google\-cloud\-storage\f[] with
+snapshot backups * grpcio * google\-cloud\-compute
 .SH EXIT STATUS
 .TP
 .B 0
 Success
 .RS
 .RE
 .TP
 .B 1
-The show command was not successful
+The restore was not successful
 .RS
 .RE
 .TP
 .B 2
 The connection to the cloud provider failed
 .RS
 .RE
```

### Comparing `barman-3.5.0/LICENSE` & `barman-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/PKG-INFO` & `barman-3.6.0/barman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barman
-Version: 3.5.0
+Version: 3.6.0
 Summary: Backup and Recovery Manager for PostgreSQL
 Home-page: https://www.pgbarman.org/
 Author: EnterpriseDB
 Author-email: barman@enterprisedb.com
 License: GPL-3.0
 Platform: Linux
 Platform: Mac OS X
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cloud
 Provides-Extra: azure
+Provides-Extra: azure-snapshots
 Provides-Extra: snappy
 Provides-Extra: google
 Provides-Extra: google-snapshots
 License-File: LICENSE
 License-File: AUTHORS
 
 Barman (Backup and Recovery Manager) is an open-source administration
```

### Comparing `barman-3.5.0/README.rst` & `barman-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/process.py` & `barman-3.6.0/barman/process.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/server.py` & `barman-3.6.0/barman/server.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/fs.py` & `barman-3.6.0/barman/fs.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/xlog.py` & `barman-3.6.0/barman/xlog.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/wal_archiver.py` & `barman-3.6.0/barman/wal_archiver.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/clients/cloud_compression.py` & `barman-3.6.0/barman/clients/cloud_compression.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/clients/walrestore.py` & `barman-3.6.0/barman/clients/walrestore.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/clients/cloud_walrestore.py` & `barman-3.6.0/barman/clients/cloud_walrestore.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/clients/cloud_restore.py` & `barman-3.6.0/barman/clients/cloud_restore.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 from barman.clients.cloud_cli import (
     CLIErrorExit,
     create_argument_parser,
     GeneralErrorExit,
     NetworkErrorExit,
     OperationErrorExit,
-    get_missing_attrs,
 )
 from barman.cloud import CloudBackupCatalog, configure_logging
 from barman.cloud_providers import (
     get_cloud_interface,
     get_snapshot_interface_from_backup_info,
 )
 from barman.exceptions import ConfigurationException
@@ -45,22 +44,14 @@
 
     Raises a ConfigurationException if any options are missing or incompatible.
 
     :param argparse.Namespace config: The backup options provided at the command line.
     :param BackupInfo backup_info: The backup info for the backup to restore
     """
     if backup_info.snapshots_info:
-        missing_options = get_missing_attrs(
-            config, ("snapshot_recovery_instance", "snapshot_recovery_zone")
-        )
-        if len(missing_options) > 0:
-            raise ConfigurationException(
-                "Incomplete options for snapshot restore - missing: %s"
-                % ", ".join(missing_options)
-            )
         if config.tablespace != []:
             raise ConfigurationException(
                 "Backup %s is a snapshot backup therefore tablespace relocation rules "
                 "cannot be used." % backup_info.backup_id,
             )
 
 
@@ -99,20 +90,25 @@
                     config.server_name,
                 )
                 raise OperationErrorExit()
 
             _validate_config(config, backup_info)
 
             if backup_info.snapshots_info:
-                downloader = CloudBackupDownloaderSnapshot(cloud_interface, catalog)
+                snapshot_interface = get_snapshot_interface_from_backup_info(
+                    backup_info, config
+                )
+                snapshot_interface.validate_restore_config(config)
+                downloader = CloudBackupDownloaderSnapshot(
+                    cloud_interface, catalog, snapshot_interface
+                )
                 downloader.download_backup(
                     backup_info,
                     config.recovery_dir,
                     config.snapshot_recovery_instance,
-                    config.snapshot_recovery_zone,
                 )
             else:
                 downloader = CloudBackupDownloaderObjectStore(cloud_interface, catalog)
                 downloader.download_backup(
                     backup_info,
                     config.recovery_dir,
                     tablespace_map(config.tablespace),
@@ -131,15 +127,15 @@
 def parse_arguments(args=None):
     """
     Parse command line arguments
 
     :return: The options parsed
     """
 
-    parser, _, _ = create_argument_parser(
+    parser, _, azure_arguments = create_argument_parser(
         description="This script can be used to download a backup "
         "previously made with barman-cloud-backup command."
         "Currently AWS S3, Azure Blob Storage and Google Cloud Storage are supported.",
     )
     parser.add_argument("backup_id", help="the backup ID")
     parser.add_argument("recovery_dir", help="the path to a directory for recovery.")
     parser.add_argument(
@@ -151,16 +147,31 @@
     )
     parser.add_argument(
         "--snapshot-recovery-instance",
         help="Instance where the disks recovered from the snapshots are attached",
     )
     parser.add_argument(
         "--snapshot-recovery-zone",
+        help=(
+            "Zone containing the instance and disks for the snapshot recovery "
+            "(deprecated: replaced by --gcp-zone)"
+        ),
+        dest="gcp_zone",
+    )
+    gcs_arguments = parser.add_argument_group(
+        "Extra options for google-cloud-storage cloud provider"
+    )
+    gcs_arguments.add_argument(
+        "--gcp-zone",
         help="Zone containing the instance and disks for the snapshot recovery",
     )
+    azure_arguments.add_argument(
+        "--azure-resource-group",
+        help="Resource group containing the instance and disks for the snapshot recovery",
+    )
     return parser.parse_args(args=args)
 
 
 def tablespace_map(rules):
     """
     Return a mapping from tablespace names to locations built from any
     `--tablespace name:/loc/ation` rules specified.
@@ -299,35 +310,49 @@
         if not os.path.exists(wal_path):
             os.mkdir(wal_path)
 
 
 class CloudBackupDownloaderSnapshot(CloudBackupDownloader):
     """A minimal downloader for cloud backups which just retrieves the backup label."""
 
+    def __init__(self, cloud_interface, catalog, snapshot_interface):
+        """
+        Object responsible for handling interactions with cloud storage
+
+        :param CloudInterface cloud_interface: The interface to use to
+          upload the backup
+        :param str server_name: The name of the server as configured in Barman
+        :param CloudBackupCatalog catalog: The cloud backup catalog
+        :param CloudSnapshotInterface snapshot_interface: Interface for managing
+            snapshots via a cloud provider API.
+        """
+        super(CloudBackupDownloaderSnapshot, self).__init__(cloud_interface, catalog)
+        self.snapshot_interface = snapshot_interface
+
     def download_backup(
-        self, backup_info, destination_dir, recovery_instance, recovery_zone
+        self,
+        backup_info,
+        destination_dir,
+        recovery_instance,
     ):
         """
         Download a backup from cloud storage
 
         :param BackupInfo backup_info: The backup info for the backup to restore
         :param str destination_dir: Path to the destination directory
         :param str recovery_instance: The name of the VM instance to which the disks
             cloned from the backup snapshots are attached.
-        :param str recovery_zone: The zone in which the recovery disks and instance
-            reside.
         """
-        snapshot_interface = get_snapshot_interface_from_backup_info(backup_info)
-        attached_snapshots = SnapshotRecoveryExecutor.get_attached_snapshots_for_backup(
-            snapshot_interface, backup_info, recovery_instance, recovery_zone
+        attached_volumes = SnapshotRecoveryExecutor.get_attached_volumes_for_backup(
+            self.snapshot_interface,
+            backup_info,
+            recovery_instance,
         )
         cmd = UnixLocalCommand()
-        SnapshotRecoveryExecutor.check_mount_points(
-            backup_info, attached_snapshots, cmd
-        )
+        SnapshotRecoveryExecutor.check_mount_points(backup_info, attached_volumes, cmd)
         SnapshotRecoveryExecutor.check_recovery_dir_exists(destination_dir, cmd)
 
         # If the target directory does not exist then we will fail here because
         # it tells us the snapshot has not been restored.
         return self.cloud_interface.download_file(
             "/".join((self.catalog.prefix, backup_info.backup_id, "backup_label")),
             os.path.join(destination_dir, "backup_label"),
```

### Comparing `barman-3.5.0/barman/clients/cloud_check_wal_archive.py` & `barman-3.6.0/barman/clients/cloud_check_wal_archive.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/clients/__init__.py` & `barman-3.6.0/barman/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/clients/walarchive.py` & `barman-3.6.0/barman/clients/walarchive.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/clients/cloud_cli.py` & `barman-3.6.0/barman/clients/cloud_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -189,33 +189,19 @@
         help="the time in seconds until a timeout is raised when waiting to "
         "read from a connection (defaults to 60 seconds)",
     )
     azure_arguments = parser.add_argument_group(
         "Extra options for the azure-blob-storage cloud provider"
     )
     azure_arguments.add_argument(
+        "--azure-credential",
         "--credential",
         choices=["azure-cli", "managed-identity"],
-        help="Optionally specify the type of credential to use when "
-        "authenticating with Azure Blob Storage. If omitted then "
-        "the credential will be obtained from the environment. If no "
-        "credentials can be found in the environment then the default "
-        "Azure authentication flow will be used",
+        help="Optionally specify the type of credential to use when authenticating "
+        "with Azure. If omitted then Azure Blob Storage credentials will be obtained "
+        "from the environment and the default Azure authentication flow will be used "
+        "for authenticating with all other Azure services. If no credentials can be "
+        "found in the environment then the default Azure authentication flow will "
+        "also be used for Azure Blob Storage.",
+        dest="azure_credential",
     )
     return parser, s3_arguments, azure_arguments
-
-
-azure = [
-    (
-        "--credential",
-        {
-            "choices": ["azure-cli", "managed-identity"],
-            "help": (
-                "Optionally specify the type of credential to use when "
-                "authenticating with Azure Blob Storage. If omitted then "
-                "the credential will be obtained from the environment. If no "
-                "credentials can be found in the environment then the default "
-                "Azure authentication flow will be used"
-            ),
-        },
-    ),
-]
```

### Comparing `barman-3.5.0/barman/clients/cloud_backup_list.py` & `barman-3.6.0/barman/clients/cloud_backup_list.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/clients/cloud_backup.py` & `barman-3.6.0/barman/clients/cloud_backup.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from barman.clients.cloud_cli import (
     add_tag_argument,
     create_argument_parser,
     GeneralErrorExit,
     NetworkErrorExit,
     OperationErrorExit,
     UrlArgumentType,
-    get_missing_attrs,
 )
 from barman.cloud import (
     CloudBackupSnapshot,
     CloudBackupUploaderBarman,
     CloudBackupUploader,
     configure_logging,
 )
@@ -112,27 +111,19 @@
     Raises a ConfigurationException if any options are missing or incompatible.
 
     :param argparse.Namespace config: The backup options provided at the command line.
     """
     required_snapshot_variables = (
         "snapshot_disks",
         "snapshot_instance",
-        "snapshot_zone",
     )
     is_snapshot_backup = any(
         [getattr(config, var) for var in required_snapshot_variables]
     )
     if is_snapshot_backup:
-        missing_options = get_missing_attrs(config, required_snapshot_variables)
-        if len(missing_options) > 0:
-            raise ConfigurationException(
-                "Incomplete options for snapshot backup - missing: %s"
-                % ", ".join(missing_options)
-            )
-
         if getattr(config, "compression"):
             raise ConfigurationException(
                 "Compression options cannot be used with snapshot backups"
             )
 
 
 def main(args=None):
@@ -205,23 +196,23 @@
                 except PostgresConnectionError as exc:
                     logging.error("Cannot connect to postgres: %s", force_str(exc))
                     logging.debug("Exception details:", exc_info=exc)
                     raise OperationErrorExit()
 
                 with closing(postgres):
                     # Take snapshot backups if snapshot backups were specified
-                    if config.snapshot_instance:
+                    if config.snapshot_disks or config.snapshot_instance:
                         snapshot_interface = get_snapshot_interface(config)
+                        snapshot_interface.validate_backup_config(config)
                         snapshot_backup = CloudBackupSnapshot(
                             config.server_name,
                             cloud_interface,
                             snapshot_interface,
                             postgres,
                             config.snapshot_instance,
-                            config.snapshot_zone,
                             config.snapshot_disks,
                             config.backup_name,
                         )
                         snapshot_backup.backup()
                     # Otherwise upload everything to the object store
                     else:
                         uploader = CloudBackupUploader(
@@ -347,28 +338,44 @@
         metavar="NAME",
         action="append",
         default=[],
         dest="snapshot_disks",
     )
     parser.add_argument(
         "--snapshot-zone",
-        help="Zone of the disks from which snapshots should be taken",
+        help=(
+            "Zone of the disks from which snapshots should be taken (deprecated: "
+            "replaced by --gcp-zone)"
+        ),
+        dest="gcp_zone",
     )
     gcs_arguments = parser.add_argument_group(
         "Extra options for google-cloud-storage cloud provider"
     )
     gcs_arguments.add_argument(
         "--snapshot-gcp-project",
+        help=(
+            "GCP project under which disk snapshots should be stored (deprecated: "
+            "replaced by --gcp-project)"
+        ),
+        dest="gcp_project",
+    )
+    gcs_arguments.add_argument(
+        "--gcp-project",
         help="GCP project under which disk snapshots should be stored",
     )
     gcs_arguments.add_argument(
         "--kms-key-name",
         help="The name of the GCP KMS key which should be used for encrypting the "
         "uploaded data in GCS.",
     )
+    gcs_arguments.add_argument(
+        "--gcp-zone",
+        help="Zone of the disks from which snapshots should be taken",
+    )
     add_tag_argument(
         parser,
         name="tags",
         help="Tags to be added to all uploaded files in cloud storage",
     )
     s3_arguments.add_argument(
         "-e",
@@ -384,12 +391,22 @@
         "the key. Only allowed if `-e/--encryption` is set to `aws:kms`.",
     )
     azure_arguments.add_argument(
         "--encryption-scope",
         help="The name of an encryption scope defined in the Azure Blob Storage "
         "service which is to be used to encrypt the data in Azure",
     )
+    azure_arguments.add_argument(
+        "--azure-subscription-id",
+        help="The ID of the Azure subscription which owns the instance and storage "
+        "volumes defined by the --snapshot-instance and --snapshot-disk arguments.",
+    )
+    azure_arguments.add_argument(
+        "--azure-resource-group",
+        help="The name of the Azure resource group to which the compute instance and "
+        "disks defined by the --snapshot-instance and --snapshot-disk arguments belong.",
+    )
     return parser.parse_args(args=args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `barman-3.5.0/barman/clients/cloud_backup_delete.py` & `barman-3.6.0/barman/clients/cloud_backup_delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,37 +162,51 @@
             catalog.remove_wal_from_cache(wal_name)
 
 
 def _delete_backup(
     cloud_interface,
     catalog,
     backup_id,
-    dry_run=True,
+    config,
     skip_wal_cleanup_if_standalone=True,
 ):
     backup_info = catalog.get_backup_info(backup_id)
     if not backup_info:
         logging.warning("Backup %s does not exist", backup_id)
         return
     if backup_info.snapshots_info:
         logging.debug(
             "Will delete the following snapshots: %s",
             ", ".join(
                 snapshot.identifier for snapshot in backup_info.snapshots_info.snapshots
             ),
         )
-        if not dry_run:
-            snapshot_interface = get_snapshot_interface_from_backup_info(backup_info)
+        if not config.dry_run:
+            snapshot_interface = get_snapshot_interface_from_backup_info(
+                backup_info, config
+            )
             snapshot_interface.delete_snapshot_backup(backup_info)
+        else:
+            print("Skipping deletion of snapshots due to --dry-run option")
+        # Delete the backup_label for snapshots backups as this is not stored in the
+        # same format used by the non-snapshot backups.
+        backup_label_path = os.path.join(
+            catalog.prefix, backup_info.backup_id, "backup_label"
+        )
+        if not config.dry_run:
+            cloud_interface.delete_objects([backup_label_path])
+        else:
+            print("Skipping deletion of %s due to --dry-run option" % backup_label_path)
+
     objects_to_delete = _get_files_for_backup(catalog, backup_info)
     backup_info_path = os.path.join(
         catalog.prefix, backup_info.backup_id, "backup.info"
     )
     logging.debug("Will delete backup.info file at %s" % backup_info_path)
-    if not dry_run:
+    if not config.dry_run:
         try:
             cloud_interface.delete_objects(objects_to_delete)
             # Do not try to delete backup.info until we have successfully deleted
             # everything else so that it is possible to retry the operation should
             # we fail to delete any backup file
             cloud_interface.delete_objects([backup_info_path])
         except Exception as exc:
@@ -201,15 +215,19 @@
     else:
         print(
             "Skipping deletion of objects %s due to --dry-run option"
             % (objects_to_delete + [backup_info_path])
         )
 
     _remove_wals_for_backup(
-        cloud_interface, catalog, backup_info, dry_run, skip_wal_cleanup_if_standalone
+        cloud_interface,
+        catalog,
+        backup_info,
+        config.dry_run,
+        skip_wal_cleanup_if_standalone,
     )
     # It is important that the backup is removed from the catalog after cleaning
     # up the WALs because the code in _remove_wals_for_backup depends on the
     # deleted backup existing in the backup catalog
     catalog.remove_backup_from_cache(backup_id)
 
 
@@ -261,15 +279,15 @@
                         "as it has a current keep request. If you really "
                         "want to delete this backup please remove the keep "
                         "and try again.",
                         backup_id,
                         config.server_name,
                     )
                     raise OperationErrorExit()
-                _delete_backup(cloud_interface, catalog, backup_id, config.dry_run)
+                _delete_backup(cloud_interface, catalog, backup_id, config)
             elif config.retention_policy:
                 try:
                     retention_policy = RetentionPolicyFactory.create(
                         "retention_policy",
                         config.retention_policy,
                         server_name=config.server_name,
                         catalog=catalog,
@@ -292,15 +310,15 @@
                     ]
                 )
                 for backup_id in backups_to_delete:
                     _delete_backup(
                         cloud_interface,
                         catalog,
                         backup_id,
-                        config.dry_run,
+                        config,
                         skip_wal_cleanup_if_standalone=False,
                     )
     except Exception as exc:
         logging.error("Barman cloud backup delete exception: %s", force_str(exc))
         logging.debug("Exception details:", exc_info=exc)
         raise GeneralErrorExit()
```

### Comparing `barman-3.5.0/barman/clients/cloud_backup_keep.py` & `barman-3.6.0/barman/clients/cloud_backup_keep.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/clients/cloud_backup_show.py` & `barman-3.6.0/barman/clients/cloud_backup_show.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/clients/cloud_walarchive.py` & `barman-3.6.0/barman/clients/cloud_walarchive.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/diagnose.py` & `barman-3.6.0/barman/diagnose.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/lockfile.py` & `barman-3.6.0/barman/lockfile.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/utils.py` & `barman-3.6.0/barman/utils.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/annotations.py` & `barman-3.6.0/barman/annotations.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/cloud_providers/google_cloud_storage.py` & `barman-3.6.0/barman/cloud_providers/google_cloud_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,18 @@
     CloudInterface,
     CloudProviderError,
     CloudSnapshotInterface,
     DecompressingStreamingIO,
     DEFAULT_DELIMITER,
     SnapshotMetadata,
     SnapshotsInfo,
+    VolumeMetadata,
 )
-from barman.exceptions import SnapshotBackupException
+
+from barman.exceptions import CommandException, SnapshotBackupException
 
 try:
     # Python 3.x
     from urllib.parse import urlparse
 except ImportError:
     # Python 2.x
     from urlparse import urlparse
@@ -367,75 +369,86 @@
     """
     Implementation of ClourSnapshotInterface for persistend disk snapshots as
     implemented in Google Cloud Platform as documented at:
 
         https://cloud.google.com/compute/docs/disks/create-snapshots
     """
 
+    _required_config_for_backup = CloudSnapshotInterface._required_config_for_backup + (
+        "gcp_zone",
+    )
+
+    _required_config_for_restore = (
+        CloudSnapshotInterface._required_config_for_restore + ("gcp_zone",)
+    )
+
     DEVICE_PREFIX = "/dev/disk/by-id/google-"
 
-    def __init__(self, project):
+    def __init__(self, project, zone=None):
         """
         Imports the google cloud compute library and creates the clients necessary for
         creating and managing snapshots.
 
         :param str project: The name of the GCP project to which all resources related
             to the snapshot backups belong.
+        :param str|None zone: The zone in which resources accessed through this
+            snapshot interface reside.
         """
         if project is None:
             raise TypeError("project cannot be None")
         self.project = project
+        self.zone = zone
 
         # The import of this module is deferred until this constructor so that it
         # does not become a spurious dependency of the main cloud interface. Doing
         # so would break backup to GCS for anyone unable to install
         # google-cloud-compute (which includes anyone using python 2.7).
         compute = import_google_cloud_compute()
 
         self.client = compute.SnapshotsClient()
         self.disks_client = compute.DisksClient()
         self.instances_client = compute.InstancesClient()
 
-    def _get_instance_metadata(self, instance_name, zone):
+    def _get_instance_metadata(self, instance_name):
         """
         Retrieve the metadata for the named instance in the specified zone.
 
         :rtype: google.cloud.compute_v1.types.Instance
         :return: An object representing the compute instance.
         """
         try:
             return self.instances_client.get(
                 instance=instance_name,
-                zone=zone,
+                zone=self.zone,
                 project=self.project,
             )
         except NotFound:
             raise SnapshotBackupException(
                 "Cannot find instance with name %s in zone %s for project %s"
-                % (instance_name, zone, self.project)
+                % (instance_name, self.zone, self.project)
             )
 
-    def _get_disk_metadata(self, disk_name, zone):
+    def _get_disk_metadata(self, disk_name):
         """
         Retrieve the metadata for the named disk in the specified zone.
 
         :rtype: google.cloud.compute_v1.types.Disk
         :return: An object representing the disk.
         """
         try:
             return self.disks_client.get(
-                disk=disk_name, zone=zone, project=self.project
+                disk=disk_name, zone=self.zone, project=self.project
             )
         except NotFound:
             raise SnapshotBackupException(
                 "Cannot find disk with name %s in zone %s for project %s"
-                % (disk_name, zone, self.project)
+                % (disk_name, self.zone, self.project)
             )
 
-    def take_snapshot(self, backup_info, disk_zone, disk_name):
+    def _take_snapshot(self, backup_info, disk_zone, disk_name):
         """
         Take a snapshot of a persistent disk in GCP.
 
         :param barman.infofile.LocalBackupInfo backup_info: Backup information.
         :param str disk_zone: The zone in which the disk resides.
         :param str disk_name: The name of the source disk for the snapshot.
         :rtype: str
@@ -479,59 +492,52 @@
                     for warning in resp.warnings
                 )
             )
 
         _logger.info("Snapshot '%s' completed", snapshot_name)
         return snapshot_name
 
-    def take_snapshot_backup(self, backup_info, instance_name, zone, disks):
+    def take_snapshot_backup(self, backup_info, instance_name, volumes):
         """
         Take a snapshot backup for the named instance.
 
         Creates a snapshot for each named disk and saves the required metadata
         to backup_info.snapshots_info as a GcpSnapshotsInfo object.
 
         :param barman.infofile.LocalBackupInfo backup_info: Backup information.
         :param str instance_name: The name of the VM instance to which the disks
             to be backed up are attached.
-        :param str zone: The zone in which the snapshot disks and instance reside.
-        :param list[str] disks: A list containing the names of the source disks.
+        :param dict[str,barman.cloud.VolumeMetadata] volumes: Metadata for the volumes
+            to be backed up.
         """
-        instance_metadata = self._get_instance_metadata(instance_name, zone)
+        instance_metadata = self._get_instance_metadata(instance_name)
         snapshots = []
-        for disk_name in disks:
-            disk_metadata = self._get_disk_metadata(disk_name, zone)
-            # Check disk is attached and find device name
-            attached_disks = [
-                d
-                for d in instance_metadata.disks
-                if d.source == disk_metadata.self_link
-            ]
-            if len(attached_disks) == 0:
-                raise SnapshotBackupException(
-                    "Disk %s not attached to instance %s" % (disk_name, instance_name)
-                )
-            # We should always have exactly one attached disk matching the name
-            assert len(attached_disks) == 1
+        for disk_name, volume_metadata in volumes.items():
+            snapshot_name = self._take_snapshot(backup_info, self.zone, disk_name)
 
-            snapshot_name = self.take_snapshot(backup_info, zone, disk_name)
+            # Save useful metadata
+            attachment_metadata = [
+                d for d in instance_metadata.disks if d.source.endswith(disk_name)
+            ][0]
             snapshots.append(
                 GcpSnapshotMetadata(
-                    device_name=attached_disks[0].device_name,
                     snapshot_name=snapshot_name,
                     snapshot_project=self.project,
+                    device_name=attachment_metadata.device_name,
+                    mount_options=volume_metadata.mount_options,
+                    mount_point=volume_metadata.mount_point,
                 )
             )
 
         # Add snapshot metadata to BackupInfo
         backup_info.snapshots_info = GcpSnapshotsInfo(
             project=self.project, snapshots=snapshots
         )
 
-    def delete_snapshot(self, snapshot_name):
+    def _delete_snapshot(self, snapshot_name):
         """
         Delete the specified snapshot.
 
         :param str snapshot_name: The short name used to reference the snapshot within GCP.
         """
         try:
             resp = self.client.delete(
@@ -571,110 +577,177 @@
         """
         for snapshot in backup_info.snapshots_info.snapshots:
             _logger.info(
                 "Deleting snapshot '%s' for backup %s",
                 snapshot.identifier,
                 backup_info.backup_id,
             )
-            self.delete_snapshot(snapshot.identifier)
+            self._delete_snapshot(snapshot.identifier)
 
-    def get_attached_devices(self, instance_name, zone):
+    def get_attached_volumes(self, instance_name, disks=None):
         """
-        Returns the non-boot devices attached to instance_name in zone.
+        Returns metadata for the volumes attached to this instance.
+
+        Queries GCP for metadata relating to the volumes attached to the named instance
+        and returns a dict of `VolumeMetadata` objects, keyed by disk name.
+
+        If the optional disks parameter is supplied then this method returns metadata
+        for the disks in the supplied list only. A SnapshotBackupException is raised if
+        any of the supplied disks are not found to be attached to the instance.
+
+        If the disks parameter is not supplied then this method returns a
+        VolumeMetadata for all disks attached to this instance.
 
         :param str instance_name: The name of the VM instance to which the disks
             to be backed up are attached.
-        :param str zone: The zone in which the snapshot disks and instance reside.
-        :rtype: dict[str,str]
-        :return: A dict where the key is the disk name and the value is the device
-            path for that disk on the specified instance.
-        """
-        instance_metadata = self._get_instance_metadata(instance_name, zone)
-        attached_devices = {}
-        for attached_disk in instance_metadata.disks:
-            disk_name = posixpath.split(urlparse(attached_disk.source).path)[-1]
+        :param list[str]|None disks: A list containing the names of disks to be
+            backed up.
+        :rtype: dict[str, VolumeMetadata]
+        :return: A dict of VolumeMetadata objects representing each volume
+            attached to the instance, keyed by volume identifier.
+        """
+        instance_metadata = self._get_instance_metadata(instance_name)
+        attached_volumes = {}
+        for attachment_metadata in instance_metadata.disks:
+            disk_name = posixpath.split(urlparse(attachment_metadata.source).path)[-1]
+            if disks and disk_name not in disks:
+                continue
             if disk_name == "":
                 raise SnapshotBackupException(
                     "Could not parse disk name for source %s attached to instance %s"
-                    % (attached_disk.source, instance_name)
+                    % (attachment_metadata.source, instance_name)
                 )
-            full_device_name = self.DEVICE_PREFIX + attached_disk.device_name
-            if disk_name in attached_devices:
+            assert disk_name not in attached_volumes
+            disk_metadata = self._get_disk_metadata(disk_name)
+            attached_volumes[disk_name] = GcpVolumeMetadata(
+                attachment_metadata,
+                disk_metadata,
+            )
+        # Check all requested disks were found and complain if necessary
+        if disks is not None:
+            unattached_disks = []
+            for disk_name in disks:
+                if disk_name not in attached_volumes:
+                    # Verify the disk definitely exists by fetching the metadata
+                    self._get_disk_metadata(disk_name)
+                    # Append to list of unattached disks
+                    unattached_disks.append(disk_name)
+            if len(unattached_disks) > 0:
                 raise SnapshotBackupException(
-                    "Disk %s appears to be attached with name %s as devices %s and %s"
-                    % (
-                        attached_disk.source,
-                        disk_name,
-                        full_device_name,
-                        attached_devices[disk_name],
-                    )
+                    "Disks not attached to instance %s: %s"
+                    % (instance_name, ", ".join(unattached_disks))
                 )
-            attached_devices[disk_name] = full_device_name
-
-        return attached_devices
+        return attached_volumes
 
-    def get_attached_snapshots(self, instance_name, zone):
+    def instance_exists(self, instance_name):
         """
-        Returns the snapshots which are sources for disks attached to instance.
-
-        Queries the instance metadata to determine which disks are attached and
-        then queries the disk metadata for each disk to determine whether it was
-        cloned from a snapshot. If it was cloned then the snapshot is added to the
-        dict which is returned once all attached devices have been checked.
+        Determine whether the named instance exists.
 
         :param str instance_name: The name of the VM instance to which the disks
             to be backed up are attached.
-        :param str zone: The zone in which the snapshot disks and instance reside.
-        :rtype: dict[str,str]
-        :return: A dict where the key is the snapshot name and the value is the
-            device path for the source disk for that snapshot on the specified
-            instance.
-        """
-        attached_devices = self.get_attached_devices(instance_name, zone)
-        attached_snapshots = {}
-        for disk_name, device_name in attached_devices.items():
-            disk_metadata = self._get_disk_metadata(disk_name, zone)
+        :rtype: bool
+        :return: True if the named instance exists, False otherwise.
+        """
+        try:
+            self.instances_client.get(
+                instance=instance_name,
+                zone=self.zone,
+                project=self.project,
+            )
+        except NotFound:
+            return False
+        return True
+
+
+class GcpVolumeMetadata(VolumeMetadata):
+    """
+    Specialization of VolumeMetadata for GCP persistent disks.
+
+    This class uses the device name obtained from the GCP API to determine the full
+    path to the device on the compute instance. This path is then resolved to the
+    mount point using findmnt.
+    """
+
+    def __init__(self, attachment_metadata=None, disk_metadata=None):
+        """
+        Creates a GcpVolumeMetadata instance using metadata obtained from the GCP API.
+
+        Uses attachment_metadata to obtain the device name and resolves this to the
+        full device path on the instance using a documented prefix.
+
+        Uses disk_metadata to obtain the source snapshot name, if such a snapshot
+        exists.
+
+        :param google.cloud.compute_v1.types.AttachedDisk attachment_metadata: An
+            object representing the disk as attached to the instance.
+        :param google.cloud.compute_v1.types.Disk disk_metadata: An object representing
+            the disk.
+        """
+        super(GcpVolumeMetadata, self).__init__()
+        self._snapshot_name = None
+        self._device_path = None
+        if (
+            attachment_metadata is not None
+            and attachment_metadata.device_name is not None
+        ):
+            self._device_path = (
+                GcpCloudSnapshotInterface.DEVICE_PREFIX
+                + attachment_metadata.device_name
+            )
+        if disk_metadata is not None:
             if disk_metadata.source_snapshot is not None:
                 attached_snapshot_name = posixpath.split(
                     urlparse(disk_metadata.source_snapshot).path
                 )[-1]
             else:
                 attached_snapshot_name = ""
             if attached_snapshot_name != "":
-                attached_snapshots[attached_snapshot_name] = device_name
-        return attached_snapshots
+                self._snapshot_name = attached_snapshot_name
 
-    def instance_exists(self, instance_name, zone):
+    def resolve_mounted_volume(self, cmd):
         """
-        Determine whether the named instance exists in the specified zone.
+        Resolve the mount point and mount options using shell commands.
 
-        :param str instance_name: The name of the VM instance to which the disks
-            to be backed up are attached.
-        :param str zone: The zone in which the snapshot disks and instance reside.
-        :rtype: bool
-        :return: True if the named instance exists in zone, False otherwise.
+        Uses findmnt to retrieve the mount point and mount options for the device
+        path at which this volume is mounted.
         """
+        if self._device_path is None:
+            raise SnapshotBackupException(
+                "Cannot resolve mounted volume: Device path unknown"
+            )
         try:
-            self.instances_client.get(
-                instance=instance_name,
-                zone=zone,
-                project=self.project,
+            mount_point, mount_options = cmd.findmnt(self._device_path)
+        except CommandException as e:
+            raise SnapshotBackupException(
+                "Error finding mount point for device %s: %s" % (self._device_path, e)
             )
-        except NotFound:
-            return False
-        return True
+        if mount_point is None:
+            raise SnapshotBackupException(
+                "Could not find device %s at any mount point" % self._device_path
+            )
+        self._mount_point = mount_point
+        self._mount_options = mount_options
+
+    @property
+    def source_snapshot(self):
+        """
+        An identifier which can reference the snapshot via the cloud provider.
+
+        :rtype: str
+        :return: The snapshot short name.
+        """
+        return self._snapshot_name
 
 
 class GcpSnapshotMetadata(SnapshotMetadata):
     """
     Specialization of SnapshotMetadata for GCP persistent disk snapshots.
 
     Stores the device_name, snapshot_name and snapshot_project in the provider-specific
-    field, uses the short snapshot name as the identifier, and forges the device path
-    using the hardcoded (but documented in the API docs) prefix.
+    field and uses the short snapshot name as the identifier.
     """
 
     _provider_fields = ("device_name", "snapshot_name", "snapshot_project")
 
     def __init__(
         self,
         mount_options=None,
@@ -688,15 +761,15 @@
 
         :param str mount_options: The mount options used for the source disk at the
             time of the backup.
         :param str mount_point: The mount point of the source disk at the time of
             the backup.
         :param str device_name: The short device name used in the GCP API.
         :param str snapshot_name: The short snapshot name used in the GCP API.
-        :param str project: The GCP project name.
+        :param str snapshot_project: The GCP project name.
         """
         super(GcpSnapshotMetadata, self).__init__(mount_options, mount_point)
         self.device_name = device_name
         self.snapshot_name = snapshot_name
         self.snapshot_project = snapshot_project
 
     @property
@@ -705,25 +778,14 @@
         An identifier which can reference the snapshot via the cloud provider.
 
         :rtype: str
         :return: The snapshot short name.
         """
         return self.snapshot_name
 
-    @property
-    def device(self):
-        """
-        The device path to the source disk on the compute instance at the time the
-        backup was taken.
-
-        :rtype: str
-        :return: The full path to the source disk device.
-        """
-        return GcpCloudSnapshotInterface.DEVICE_PREFIX + self.device_name
-
 
 class GcpSnapshotsInfo(SnapshotsInfo):
     """
     Represents the snapshots_info field for GCP persistent disk snapshots.
     """
 
     _provider_fields = ("project",)
```

### Comparing `barman-3.5.0/barman/cloud_providers/__init__.py` & `barman-3.6.0/barman/cloud_providers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -63,46 +63,53 @@
             raise CloudProviderOptionUnsupported(
                 'Encryption type must be "aws:kms" if SSE KMS Key ID is specified'
             )
         cloud_interface_kwargs["sse_kms_key_id"] = config.sse_kms_key_id
     return S3CloudInterface(**cloud_interface_kwargs)
 
 
+def _get_azure_credential(credential_type):
+    if credential_type is None:
+        return None
+
+    try:
+        from azure.identity import AzureCliCredential, ManagedIdentityCredential
+    except ImportError:
+        raise SystemExit("Missing required python module: azure-identity")
+
+    supported_credentials = {
+        "azure-cli": AzureCliCredential,
+        "managed-identity": ManagedIdentityCredential,
+    }
+    try:
+        return supported_credentials[credential_type]
+    except KeyError:
+        raise CloudProviderOptionUnsupported(
+            "Unsupported credential: %s" % credential_type
+        )
+
+
 def _make_azure_cloud_interface(config, cloud_interface_kwargs):
     from barman.cloud_providers.azure_blob_storage import AzureCloudInterface
 
     _update_kwargs(
         cloud_interface_kwargs,
         config,
         (
             "encryption_scope",
             "max_block_size",
             "max_concurrency",
             "max_single_put_size",
         ),
     )
 
-    if "credential" in config and config.credential is not None:
-        try:
-            from azure.identity import AzureCliCredential, ManagedIdentityCredential
-        except ImportError:
-            raise SystemExit("Missing required python module: azure-identity")
-
-        supported_credentials = {
-            "azure-cli": AzureCliCredential,
-            "managed-identity": ManagedIdentityCredential,
-        }
-        try:
-            cloud_interface_kwargs["credential"] = supported_credentials[
-                config.credential
-            ]()
-        except KeyError:
-            raise CloudProviderOptionUnsupported(
-                "Unsupported credential: %s" % config.credential
-            )
+    if "azure_credential" in config:
+        credential = _get_azure_credential(config.azure_credential)
+        if credential is not None:
+            cloud_interface_kwargs["credential"] = credential()
 
     return AzureCloudInterface(**cloud_interface_kwargs)
 
 
 def _make_google_cloud_interface(config, cloud_interface_kwargs):
     """
     :param config: Not used yet
@@ -162,20 +169,35 @@
     :returns: A CloudSnapshotInterface for the specified snapshot_provider.
     """
     if config.cloud_provider == "google-cloud-storage":
         from barman.cloud_providers.google_cloud_storage import (
             GcpCloudSnapshotInterface,
         )
 
-        if config.snapshot_gcp_project is None:
+        if config.gcp_project is None:
             raise ConfigurationException(
-                "--snapshot-gcp-project option must be set for snapshot backups "
+                "--gcp-project option must be set for snapshot backups "
                 "when cloud provider is google-cloud-storage"
             )
-        return GcpCloudSnapshotInterface(config.snapshot_gcp_project)
+        return GcpCloudSnapshotInterface(config.gcp_project, config.gcp_zone)
+    elif config.cloud_provider == "azure-blob-storage":
+        from barman.cloud_providers.azure_blob_storage import (
+            AzureCloudSnapshotInterface,
+        )
+
+        if config.azure_subscription_id is None:
+            raise ConfigurationException(
+                "--azure-subscription-id option must be set for snapshot "
+                "backups when cloud provider is azure-blob-storage"
+            )
+        return AzureCloudSnapshotInterface(
+            config.azure_subscription_id,
+            resource_group=config.azure_resource_group,
+            credential=_get_azure_credential(config.azure_credential),
+        )
     else:
         raise CloudProviderUnsupported(
             "No snapshot provider for cloud provider: %s" % config.cloud_provider
         )
 
 
 def get_snapshot_interface_from_server_config(server_config):
@@ -189,44 +211,93 @@
     :returns: A CloudSnapshotInterface for the specified snapshot_provider.
     """
     if server_config.snapshot_provider == "gcp":
         from barman.cloud_providers.google_cloud_storage import (
             GcpCloudSnapshotInterface,
         )
 
-        if server_config.snapshot_gcp_project is None:
+        gcp_project = server_config.gcp_project or server_config.snapshot_gcp_project
+        if gcp_project is None:
             raise ConfigurationException(
-                "snapshot_gcp_project option must be set when snapshot_provider is gcp"
+                "gcp_project option must be set when snapshot_provider is gcp"
             )
-        return GcpCloudSnapshotInterface(server_config.snapshot_gcp_project)
+        gcp_zone = server_config.gcp_zone or server_config.snapshot_zone
+        return GcpCloudSnapshotInterface(gcp_project, gcp_zone)
+    elif server_config.snapshot_provider == "azure":
+        from barman.cloud_providers.azure_blob_storage import (
+            AzureCloudSnapshotInterface,
+        )
+
+        if server_config.azure_subscription_id is None:
+            raise ConfigurationException(
+                "azure_subscription_id option must be set when snapshot_provider "
+                "is azure"
+            )
+        return AzureCloudSnapshotInterface(
+            server_config.azure_subscription_id,
+            resource_group=server_config.azure_resource_group,
+            credential=_get_azure_credential(server_config.azure_credential),
+        )
     else:
         raise CloudProviderUnsupported(
             "Unsupported snapshot provider: %s" % server_config.snapshot_provider
         )
 
 
-def get_snapshot_interface_from_backup_info(backup_info):
+def get_snapshot_interface_from_backup_info(backup_info, config=None):
     """
     Factory function that creates CloudSnapshotInterface for the snapshot provider
     specified in the supplied backup info.
 
     :param barman.infofile.BackupInfo backup_info: The metadata for a specific backup.
+        cloud provider.
+    :param argparse.Namespace|barman.config.Config config: The backup options provided
+        by the command line or the Barman configuration.
     :rtype: CloudSnapshotInterface
     :returns: A CloudSnapshotInterface for the specified snapshot provider.
     """
     if backup_info.snapshots_info.provider == "gcp":
         from barman.cloud_providers.google_cloud_storage import (
             GcpCloudSnapshotInterface,
         )
 
         if backup_info.snapshots_info.project is None:
             raise BarmanException(
                 "backup_info has snapshot provider 'gcp' but project is not set"
             )
-        return GcpCloudSnapshotInterface(backup_info.snapshots_info.project)
+        gcp_zone = config is not None and config.gcp_zone or None
+        return GcpCloudSnapshotInterface(
+            backup_info.snapshots_info.project,
+            gcp_zone,
+        )
+    elif backup_info.snapshots_info.provider == "azure":
+        from barman.cloud_providers.azure_blob_storage import (
+            AzureCloudSnapshotInterface,
+        )
+
+        # When creating a snapshot interface for dealing with existing backups we use
+        # the subscription ID from that backup and the resource group specified in
+        # provider_args. This means that:
+        #   1. Resources will always belong to the same subscription.
+        #   2. Recovery resources can be in a different resource group to the one used
+        #      to create the backup.
+        if backup_info.snapshots_info.subscription_id is None:
+            raise ConfigurationException(
+                "backup_info has snapshot provider 'azure' but "
+                "subscription_id is not set"
+            )
+        if config is not None and hasattr(config, "azure_resource_group"):
+            resource_group = config.azure_resource_group
+        else:
+            resource_group = None
+        return AzureCloudSnapshotInterface(
+            backup_info.snapshots_info.subscription_id,
+            resource_group=resource_group,
+            credential=_get_azure_credential(config.azure_credential),
+        )
     else:
         raise CloudProviderUnsupported(
             "Unsupported snapshot provider in backup info: %s"
             % backup_info.snapshots_info.provider
         )
 
 
@@ -240,12 +311,18 @@
     :return: A SnapshotInfo subclass for the snapshots provider listed in the
         `provider` field of the snapshots_info.
     """
     if "provider" in snapshots_info and snapshots_info["provider"] == "gcp":
         from barman.cloud_providers.google_cloud_storage import GcpSnapshotsInfo
 
         return GcpSnapshotsInfo.from_dict(snapshots_info)
+    elif "provider" in snapshots_info and snapshots_info["provider"] == "azure":
+        from barman.cloud_providers.azure_blob_storage import (
+            AzureSnapshotsInfo,
+        )
+
+        return AzureSnapshotsInfo.from_dict(snapshots_info)
     else:
         raise CloudProviderUnsupported(
             "Unsupported snapshot provider in backup info: %s"
             % snapshots_info["provider"]
         )
```

### Comparing `barman-3.5.0/barman/cloud_providers/aws_s3.py` & `barman-3.6.0/barman/cloud_providers/aws_s3.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/config.py` & `barman-3.6.0/barman/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,14 +425,17 @@
     This class represents the configuration for a specific Server instance.
     """
 
     KEYS = [
         "active",
         "archiver",
         "archiver_batch_size",
+        "azure_credential",
+        "azure_resource_group",
+        "azure_subscription_id",
         "backup_compression",
         "backup_compression_format",
         "backup_compression_level",
         "backup_compression_location",
         "backup_compression_workers",
         "backup_directory",
         "backup_method",
@@ -447,14 +450,16 @@
         "custom_compression_filter",
         "custom_decompression_filter",
         "custom_compression_magic",
         "description",
         "disabled",
         "errors_directory",
         "forward_config_path",
+        "gcp_project",
+        "gcp_zone",
         "immediate_checkpoint",
         "incoming_wals_directory",
         "last_backup_maximum_age",
         "last_backup_minimum_size",
         "last_wal_maximum_age",
         "max_incoming_wals_queue",
         "minimum_redundancy",
@@ -489,18 +494,18 @@
         "recovery_staging_path",
         "create_slot",
         "retention_policy",
         "retention_policy_mode",
         "reuse_backup",
         "slot_name",
         "snapshot_disks",
-        "snapshot_gcp_project",
+        "snapshot_gcp_project",  # Deprecated, replaced by gcp_project
         "snapshot_instance",
         "snapshot_provider",
-        "snapshot_zone",
+        "snapshot_zone",  # Deprecated, replaced by gcp_zone
         "ssh_command",
         "streaming_archiver",
         "streaming_archiver_batch_size",
         "streaming_archiver_name",
         "streaming_backup_name",
         "streaming_conninfo",
         "streaming_wals_directory",
@@ -508,14 +513,17 @@
         "wal_retention_policy",
         "wals_directory",
     ]
 
     BARMAN_KEYS = [
         "archiver",
         "archiver_batch_size",
+        "azure_credential",
+        "azure_resource_group",
+        "azure_subscription_id",
         "backup_compression",
         "backup_compression_format",
         "backup_compression_level",
         "backup_compression_location",
         "backup_compression_workers",
         "backup_method",
         "backup_options",
@@ -525,14 +533,15 @@
         "check_timeout",
         "compression",
         "configuration_files_directory",
         "custom_compression_filter",
         "custom_decompression_filter",
         "custom_compression_magic",
         "forward_config_path",
+        "gcp_project",
         "immediate_checkpoint",
         "last_backup_maximum_age",
         "last_backup_minimum_size",
         "last_wal_maximum_age",
         "max_incoming_wals_queue",
         "minimum_redundancy",
         "network_compression",
@@ -564,15 +573,15 @@
         "recovery_options",
         "recovery_staging_path",
         "create_slot",
         "retention_policy",
         "retention_policy_mode",
         "reuse_backup",
         "slot_name",
-        "snapshot_gcp_project",
+        "snapshot_gcp_project",  # Deprecated, replaced by gcp_project
         "snapshot_provider",
         "streaming_archiver",
         "streaming_archiver_batch_size",
         "streaming_archiver_name",
         "streaming_backup_name",
         "tablespace_bandwidth_limit",
         "wal_retention_policy",
```

### Comparing `barman-3.5.0/barman/backup_executor.py` & `barman-3.6.0/barman/backup_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 from barman.exceptions import (
     BackupException,
     CommandFailedException,
     DataTransferFailure,
     FsOperationFailed,
     PostgresConnectionError,
     PostgresIsInRecovery,
+    SnapshotBackupException,
     SshCommandException,
     FileNotFoundException,
 )
 from barman.fs import UnixLocalCommand, UnixRemoteCommand, unix_command_factory
 from barman.infofile import BackupInfo
 from barman.postgres_plumbing import EXCLUDE_LIST, PGDATA_EXCLUDE_LIST
 from barman.remote_status import RemoteStatusMixin
@@ -1442,15 +1443,14 @@
         Constructor for the SnapshotBackupExecutor
 
         :param barman.backup.BackupManager backup_manager: the BackupManager
             assigned to the strategy
         """
         super(SnapshotBackupExecutor, self).__init__(backup_manager, "snapshot")
         self.snapshot_instance = self.config.snapshot_instance
-        self.snapshot_zone = self.config.snapshot_zone
         self.snapshot_disks = self.config.snapshot_disks
         self.validate_configuration()
         try:
             self.snapshot_interface = get_snapshot_interface_from_server_config(
                 self.config
             )
         except Exception as exc:
@@ -1478,117 +1478,123 @@
                 "reuse_backup option is not supported by snapshot backup_method"
             )
 
         required_config = (
             "snapshot_disks",
             "snapshot_instance",
             "snapshot_provider",
-            "snapshot_zone",
         )
         for config_var in required_config:
             if not getattr(self.server.config, config_var):
                 self.server.config.update_msg_list_and_disable_server(
                     "%s option is required by snapshot backup_method" % config_var
                 )
 
     @staticmethod
-    def add_mount_data_to_backup_info(backup_info, remote_cmd):
+    def add_mount_data_to_volume_metadata(volumes, remote_cmd):
         """
-        Adds the mount point and mount options for each disk to the backup info.
+        Adds the mount point and mount options for each supplied volume.
 
-        Each disk for which a snapshot was created during the backup is attached to the
-        instance at a given device path. This function uses the `findmnt` Unix command
-        to retrieve the mount point and mount options for each of those devices. The
-        mount data for each disk is then added to the metadata for the corresponding
-        snapshot in the backup info.
+        Calls `resolve_mounted_volume` on each supplied volume so that the volume
+        metadata (which originated from the cloud provider) can be resolved to the
+        mount point and mount options of the volume as mounted on a compute instance.
 
-        :param barman.infofile.LocalBackupInfo backup_info: Backup information.
-        :param UnixLocalCommand remote_cmd: Wrapper for local/remote commands.
+        This will set the current mount point and mount options of the volume so that
+        they can be stored in the snapshot metadata for the backup when the backup is
+        taken.
+
+        :param dict[str,barman.cloud.VolumeMetadata] volumes: Metadata for the volumes
+            attached to a specific compute instance.
+        :param UnixLocalCommand remote_cmd: Wrapper for executing local/remote commands
+            on the compute instance to which the volumes are attached.
         """
-        for snapshot in backup_info.snapshots_info.snapshots:
-            mount_point, mount_options = remote_cmd.findmnt(snapshot.device)
-            if mount_point is None:
-                raise BackupException(
-                    "Could not find mount point for device %s" % snapshot.device
-                )
-            else:
-                snapshot.mount_point = mount_point
-                snapshot.mount_options = mount_options
+        for volume in volumes.values():
+            volume.resolve_mounted_volume(remote_cmd)
 
     def backup_copy(self, backup_info):
         """
         Perform the backup using cloud provider disk snapshots.
 
         :param barman.infofile.LocalBackupInfo backup_info: Backup information.
         """
         # Create data dir so backup_label can be written
         cmd = UnixLocalCommand(path=self.server.path)
         cmd.create_dir_if_not_exists(backup_info.get_data_directory())
 
         # Start the snapshot
         self.copy_start_time = datetime.datetime.now()
 
+        # Get volume metadata for the disks to be backed up
+        volumes_to_snapshot = self.snapshot_interface.get_attached_volumes(
+            self.snapshot_instance, self.snapshot_disks
+        )
+
+        # Resolve volume metadata to mount metadata using shell commands on the
+        # compute instance to which the volumes are attached - this information
+        # can then be added to the metadata for each snapshot when the backup is
+        # taken.
+        remote_cmd = UnixRemoteCommand(ssh_command=self.server.config.ssh_command)
+        self.add_mount_data_to_volume_metadata(volumes_to_snapshot, remote_cmd)
+
         self.snapshot_interface.take_snapshot_backup(
-            backup_info, self.snapshot_instance, self.snapshot_zone, self.snapshot_disks
+            backup_info,
+            self.snapshot_instance,
+            volumes_to_snapshot,
         )
 
         self.copy_end_time = datetime.datetime.now()
 
-        # Gather additional metadata to assist recovery of snapshots
-        remote_cmd = UnixRemoteCommand(ssh_command=self.server.config.ssh_command)
-        self.add_mount_data_to_backup_info(backup_info, remote_cmd)
-
         # Store statistics about the copy
         copy_time = total_seconds(self.copy_end_time - self.copy_start_time)
         backup_info.copy_stats = {
             "copy_time": copy_time,
             "total_time": copy_time,
         }
 
     @staticmethod
     def find_missing_and_unmounted_disks(
-        cmd, snapshot_interface, snapshot_instance, snapshot_zone, snapshot_disks
+        cmd, snapshot_interface, snapshot_instance, snapshot_disks
     ):
         """
         Checks for any disks listed in snapshot_disks which are not correctly attached
         and mounted on the named instance and returns them as a tuple of two lists.
 
         This is used for checking that the disks which are to be used as sources for
         snapshots at backup time are attached and mounted on the instance to be backed
         up.
 
         :param UnixLocalCommand cmd: Wrapper for local/remote commands.
         :param barman.cloud.CloudSnapshotInterface snapshot_interface: Interface for
             taking snapshots and associated operations via cloud provider APIs.
         :param str snapshot_instance: The name of the VM instance to which the disks
             to be backed up are attached.
-        :param str snapshot_zone: The zone in which the snapshot disks and instance
-            reside.
         :param list[str] snapshot_disks: A list containing the names of the disks for
             which snapshots should be taken at backup time.
         :rtype tuple[list[str],list[str]]
         :return: A tuple where the first element is a list of all disks which are not
             attached to the VM instance and the second element is a list of all disks
             which are attached but not mounted.
         """
-        attached_devices = snapshot_interface.get_attached_devices(
-            snapshot_instance, snapshot_zone
-        )
+        attached_volumes = snapshot_interface.get_attached_volumes(snapshot_instance)
         missing_disks = []
         for disk in snapshot_disks:
-            if disk not in attached_devices.keys():
+            if disk not in attached_volumes.keys():
                 missing_disks.append(disk)
 
         unmounted_disks = []
         for disk in snapshot_disks:
             try:
-                mount_point, _mount_options = cmd.findmnt(attached_devices[disk])
+                attached_volumes[disk].resolve_mounted_volume(cmd)
+                mount_point = attached_volumes[disk].mount_point
             except KeyError:
                 # Ignore disks which were not attached
                 continue
+            except SnapshotBackupException as exc:
+                logging.warn("Error resolving mount point: {}".format(exc))
+                mount_point = None
             if mount_point is None:
                 unmounted_disks.append(disk)
 
         return missing_disks, unmounted_disks
 
     def check(self, check_strategy):
         """
@@ -1601,35 +1607,31 @@
         :param CheckStrategy check_strategy: the strategy for the management
              of the results of the various checks
         """
         super(SnapshotBackupExecutor, self).check(check_strategy)
         if self.server.config.disabled:
             # Skip checks if the server is not active
             return
-        check_strategy.init_check("snapshot instance exists in zone")
-        if not self.snapshot_interface.instance_exists(
-            self.snapshot_instance, self.snapshot_zone
-        ):
+        check_strategy.init_check("snapshot instance exists")
+        if not self.snapshot_interface.instance_exists(self.snapshot_instance):
             check_strategy.result(
                 self.config.name,
                 False,
-                hint="cannot find compute instance %s in zone %s"
-                % (self.snapshot_instance, self.snapshot_zone),
+                hint="cannot find compute instance %s" % self.snapshot_instance,
             )
             return
         else:
             check_strategy.result(self.config.name, True)
 
         check_strategy.init_check("snapshot disks attached to instance")
         cmd = unix_command_factory(self.config.ssh_command, self.server.path)
         missing_disks, unmounted_disks = self.find_missing_and_unmounted_disks(
             cmd,
             self.snapshot_interface,
             self.snapshot_instance,
-            self.snapshot_zone,
             self.snapshot_disks,
         )
 
         if len(missing_disks) > 0:
             check_strategy.result(
                 self.config.name,
                 False,
```

### Comparing `barman-3.5.0/barman/copy_controller.py` & `barman-3.6.0/barman/copy_controller.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/__init__.py` & `barman-3.6.0/barman/__init__.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/postgres.py` & `barman-3.6.0/barman/postgres.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/recovery_executor.py` & `barman-3.6.0/barman/recovery_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,22 +39,22 @@
 from barman import output, xlog
 from barman.cloud_providers import get_snapshot_interface_from_backup_info
 from barman.command_wrappers import RsyncPgData
 from barman.config import RecoveryOptions
 from barman.copy_controller import RsyncCopyController
 from barman.exceptions import (
     BadXlogSegmentName,
-    CommandException,
     CommandFailedException,
     DataTransferFailure,
     FsOperationFailed,
     RecoveryInvalidTargetException,
     RecoveryStandbyModeException,
     RecoveryTargetActionException,
     RecoveryPreconditionException,
+    SnapshotBackupException,
 )
 from barman.compression import GZipCompression, LZ4Compression, ZSTDCompression
 import barman.fs as fs
 from barman.infofile import BackupInfo, LocalBackupInfo
 from barman.utils import force_str, mkpath
 
 # generic logger for this module
@@ -1539,112 +1539,118 @@
             message = (
                 "Recovery directory '{}' does not exist on the recovery instance. "
                 "Check all required disks have been created, attached and mounted."
             ).format(recovery_dir)
             raise RecoveryPreconditionException(message)
 
     @staticmethod
-    def get_attached_snapshots_for_backup(
-        snapshot_interface, backup_info, instance_name, zone
-    ):
+    def get_attached_volumes_for_backup(snapshot_interface, backup_info, instance_name):
         """
         Verifies that disks cloned from the snapshots specified in the supplied
-        backup_info are attached to the named instance in the specified zone and
-        returns them as a dict where the keys are snapshot names and the values
-        are the names of the attached devices.
+        backup_info are attached to the named instance and returns them as a dict
+        where the keys are snapshot names and the values are the names of the
+        attached devices.
 
         If any snapshot associated with this backup is not found as the source
         for any disk attached to the instance then a RecoveryPreconditionException
         is raised.
 
         :param CloudSnapshotInterface snapshot_interface: Interface for managing
             snapshots via a cloud provider API.
         :param BackupInfo backup_info: Backup information for the backup being
             recovered.
         :param str instance_name: The name of the VM instance to which the disks
             to be backed up are attached.
-        :param str zone: The zone in which the snapshot disks and instance reside.
         :rtype: dict[str,str]
         :return: A dict where the key is the snapshot name and the value is the
             device path for the source disk for that snapshot on the specified
             instance.
         """
         if backup_info.snapshots_info is None:
             return {}
-        attached_snapshots = snapshot_interface.get_attached_snapshots(
-            instance_name, zone
-        )
-        attached_snapshots_for_backup = {}
+        attached_volumes = snapshot_interface.get_attached_volumes(instance_name)
+        attached_volumes_for_backup = {}
         missing_snapshots = []
         for source_snapshot in backup_info.snapshots_info.snapshots:
             try:
-                attached_snapshots_for_backup[
-                    source_snapshot.identifier
-                ] = attached_snapshots[source_snapshot.identifier]
-            except KeyError:
+                disk, attached_volume = [
+                    (k, v)
+                    for k, v in attached_volumes.items()
+                    if v.source_snapshot == source_snapshot.identifier
+                ][0]
+
+                attached_volumes_for_backup[disk] = attached_volume
+            except IndexError:
                 missing_snapshots.append(source_snapshot.identifier)
 
         if len(missing_snapshots) > 0:
             raise RecoveryPreconditionException(
                 "The following snapshots are not attached to recovery instance %s: %s"
                 % (instance_name, ", ".join(missing_snapshots))
             )
         else:
-            return attached_snapshots_for_backup
+            return attached_volumes_for_backup
 
     @staticmethod
-    def check_mount_points(backup_info, attached_snapshots, cmd):
+    def check_mount_points(backup_info, attached_volumes, cmd):
         """
         Check that each disk cloned from a snapshot is mounted at the same mount point
         as the original disk and with the same mount options.
 
         Raises a RecoveryPreconditionException if any of the devices supplied in
         attached_snapshots are not mounted at the mount point or with the mount options
         specified in the snapshot metadata.
 
         :param BackupInfo backup_info: Backup information for the backup being
             recovered.
-        :param dict[str,str] attached_snapshots: A dict of snapshot_name:device_path
-            mappings where the device_path is the path at which the disk cloned from
-            that snapshot is attached to the recovery instance.
+        :param dict[str,barman.cloud.VolumeMetadata] attached_volumes: Metadata for the
+            volumes attached to the recovery instance.
         :param UnixLocalCommand cmd: The command wrapper for running commands on the
             recovery instance.
         """
         mount_point_errors = []
         mount_options_errors = []
-        for snapshot, device in sorted(attached_snapshots.items()):
+        for disk, volume in sorted(attached_volumes.items()):
             try:
-                mount_point, mount_options = cmd.findmnt(device)
-            except CommandException as e:
+                volume.resolve_mounted_volume(cmd)
+                mount_point = volume.mount_point
+                mount_options = volume.mount_options
+            except SnapshotBackupException as e:
                 mount_point_errors.append(
-                    "Error finding mount point for device %s: %s" % (device, e)
+                    "Error finding mount point for disk %s: %s" % (disk, e)
                 )
                 continue
             if mount_point is None:
                 mount_point_errors.append(
-                    "Could not find device %s at any mount point" % device
+                    "Could not find disk %s at any mount point" % disk
                 )
                 continue
             snapshot_metadata = next(
                 metadata
                 for metadata in backup_info.snapshots_info.snapshots
-                if metadata.identifier == snapshot
+                if metadata.identifier == volume.source_snapshot
             )
             expected_mount_point = snapshot_metadata.mount_point
             expected_mount_options = snapshot_metadata.mount_options
             if mount_point != expected_mount_point:
                 mount_point_errors.append(
-                    "Device %s cloned from snapshot %s is mounted at %s but %s was "
-                    "expected." % (device, snapshot, mount_point, expected_mount_point)
+                    "Disk %s cloned from snapshot %s is mounted at %s but %s was "
+                    "expected."
+                    % (disk, volume.source_snapshot, mount_point, expected_mount_point)
                 )
             if mount_options != expected_mount_options:
                 mount_options_errors.append(
-                    "Device %s cloned from snapshot %s is mounted with %s but %s was "
+                    "Disk %s cloned from snapshot %s is mounted with %s but %s was "
                     "expected."
-                    % (device, snapshot, mount_options, expected_mount_options)
+                    % (
+                        disk,
+                        volume.source_snapshot,
+                        mount_options,
+                        expected_mount_options,
+                    )
                 )
         if len(mount_point_errors) > 0:
             raise RecoveryPreconditionException(
                 "Error checking mount points: %s" % ", ".join(mount_point_errors)
             )
         if len(mount_options_errors) > 0:
             raise RecoveryPreconditionException(
@@ -1664,15 +1670,14 @@
         target_name=None,
         target_immediate=False,
         exclusive=False,
         target_action=None,
         standby_mode=None,
         recovery_conf_filename=None,
         recovery_instance=None,
-        recovery_zone=None,
     ):
         """
         Performs a recovery of a snapshot backup.
 
         This method should be called in a closing context.
 
         :param barman.infofile.BackupInfo backup_info: the backup to recover
@@ -1690,26 +1695,25 @@
         :param str|None target_immediate: end recovery as soon as consistency
             is reached
         :param bool exclusive: whether the recovery is exclusive or not
         :param str|None target_action: The recovery target action
         :param bool|None standby_mode: standby mode
         :param str|None recovery_conf_filename: filename for storing recovery
             configurations
-        :param str|None recovery_instance: The name of the recovery node as it is
-            known by the cloud provider
-        :param str|None recovery_zone: The zone in which the recovery node is located
-        """
-        snapshot_interface = get_snapshot_interface_from_backup_info(backup_info)
-        attached_snapshots = self.get_attached_snapshots_for_backup(
-            snapshot_interface, backup_info, recovery_instance, recovery_zone
+        :param str|None recovery_instance: The name of the recovery node as it
+            is known by the cloud provider
+        """
+        snapshot_interface = get_snapshot_interface_from_backup_info(
+            backup_info, self.server.config
         )
-        cmd = fs.unix_command_factory(remote_command, self.server.path)
-        SnapshotRecoveryExecutor.check_mount_points(
-            backup_info, attached_snapshots, cmd
+        attached_volumes = self.get_attached_volumes_for_backup(
+            snapshot_interface, backup_info, recovery_instance
         )
+        cmd = fs.unix_command_factory(remote_command, self.server.path)
+        SnapshotRecoveryExecutor.check_mount_points(backup_info, attached_volumes, cmd)
         self.check_recovery_dir_exists(dest, cmd)
 
         return super(SnapshotRecoveryExecutor, self).recover(
             backup_info,
             dest,
             tablespaces=None,
             remote_command=remote_command,
```

### Comparing `barman-3.5.0/barman/backup_manifest.py` & `barman-3.6.0/barman/backup_manifest.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/output.py` & `barman-3.6.0/barman/output.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/command_wrappers.py` & `barman-3.6.0/barman/command_wrappers.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/backup.py` & `barman-3.6.0/barman/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -860,15 +860,17 @@
         if backup.snapshots_info:
             _logger.debug(
                 "Deleting the following snapshots: %s"
                 % ", ".join(
                     snapshot.identifier for snapshot in backup.snapshots_info.snapshots
                 )
             )
-            snapshot_interface = get_snapshot_interface_from_backup_info(backup)
+            snapshot_interface = get_snapshot_interface_from_backup_info(
+                backup, self.server.config
+            )
             snapshot_interface.delete_snapshot_backup(backup)
         # If this backup does *not* have snapshots then tablespaces are stored on the
         # barman server so must be deleted.
         elif backup.tablespaces:
             if backup.backup_version == 2:
                 tbs_dir = backup.get_basebackup_directory()
             else:
```

### Comparing `barman-3.5.0/barman/cli.py` & `barman-3.6.0/barman/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -569,15 +569,15 @@
         ),
     ]
 )
 def replication_status(args):
     """
     Shows live information and status of any streaming client
     """
-    servers = get_server_list(args, skip_inactive=True)
+    servers = get_server_list(args, skip_inactive=True, skip_passive=True)
     for name in sorted(servers):
         server = servers[name]
 
         # Skip the server (apply general rule)
         if not manage_server_command(server, name):
             continue
 
@@ -778,16 +778,28 @@
         ),
         argument(
             "--snapshot-recovery-instance",
             help="Instance where the disks recovered from the snapshots are attached",
         ),
         argument(
             "--snapshot-recovery-zone",
+            help=(
+                "Zone containing the instance and disks for the snapshot recovery "
+                "(deprecated: replaced by --gcp-zone)"
+            ),
+        ),
+        argument(
+            "--gcp-zone",
             help="Zone containing the instance and disks for the snapshot recovery",
         ),
+        argument(
+            "--azure-resource-group",
+            help="Azure resource group containing the instance and disks for recovery "
+            "of a snapshot backup",
+        ),
     ]
 )
 def recover(args):
     """
     Recover a server at a given time, name, LSN or xid
     """
     server = get_server(args)
@@ -926,16 +938,14 @@
             output.close_and_exit()
         server.config.network_compression = args.network_compression
 
     if backup_id.snapshots_info is not None:
         missing_args = []
         if not args.snapshot_recovery_instance:
             missing_args.append("--snapshot-recovery-instance")
-        if not args.snapshot_recovery_zone:
-            missing_args.append("--snapshot-recovery-zone")
         if len(missing_args) > 0:
             output.error(
                 "Backup %s is a snapshot backup and the following required arguments "
                 "have not been provided: %s",
                 backup_id.backup_id,
                 ", ".join(missing_args),
             )
@@ -943,32 +953,43 @@
         if tablespaces != {}:
             output.error(
                 "Backup %s is a snapshot backup therefore tablespace relocation rules "
                 "cannot be used.",
                 backup_id.backup_id,
             )
             output.close_and_exit()
+        # Set the snapshot keyword arguments to be passed to the recovery executor
         snapshot_kwargs = {
             "recovery_instance": args.snapshot_recovery_instance,
-            "recovery_zone": args.snapshot_recovery_zone,
         }
+        # Special handling for deprecated snapshot_recovery_zone arg
+        if args.gcp_zone is None and args.snapshot_recovery_zone is not None:
+            args.gcp_zone = args.snapshot_recovery_zone
+        # Override provider-specific options in the config
+        for arg in (
+            "azure_resource_group",
+            "gcp_zone",
+        ):
+            value = getattr(args, arg)
+            if value is not None:
+                setattr(server.config, arg, value)
     else:
         unexpected_args = []
         if args.snapshot_recovery_instance:
             unexpected_args.append("--snapshot-recovery-instance")
-        if args.snapshot_recovery_zone:
-            unexpected_args.append("--snapshot-recovery-zone")
         if len(unexpected_args) > 0:
             output.error(
                 "Backup %s is not a snapshot backup but the following snapshot "
                 "arguments have been used: %s",
                 backup_id.backup_id,
                 ", ".join(unexpected_args),
             )
             output.close_and_exit()
+        # An empty dict is used so that snapshot-specific arguments are not passed to
+        # non-snapshot recovery executors
         snapshot_kwargs = {}
 
     with closing(server):
         try:
             server.recover(
                 backup_id,
                 args.destination_directory,
```

### Comparing `barman-3.5.0/barman/storage/file_stats.py` & `barman-3.6.0/barman/storage/file_stats.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/storage/__init__.py` & `barman-3.6.0/barman/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/storage/file_manager.py` & `barman-3.6.0/barman/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/storage/local_file_manager.py` & `barman-3.6.0/barman/storage/local_file_manager.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/retention_policies.py` & `barman-3.6.0/barman/retention_policies.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/exceptions.py` & `barman-3.6.0/barman/exceptions.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/postgres_plumbing.py` & `barman-3.6.0/barman/postgres_plumbing.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/compression.py` & `barman-3.6.0/barman/compression.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/version.py` & `barman-3.6.0/barman/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # You should have received a copy of the GNU General Public License
 # along with Barman.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 This module contains the current Barman version.
 """
 
-__version__ = '3.5.0'
+__version__ = '3.6.0'
```

### Comparing `barman-3.5.0/barman/infofile.py` & `barman-3.6.0/barman/infofile.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/cloud.py` & `barman-3.6.0/barman/cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,20 @@
 from functools import partial
 from io import BytesIO, RawIOBase
 from tempfile import NamedTemporaryFile
 
 from barman.annotations import KeepManagerMixinCloud
 from barman.backup_executor import ConcurrentBackupStrategy, SnapshotBackupExecutor
 from barman.clients import cloud_compression
+from barman.clients.cloud_cli import get_missing_attrs
 from barman.exceptions import (
     BackupPreconditionException,
     BarmanException,
     BackupException,
+    ConfigurationException,
 )
 from barman.fs import UnixLocalCommand, path_allowed
 from barman.infofile import BackupInfo
 from barman.postgres_plumbing import EXCLUDE_LIST, PGDATA_EXCLUDE_LIST
 from barman.utils import (
     BarmanEncoder,
     force_str,
@@ -1834,15 +1836,14 @@
     def __init__(
         self,
         server_name,
         cloud_interface,
         snapshot_interface,
         postgres,
         snapshot_instance,
-        snapshot_zone,
         snapshot_disks,
         backup_name=None,
     ):
         """
         Create the backup client for snapshot backups
 
         :param str server_name: The name of the server as configured in Barman
@@ -1850,40 +1851,35 @@
           upload the backup
         :param SnapshotInterface snapshot_interface: The interface to use for
           creating a backup using snapshots
         :param barman.postgres.PostgreSQLConnection|None postgres: A connection to the
             PostgreSQL instance being backed up.
         :param str snapshot_instance: The name of the VM instance to which the disks
             to be backed up are attached.
-        :param str snapshot_zone: The zone in which the snapshot disks and instance
-            reside.
         :param list[str] snapshot_disks: A list containing the names of the disks for
             which snapshots should be taken at backup time.
         :param str|None backup_name: A friendly name which can be used to reference
             this backup in the future.
         """
         super(CloudBackupSnapshot, self).__init__(
             server_name, cloud_interface, postgres, backup_name
         )
         self.snapshot_interface = snapshot_interface
         self.snapshot_instance = snapshot_instance
-        self.snapshot_zone = snapshot_zone
         self.snapshot_disks = snapshot_disks
 
     # The remaining methods are the concrete implementations of the abstract methods from
     # the parent class.
     def _finalise_copy(self):
         """
         Perform any finalisation required to complete the copy of backup data.
 
-        For snapshot backups this means gathering the mount point and mount options
-        from the local node.
+        This is a no-op for snapshot backups.
         """
-        cmd = UnixLocalCommand()
-        SnapshotBackupExecutor.add_mount_data_to_backup_info(self.backup_info, cmd)
+        pass
 
     def _add_stats_to_backup_info(self):
         """
         Add statistics about the backup to self.backup_info.
         """
         self.backup_info.set_attribute(
             "copy_stats",
@@ -1912,49 +1908,51 @@
             backup_label_key,
         )
 
     def _take_backup(self):
         """
         Make a backup by creating snapshots of the specified disks.
         """
+        volumes_to_snapshot = self.snapshot_interface.get_attached_volumes(
+            self.snapshot_instance, self.snapshot_disks
+        )
+        cmd = UnixLocalCommand()
+        SnapshotBackupExecutor.add_mount_data_to_volume_metadata(
+            volumes_to_snapshot, cmd
+        )
         self.snapshot_interface.take_snapshot_backup(
             self.backup_info,
             self.snapshot_instance,
-            self.snapshot_zone,
-            self.snapshot_disks,
+            volumes_to_snapshot,
         )
 
     # The following method implements specific functionality for snapshot backups.
     def _check_backup_preconditions(self):
         """
         Perform additional checks for snapshot backups, specifically:
 
           - check that the VM instance for which snapshots should be taken exists
           - check that the expected disks are attached to that instance
           - check that the attached disks are mounted on the filesystem
 
         Raises a BackupPreconditionException if any of the checks fail.
         """
-        if not self.snapshot_interface.instance_exists(
-            self.snapshot_instance, self.snapshot_zone
-        ):
+        if not self.snapshot_interface.instance_exists(self.snapshot_instance):
             raise BackupPreconditionException(
-                "Cannot find compute instance %s in zone %s"
-                % (self.snapshot_instance, self.snapshot_zone)
+                "Cannot find compute instance %s" % self.snapshot_instance
             )
 
         cmd = UnixLocalCommand()
         (
             missing_disks,
             unmounted_disks,
         ) = SnapshotBackupExecutor.find_missing_and_unmounted_disks(
             cmd,
             self.snapshot_interface,
             self.snapshot_instance,
-            self.snapshot_zone,
             self.snapshot_disks,
         )
 
         if len(missing_disks) > 0:
             raise BackupPreconditionException(
                 "Cannot find disks attached to compute instance %s: %s"
                 % (self.snapshot_instance, ", ".join(missing_disks))
@@ -2211,108 +2209,182 @@
 
         return backup_files
 
 
 class CloudSnapshotInterface(with_metaclass(ABCMeta)):
     """Defines a common interface for handling cloud snapshots."""
 
-    @abstractmethod
-    def take_snapshot(self, backup_info, disk_zone, disk_name):
+    _required_config_for_backup = ("snapshot_disks", "snapshot_instance")
+    _required_config_for_restore = ("snapshot_recovery_instance",)
+
+    @classmethod
+    def validate_backup_config(cls, config):
         """
-        Take a snapshot of a disk in the cloud.
+        Additional validation for backup options.
 
-        :param barman.infofile.LocalBackupInfo backup_info: Backup information.
-        :param str disk_zone: The zone in which the disk resides.
-        :param str disk_name: The name of the source disk for the snapshot.
-        :rtype: str
-        :return: The name used to reference the snapshot with the cloud provider.
+        Raises a ConfigurationException if any required options are missing.
+
+        :param argparse.Namespace config: The backup options provided at the command line.
+        """
+        missing_options = get_missing_attrs(config, cls._required_config_for_backup)
+        if len(missing_options) > 0:
+            raise ConfigurationException(
+                "Incomplete options for snapshot backup - missing: %s"
+                % ", ".join(missing_options)
+            )
+
+    @classmethod
+    def validate_restore_config(cls, config):
         """
+        Additional validation for restore options.
+
+        Raises a ConfigurationException if any required options are missing.
+
+        :param argparse.Namespace config: The backup options provided at the command line.
+        """
+        missing_options = get_missing_attrs(config, cls._required_config_for_restore)
+        if len(missing_options) > 0:
+            raise ConfigurationException(
+                "Incomplete options for snapshot restore - missing: %s"
+                % ", ".join(missing_options)
+            )
 
     @abstractmethod
-    def take_snapshot_backup(self, backup_info, instance_name, zone, disks):
+    def take_snapshot_backup(self, backup_info, instance_name, volumes):
         """
         Take a snapshot backup for the named instance.
 
         Implementations of this method must do the following:
 
             * Create a snapshot of the disk.
             * Set the snapshots_info field of the backup_info to a SnapshotsInfo
               implementation which contains the snapshot metadata required both
               by Barman and any third party tooling which needs to recover the
               snapshots.
 
         :param barman.infofile.LocalBackupInfo backup_info: Backup information.
         :param str instance_name: The name of the VM instance to which the disks
             to be backed up are attached.
-        :param str zone: The zone in which the snapshot disks and instance reside.
-        :param list[str] disks: A list containing the names of the source disks.
-        """
-
-    @abstractmethod
-    def delete_snapshot(self, snapshot_identifier):
-        """
-        Delete the specified snapshot.
-
-        :param str snapshot_identifier: An identifier used to reference this snapshot
-            within the cloud provider API.
+        :param dict[str,barman.cloud.VolumeMetadata] volumes: Metadata for the volumes
+            to be backed up.
         """
 
     @abstractmethod
     def delete_snapshot_backup(self, backup_info):
         """
         Delete all snapshots for the supplied backup.
 
         :param barman.infofile.LocalBackupInfo backup_info: Backup information.
         """
 
     @abstractmethod
-    def get_attached_devices(self, instance_name, zone):
+    def get_attached_volumes(self, instance_name, disks=None):
         """
-        Returns the non-boot devices attached to instance_name in zone.
+        Returns metadata for the volumes attached to this instance.
 
-        Implementations must return a dict where the key is the name of the attached
-        disk and the value is the full path to the device at which the disk is attached
-        on the instance.
+        Queries the cloud provider for metadata relating to the volumes attached to
+        the named instance and returns a dict of `VolumeMetadata` objects, keyed by
+        disk name.
+
+        If the optional disks parameter is supplied then this method must return
+        metadata for the disks in the supplied list only. A SnapshotBackupException
+        must be raised if any of the supplied disks are not found to be attached to
+        the instance.
+
+        If the disks parameter is not supplied then this method must return a
+        VolumeMetadata for all disks attached to this instance.
 
         :param str instance_name: The name of the VM instance to which the disks
             to be backed up are attached.
-        :param str zone: The zone in which the snapshot disks and instance reside.
-        :rtype: dict[str,str]
-        :return: A dict where the key is the disk name and the value is the device
-            path for that disk on the specified instance.
+        :param list[str]|None disks: A list containing the names of disks to be
+            backed up.
+        :rtype: dict[str, VolumeMetadata]
+        :return: A dict of VolumeMetadata objects representing each volume
+            attached to the instance, keyed by volume identifier.
         """
 
     @abstractmethod
-    def get_attached_snapshots(self, instance_name, zone):
+    def instance_exists(self, instance_name):
         """
-        Returns the snapshots which are sources for disks attached to instance.
-
-        Implementations must return each snapshot which is the source for a disk
-        attache to the instance along with the device path at which it is attached.
+        Determine whether the named instance exists.
 
         :param str instance_name: The name of the VM instance to which the disks
             to be backed up are attached.
-        :param str zone: The zone in which the snapshot disks and instance reside.
-        :rtype: dict[str,str]
-        :return: A dict where the key is the snapshot name and the value is the
-            device path for the source disk for that snapshot on the specified
-            instance.
+        :rtype: bool
+        :return: True if the named instance exists, False otherwise.
         """
 
+
+class VolumeMetadata(object):
+    """
+    Represents metadata for a single volume attached to a cloud VM.
+
+    The main purpose of this class is to allow calling code to determine the mount
+    point and mount options for an attached volume without needing to know the
+    details of how these are determined for a specific cloud provider.
+
+    Implementations must therefore:
+
+    - Store metadata obtained from the cloud provider which can be used to resolve
+      this volume to an attached and mounted volume on the instance. This will
+      typically be a device name or something which can be resolved to a device name.
+    - Provide an implementation of `resolve_mounted_volume` which executes commands
+      on the cloud VM via a supplied UnixLocalCommand object in order to set the
+      _mount_point and _mount_options properties.
+
+    If the volume was cloned from a snapshot then the source snapshot identifier
+    must also be stored in this class so that calling code can determine if/how/where
+    a volume cloned from a given snapshot is mounted.
+    """
+
+    def __init__(self):
+        self._mount_point = None
+        self._mount_options = None
+
     @abstractmethod
-    def instance_exists(self, instance_name, zone):
+    def resolve_mounted_volume(self, cmd):
         """
-        Determine whether the named instance exists in the specified zone.
+        Resolve the mount point and mount options using shell commands.
 
-        :param str instance_name: The name of the VM instance to which the disks
-            to be backed up are attached.
-        :param str zone: The zone in which the snapshot disks and instance reside.
-        :rtype: bool
-        :return: True if the named instance exists in zone, False otherwise.
+        This method must use cmd together with any additional private properties
+        available in the provider-specific implementation in order to resolve the
+        mount point and mount options for this volume.
+
+        :param UnixLocalCommand cmd: Wrapper for local/remote commands on the instance
+            to which this volume is attached.
+        """
+
+    @abstractproperty
+    def source_snapshot(self):
+        """
+        The source snapshot from which this volume was cloned.
+
+        :rtype: str|None
+        :return: A snapshot identifier.
+        """
+
+    @property
+    def mount_point(self):
+        """
+        The mount point at which this volume is currently mounted.
+
+        This must be resolved using metadata obtained from the cloud provider which
+        describes how the volume is attached to the VM.
+        """
+        return self._mount_point
+
+    @property
+    def mount_options(self):
+        """
+        The mount options with which this device is currently mounted.
+
+        This must be resolved using metadata obtained from the cloud provider which
+        describes how the volume is attached to the VM.
         """
+        return self._mount_options
 
 
 class SnapshotMetadata(object):
     """
     Represents metadata for a single snapshot.
 
     This class holds the snapshot metadata common to all snapshot providers.
@@ -2409,28 +2481,14 @@
         Subclasses must ensure this returns a string which can be used by Barman to
         reference the snapshot when interacting with the cloud provider API.
 
         :rtype: str
         :return: A snapshot identifier.
         """
 
-    @abstractproperty
-    def device(self):
-        """
-        The device path to the source disk on the compute instance at the time the
-        backup was taken.
-
-        Subclasses must ensure this returns a full path. Certain cloud platforms,
-        such as GCP, provide only a short name which must be forged into a full path.
-        Such forging should take place here.
-
-        :rtype: str
-        :return: The device path.
-        """
-
 
 class SnapshotsInfo(object):
     """
     Represents the snapshots_info field of backup metadata stored in BackupInfo.
 
     This class holds the metadata for a snapshot backup which is common to all
     snapshot providers. This is the list of SnapshotMetadata objects representing the
```

### Comparing `barman-3.5.0/barman/hooks.py` & `barman-3.6.0/barman/hooks.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman/remote_status.py` & `barman-3.6.0/barman/remote_status.py`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/setup.py` & `barman-3.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     license="GPL-3.0",
     description=__doc__.split("\n")[0],
     long_description="\n".join(__doc__.split("\n")[2:]),
     install_requires=install_requires,
     extras_require={
         "cloud": ["boto3"],
         "azure": ["azure-identity", "azure-storage-blob"],
+        "azure-snapshots": ["azure-identity", "azure-mgmt-compute"],
         "snappy": ["python-snappy"],
         "google": [
             "google-cloud-storage",
         ],
         "google-snapshots": [
             "grpcio",
             "google-cloud-compute",  # requires minimum python3.7
```

### Comparing `barman-3.5.0/barman.egg-info/entry_points.txt` & `barman-3.6.0/barman.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `barman-3.5.0/barman.egg-info/SOURCES.txt` & `barman-3.6.0/barman.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 doc/barman.1.d/50-backup.md
 doc/barman.1.d/50-check-backup.md
 doc/barman.1.d/50-check-wal-archive.md
 doc/barman.1.d/50-check.md
 doc/barman.1.d/50-cron.md
 doc/barman.1.d/50-delete.md
 doc/barman.1.d/50-diagnose.md
+doc/barman.1.d/50-generate-manifest.md
 doc/barman.1.d/50-get-wal.md
 doc/barman.1.d/50-keep.md
 doc/barman.1.d/50-list-backups.md
 doc/barman.1.d/50-list-files.md
 doc/barman.1.d/50-list-servers.md
 doc/barman.1.d/50-put-wal.md
 doc/barman.1.d/50-rebuild-xlogdb.md
@@ -118,14 +119,16 @@
 doc/barman.1.d/50-show-servers.md
 doc/barman.1.d/50-status.md
 doc/barman.1.d/50-switch-wal.md
 doc/barman.1.d/50-switch-xlog.md
 doc/barman.1.d/50-sync-backup.md
 doc/barman.1.d/50-sync-info.md
 doc/barman.1.d/50-sync-wals.md
+doc/barman.1.d/50-verify-backup.md
+doc/barman.1.d/50-verify.md
 doc/barman.1.d/70-backup-id-shortcuts.md
 doc/barman.1.d/75-exit-status.md
 doc/barman.1.d/80-see-also.md
 doc/barman.1.d/85-bugs.md
 doc/barman.1.d/90-authors.md
 doc/barman.1.d/95-resources.md
 doc/barman.1.d/99-copying.md
@@ -135,14 +138,17 @@
 doc/barman.5.d/20-configuration-file-locations.md
 doc/barman.5.d/25-configuration-file-syntax.md
 doc/barman.5.d/30-configuration-file-directory.md
 doc/barman.5.d/45-options.md
 doc/barman.5.d/50-active.md
 doc/barman.5.d/50-archiver.md
 doc/barman.5.d/50-archiver_batch_size.md
+doc/barman.5.d/50-azure_credential.md
+doc/barman.5.d/50-azure_resource_group.md
+doc/barman.5.d/50-azure_subscription_id.md
 doc/barman.5.d/50-backup_compression.md
 doc/barman.5.d/50-backup_compression_format.md
 doc/barman.5.d/50-backup_compression_level.md
 doc/barman.5.d/50-backup_compression_location.md
 doc/barman.5.d/50-backup_compression_workers.md
 doc/barman.5.d/50-backup_directory.md
 doc/barman.5.d/50-backup_method.md
@@ -159,14 +165,16 @@
 doc/barman.5.d/50-create_slot.md
 doc/barman.5.d/50-custom_compression_filter.md
 doc/barman.5.d/50-custom_compression_magic.md
 doc/barman.5.d/50-custom_decompression_filter.md
 doc/barman.5.d/50-description.md
 doc/barman.5.d/50-errors_directory.md
 doc/barman.5.d/50-forward-config-path.md
+doc/barman.5.d/50-gcp-project.md
+doc/barman.5.d/50-gcp-zone.md
 doc/barman.5.d/50-immediate_checkpoint.md
 doc/barman.5.d/50-incoming_wals_directory.md
 doc/barman.5.d/50-last_backup_maximum_age.md
 doc/barman.5.d/50-last_backup_minimum_size.md
 doc/barman.5.d/50-last_wal_maximum_age.md
 doc/barman.5.d/50-log_file.md
 doc/barman.5.d/50-log_level.md
@@ -202,18 +210,16 @@
 doc/barman.5.d/50-recovery_options.md
 doc/barman.5.d/50-recovery_staging_path.md
 doc/barman.5.d/50-retention_policy.md
 doc/barman.5.d/50-retention_policy_mode.md
 doc/barman.5.d/50-reuse_backup.md
 doc/barman.5.d/50-slot_name.md
 doc/barman.5.d/50-snapshot-disks.md
-doc/barman.5.d/50-snapshot-gcp-project.md
 doc/barman.5.d/50-snapshot-instance.md
 doc/barman.5.d/50-snapshot-provider.md
-doc/barman.5.d/50-snapshot-zone.md
 doc/barman.5.d/50-ssh_command.md
 doc/barman.5.d/50-streaming_archiver.md
 doc/barman.5.d/50-streaming_archiver_batch_size.md
 doc/barman.5.d/50-streaming_archiver_name.md
 doc/barman.5.d/50-streaming_backup_name.md
 doc/barman.5.d/50-streaming_conninfo.md
 doc/barman.5.d/50-streaming_wals_directory.md
@@ -274,8 +280,9 @@
 doc/manual/43-backup-commands.en.md
 doc/manual/50-feature-details.en.md
 doc/manual/55-barman-cli.en.md
 doc/manual/65-troubleshooting.en.md
 doc/manual/66-about.en.md
 doc/manual/99-references.en.md
 doc/manual/Makefile
+doc/runbooks/snapshot_recovery_azure.md
 scripts/barman.bash_completion
```

### Comparing `barman-3.5.0/barman.egg-info/PKG-INFO` & `barman-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barman
-Version: 3.5.0
+Version: 3.6.0
 Summary: Backup and Recovery Manager for PostgreSQL
 Home-page: https://www.pgbarman.org/
 Author: EnterpriseDB
 Author-email: barman@enterprisedb.com
 License: GPL-3.0
 Platform: Linux
 Platform: Mac OS X
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cloud
 Provides-Extra: azure
+Provides-Extra: azure-snapshots
 Provides-Extra: snappy
 Provides-Extra: google
 Provides-Extra: google-snapshots
 License-File: LICENSE
 License-File: AUTHORS
 
 Barman (Backup and Recovery Manager) is an open-source administration
```

### Comparing `barman-3.5.0/AUTHORS` & `barman-3.6.0/AUTHORS`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Barman maintainers (in alphabetical order):
 
 * Abhijit Menon-Sen
 * Didier Michel
+* Giulio Calacoci
 * Jane Threefoot
 * Michael Wallace
 
 Past contributors (in alphabetical order):
 
 * Anna Bellandi (QA/testing)
 * Britt Cole (documentation reviewer)
```

### Comparing `barman-3.5.0/NEWS` & `barman-3.6.0/NEWS`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,41 @@
 Barman News - History of user-visible changes
 
+Version 3.6.0 - 15 June 2023
+
+- PostgreSQL version 10 is no longer supported.
+
+- Support is added for snapshot backups on Microsoft Azure using
+  Managed Disks.
+
+- The `--snapshot-recovery-zone` option is renamed `--gcp-zone` for
+  consistency with other provider-specific options. The old name
+  is deprecated and will be removed in a future release.
+
+- The `snapshot_zone` option and `--snapshot-zone` argument are
+  renamed `gcp_zone` and `--gcp-zone` respectively. The old names
+  are deprecated and will be removed in a future release.
+
+- The `snapshot_gcp_project` option and `--snapshot-gcp-project`
+  argument are renamed to `gcp_project` and `--gcp-project`. The
+  old names are deprecated and will be removed in a future release.
+
+- Bug fixes:
+
+    - Barman will no longer attempt to execute the `replication-status`
+      command for a passive node.
+
+    - The `backup_label` is deleted from cloud storage when a
+      snapshot backup is deleted with `barman-cloud-backup-delete`.
+
+    - Man pages for the `generate-manifest` and `verify-backup`
+      commands are added.
+
+    - Minor documentation fixes.
+
 Version 3.5.0 - 29 March 2023
 
 - Python 2.7 is no longer supported. The earliest Python version
   supported is now 3.6.
 
 - The `barman`, `barman-cli` and `barman-cli-cloud` packages for
   EL7 now require python 3.6 instead of python 2.7. For other
```

