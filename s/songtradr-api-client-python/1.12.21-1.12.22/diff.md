# Comparing `tmp/songtradr-api-client-python-1.12.21.tar.gz` & `tmp/songtradr-api-client-python-1.12.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songtradr-api-client-python-1.12.21.tar", last modified: Wed Jun 14 15:38:31 2023, max compression
+gzip compressed data, was "songtradr-api-client-python-1.12.22.tar", last modified: Thu Jun 15 13:45:40 2023, max compression
```

## Comparing `songtradr-api-client-python-1.12.21.tar` & `songtradr-api-client-python-1.12.22.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.069454 songtradr-api-client-python-1.12.21/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-14 15:38:31.069454 songtradr-api-client-python-1.12.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 15:38:31.069454 songtradr-api-client-python-1.12.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.021454 songtradr-api-client-python-1.12.21/songtradr_api_client_python/
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.025454 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21722 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/allowed_values_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/party_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/playlist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    96081 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/recording_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   255960 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31745 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.045454 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/category_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/category_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/config_access_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/config_identifier_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/contributor_type_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/field_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_minimal_with_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_upload_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_w_ith_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/files_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/forgot_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/genre_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/genres_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/init_put_recording_audio_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/jwt_token_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/login_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    41920 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/p_line_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/party_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/party_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/playlist_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/product_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/product_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_for_similarity_search_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_genre_prediction_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    66338 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_file_recording_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_referrer_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/search_filter_values_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/search_recording_granular_abstraction_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/search_recording_granular_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/sign_up_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/taggram_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tags_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tagstrength_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/title_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/track_to_medium_product_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/update_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/usage_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/user_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.025454 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-14 15:38:31.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-14 15:38:31.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:38:31.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 15:38:31.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 15:38:31.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.069454 songtradr-api-client-python-1.12.21/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_allowed_values_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_category_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_category_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_config_access_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_config_identifier_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_contributor_type_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_field_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_minimal_with_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_upload_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    21599 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_w_ith_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_files_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_forgot_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_genre_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_genres_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_init_put_recording_audio_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_jwt_token_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_login_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_p_line_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/test/test_party_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_party_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_party_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/test/test_playlist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_playlist_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_product_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_product_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/test/test_recording_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_for_similarity_search_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_genre_prediction_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    19341 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_minimal_with_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_minimal_with_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_minimal_with_tagstrengths_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_file_recording_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_recording_genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_recording_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_recording_tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_referrer_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_search_filter_values_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_search_recording_granular_abstraction_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_search_recording_granular_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_sign_up_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_taggram_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_tags_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_tagstrength_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_title_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_track_to_medium_product_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_update_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_usage_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_user_dto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:45:40.862064 songtradr-api-client-python-1.12.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-15 13:45:40.862064 songtradr-api-client-python-1.12.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 13:45:40.862064 songtradr-api-client-python-1.12.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:45:40.838063 songtradr-api-client-python-1.12.22/songtradr_api_client_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:45:40.842064 songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21722 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/allowed_values_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/party_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/playlist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96081 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/recording_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   255960 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31745 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:45:40.850063 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/category_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/category_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/config_access_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/config_identifier_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/contributor_type_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/field_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_minimal_with_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_upload_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_w_ith_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/files_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/forgot_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/genre_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/genres_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/init_put_recording_audio_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/jwt_token_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/login_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41920 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/p_line_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/party_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/party_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/playlist_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/product_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/product_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_for_similarity_search_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_genre_prediction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66338 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_file_recording_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_recording_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_recording_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_referrer_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24182 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/search_filter_values_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/search_recording_granular_abstraction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/search_recording_granular_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/sign_up_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/taggram_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/tags_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/tagstrength_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/title_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/track_to_medium_product_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/update_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/usage_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:45:40.838063 songtradr-api-client-python-1.12.22/songtradr_api_client_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-15 13:45:40.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-15 13:45:40.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:45:40.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 13:45:40.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 13:45:40.000000 songtradr-api-client-python-1.12.22/songtradr_api_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:45:40.862064 songtradr-api-client-python-1.12.22/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/test/test_allowed_values_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_category_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_category_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_config_access_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_config_identifier_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_contributor_type_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_field_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_file_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_file_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_file_minimal_with_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_file_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_file_upload_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21599 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_file_w_ith_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_files_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_forgot_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_genre_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_genres_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_init_put_recording_audio_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_jwt_token_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_login_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_p_line_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/test/test_party_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_party_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_party_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/test/test_playlist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_playlist_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_product_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_product_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/test/test_recording_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_for_similarity_search_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_genre_prediction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19341 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_minimal_with_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_minimal_with_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_minimal_with_tagstrengths_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_recording_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_save_file_recording_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_save_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_save_recording_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_save_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_save_recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_save_recording_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_save_referrer_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_save_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_save_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_search_filter_values_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_search_recording_granular_abstraction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_search_recording_granular_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_sign_up_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_taggram_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_tags_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_tagstrength_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_title_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_track_to_medium_product_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_update_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_usage_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-15 13:45:28.000000 songtradr-api-client-python-1.12.22/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-15 13:45:27.000000 songtradr-api-client-python-1.12.22/test/test_user_dto.py
```

### Comparing `songtradr-api-client-python-1.12.21/PKG-INFO` & `songtradr-api-client-python-1.12.22/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: songtradr-api-client-python
-Version: 1.12.21
+Version: 1.12.22
 Summary: Songtradr API
-Home-page: https://pypi.org/project/songtradr-api-client-python/
+Home-page: https://github.com/songtradr/songtradr-python-api-client-docs
 Author: Songtradr Inc.
 Author-email: info@songtradr.com
 Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
 Description-Content-Type: text/markdown
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world&#39;s released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
```

### Comparing `songtradr-api-client-python-1.12.21/README.md` & `songtradr-api-client-python-1.12.22/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.
 
 1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters.
 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.12.21
-- Package version: 1.12.21
+- API version: 1.12.22
+- Package version: 1.12.22
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://songtradr.com](https://songtradr.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `songtradr-api-client-python-1.12.21/pyproject.toml` & `songtradr-api-client-python-1.12.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "songtradr_api_client_python"
-version = "1.12.21"
+version = "1.12.22"
 description = "Songtradr API"
 authors = ["Songtradr Inc. <info@songtradr.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Songtradr API"]
 include = ["songtradr_api_client_python/py.typed"]
```

### Comparing `songtradr-api-client-python-1.12.21/setup.py` & `songtradr-api-client-python-1.12.22/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,30 +18,30 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "songtradr-api-client-python"
-VERSION = "1.12.21"
+VERSION = "1.12.22"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Songtradr API",
     author="Songtradr Inc.",
     author_email="info@songtradr.com",
-    url="https://pypi.org/project/songtradr-api-client-python/",
+    url="https://github.com/songtradr/songtradr-python-api-client-docs",
     keywords=["OpenAPI", "OpenAPI-Generator", "Songtradr API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     long_description_content_type='text/markdown',
     long_description="""\
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world&#39;s released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/__init__.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "1.12.21"
+__version__ = "1.12.22"
 
 # import apis into sdk package
 from songtradr_api_client_python.api.allowed_values_api import AllowedValuesApi
 from songtradr_api_client_python.api.party_api import PartyApi
 from songtradr_api_client_python.api.playlist_api import PlaylistApi
 from songtradr_api_client_python.api.recording_api import RecordingApi
 from songtradr_api_client_python.api.user_api import UserApi
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/allowed_values_api.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/allowed_values_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/party_api.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/party_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/playlist_api.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/playlist_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -333,16 +333,16 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearer-jwt']  # noqa: E501
 
         _response_types_map = {
-            '403': "ErrorResponse",
             '200': "object",
+            '403': "ErrorResponse",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
 
         return self.api_client.call_api(
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/recording_api.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/recording_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/user_api.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -2090,16 +2090,16 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearer-jwt']  # noqa: E501
 
         _response_types_map = {
-            '200': "FileListDTO",
             '403': "ErrorResponse",
+            '200': "FileListDTO",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
 
         return self.api_client.call_api(
@@ -2239,17 +2239,17 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearer-jwt']  # noqa: E501
 
         _response_types_map = {
+            '200': "SignUpDTO",
             '403': "ErrorResponse",
             '409': "ErrorResponse",
-            '200': "SignUpDTO",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
 
         return self.api_client.call_api(
@@ -4178,16 +4178,16 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearer-jwt']  # noqa: E501
 
         _response_types_map = {
-            '404': "ErrorResponse",
             '200': "List[FileSmallDTO]",
+            '404': "ErrorResponse",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
         }
 
         return self.api_client.call_api(
             '/api/v1/user/filesStatus', 'GET',
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/api_client.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.12.21/python'
+        self.user_agent = 'OpenAPI-Generator/1.12.22/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/api_response.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/api_response.py`

 * *Files identical despite different names*

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/configuration.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -373,16 +373,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.12.21\n"\
-               "SDK Package Version: 1.12.21".\
+               "Version of the API: 1.12.22\n"\
+               "SDK Package Version: 1.12.22".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/exceptions.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/__init__.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/category_medium_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/category_medium_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -24,17 +24,17 @@
 from songtradr_api_client_python.models.tag_small_dto import TagSmallDTO
 
 class CategoryMediumDTO(BaseModel):
     """
     A category of tags with its underlying tags.
     """
     id: StrictInt = Field(...)
-    tags: Optional[conlist(TagSmallDTO)] = None
     name: StrictStr = Field(...)
-    __properties = ["id", "tags", "name"]
+    tags: Optional[conlist(TagSmallDTO)] = None
+    __properties = ["id", "name", "tags"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -72,12 +72,12 @@
             return None
 
         if not isinstance(obj, dict):
             return CategoryMediumDTO.parse_obj(obj)
 
         _obj = CategoryMediumDTO.parse_obj({
             "id": obj.get("id"),
-            "tags": [TagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None,
-            "name": obj.get("name")
+            "name": obj.get("name"),
+            "tags": [TagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None
         })
         return _obj
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/category_minimal_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/category_minimal_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/config_access_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/config_access_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/config_identifier_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/config_identifier_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/contributor_type_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/contributor_type_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/error_response.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/field_summary_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/field_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_list_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_list_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_minimal_with_url_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_minimal_with_url_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_small_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_upload_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_upload_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_w_ith_url_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/file_w_ith_url_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/files_summary_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/files_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/forgot_password_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/forgot_password_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/genre_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/genre_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/genre_minimal_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/genre_minimal_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/genres_summary_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/genres_summary_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/init_put_recording_audio_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/init_put_recording_audio_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/jwt_token_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/jwt_token_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/login_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/login_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/musical_features_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/musical_features_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -23,27 +23,35 @@
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, validator
 
 class MusicalFeaturesDTO(BaseModel):
     """
     AI generated musical features of a recording.
     """
     space: Optional[StrictStr] = Field(None, description="Search for space")
-    primary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="primaryMoodClusterAffinity")
-    secondary_mood_cluster: Optional[StrictStr] = Field(None, alias="secondaryMoodCluster", description="Search for a language of the lyrics")
-    secondary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="secondaryMoodClusterAffinity")
-    tertiary_mood_cluster: Optional[StrictStr] = Field(None, alias="tertiaryMoodCluster", description="Search for a language of the lyrics")
-    tertiary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="tertiaryMoodClusterAffinity")
-    vocals_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="vocalsAffinity")
-    dominant_instrument_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="dominantInstrumentAffinity")
-    secondary_instrument: Optional[StrictStr] = Field(None, alias="secondaryInstrument", description="Search for a dominant instrument")
-    secondary_instrument_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="secondaryInstrumentAffinity")
-    tertiary_instrument: Optional[StrictStr] = Field(None, alias="tertiaryInstrument", description="Search for a dominant instrument")
-    tertiary_instrument_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="tertiaryInstrumentAffinity")
-    sound_generation_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="soundGenerationAffinity")
-    rhythm_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="rhythmAffinity")
+    arousal: Optional[StrictStr] = Field(None, description="Search for an arousal")
+    dominant_instrument: Optional[StrictStr] = Field(None, alias="dominantInstrument", description="Search for a dominant instrument")
+    energy: Optional[StrictStr] = Field(None, description="Search for energy")
+    engagement: Optional[StrictStr] = Field(None, description="Search for an engagement")
+    groovyness: Optional[StrictStr] = Field(None, description="Search for groovyness")
+    harmony: Optional[StrictStr] = Field(None, description="Search for a degree of harmoniousness")
+    pleasantness: Optional[StrictStr] = Field(None, description="Search for pleasantness")
+    primary_mood_cluster: Optional[StrictStr] = Field(None, alias="primaryMoodCluster", description="Search for a language of the lyrics")
+    primary_sound_character: Optional[StrictStr] = Field(None, alias="primarySoundCharacter", description="Search for a sound character")
+    rhythm: Optional[StrictStr] = Field(None, description="Search for rhythm")
+    roughness: Optional[StrictStr] = Field(None, description="Search for roughness")
+    scale: Optional[StrictStr] = Field(None, description="Search for a tonal scale")
+    sound_generation: Optional[StrictStr] = Field(None, alias="soundGeneration", description="Search for type of sound generation")
+    tempo: Optional[StrictStr] = Field(None, description="Search for tempo")
+    texture: Optional[StrictStr] = Field(None, description="Search for texture")
+    timbre: Optional[StrictStr] = Field(None, description="Search for timbre")
+    tonality: Optional[StrictStr] = Field(None, description="Search for tonality")
+    valence: Optional[StrictStr] = Field(None, description="Search for a valence")
+    vocals: Optional[StrictStr] = Field(None, description="Search for a vocal gender or instrumental songs")
+    origin_decade: Optional[StrictStr] = Field(None, alias="originDecade", description="Search for origin decade")
+    language_of_performance: Optional[StrictStr] = Field(None, alias="languageOfPerformance")
     primary_sound_character_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="primarySoundCharacterAffinity")
     tonality_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="tonalityAffinity")
     bpm: Optional[Union[StrictFloat, StrictInt]] = None
     production_rating: Optional[StrictStr] = Field(None, alias="productionRating")
     production_rating_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="productionRatingAffinity")
     performance_rating: Optional[StrictStr] = Field(None, alias="performanceRating")
     performance_rating_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="performanceRatingAffinity")
@@ -67,38 +75,30 @@
     origin_decade_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="originDecadeAffinity")
     language_of_performance_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="languageOfPerformanceAffinity")
     curateability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="curateabilityAffinity")
     use_case_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="useCaseAffinity")
     industry_suitability: Optional[StrictStr] = Field(None, alias="industrySuitability", description="Search for Industry suitability")
     industry_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="industrySuitabilityAffinity")
     audience_region: Optional[StrictStr] = Field(None, alias="audienceRegion")
-    arousal: Optional[StrictStr] = Field(None, description="Search for an arousal")
-    dominant_instrument: Optional[StrictStr] = Field(None, alias="dominantInstrument", description="Search for a dominant instrument")
-    energy: Optional[StrictStr] = Field(None, description="Search for energy")
-    engagement: Optional[StrictStr] = Field(None, description="Search for an engagement")
-    groovyness: Optional[StrictStr] = Field(None, description="Search for groovyness")
-    harmony: Optional[StrictStr] = Field(None, description="Search for a degree of harmoniousness")
-    pleasantness: Optional[StrictStr] = Field(None, description="Search for pleasantness")
-    primary_mood_cluster: Optional[StrictStr] = Field(None, alias="primaryMoodCluster", description="Search for a language of the lyrics")
-    language_of_performance: Optional[StrictStr] = Field(None, alias="languageOfPerformance")
-    primary_sound_character: Optional[StrictStr] = Field(None, alias="primarySoundCharacter", description="Search for a sound character")
-    rhythm: Optional[StrictStr] = Field(None, description="Search for rhythm")
-    roughness: Optional[StrictStr] = Field(None, description="Search for roughness")
-    scale: Optional[StrictStr] = Field(None, description="Search for a tonal scale")
-    sound_generation: Optional[StrictStr] = Field(None, alias="soundGeneration", description="Search for type of sound generation")
-    tempo: Optional[StrictStr] = Field(None, description="Search for tempo")
-    texture: Optional[StrictStr] = Field(None, description="Search for texture")
-    timbre: Optional[StrictStr] = Field(None, description="Search for timbre")
-    tonality: Optional[StrictStr] = Field(None, description="Search for tonality")
-    valence: Optional[StrictStr] = Field(None, description="Search for a valence")
-    vocals: Optional[StrictStr] = Field(None, description="Search for a vocal gender or instrumental songs")
-    origin_decade: Optional[StrictStr] = Field(None, alias="originDecade", description="Search for origin decade")
     curateability: Optional[StrictStr] = Field(None, description="Search for curatebility")
     use_case: Optional[StrictStr] = Field(None, alias="useCase", description="Search for use case")
     channel_suitability: Optional[StrictStr] = Field(None, alias="channelSuitability", description="Search for social media suitability")
+    primary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="primaryMoodClusterAffinity")
+    secondary_mood_cluster: Optional[StrictStr] = Field(None, alias="secondaryMoodCluster", description="Search for a language of the lyrics")
+    secondary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="secondaryMoodClusterAffinity")
+    tertiary_mood_cluster: Optional[StrictStr] = Field(None, alias="tertiaryMoodCluster", description="Search for a language of the lyrics")
+    tertiary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="tertiaryMoodClusterAffinity")
+    vocals_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="vocalsAffinity")
+    dominant_instrument_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="dominantInstrumentAffinity")
+    secondary_instrument: Optional[StrictStr] = Field(None, alias="secondaryInstrument", description="Search for a dominant instrument")
+    secondary_instrument_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="secondaryInstrumentAffinity")
+    tertiary_instrument: Optional[StrictStr] = Field(None, alias="tertiaryInstrument", description="Search for a dominant instrument")
+    tertiary_instrument_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="tertiaryInstrumentAffinity")
+    sound_generation_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="soundGenerationAffinity")
+    rhythm_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="rhythmAffinity")
     valence_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="valenceAffinity")
     arousal_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="arousalAffinity")
     pleasantness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="pleasantnessAffinity")
     engagement_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="engagementAffinity")
     energy_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="energyAffinity")
     tempo_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="tempoAffinity")
     scale_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="scaleAffinity")
@@ -107,424 +107,424 @@
     harmony_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="harmonyAffinity")
     texture_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="textureAffinity")
     groovyness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="groovynessAffinity")
     space_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="spaceAffinity")
     key_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="keyAffinity")
     channel_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="channelSuitabilityAffinity")
     key: Optional[StrictStr] = Field(None, description="Search for a harmonic key")
-    __properties = ["space", "primaryMoodClusterAffinity", "secondaryMoodCluster", "secondaryMoodClusterAffinity", "tertiaryMoodCluster", "tertiaryMoodClusterAffinity", "vocalsAffinity", "dominantInstrumentAffinity", "secondaryInstrument", "secondaryInstrumentAffinity", "tertiaryInstrument", "tertiaryInstrumentAffinity", "soundGenerationAffinity", "rhythmAffinity", "primarySoundCharacterAffinity", "tonalityAffinity", "bpm", "productionRating", "productionRatingAffinity", "performanceRating", "performanceRatingAffinity", "songRating", "songRatingAffinity", "audienceAge", "audienceAgeAffinity", "secondaryAudienceAge", "secondaryAudienceAgeAffinity", "tertiaryAudienceAge", "tertiaryAudienceAgeAffinity", "audienceGender", "audienceGenderAffinity", "audienceRegionAffinity", "secondaryAudienceRegion", "secondaryAudienceRegionAffinity", "tertiaryAudienceRegion", "tertiaryAudienceRegionAffinity", "originRegion", "originRegionAffinity", "originDecadeAffinity", "languageOfPerformanceAffinity", "curateabilityAffinity", "useCaseAffinity", "industrySuitability", "industrySuitabilityAffinity", "audienceRegion", "arousal", "dominantInstrument", "energy", "engagement", "groovyness", "harmony", "pleasantness", "primaryMoodCluster", "languageOfPerformance", "primarySoundCharacter", "rhythm", "roughness", "scale", "soundGeneration", "tempo", "texture", "timbre", "tonality", "valence", "vocals", "originDecade", "curateability", "useCase", "channelSuitability", "valenceAffinity", "arousalAffinity", "pleasantnessAffinity", "engagementAffinity", "energyAffinity", "tempoAffinity", "scaleAffinity", "timbreAffinity", "roughnessAffinity", "harmonyAffinity", "textureAffinity", "groovynessAffinity", "spaceAffinity", "keyAffinity", "channelSuitabilityAffinity", "key"]
+    __properties = ["space", "arousal", "dominantInstrument", "energy", "engagement", "groovyness", "harmony", "pleasantness", "primaryMoodCluster", "primarySoundCharacter", "rhythm", "roughness", "scale", "soundGeneration", "tempo", "texture", "timbre", "tonality", "valence", "vocals", "originDecade", "languageOfPerformance", "primarySoundCharacterAffinity", "tonalityAffinity", "bpm", "productionRating", "productionRatingAffinity", "performanceRating", "performanceRatingAffinity", "songRating", "songRatingAffinity", "audienceAge", "audienceAgeAffinity", "secondaryAudienceAge", "secondaryAudienceAgeAffinity", "tertiaryAudienceAge", "tertiaryAudienceAgeAffinity", "audienceGender", "audienceGenderAffinity", "audienceRegionAffinity", "secondaryAudienceRegion", "secondaryAudienceRegionAffinity", "tertiaryAudienceRegion", "tertiaryAudienceRegionAffinity", "originRegion", "originRegionAffinity", "originDecadeAffinity", "languageOfPerformanceAffinity", "curateabilityAffinity", "useCaseAffinity", "industrySuitability", "industrySuitabilityAffinity", "audienceRegion", "curateability", "useCase", "channelSuitability", "primaryMoodClusterAffinity", "secondaryMoodCluster", "secondaryMoodClusterAffinity", "tertiaryMoodCluster", "tertiaryMoodClusterAffinity", "vocalsAffinity", "dominantInstrumentAffinity", "secondaryInstrument", "secondaryInstrumentAffinity", "tertiaryInstrument", "tertiaryInstrumentAffinity", "soundGenerationAffinity", "rhythmAffinity", "valenceAffinity", "arousalAffinity", "pleasantnessAffinity", "engagementAffinity", "energyAffinity", "tempoAffinity", "scaleAffinity", "timbreAffinity", "roughnessAffinity", "harmonyAffinity", "textureAffinity", "groovynessAffinity", "spaceAffinity", "keyAffinity", "channelSuitabilityAffinity", "key"]
 
     @validator('space')
     def space_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
         if value not in ('very compact', 'compact', 'moderate space', 'wide', 'very wide'):
             raise ValueError("must be one of enum values ('very compact', 'compact', 'moderate space', 'wide', 'very wide')")
         return value
 
-    @validator('secondary_mood_cluster')
-    def secondary_mood_cluster_validate_enum(cls, value):
+    @validator('arousal')
+    def arousal_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild'):
-            raise ValueError("must be one of enum values ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild')")
+        if value not in ('very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal'):
+            raise ValueError("must be one of enum values ('very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal')")
         return value
 
-    @validator('tertiary_mood_cluster')
-    def tertiary_mood_cluster_validate_enum(cls, value):
+    @validator('dominant_instrument')
+    def dominant_instrument_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild'):
-            raise ValueError("must be one of enum values ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild')")
+        if value not in ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp'):
+            raise ValueError("must be one of enum values ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp')")
         return value
 
-    @validator('secondary_instrument')
-    def secondary_instrument_validate_enum(cls, value):
+    @validator('energy')
+    def energy_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp'):
-            raise ValueError("must be one of enum values ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp')")
+        if value not in ('very quiet', 'quiet', 'moderate', 'loud', 'very loud', 'dynamic'):
+            raise ValueError("must be one of enum values ('very quiet', 'quiet', 'moderate', 'loud', 'very loud', 'dynamic')")
         return value
 
-    @validator('tertiary_instrument')
-    def tertiary_instrument_validate_enum(cls, value):
+    @validator('engagement')
+    def engagement_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp'):
-            raise ValueError("must be one of enum values ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp')")
+        if value not in ('very unengaging', 'unengaging', 'neutral engagement', 'engaging', 'very engaging', 'varying engagement'):
+            raise ValueError("must be one of enum values ('very unengaging', 'unengaging', 'neutral engagement', 'engaging', 'very engaging', 'varying engagement')")
         return value
 
-    @validator('production_rating')
-    def production_rating_validate_enum(cls, value):
+    @validator('groovyness')
+    def groovyness_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('low production quality', 'medium production quality', 'high production quality'):
-            raise ValueError("must be one of enum values ('low production quality', 'medium production quality', 'high production quality')")
+        if value not in ('very steady', 'steady', 'moderate rhythm feel', 'groovy', 'very groovy'):
+            raise ValueError("must be one of enum values ('very steady', 'steady', 'moderate rhythm feel', 'groovy', 'very groovy')")
         return value
 
-    @validator('performance_rating')
-    def performance_rating_validate_enum(cls, value):
+    @validator('harmony')
+    def harmony_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('low performance quality', 'medium performance quality', 'high performance quality'):
-            raise ValueError("must be one of enum values ('low performance quality', 'medium performance quality', 'high performance quality')")
+        if value not in ('very dissonant', 'dissonant', 'moderate harmonies', 'harmonious', 'very harmonious'):
+            raise ValueError("must be one of enum values ('very dissonant', 'dissonant', 'moderate harmonies', 'harmonious', 'very harmonious')")
         return value
 
-    @validator('song_rating')
-    def song_rating_validate_enum(cls, value):
+    @validator('pleasantness')
+    def pleasantness_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('low song quality', 'medium song quality', 'high song quality'):
-            raise ValueError("must be one of enum values ('low song quality', 'medium song quality', 'high song quality')")
+        if value not in ('very unpleasant', 'unpleasant', 'neutral pleasantness', 'pleasant', 'very pleasant', 'varying pleasantness'):
+            raise ValueError("must be one of enum values ('very unpleasant', 'unpleasant', 'neutral pleasantness', 'pleasant', 'very pleasant', 'varying pleasantness')")
         return value
 
-    @validator('audience_age')
-    def audience_age_validate_enum(cls, value):
+    @validator('primary_mood_cluster')
+    def primary_mood_cluster_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B'):
-            raise ValueError("must be one of enum values ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B')")
+        if value not in ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild'):
+            raise ValueError("must be one of enum values ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild')")
         return value
 
-    @validator('secondary_audience_age')
-    def secondary_audience_age_validate_enum(cls, value):
+    @validator('primary_sound_character')
+    def primary_sound_character_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B'):
-            raise ValueError("must be one of enum values ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B')")
+        if value not in ('brassy', 'bright', 'clear', 'deep', 'distorted', 'flat', 'full', 'groovy', 'melodious', 'natural', 'resonant', 'shrill', 'steady', 'thin', 'warm'):
+            raise ValueError("must be one of enum values ('brassy', 'bright', 'clear', 'deep', 'distorted', 'flat', 'full', 'groovy', 'melodious', 'natural', 'resonant', 'shrill', 'steady', 'thin', 'warm')")
         return value
 
-    @validator('tertiary_audience_age')
-    def tertiary_audience_age_validate_enum(cls, value):
+    @validator('rhythm')
+    def rhythm_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B'):
-            raise ValueError("must be one of enum values ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B')")
+        if value not in ('common time', 'triple meter', 'complex time signature', 'binary rhythm', 'ternary rhythm'):
+            raise ValueError("must be one of enum values ('common time', 'triple meter', 'complex time signature', 'binary rhythm', 'ternary rhythm')")
         return value
 
-    @validator('audience_gender')
-    def audience_gender_validate_enum(cls, value):
+    @validator('roughness')
+    def roughness_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('male', 'female'):
-            raise ValueError("must be one of enum values ('male', 'female')")
+        if value not in ('very clear', 'clear', 'moderate roughness', 'distorted', 'very distorted'):
+            raise ValueError("must be one of enum values ('very clear', 'clear', 'moderate roughness', 'distorted', 'very distorted')")
         return value
 
-    @validator('secondary_audience_region')
-    def secondary_audience_region_validate_enum(cls, value):
+    @validator('scale')
+    def scale_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe'):
-            raise ValueError("must be one of enum values ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe')")
+        if value not in ('major key', 'minor key', 'neutral key'):
+            raise ValueError("must be one of enum values ('major key', 'minor key', 'neutral key')")
         return value
 
-    @validator('tertiary_audience_region')
-    def tertiary_audience_region_validate_enum(cls, value):
+    @validator('sound_generation')
+    def sound_generation_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe'):
-            raise ValueError("must be one of enum values ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe')")
+        if value not in ('acoustic', 'electric', 'electronic', 'mixed sound generation'):
+            raise ValueError("must be one of enum values ('acoustic', 'electric', 'electronic', 'mixed sound generation')")
         return value
 
-    @validator('origin_region')
-    def origin_region_validate_enum(cls, value):
+    @validator('tempo')
+    def tempo_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe'):
-            raise ValueError("must be one of enum values ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe')")
+        if value not in ('very slow', 'slow', 'mid-tempo', 'fast', 'very fast', 'varying tempo'):
+            raise ValueError("must be one of enum values ('very slow', 'slow', 'mid-tempo', 'fast', 'very fast', 'varying tempo')")
         return value
 
-    @validator('industry_suitability')
-    def industry_suitability_validate_enum(cls, value):
+    @validator('texture')
+    def texture_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Automobiles and Parts', 'Consumer Products and Services', 'Financial Services', 'Food, Beverage and Tobacco', 'Health Care', 'Insurance', 'Media', 'Politics, Government and Organizations', 'Real Estate', 'Retail', 'Technology', 'Telecommunications', 'Travel and Leisure'):
-            raise ValueError("must be one of enum values ('Automobiles and Parts', 'Consumer Products and Services', 'Financial Services', 'Food, Beverage and Tobacco', 'Health Care', 'Insurance', 'Media', 'Politics, Government and Organizations', 'Real Estate', 'Retail', 'Technology', 'Telecommunications', 'Travel and Leisure')")
+        if value not in ('very thin', 'thin', 'moderate texture', 'full', 'very full'):
+            raise ValueError("must be one of enum values ('very thin', 'thin', 'moderate texture', 'full', 'very full')")
         return value
 
-    @validator('audience_region')
-    def audience_region_validate_enum(cls, value):
+    @validator('timbre')
+    def timbre_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe'):
-            raise ValueError("must be one of enum values ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe')")
+        if value not in ('very warm', 'warm', 'moderate timbre', 'bright', 'very bright'):
+            raise ValueError("must be one of enum values ('very warm', 'warm', 'moderate timbre', 'bright', 'very bright')")
         return value
 
-    @validator('arousal')
-    def arousal_validate_enum(cls, value):
+    @validator('tonality')
+    def tonality_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal'):
-            raise ValueError("must be one of enum values ('very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal')")
+        if value not in ('monotonous', 'moderate melodiousness', 'melodious', 'atonal'):
+            raise ValueError("must be one of enum values ('monotonous', 'moderate melodiousness', 'melodious', 'atonal')")
         return value
 
-    @validator('dominant_instrument')
-    def dominant_instrument_validate_enum(cls, value):
+    @validator('valence')
+    def valence_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp'):
-            raise ValueError("must be one of enum values ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp')")
+        if value not in ('very sad', 'sad', 'moderate valence', 'positive', 'very positive', 'varying valence'):
+            raise ValueError("must be one of enum values ('very sad', 'sad', 'moderate valence', 'positive', 'very positive', 'varying valence')")
         return value
 
-    @validator('energy')
-    def energy_validate_enum(cls, value):
+    @validator('vocals')
+    def vocals_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very quiet', 'quiet', 'moderate', 'loud', 'very loud', 'dynamic'):
-            raise ValueError("must be one of enum values ('very quiet', 'quiet', 'moderate', 'loud', 'very loud', 'dynamic')")
+        if value not in ('instrumental', 'female vocals', 'male vocals', 'mixed vocals', 'diverse gender vocals'):
+            raise ValueError("must be one of enum values ('instrumental', 'female vocals', 'male vocals', 'mixed vocals', 'diverse gender vocals')")
         return value
 
-    @validator('engagement')
-    def engagement_validate_enum(cls, value):
+    @validator('origin_decade')
+    def origin_decade_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very unengaging', 'unengaging', 'neutral engagement', 'engaging', 'very engaging', 'varying engagement'):
-            raise ValueError("must be one of enum values ('very unengaging', 'unengaging', 'neutral engagement', 'engaging', 'very engaging', 'varying engagement')")
+        if value not in ('pre-1950s', '1950s', '1960s', '1970s', '1980s', '1990s', '2000s', '2010s', '2020s'):
+            raise ValueError("must be one of enum values ('pre-1950s', '1950s', '1960s', '1970s', '1980s', '1990s', '2000s', '2010s', '2020s')")
         return value
 
-    @validator('groovyness')
-    def groovyness_validate_enum(cls, value):
+    @validator('language_of_performance')
+    def language_of_performance_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very steady', 'steady', 'moderate rhythm feel', 'groovy', 'very groovy'):
-            raise ValueError("must be one of enum values ('very steady', 'steady', 'moderate rhythm feel', 'groovy', 'very groovy')")
+        if value not in ('en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi'):
+            raise ValueError("must be one of enum values ('en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi')")
         return value
 
-    @validator('harmony')
-    def harmony_validate_enum(cls, value):
+    @validator('production_rating')
+    def production_rating_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very dissonant', 'dissonant', 'moderate harmonies', 'harmonious', 'very harmonious'):
-            raise ValueError("must be one of enum values ('very dissonant', 'dissonant', 'moderate harmonies', 'harmonious', 'very harmonious')")
+        if value not in ('low production quality', 'medium production quality', 'high production quality'):
+            raise ValueError("must be one of enum values ('low production quality', 'medium production quality', 'high production quality')")
         return value
 
-    @validator('pleasantness')
-    def pleasantness_validate_enum(cls, value):
+    @validator('performance_rating')
+    def performance_rating_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very unpleasant', 'unpleasant', 'neutral pleasantness', 'pleasant', 'very pleasant', 'varying pleasantness'):
-            raise ValueError("must be one of enum values ('very unpleasant', 'unpleasant', 'neutral pleasantness', 'pleasant', 'very pleasant', 'varying pleasantness')")
+        if value not in ('low performance quality', 'medium performance quality', 'high performance quality'):
+            raise ValueError("must be one of enum values ('low performance quality', 'medium performance quality', 'high performance quality')")
         return value
 
-    @validator('primary_mood_cluster')
-    def primary_mood_cluster_validate_enum(cls, value):
+    @validator('song_rating')
+    def song_rating_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild'):
-            raise ValueError("must be one of enum values ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild')")
+        if value not in ('low song quality', 'medium song quality', 'high song quality'):
+            raise ValueError("must be one of enum values ('low song quality', 'medium song quality', 'high song quality')")
         return value
 
-    @validator('language_of_performance')
-    def language_of_performance_validate_enum(cls, value):
+    @validator('audience_age')
+    def audience_age_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi'):
-            raise ValueError("must be one of enum values ('en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi')")
+        if value not in ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B'):
+            raise ValueError("must be one of enum values ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B')")
         return value
 
-    @validator('primary_sound_character')
-    def primary_sound_character_validate_enum(cls, value):
+    @validator('secondary_audience_age')
+    def secondary_audience_age_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('brassy', 'bright', 'clear', 'deep', 'distorted', 'flat', 'full', 'groovy', 'melodious', 'natural', 'resonant', 'shrill', 'steady', 'thin', 'warm'):
-            raise ValueError("must be one of enum values ('brassy', 'bright', 'clear', 'deep', 'distorted', 'flat', 'full', 'groovy', 'melodious', 'natural', 'resonant', 'shrill', 'steady', 'thin', 'warm')")
+        if value not in ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B'):
+            raise ValueError("must be one of enum values ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B')")
         return value
 
-    @validator('rhythm')
-    def rhythm_validate_enum(cls, value):
+    @validator('tertiary_audience_age')
+    def tertiary_audience_age_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('common time', 'triple meter', 'complex time signature', 'binary rhythm', 'ternary rhythm'):
-            raise ValueError("must be one of enum values ('common time', 'triple meter', 'complex time signature', 'binary rhythm', 'ternary rhythm')")
+        if value not in ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B'):
+            raise ValueError("must be one of enum values ('Generation Z', 'Younger Generation Y', 'Older Generation Y', 'Generation X', 'Younger Generation B', 'Older Generation B')")
         return value
 
-    @validator('roughness')
-    def roughness_validate_enum(cls, value):
+    @validator('audience_gender')
+    def audience_gender_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very clear', 'clear', 'moderate roughness', 'distorted', 'very distorted'):
-            raise ValueError("must be one of enum values ('very clear', 'clear', 'moderate roughness', 'distorted', 'very distorted')")
+        if value not in ('male', 'female'):
+            raise ValueError("must be one of enum values ('male', 'female')")
         return value
 
-    @validator('scale')
-    def scale_validate_enum(cls, value):
+    @validator('secondary_audience_region')
+    def secondary_audience_region_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('major key', 'minor key', 'neutral key'):
-            raise ValueError("must be one of enum values ('major key', 'minor key', 'neutral key')")
+        if value not in ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe'):
+            raise ValueError("must be one of enum values ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe')")
         return value
 
-    @validator('sound_generation')
-    def sound_generation_validate_enum(cls, value):
+    @validator('tertiary_audience_region')
+    def tertiary_audience_region_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('acoustic', 'electric', 'electronic', 'mixed sound generation'):
-            raise ValueError("must be one of enum values ('acoustic', 'electric', 'electronic', 'mixed sound generation')")
+        if value not in ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe'):
+            raise ValueError("must be one of enum values ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe')")
         return value
 
-    @validator('tempo')
-    def tempo_validate_enum(cls, value):
+    @validator('origin_region')
+    def origin_region_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very slow', 'slow', 'mid-tempo', 'fast', 'very fast', 'varying tempo'):
-            raise ValueError("must be one of enum values ('very slow', 'slow', 'mid-tempo', 'fast', 'very fast', 'varying tempo')")
+        if value not in ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe'):
+            raise ValueError("must be one of enum values ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe')")
         return value
 
-    @validator('texture')
-    def texture_validate_enum(cls, value):
+    @validator('industry_suitability')
+    def industry_suitability_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very thin', 'thin', 'moderate texture', 'full', 'very full'):
-            raise ValueError("must be one of enum values ('very thin', 'thin', 'moderate texture', 'full', 'very full')")
+        if value not in ('Automobiles and Parts', 'Consumer Products and Services', 'Financial Services', 'Food, Beverage and Tobacco', 'Health Care', 'Insurance', 'Media', 'Politics, Government and Organizations', 'Real Estate', 'Retail', 'Technology', 'Telecommunications', 'Travel and Leisure'):
+            raise ValueError("must be one of enum values ('Automobiles and Parts', 'Consumer Products and Services', 'Financial Services', 'Food, Beverage and Tobacco', 'Health Care', 'Insurance', 'Media', 'Politics, Government and Organizations', 'Real Estate', 'Retail', 'Technology', 'Telecommunications', 'Travel and Leisure')")
         return value
 
-    @validator('timbre')
-    def timbre_validate_enum(cls, value):
+    @validator('audience_region')
+    def audience_region_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very warm', 'warm', 'moderate timbre', 'bright', 'very bright'):
-            raise ValueError("must be one of enum values ('very warm', 'warm', 'moderate timbre', 'bright', 'very bright')")
+        if value not in ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe'):
+            raise ValueError("must be one of enum values ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe')")
         return value
 
-    @validator('tonality')
-    def tonality_validate_enum(cls, value):
+    @validator('curateability')
+    def curateability_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('monotonous', 'moderate melodiousness', 'melodious', 'atonal'):
-            raise ValueError("must be one of enum values ('monotonous', 'moderate melodiousness', 'melodious', 'atonal')")
+        if value not in ('curateable', 'uncurateable'):
+            raise ValueError("must be one of enum values ('curateable', 'uncurateable')")
         return value
 
-    @validator('valence')
-    def valence_validate_enum(cls, value):
+    @validator('use_case')
+    def use_case_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('very sad', 'sad', 'moderate valence', 'positive', 'very positive', 'varying valence'):
-            raise ValueError("must be one of enum values ('very sad', 'sad', 'moderate valence', 'positive', 'very positive', 'varying valence')")
+        if value not in ('background', 'sport', 'focus', 'christmas', 'film', 'summer', 'adverts', 'party', 'relax'):
+            raise ValueError("must be one of enum values ('background', 'sport', 'focus', 'christmas', 'film', 'summer', 'adverts', 'party', 'relax')")
         return value
 
-    @validator('vocals')
-    def vocals_validate_enum(cls, value):
+    @validator('channel_suitability')
+    def channel_suitability_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('instrumental', 'female vocals', 'male vocals', 'mixed vocals', 'diverse gender vocals'):
-            raise ValueError("must be one of enum values ('instrumental', 'female vocals', 'male vocals', 'mixed vocals', 'diverse gender vocals')")
+        if value not in ('Spotify', 'TikTok', 'Unfitting', 'YouTube'):
+            raise ValueError("must be one of enum values ('Spotify', 'TikTok', 'Unfitting', 'YouTube')")
         return value
 
-    @validator('origin_decade')
-    def origin_decade_validate_enum(cls, value):
+    @validator('secondary_mood_cluster')
+    def secondary_mood_cluster_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('pre-1950s', '1950s', '1960s', '1970s', '1980s', '1990s', '2000s', '2010s', '2020s'):
-            raise ValueError("must be one of enum values ('pre-1950s', '1950s', '1960s', '1970s', '1980s', '1990s', '2000s', '2010s', '2020s')")
+        if value not in ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild'):
+            raise ValueError("must be one of enum values ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild')")
         return value
 
-    @validator('curateability')
-    def curateability_validate_enum(cls, value):
+    @validator('tertiary_mood_cluster')
+    def tertiary_mood_cluster_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('curateable', 'uncurateable'):
-            raise ValueError("must be one of enum values ('curateable', 'uncurateable')")
+        if value not in ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild'):
+            raise ValueError("must be one of enum values ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild')")
         return value
 
-    @validator('use_case')
-    def use_case_validate_enum(cls, value):
+    @validator('secondary_instrument')
+    def secondary_instrument_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('background', 'sport', 'focus', 'christmas', 'film', 'summer', 'adverts', 'party', 'relax'):
-            raise ValueError("must be one of enum values ('background', 'sport', 'focus', 'christmas', 'film', 'summer', 'adverts', 'party', 'relax')")
+        if value not in ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp'):
+            raise ValueError("must be one of enum values ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp')")
         return value
 
-    @validator('channel_suitability')
-    def channel_suitability_validate_enum(cls, value):
+    @validator('tertiary_instrument')
+    def tertiary_instrument_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Spotify', 'TikTok', 'Unfitting', 'YouTube'):
-            raise ValueError("must be one of enum values ('Spotify', 'TikTok', 'Unfitting', 'YouTube')")
+        if value not in ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp'):
+            raise ValueError("must be one of enum values ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp')")
         return value
 
     @validator('key')
     def key_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -566,27 +566,35 @@
             return None
 
         if not isinstance(obj, dict):
             return MusicalFeaturesDTO.parse_obj(obj)
 
         _obj = MusicalFeaturesDTO.parse_obj({
             "space": obj.get("space"),
-            "primary_mood_cluster_affinity": obj.get("primaryMoodClusterAffinity"),
-            "secondary_mood_cluster": obj.get("secondaryMoodCluster"),
-            "secondary_mood_cluster_affinity": obj.get("secondaryMoodClusterAffinity"),
-            "tertiary_mood_cluster": obj.get("tertiaryMoodCluster"),
-            "tertiary_mood_cluster_affinity": obj.get("tertiaryMoodClusterAffinity"),
-            "vocals_affinity": obj.get("vocalsAffinity"),
-            "dominant_instrument_affinity": obj.get("dominantInstrumentAffinity"),
-            "secondary_instrument": obj.get("secondaryInstrument"),
-            "secondary_instrument_affinity": obj.get("secondaryInstrumentAffinity"),
-            "tertiary_instrument": obj.get("tertiaryInstrument"),
-            "tertiary_instrument_affinity": obj.get("tertiaryInstrumentAffinity"),
-            "sound_generation_affinity": obj.get("soundGenerationAffinity"),
-            "rhythm_affinity": obj.get("rhythmAffinity"),
+            "arousal": obj.get("arousal"),
+            "dominant_instrument": obj.get("dominantInstrument"),
+            "energy": obj.get("energy"),
+            "engagement": obj.get("engagement"),
+            "groovyness": obj.get("groovyness"),
+            "harmony": obj.get("harmony"),
+            "pleasantness": obj.get("pleasantness"),
+            "primary_mood_cluster": obj.get("primaryMoodCluster"),
+            "primary_sound_character": obj.get("primarySoundCharacter"),
+            "rhythm": obj.get("rhythm"),
+            "roughness": obj.get("roughness"),
+            "scale": obj.get("scale"),
+            "sound_generation": obj.get("soundGeneration"),
+            "tempo": obj.get("tempo"),
+            "texture": obj.get("texture"),
+            "timbre": obj.get("timbre"),
+            "tonality": obj.get("tonality"),
+            "valence": obj.get("valence"),
+            "vocals": obj.get("vocals"),
+            "origin_decade": obj.get("originDecade"),
+            "language_of_performance": obj.get("languageOfPerformance"),
             "primary_sound_character_affinity": obj.get("primarySoundCharacterAffinity"),
             "tonality_affinity": obj.get("tonalityAffinity"),
             "bpm": obj.get("bpm"),
             "production_rating": obj.get("productionRating"),
             "production_rating_affinity": obj.get("productionRatingAffinity"),
             "performance_rating": obj.get("performanceRating"),
             "performance_rating_affinity": obj.get("performanceRatingAffinity"),
@@ -610,38 +618,30 @@
             "origin_decade_affinity": obj.get("originDecadeAffinity"),
             "language_of_performance_affinity": obj.get("languageOfPerformanceAffinity"),
             "curateability_affinity": obj.get("curateabilityAffinity"),
             "use_case_affinity": obj.get("useCaseAffinity"),
             "industry_suitability": obj.get("industrySuitability"),
             "industry_suitability_affinity": obj.get("industrySuitabilityAffinity"),
             "audience_region": obj.get("audienceRegion"),
-            "arousal": obj.get("arousal"),
-            "dominant_instrument": obj.get("dominantInstrument"),
-            "energy": obj.get("energy"),
-            "engagement": obj.get("engagement"),
-            "groovyness": obj.get("groovyness"),
-            "harmony": obj.get("harmony"),
-            "pleasantness": obj.get("pleasantness"),
-            "primary_mood_cluster": obj.get("primaryMoodCluster"),
-            "language_of_performance": obj.get("languageOfPerformance"),
-            "primary_sound_character": obj.get("primarySoundCharacter"),
-            "rhythm": obj.get("rhythm"),
-            "roughness": obj.get("roughness"),
-            "scale": obj.get("scale"),
-            "sound_generation": obj.get("soundGeneration"),
-            "tempo": obj.get("tempo"),
-            "texture": obj.get("texture"),
-            "timbre": obj.get("timbre"),
-            "tonality": obj.get("tonality"),
-            "valence": obj.get("valence"),
-            "vocals": obj.get("vocals"),
-            "origin_decade": obj.get("originDecade"),
             "curateability": obj.get("curateability"),
             "use_case": obj.get("useCase"),
             "channel_suitability": obj.get("channelSuitability"),
+            "primary_mood_cluster_affinity": obj.get("primaryMoodClusterAffinity"),
+            "secondary_mood_cluster": obj.get("secondaryMoodCluster"),
+            "secondary_mood_cluster_affinity": obj.get("secondaryMoodClusterAffinity"),
+            "tertiary_mood_cluster": obj.get("tertiaryMoodCluster"),
+            "tertiary_mood_cluster_affinity": obj.get("tertiaryMoodClusterAffinity"),
+            "vocals_affinity": obj.get("vocalsAffinity"),
+            "dominant_instrument_affinity": obj.get("dominantInstrumentAffinity"),
+            "secondary_instrument": obj.get("secondaryInstrument"),
+            "secondary_instrument_affinity": obj.get("secondaryInstrumentAffinity"),
+            "tertiary_instrument": obj.get("tertiaryInstrument"),
+            "tertiary_instrument_affinity": obj.get("tertiaryInstrumentAffinity"),
+            "sound_generation_affinity": obj.get("soundGenerationAffinity"),
+            "rhythm_affinity": obj.get("rhythmAffinity"),
             "valence_affinity": obj.get("valenceAffinity"),
             "arousal_affinity": obj.get("arousalAffinity"),
             "pleasantness_affinity": obj.get("pleasantnessAffinity"),
             "engagement_affinity": obj.get("engagementAffinity"),
             "energy_affinity": obj.get("energyAffinity"),
             "tempo_affinity": obj.get("tempoAffinity"),
             "scale_affinity": obj.get("scaleAffinity"),
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/p_line_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/p_line_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/party_large_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/party_large_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/party_small_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/party_small_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/playlist_large_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/playlist_large_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -26,24 +26,24 @@
 
 class PlaylistLargeDTO(BaseModel):
     """
     Details on a playlist
     """
     name: StrictStr = Field(...)
     state: Optional[StrictStr] = None
+    description: Optional[StrictStr] = None
+    usages: Optional[conlist(UsageDTO)] = None
     created: Optional[datetime] = None
     updated: Optional[datetime] = None
-    description: Optional[StrictStr] = None
+    songtradr_playlist_guid: Optional[StrictStr] = Field(None, alias="songtradrPlaylistGuid")
+    tracks: Optional[conlist(RecordingPlaylistDTO)] = None
     asset_url: Optional[StrictStr] = Field(None, alias="assetURL")
     pretzel_tier: Optional[StrictStr] = Field(None, alias="pretzelTier")
     usage: Optional[StrictStr] = None
-    tracks: Optional[conlist(RecordingPlaylistDTO)] = None
-    songtradr_playlist_guid: Optional[StrictStr] = Field(None, alias="songtradrPlaylistGuid")
-    usages: Optional[conlist(UsageDTO)] = None
-    __properties = ["name", "state", "created", "updated", "description", "assetURL", "pretzelTier", "usage", "tracks", "songtradrPlaylistGuid", "usages"]
+    __properties = ["name", "state", "description", "usages", "created", "updated", "songtradrPlaylistGuid", "tracks", "assetURL", "pretzelTier", "usage"]
 
     @validator('state')
     def state_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
@@ -71,47 +71,47 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in tracks (list)
-        _items = []
-        if self.tracks:
-            for _item in self.tracks:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['tracks'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in usages (list)
         _items = []
         if self.usages:
             for _item in self.usages:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['usages'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in tracks (list)
+        _items = []
+        if self.tracks:
+            for _item in self.tracks:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tracks'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> PlaylistLargeDTO:
         """Create an instance of PlaylistLargeDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return PlaylistLargeDTO.parse_obj(obj)
 
         _obj = PlaylistLargeDTO.parse_obj({
             "name": obj.get("name"),
             "state": obj.get("state"),
+            "description": obj.get("description"),
+            "usages": [UsageDTO.from_dict(_item) for _item in obj.get("usages")] if obj.get("usages") is not None else None,
             "created": obj.get("created"),
             "updated": obj.get("updated"),
-            "description": obj.get("description"),
+            "songtradr_playlist_guid": obj.get("songtradrPlaylistGuid"),
+            "tracks": [RecordingPlaylistDTO.from_dict(_item) for _item in obj.get("tracks")] if obj.get("tracks") is not None else None,
             "asset_url": obj.get("assetURL"),
             "pretzel_tier": obj.get("pretzelTier"),
-            "usage": obj.get("usage"),
-            "tracks": [RecordingPlaylistDTO.from_dict(_item) for _item in obj.get("tracks")] if obj.get("tracks") is not None else None,
-            "songtradr_playlist_guid": obj.get("songtradrPlaylistGuid"),
-            "usages": [UsageDTO.from_dict(_item) for _item in obj.get("usages")] if obj.get("usages") is not None else None
+            "usage": obj.get("usage")
         })
         return _obj
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/product_medium_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/product_medium_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -27,23 +27,23 @@
 from songtradr_api_client_python.models.title_dto import TitleDTO
 
 class ProductMediumDTO(BaseModel):
     """
     Product details with a mid-sized field-set.
     """
     duration: Optional[datetime] = None
-    parties: Optional[conlist(ProductPartyDTO, unique_items=True)] = None
-    grid: Optional[StrictStr] = None
-    release_date: Optional[datetime] = Field(None, alias="releaseDate")
-    takedown_date: Optional[datetime] = Field(None, alias="takedownDate")
     pline: Optional[PLineDTO] = None
-    titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     genres: Optional[conlist(GenreMinimalDTO, unique_items=True)] = None
+    titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     gtin: Optional[StrictStr] = None
-    __properties = ["duration", "parties", "grid", "releaseDate", "takedownDate", "pline", "titles", "genres", "gtin"]
+    grid: Optional[StrictStr] = None
+    release_date: Optional[datetime] = Field(None, alias="releaseDate")
+    takedown_date: Optional[datetime] = Field(None, alias="takedownDate")
+    parties: Optional[conlist(ProductPartyDTO, unique_items=True)] = None
+    __properties = ["duration", "pline", "genres", "titles", "gtin", "grid", "releaseDate", "takedownDate", "parties"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -61,55 +61,55 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in parties (list)
-        _items = []
-        if self.parties:
-            for _item in self.parties:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['parties'] = _items
         # override the default output from pydantic by calling `to_dict()` of pline
         if self.pline:
             _dict['pline'] = self.pline.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in genres (list)
+        _items = []
+        if self.genres:
+            for _item in self.genres:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['genres'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
         _items = []
         if self.titles:
             for _item in self.titles:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['titles'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in genres (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in parties (list)
         _items = []
-        if self.genres:
-            for _item in self.genres:
+        if self.parties:
+            for _item in self.parties:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['genres'] = _items
+            _dict['parties'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> ProductMediumDTO:
         """Create an instance of ProductMediumDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return ProductMediumDTO.parse_obj(obj)
 
         _obj = ProductMediumDTO.parse_obj({
             "duration": obj.get("duration"),
-            "parties": [ProductPartyDTO.from_dict(_item) for _item in obj.get("parties")] if obj.get("parties") is not None else None,
+            "pline": PLineDTO.from_dict(obj.get("pline")) if obj.get("pline") is not None else None,
+            "genres": [GenreMinimalDTO.from_dict(_item) for _item in obj.get("genres")] if obj.get("genres") is not None else None,
+            "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
+            "gtin": obj.get("gtin"),
             "grid": obj.get("grid"),
             "release_date": obj.get("releaseDate"),
             "takedown_date": obj.get("takedownDate"),
-            "pline": PLineDTO.from_dict(obj.get("pline")) if obj.get("pline") is not None else None,
-            "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
-            "genres": [GenreMinimalDTO.from_dict(_item) for _item in obj.get("genres")] if obj.get("genres") is not None else None,
-            "gtin": obj.get("gtin")
+            "parties": [ProductPartyDTO.from_dict(_item) for _item in obj.get("parties")] if obj.get("parties") is not None else None
         })
         return _obj
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/product_party_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/product_party_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -24,17 +24,17 @@
 from songtradr_api_client_python.models.contributor_type_dto import ContributorTypeDTO
 from songtradr_api_client_python.models.party_small_dto import PartySmallDTO
 
 class ProductPartyDTO(BaseModel):
     """
     Parties (persons, groups or organizations) that have contributed to a product.
     """
-    contributor_types: Optional[conlist(ContributorTypeDTO)] = Field(None, alias="contributorTypes")
     party: PartySmallDTO = Field(...)
-    __properties = ["contributorTypes", "party"]
+    contributor_types: Optional[conlist(ContributorTypeDTO)] = Field(None, alias="contributorTypes")
+    __properties = ["party", "contributorTypes"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -52,34 +52,34 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of party
+        if self.party:
+            _dict['party'] = self.party.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in contributor_types (list)
         _items = []
         if self.contributor_types:
             for _item in self.contributor_types:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['contributorTypes'] = _items
-        # override the default output from pydantic by calling `to_dict()` of party
-        if self.party:
-            _dict['party'] = self.party.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> ProductPartyDTO:
         """Create an instance of ProductPartyDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return ProductPartyDTO.parse_obj(obj)
 
         _obj = ProductPartyDTO.parse_obj({
-            "contributor_types": [ContributorTypeDTO.from_dict(_item) for _item in obj.get("contributorTypes")] if obj.get("contributorTypes") is not None else None,
-            "party": PartySmallDTO.from_dict(obj.get("party")) if obj.get("party") is not None else None
+            "party": PartySmallDTO.from_dict(obj.get("party")) if obj.get("party") is not None else None,
+            "contributor_types": [ContributorTypeDTO.from_dict(_item) for _item in obj.get("contributorTypes")] if obj.get("contributorTypes") is not None else None
         })
         return _obj
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_for_similarity_search_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_for_similarity_search_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_genre_prediction_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_genre_prediction_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_large_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_large_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -31,26 +31,26 @@
 from songtradr_api_client_python.models.track_to_medium_product_dto import TrackToMediumProductDTO
 
 class RecordingLargeDTO(BaseModel):
     """
     Recording with a large field set.
     """
     duration: Optional[StrictInt] = None
-    spotify_id: Optional[StrictStr] = Field(None, alias="spotifyId")
-    genre_predictions: Optional[conlist(RecordingGenrePredictionDTO, unique_items=True)] = Field(None, alias="genrePredictions")
-    pline: Optional[PLineDTO] = None
-    tags: Optional[conlist(RecordingTagSmallDTO)] = None
-    titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     tracks: Optional[conlist(TrackToMediumProductDTO, unique_items=True)] = None
     musical_features: Optional[MusicalFeaturesDTO] = Field(None, alias="musicalFeatures")
+    pline: Optional[PLineDTO] = None
+    genre_predictions: Optional[conlist(RecordingGenrePredictionDTO, unique_items=True)] = Field(None, alias="genrePredictions")
     parties: Optional[conlist(RecordingPartyDTO, unique_items=True)] = None
     genres: Optional[conlist(GenreDTO, unique_items=True)] = None
     language_of_performance: Optional[StrictStr] = Field(None, alias="languageOfPerformance")
+    titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     isrc: StrictStr = Field(...)
-    __properties = ["duration", "spotifyId", "genrePredictions", "pline", "tags", "titles", "tracks", "musicalFeatures", "parties", "genres", "languageOfPerformance", "isrc"]
+    tags: Optional[conlist(RecordingTagSmallDTO)] = None
+    spotify_id: Optional[StrictStr] = Field(None, alias="spotifyId")
+    __properties = ["duration", "tracks", "musicalFeatures", "pline", "genrePredictions", "parties", "genres", "languageOfPerformance", "titles", "isrc", "tags", "spotifyId"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -68,82 +68,82 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in genre_predictions (list)
-        _items = []
-        if self.genre_predictions:
-            for _item in self.genre_predictions:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['genrePredictions'] = _items
-        # override the default output from pydantic by calling `to_dict()` of pline
-        if self.pline:
-            _dict['pline'] = self.pline.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
-        _items = []
-        if self.tags:
-            for _item in self.tags:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['tags'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
-        _items = []
-        if self.titles:
-            for _item in self.titles:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['titles'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in tracks (list)
         _items = []
         if self.tracks:
             for _item in self.tracks:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['tracks'] = _items
         # override the default output from pydantic by calling `to_dict()` of musical_features
         if self.musical_features:
             _dict['musicalFeatures'] = self.musical_features.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of pline
+        if self.pline:
+            _dict['pline'] = self.pline.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in genre_predictions (list)
+        _items = []
+        if self.genre_predictions:
+            for _item in self.genre_predictions:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['genrePredictions'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in parties (list)
         _items = []
         if self.parties:
             for _item in self.parties:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['parties'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in genres (list)
         _items = []
         if self.genres:
             for _item in self.genres:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['genres'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
+        _items = []
+        if self.titles:
+            for _item in self.titles:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['titles'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
+        _items = []
+        if self.tags:
+            for _item in self.tags:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tags'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> RecordingLargeDTO:
         """Create an instance of RecordingLargeDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return RecordingLargeDTO.parse_obj(obj)
 
         _obj = RecordingLargeDTO.parse_obj({
             "duration": obj.get("duration"),
-            "spotify_id": obj.get("spotifyId"),
-            "genre_predictions": [RecordingGenrePredictionDTO.from_dict(_item) for _item in obj.get("genrePredictions")] if obj.get("genrePredictions") is not None else None,
-            "pline": PLineDTO.from_dict(obj.get("pline")) if obj.get("pline") is not None else None,
-            "tags": [RecordingTagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None,
-            "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
             "tracks": [TrackToMediumProductDTO.from_dict(_item) for _item in obj.get("tracks")] if obj.get("tracks") is not None else None,
             "musical_features": MusicalFeaturesDTO.from_dict(obj.get("musicalFeatures")) if obj.get("musicalFeatures") is not None else None,
+            "pline": PLineDTO.from_dict(obj.get("pline")) if obj.get("pline") is not None else None,
+            "genre_predictions": [RecordingGenrePredictionDTO.from_dict(_item) for _item in obj.get("genrePredictions")] if obj.get("genrePredictions") is not None else None,
             "parties": [RecordingPartyDTO.from_dict(_item) for _item in obj.get("parties")] if obj.get("parties") is not None else None,
             "genres": [GenreDTO.from_dict(_item) for _item in obj.get("genres")] if obj.get("genres") is not None else None,
             "language_of_performance": obj.get("languageOfPerformance"),
-            "isrc": obj.get("isrc")
+            "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
+            "isrc": obj.get("isrc"),
+            "tags": [RecordingTagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None,
+            "spotify_id": obj.get("spotifyId")
         })
         return _obj
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_list_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_list_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_medium_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_medium_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -28,25 +28,25 @@
 from songtradr_api_client_python.models.recording_tag_small_dto import RecordingTagSmallDTO
 from songtradr_api_client_python.models.title_dto import TitleDTO
 
 class RecordingMediumDTO(BaseModel):
     """
     Recording with a mid-sized field set.
     """
-    spotify_id: Optional[StrictStr] = Field(None, alias="spotifyId")
-    genre_predictions: Optional[conlist(RecordingGenrePredictionDTO, unique_items=True)] = Field(None, alias="genrePredictions")
-    tags: Optional[conlist(RecordingTagSmallDTO)] = None
-    titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     musical_features: Optional[MusicalFeaturesDTO] = Field(None, alias="musicalFeatures")
+    genre_predictions: Optional[conlist(RecordingGenrePredictionDTO, unique_items=True)] = Field(None, alias="genrePredictions")
     recording_party_entities: Optional[conlist(RecordingPartyDTO, unique_items=True)] = Field(None, alias="recordingPartyEntities")
     genres: Optional[conlist(GenreDTO, unique_items=True)] = None
     language_of_performance: Optional[StrictStr] = Field(None, alias="languageOfPerformance")
     release_date: Optional[datetime] = Field(None, alias="releaseDate")
+    titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     isrc: StrictStr = Field(...)
-    __properties = ["spotifyId", "genrePredictions", "tags", "titles", "musicalFeatures", "recordingPartyEntities", "genres", "languageOfPerformance", "releaseDate", "isrc"]
+    tags: Optional[conlist(RecordingTagSmallDTO)] = None
+    spotify_id: Optional[StrictStr] = Field(None, alias="spotifyId")
+    __properties = ["musicalFeatures", "genrePredictions", "recordingPartyEntities", "genres", "languageOfPerformance", "releaseDate", "titles", "isrc", "tags", "spotifyId"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -64,70 +64,70 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of musical_features
+        if self.musical_features:
+            _dict['musicalFeatures'] = self.musical_features.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in genre_predictions (list)
         _items = []
         if self.genre_predictions:
             for _item in self.genre_predictions:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['genrePredictions'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
-        _items = []
-        if self.tags:
-            for _item in self.tags:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['tags'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
-        _items = []
-        if self.titles:
-            for _item in self.titles:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['titles'] = _items
-        # override the default output from pydantic by calling `to_dict()` of musical_features
-        if self.musical_features:
-            _dict['musicalFeatures'] = self.musical_features.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in recording_party_entities (list)
         _items = []
         if self.recording_party_entities:
             for _item in self.recording_party_entities:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['recordingPartyEntities'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in genres (list)
         _items = []
         if self.genres:
             for _item in self.genres:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['genres'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
+        _items = []
+        if self.titles:
+            for _item in self.titles:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['titles'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
+        _items = []
+        if self.tags:
+            for _item in self.tags:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tags'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> RecordingMediumDTO:
         """Create an instance of RecordingMediumDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return RecordingMediumDTO.parse_obj(obj)
 
         _obj = RecordingMediumDTO.parse_obj({
-            "spotify_id": obj.get("spotifyId"),
-            "genre_predictions": [RecordingGenrePredictionDTO.from_dict(_item) for _item in obj.get("genrePredictions")] if obj.get("genrePredictions") is not None else None,
-            "tags": [RecordingTagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None,
-            "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
             "musical_features": MusicalFeaturesDTO.from_dict(obj.get("musicalFeatures")) if obj.get("musicalFeatures") is not None else None,
+            "genre_predictions": [RecordingGenrePredictionDTO.from_dict(_item) for _item in obj.get("genrePredictions")] if obj.get("genrePredictions") is not None else None,
             "recording_party_entities": [RecordingPartyDTO.from_dict(_item) for _item in obj.get("recordingPartyEntities")] if obj.get("recordingPartyEntities") is not None else None,
             "genres": [GenreDTO.from_dict(_item) for _item in obj.get("genres")] if obj.get("genres") is not None else None,
             "language_of_performance": obj.get("languageOfPerformance"),
             "release_date": obj.get("releaseDate"),
-            "isrc": obj.get("isrc")
+            "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
+            "isrc": obj.get("isrc"),
+            "tags": [RecordingTagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None,
+            "spotify_id": obj.get("spotifyId")
         })
         return _obj
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_party_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_party_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -24,17 +24,17 @@
 from songtradr_api_client_python.models.contributor_type_dto import ContributorTypeDTO
 from songtradr_api_client_python.models.party_small_dto import PartySmallDTO
 
 class RecordingPartyDTO(BaseModel):
     """
     Party (person, group or organization) that contributed to a recording.
     """
-    contributor_types: Optional[conlist(ContributorTypeDTO)] = Field(None, alias="contributorTypes")
     party: PartySmallDTO = Field(...)
-    __properties = ["contributorTypes", "party"]
+    contributor_types: Optional[conlist(ContributorTypeDTO)] = Field(None, alias="contributorTypes")
+    __properties = ["party", "contributorTypes"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -52,34 +52,34 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of party
+        if self.party:
+            _dict['party'] = self.party.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in contributor_types (list)
         _items = []
         if self.contributor_types:
             for _item in self.contributor_types:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['contributorTypes'] = _items
-        # override the default output from pydantic by calling `to_dict()` of party
-        if self.party:
-            _dict['party'] = self.party.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> RecordingPartyDTO:
         """Create an instance of RecordingPartyDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return RecordingPartyDTO.parse_obj(obj)
 
         _obj = RecordingPartyDTO.parse_obj({
-            "contributor_types": [ContributorTypeDTO.from_dict(_item) for _item in obj.get("contributorTypes")] if obj.get("contributorTypes") is not None else None,
-            "party": PartySmallDTO.from_dict(obj.get("party")) if obj.get("party") is not None else None
+            "party": PartySmallDTO.from_dict(obj.get("party")) if obj.get("party") is not None else None,
+            "contributor_types": [ContributorTypeDTO.from_dict(_item) for _item in obj.get("contributorTypes")] if obj.get("contributorTypes") is not None else None
         })
         return _obj
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_playlist_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_playlist_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -24,18 +24,18 @@
 from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO
 
 class RecordingPlaylistDTO(BaseModel):
     """
     Recording Playlist connection
     """
     recording: Optional[RecordingMediumDTO] = None
-    songtradr_track_guid: Optional[StrictStr] = Field(None, alias="songtradrTrackGuid")
     assigned_by_id: Optional[StrictInt] = Field(None, alias="assignedById")
     sequence: Optional[StrictInt] = None
-    __properties = ["recording", "songtradrTrackGuid", "assignedById", "sequence"]
+    songtradr_track_guid: Optional[StrictStr] = Field(None, alias="songtradrTrackGuid")
+    __properties = ["recording", "assignedById", "sequence", "songtradrTrackGuid"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -69,13 +69,13 @@
             return None
 
         if not isinstance(obj, dict):
             return RecordingPlaylistDTO.parse_obj(obj)
 
         _obj = RecordingPlaylistDTO.parse_obj({
             "recording": RecordingMediumDTO.from_dict(obj.get("recording")) if obj.get("recording") is not None else None,
-            "songtradr_track_guid": obj.get("songtradrTrackGuid"),
             "assigned_by_id": obj.get("assignedById"),
-            "sequence": obj.get("sequence")
+            "sequence": obj.get("sequence"),
+            "songtradr_track_guid": obj.get("songtradrTrackGuid")
         })
         return _obj
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_small_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -25,18 +25,18 @@
 from songtradr_api_client_python.models.title_dto import TitleDTO
 
 class RecordingSmallDTO(BaseModel):
     """
     Recording with a small field set.
     """
     duration: Optional[StrictInt] = None
-    titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     parties: Optional[conlist(RecordingPartyDTO, unique_items=True)] = None
+    titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     isrc: StrictStr = Field(...)
-    __properties = ["duration", "titles", "parties", "isrc"]
+    __properties = ["duration", "parties", "titles", "isrc"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -54,40 +54,40 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
-        _items = []
-        if self.titles:
-            for _item in self.titles:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['titles'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in parties (list)
         _items = []
         if self.parties:
             for _item in self.parties:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['parties'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
+        _items = []
+        if self.titles:
+            for _item in self.titles:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['titles'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> RecordingSmallDTO:
         """Create an instance of RecordingSmallDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return RecordingSmallDTO.parse_obj(obj)
 
         _obj = RecordingSmallDTO.parse_obj({
             "duration": obj.get("duration"),
-            "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
             "parties": [RecordingPartyDTO.from_dict(_item) for _item in obj.get("parties")] if obj.get("parties") is not None else None,
+            "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
             "isrc": obj.get("isrc")
         })
         return _obj
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_tag_small_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/recording_tag_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_file_recording_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_file_recording_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_playlist_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_playlist_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_genre_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_recording_genre_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_party_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_recording_party_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_playlist_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_recording_playlist_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_tag_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_recording_tag_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_referrer_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_referrer_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_user_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/save_user_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/search_filter_values_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/search_filter_values_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/search_recording_granular_abstraction_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/search_recording_granular_abstraction_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/search_recording_granular_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/search_recording_granular_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/sign_up_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/sign_up_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tag_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/tag_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -24,17 +24,17 @@
 from songtradr_api_client_python.models.category_minimal_dto import CategoryMinimalDTO
 
 class TagDTO(BaseModel):
     """
     A tag for recordings.
     """
     id: StrictInt = Field(...)
-    categories: Optional[conlist(CategoryMinimalDTO)] = None
     name: StrictStr = Field(...)
-    __properties = ["id", "categories", "name"]
+    categories: Optional[conlist(CategoryMinimalDTO)] = None
+    __properties = ["id", "name", "categories"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -72,12 +72,12 @@
             return None
 
         if not isinstance(obj, dict):
             return TagDTO.parse_obj(obj)
 
         _obj = TagDTO.parse_obj({
             "id": obj.get("id"),
-            "categories": [CategoryMinimalDTO.from_dict(_item) for _item in obj.get("categories")] if obj.get("categories") is not None else None,
-            "name": obj.get("name")
+            "name": obj.get("name"),
+            "categories": [CategoryMinimalDTO.from_dict(_item) for _item in obj.get("categories")] if obj.get("categories") is not None else None
         })
         return _obj
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tag_small_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/tag_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/taggram_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/taggram_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tags_summary_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/tags_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tagstrength_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/tagstrength_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/title_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/title_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/token_request.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/track_to_medium_product_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/track_to_medium_product_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/update_password_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/update_password_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/usage_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/usage_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/user_dto.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/models/user_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python/rest.py` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/PKG-INFO` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: songtradr-api-client-python
-Version: 1.12.21
+Version: 1.12.22
 Summary: Songtradr API
-Home-page: https://pypi.org/project/songtradr-api-client-python/
+Home-page: https://github.com/songtradr/songtradr-python-api-client-docs
 Author: Songtradr Inc.
 Author-email: info@songtradr.com
 Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
 Description-Content-Type: text/markdown
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world&#39;s released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
```

### Comparing `songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/SOURCES.txt` & `songtradr-api-client-python-1.12.22/songtradr_api_client_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `songtradr-api-client-python-1.12.21/test/test_allowed_values_api.py` & `songtradr-api-client-python-1.12.22/test/test_allowed_values_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_category_medium_dto.py` & `songtradr-api-client-python-1.12.22/test/test_category_medium_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,20 +36,20 @@
             optional params are included """
         # uncomment below to create an instance of `CategoryMediumDTO`
         """
         model = songtradr_api_client_python.models.category_medium_dto.CategoryMediumDTO()  # noqa: E501
         if include_optional :
             return CategoryMediumDTO(
                 id = 56, 
+                name = '', 
                 tags = [
                     songtradr_api_client_python.models.tag_small_dto.TagSmallDTO(
                         id = 56, 
                         name = '', )
-                    ], 
-                name = ''
+                    ]
             )
         else :
             return CategoryMediumDTO(
                 id = 56,
                 name = '',
         )
         """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_category_minimal_dto.py` & `songtradr-api-client-python-1.12.22/test/test_category_minimal_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_config_access_dto.py` & `songtradr-api-client-python-1.12.22/test/test_config_access_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_config_identifier_dto.py` & `songtradr-api-client-python-1.12.22/test/test_config_identifier_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_contributor_type_dto.py` & `songtradr-api-client-python-1.12.22/test/test_contributor_type_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_error_response.py` & `songtradr-api-client-python-1.12.22/test/test_error_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_field_summary_dto.py` & `songtradr-api-client-python-1.12.22/test/test_field_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_file_dto.py` & `songtradr-api-client-python-1.12.22/test/test_file_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -50,51 +50,37 @@
                 fingerprint_status = 'processing', 
                 fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 inference_status = 'processing', 
                 inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
-                    spotify_id = '', 
-                    genre_predictions = [
-                        songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                            genre_type = '', 
-                            genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                                genre_name = '', ), 
-                            probability = 1.337, )
-                        ], 
-                    tags = [
-                        songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                            tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                id = 56, 
-                                categories = [
-                                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                        category_name = '', )
-                                    ], 
-                                name = '', ), )
-                        ], 
-                    titles = [
-                        songtradr_api_client_python.models.title_dto.TitleDTO(
-                            title_text = '', )
-                        ], 
                     musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                         space = 'very compact', 
-                        primary_mood_cluster_affinity = 1.337, 
-                        secondary_mood_cluster = 'aggressive', 
-                        secondary_mood_cluster_affinity = 1.337, 
-                        tertiary_mood_cluster = 'aggressive', 
-                        tertiary_mood_cluster_affinity = 1.337, 
-                        vocals_affinity = 1.337, 
-                        dominant_instrument_affinity = 1.337, 
-                        secondary_instrument = 'electric guitar', 
-                        secondary_instrument_affinity = 1.337, 
-                        tertiary_instrument = 'electric guitar', 
-                        tertiary_instrument_affinity = 1.337, 
-                        sound_generation_affinity = 1.337, 
-                        rhythm_affinity = 1.337, 
+                        arousal = 'very calm', 
+                        dominant_instrument = 'electric guitar', 
+                        energy = 'very quiet', 
+                        engagement = 'very unengaging', 
+                        groovyness = 'very steady', 
+                        harmony = 'very dissonant', 
+                        pleasantness = 'very unpleasant', 
+                        primary_mood_cluster = 'aggressive', 
+                        primary_sound_character = 'brassy', 
+                        rhythm = 'common time', 
+                        roughness = 'very clear', 
+                        scale = 'major key', 
+                        sound_generation = 'acoustic', 
+                        tempo = 'very slow', 
+                        texture = 'very thin', 
+                        timbre = 'very warm', 
+                        tonality = 'monotonous', 
+                        valence = 'very sad', 
+                        vocals = 'instrumental', 
+                        origin_decade = 'pre-1950s', 
+                        language_of_performance = 'en', 
                         primary_sound_character_affinity = 1.337, 
                         tonality_affinity = 1.337, 
                         bpm = 1.337, 
                         production_rating = 'low production quality', 
                         production_rating_affinity = 1.337, 
                         performance_rating = 'low performance quality', 
                         performance_rating_affinity = 1.337, 
@@ -118,38 +104,30 @@
                         origin_decade_affinity = 1.337, 
                         language_of_performance_affinity = 1.337, 
                         curateability_affinity = 1.337, 
                         use_case_affinity = 1.337, 
                         industry_suitability = 'Automobiles and Parts', 
                         industry_suitability_affinity = 1.337, 
                         audience_region = 'Australia and New Zealand', 
-                        arousal = 'very calm', 
-                        dominant_instrument = 'electric guitar', 
-                        energy = 'very quiet', 
-                        engagement = 'very unengaging', 
-                        groovyness = 'very steady', 
-                        harmony = 'very dissonant', 
-                        pleasantness = 'very unpleasant', 
-                        primary_mood_cluster = 'aggressive', 
-                        language_of_performance = 'en', 
-                        primary_sound_character = 'brassy', 
-                        rhythm = 'common time', 
-                        roughness = 'very clear', 
-                        scale = 'major key', 
-                        sound_generation = 'acoustic', 
-                        tempo = 'very slow', 
-                        texture = 'very thin', 
-                        timbre = 'very warm', 
-                        tonality = 'monotonous', 
-                        valence = 'very sad', 
-                        vocals = 'instrumental', 
-                        origin_decade = 'pre-1950s', 
                         curateability = 'curateable', 
                         use_case = 'background', 
                         channel_suitability = 'Spotify', 
+                        primary_mood_cluster_affinity = 1.337, 
+                        secondary_mood_cluster = 'aggressive', 
+                        secondary_mood_cluster_affinity = 1.337, 
+                        tertiary_mood_cluster = 'aggressive', 
+                        tertiary_mood_cluster_affinity = 1.337, 
+                        vocals_affinity = 1.337, 
+                        dominant_instrument_affinity = 1.337, 
+                        secondary_instrument = 'electric guitar', 
+                        secondary_instrument_affinity = 1.337, 
+                        tertiary_instrument = 'electric guitar', 
+                        tertiary_instrument_affinity = 1.337, 
+                        sound_generation_affinity = 1.337, 
+                        rhythm_affinity = 1.337, 
                         valence_affinity = 1.337, 
                         arousal_affinity = 1.337, 
                         pleasantness_affinity = 1.337, 
                         engagement_affinity = 1.337, 
                         energy_affinity = 1.337, 
                         tempo_affinity = 1.337, 
                         scale_affinity = 1.337, 
@@ -158,32 +136,54 @@
                         harmony_affinity = 1.337, 
                         texture_affinity = 1.337, 
                         groovyness_affinity = 1.337, 
                         space_affinity = 1.337, 
                         key_affinity = 1.337, 
                         channel_suitability_affinity = 1.337, 
                         key = 'C', ), 
+                    genre_predictions = [
+                        songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                            genre_type = '', 
+                            genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                                genre_name = '', ), 
+                            probability = 1.337, )
+                        ], 
                     recording_party_entities = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                id = '', 
+                                full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                     type_name = '', )
-                                ], 
-                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                id = '', 
-                                full_name = '', ), )
+                                ], )
                         ], 
                     genres = [
                         songtradr_api_client_python.models.genre_dto.GenreDTO(
                             id = 56, 
                             name = '', )
                         ], 
                     language_of_performance = '', 
                     release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    isrc = '', ), 
+                    titles = [
+                        songtradr_api_client_python.models.title_dto.TitleDTO(
+                            title_text = '', )
+                        ], 
+                    isrc = '', 
+                    tags = [
+                        songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                            tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                id = 56, 
+                                name = '', 
+                                categories = [
+                                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                        category_name = '', )
+                                    ], ), )
+                        ], 
+                    spotify_id = '', ), 
                 error_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 error_message = ''
             )
         else :
             return FileDTO(
                 id = 56,
                 name = '',
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_file_list_dto.py` & `songtradr-api-client-python-1.12.22/test/test_file_list_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -52,51 +52,37 @@
                         fingerprint_status = 'processing', 
                         fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_status = 'processing', 
                         inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
-                            spotify_id = '', 
-                            genre_predictions = [
-                                songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                                    genre_type = '', 
-                                    genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                                        genre_name = '', ), 
-                                    probability = 1.337, )
-                                ], 
-                            tags = [
-                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                        id = 56, 
-                                        categories = [
-                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                                category_name = '', )
-                                            ], 
-                                        name = '', ), )
-                                ], 
-                            titles = [
-                                songtradr_api_client_python.models.title_dto.TitleDTO(
-                                    title_text = '', )
-                                ], 
                             musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                                 space = 'very compact', 
-                                primary_mood_cluster_affinity = 1.337, 
-                                secondary_mood_cluster = 'aggressive', 
-                                secondary_mood_cluster_affinity = 1.337, 
-                                tertiary_mood_cluster = 'aggressive', 
-                                tertiary_mood_cluster_affinity = 1.337, 
-                                vocals_affinity = 1.337, 
-                                dominant_instrument_affinity = 1.337, 
-                                secondary_instrument = 'electric guitar', 
-                                secondary_instrument_affinity = 1.337, 
-                                tertiary_instrument = 'electric guitar', 
-                                tertiary_instrument_affinity = 1.337, 
-                                sound_generation_affinity = 1.337, 
-                                rhythm_affinity = 1.337, 
+                                arousal = 'very calm', 
+                                dominant_instrument = 'electric guitar', 
+                                energy = 'very quiet', 
+                                engagement = 'very unengaging', 
+                                groovyness = 'very steady', 
+                                harmony = 'very dissonant', 
+                                pleasantness = 'very unpleasant', 
+                                primary_mood_cluster = 'aggressive', 
+                                primary_sound_character = 'brassy', 
+                                rhythm = 'common time', 
+                                roughness = 'very clear', 
+                                scale = 'major key', 
+                                sound_generation = 'acoustic', 
+                                tempo = 'very slow', 
+                                texture = 'very thin', 
+                                timbre = 'very warm', 
+                                tonality = 'monotonous', 
+                                valence = 'very sad', 
+                                vocals = 'instrumental', 
+                                origin_decade = 'pre-1950s', 
+                                language_of_performance = 'en', 
                                 primary_sound_character_affinity = 1.337, 
                                 tonality_affinity = 1.337, 
                                 bpm = 1.337, 
                                 production_rating = 'low production quality', 
                                 production_rating_affinity = 1.337, 
                                 performance_rating = 'low performance quality', 
                                 performance_rating_affinity = 1.337, 
@@ -120,38 +106,30 @@
                                 origin_decade_affinity = 1.337, 
                                 language_of_performance_affinity = 1.337, 
                                 curateability_affinity = 1.337, 
                                 use_case_affinity = 1.337, 
                                 industry_suitability = 'Automobiles and Parts', 
                                 industry_suitability_affinity = 1.337, 
                                 audience_region = 'Australia and New Zealand', 
-                                arousal = 'very calm', 
-                                dominant_instrument = 'electric guitar', 
-                                energy = 'very quiet', 
-                                engagement = 'very unengaging', 
-                                groovyness = 'very steady', 
-                                harmony = 'very dissonant', 
-                                pleasantness = 'very unpleasant', 
-                                primary_mood_cluster = 'aggressive', 
-                                language_of_performance = 'en', 
-                                primary_sound_character = 'brassy', 
-                                rhythm = 'common time', 
-                                roughness = 'very clear', 
-                                scale = 'major key', 
-                                sound_generation = 'acoustic', 
-                                tempo = 'very slow', 
-                                texture = 'very thin', 
-                                timbre = 'very warm', 
-                                tonality = 'monotonous', 
-                                valence = 'very sad', 
-                                vocals = 'instrumental', 
-                                origin_decade = 'pre-1950s', 
                                 curateability = 'curateable', 
                                 use_case = 'background', 
                                 channel_suitability = 'Spotify', 
+                                primary_mood_cluster_affinity = 1.337, 
+                                secondary_mood_cluster = 'aggressive', 
+                                secondary_mood_cluster_affinity = 1.337, 
+                                tertiary_mood_cluster = 'aggressive', 
+                                tertiary_mood_cluster_affinity = 1.337, 
+                                vocals_affinity = 1.337, 
+                                dominant_instrument_affinity = 1.337, 
+                                secondary_instrument = 'electric guitar', 
+                                secondary_instrument_affinity = 1.337, 
+                                tertiary_instrument = 'electric guitar', 
+                                tertiary_instrument_affinity = 1.337, 
+                                sound_generation_affinity = 1.337, 
+                                rhythm_affinity = 1.337, 
                                 valence_affinity = 1.337, 
                                 arousal_affinity = 1.337, 
                                 pleasantness_affinity = 1.337, 
                                 engagement_affinity = 1.337, 
                                 energy_affinity = 1.337, 
                                 tempo_affinity = 1.337, 
                                 scale_affinity = 1.337, 
@@ -160,32 +138,54 @@
                                 harmony_affinity = 1.337, 
                                 texture_affinity = 1.337, 
                                 groovyness_affinity = 1.337, 
                                 space_affinity = 1.337, 
                                 key_affinity = 1.337, 
                                 channel_suitability_affinity = 1.337, 
                                 key = 'C', ), 
+                            genre_predictions = [
+                                songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                                    genre_type = '', 
+                                    genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                                        genre_name = '', ), 
+                                    probability = 1.337, )
+                                ], 
                             recording_party_entities = [
                                 songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                        id = '', 
+                                        full_name = '', ), 
                                     contributor_types = [
                                         songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                             type_name = '', )
-                                        ], 
-                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                        id = '', 
-                                        full_name = '', ), )
+                                        ], )
                                 ], 
                             genres = [
                                 songtradr_api_client_python.models.genre_dto.GenreDTO(
                                     id = 56, 
                                     name = '', )
                                 ], 
                             language_of_performance = '', 
                             release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            isrc = '', ), 
+                            titles = [
+                                songtradr_api_client_python.models.title_dto.TitleDTO(
+                                    title_text = '', )
+                                ], 
+                            isrc = '', 
+                            tags = [
+                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                        id = 56, 
+                                        name = '', 
+                                        categories = [
+                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                                category_name = '', )
+                                            ], ), )
+                                ], 
+                            spotify_id = '', ), 
                         error_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         error_message = '', )
                     ], 
                 has_next_page = True, 
                 current_page_number = 56, 
                 total_results = 56
             )
@@ -204,51 +204,37 @@
                         fingerprint_status = 'processing', 
                         fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_status = 'processing', 
                         inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
-                            spotify_id = '', 
-                            genre_predictions = [
-                                songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                                    genre_type = '', 
-                                    genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                                        genre_name = '', ), 
-                                    probability = 1.337, )
-                                ], 
-                            tags = [
-                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                        id = 56, 
-                                        categories = [
-                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                                category_name = '', )
-                                            ], 
-                                        name = '', ), )
-                                ], 
-                            titles = [
-                                songtradr_api_client_python.models.title_dto.TitleDTO(
-                                    title_text = '', )
-                                ], 
                             musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                                 space = 'very compact', 
-                                primary_mood_cluster_affinity = 1.337, 
-                                secondary_mood_cluster = 'aggressive', 
-                                secondary_mood_cluster_affinity = 1.337, 
-                                tertiary_mood_cluster = 'aggressive', 
-                                tertiary_mood_cluster_affinity = 1.337, 
-                                vocals_affinity = 1.337, 
-                                dominant_instrument_affinity = 1.337, 
-                                secondary_instrument = 'electric guitar', 
-                                secondary_instrument_affinity = 1.337, 
-                                tertiary_instrument = 'electric guitar', 
-                                tertiary_instrument_affinity = 1.337, 
-                                sound_generation_affinity = 1.337, 
-                                rhythm_affinity = 1.337, 
+                                arousal = 'very calm', 
+                                dominant_instrument = 'electric guitar', 
+                                energy = 'very quiet', 
+                                engagement = 'very unengaging', 
+                                groovyness = 'very steady', 
+                                harmony = 'very dissonant', 
+                                pleasantness = 'very unpleasant', 
+                                primary_mood_cluster = 'aggressive', 
+                                primary_sound_character = 'brassy', 
+                                rhythm = 'common time', 
+                                roughness = 'very clear', 
+                                scale = 'major key', 
+                                sound_generation = 'acoustic', 
+                                tempo = 'very slow', 
+                                texture = 'very thin', 
+                                timbre = 'very warm', 
+                                tonality = 'monotonous', 
+                                valence = 'very sad', 
+                                vocals = 'instrumental', 
+                                origin_decade = 'pre-1950s', 
+                                language_of_performance = 'en', 
                                 primary_sound_character_affinity = 1.337, 
                                 tonality_affinity = 1.337, 
                                 bpm = 1.337, 
                                 production_rating = 'low production quality', 
                                 production_rating_affinity = 1.337, 
                                 performance_rating = 'low performance quality', 
                                 performance_rating_affinity = 1.337, 
@@ -272,38 +258,30 @@
                                 origin_decade_affinity = 1.337, 
                                 language_of_performance_affinity = 1.337, 
                                 curateability_affinity = 1.337, 
                                 use_case_affinity = 1.337, 
                                 industry_suitability = 'Automobiles and Parts', 
                                 industry_suitability_affinity = 1.337, 
                                 audience_region = 'Australia and New Zealand', 
-                                arousal = 'very calm', 
-                                dominant_instrument = 'electric guitar', 
-                                energy = 'very quiet', 
-                                engagement = 'very unengaging', 
-                                groovyness = 'very steady', 
-                                harmony = 'very dissonant', 
-                                pleasantness = 'very unpleasant', 
-                                primary_mood_cluster = 'aggressive', 
-                                language_of_performance = 'en', 
-                                primary_sound_character = 'brassy', 
-                                rhythm = 'common time', 
-                                roughness = 'very clear', 
-                                scale = 'major key', 
-                                sound_generation = 'acoustic', 
-                                tempo = 'very slow', 
-                                texture = 'very thin', 
-                                timbre = 'very warm', 
-                                tonality = 'monotonous', 
-                                valence = 'very sad', 
-                                vocals = 'instrumental', 
-                                origin_decade = 'pre-1950s', 
                                 curateability = 'curateable', 
                                 use_case = 'background', 
                                 channel_suitability = 'Spotify', 
+                                primary_mood_cluster_affinity = 1.337, 
+                                secondary_mood_cluster = 'aggressive', 
+                                secondary_mood_cluster_affinity = 1.337, 
+                                tertiary_mood_cluster = 'aggressive', 
+                                tertiary_mood_cluster_affinity = 1.337, 
+                                vocals_affinity = 1.337, 
+                                dominant_instrument_affinity = 1.337, 
+                                secondary_instrument = 'electric guitar', 
+                                secondary_instrument_affinity = 1.337, 
+                                tertiary_instrument = 'electric guitar', 
+                                tertiary_instrument_affinity = 1.337, 
+                                sound_generation_affinity = 1.337, 
+                                rhythm_affinity = 1.337, 
                                 valence_affinity = 1.337, 
                                 arousal_affinity = 1.337, 
                                 pleasantness_affinity = 1.337, 
                                 engagement_affinity = 1.337, 
                                 energy_affinity = 1.337, 
                                 tempo_affinity = 1.337, 
                                 scale_affinity = 1.337, 
@@ -312,32 +290,54 @@
                                 harmony_affinity = 1.337, 
                                 texture_affinity = 1.337, 
                                 groovyness_affinity = 1.337, 
                                 space_affinity = 1.337, 
                                 key_affinity = 1.337, 
                                 channel_suitability_affinity = 1.337, 
                                 key = 'C', ), 
+                            genre_predictions = [
+                                songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                                    genre_type = '', 
+                                    genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                                        genre_name = '', ), 
+                                    probability = 1.337, )
+                                ], 
                             recording_party_entities = [
                                 songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                        id = '', 
+                                        full_name = '', ), 
                                     contributor_types = [
                                         songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                             type_name = '', )
-                                        ], 
-                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                        id = '', 
-                                        full_name = '', ), )
+                                        ], )
                                 ], 
                             genres = [
                                 songtradr_api_client_python.models.genre_dto.GenreDTO(
                                     id = 56, 
                                     name = '', )
                                 ], 
                             language_of_performance = '', 
                             release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            isrc = '', ), 
+                            titles = [
+                                songtradr_api_client_python.models.title_dto.TitleDTO(
+                                    title_text = '', )
+                                ], 
+                            isrc = '', 
+                            tags = [
+                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                        id = 56, 
+                                        name = '', 
+                                        categories = [
+                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                                category_name = '', )
+                                            ], ), )
+                                ], 
+                            spotify_id = '', ), 
                         error_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         error_message = '', )
                     ],
                 has_next_page = True,
                 current_page_number = 56,
                 total_results = 56,
         )
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_file_minimal_with_url_dto.py` & `songtradr-api-client-python-1.12.22/test/test_file_minimal_with_url_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_file_small_dto.py` & `songtradr-api-client-python-1.12.22/test/test_file_small_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_file_upload_dto.py` & `songtradr-api-client-python-1.12.22/test/test_file_upload_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_file_w_ith_url_dto.py` & `songtradr-api-client-python-1.12.22/test/test_file_w_ith_url_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -51,51 +51,37 @@
                     fingerprint_status = 'processing', 
                     fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_status = 'processing', 
                     inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
-                        spotify_id = '', 
-                        genre_predictions = [
-                            songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                                genre_type = '', 
-                                genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                                    genre_name = '', ), 
-                                probability = 1.337, )
-                            ], 
-                        tags = [
-                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                    id = 56, 
-                                    categories = [
-                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                            category_name = '', )
-                                        ], 
-                                    name = '', ), )
-                            ], 
-                        titles = [
-                            songtradr_api_client_python.models.title_dto.TitleDTO(
-                                title_text = '', )
-                            ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            primary_mood_cluster_affinity = 1.337, 
-                            secondary_mood_cluster = 'aggressive', 
-                            secondary_mood_cluster_affinity = 1.337, 
-                            tertiary_mood_cluster = 'aggressive', 
-                            tertiary_mood_cluster_affinity = 1.337, 
-                            vocals_affinity = 1.337, 
-                            dominant_instrument_affinity = 1.337, 
-                            secondary_instrument = 'electric guitar', 
-                            secondary_instrument_affinity = 1.337, 
-                            tertiary_instrument = 'electric guitar', 
-                            tertiary_instrument_affinity = 1.337, 
-                            sound_generation_affinity = 1.337, 
-                            rhythm_affinity = 1.337, 
+                            arousal = 'very calm', 
+                            dominant_instrument = 'electric guitar', 
+                            energy = 'very quiet', 
+                            engagement = 'very unengaging', 
+                            groovyness = 'very steady', 
+                            harmony = 'very dissonant', 
+                            pleasantness = 'very unpleasant', 
+                            primary_mood_cluster = 'aggressive', 
+                            primary_sound_character = 'brassy', 
+                            rhythm = 'common time', 
+                            roughness = 'very clear', 
+                            scale = 'major key', 
+                            sound_generation = 'acoustic', 
+                            tempo = 'very slow', 
+                            texture = 'very thin', 
+                            timbre = 'very warm', 
+                            tonality = 'monotonous', 
+                            valence = 'very sad', 
+                            vocals = 'instrumental', 
+                            origin_decade = 'pre-1950s', 
+                            language_of_performance = 'en', 
                             primary_sound_character_affinity = 1.337, 
                             tonality_affinity = 1.337, 
                             bpm = 1.337, 
                             production_rating = 'low production quality', 
                             production_rating_affinity = 1.337, 
                             performance_rating = 'low performance quality', 
                             performance_rating_affinity = 1.337, 
@@ -119,38 +105,30 @@
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', 
-                            arousal = 'very calm', 
-                            dominant_instrument = 'electric guitar', 
-                            energy = 'very quiet', 
-                            engagement = 'very unengaging', 
-                            groovyness = 'very steady', 
-                            harmony = 'very dissonant', 
-                            pleasantness = 'very unpleasant', 
-                            primary_mood_cluster = 'aggressive', 
-                            language_of_performance = 'en', 
-                            primary_sound_character = 'brassy', 
-                            rhythm = 'common time', 
-                            roughness = 'very clear', 
-                            scale = 'major key', 
-                            sound_generation = 'acoustic', 
-                            tempo = 'very slow', 
-                            texture = 'very thin', 
-                            timbre = 'very warm', 
-                            tonality = 'monotonous', 
-                            valence = 'very sad', 
-                            vocals = 'instrumental', 
-                            origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            primary_mood_cluster_affinity = 1.337, 
+                            secondary_mood_cluster = 'aggressive', 
+                            secondary_mood_cluster_affinity = 1.337, 
+                            tertiary_mood_cluster = 'aggressive', 
+                            tertiary_mood_cluster_affinity = 1.337, 
+                            vocals_affinity = 1.337, 
+                            dominant_instrument_affinity = 1.337, 
+                            secondary_instrument = 'electric guitar', 
+                            secondary_instrument_affinity = 1.337, 
+                            tertiary_instrument = 'electric guitar', 
+                            tertiary_instrument_affinity = 1.337, 
+                            sound_generation_affinity = 1.337, 
+                            rhythm_affinity = 1.337, 
                             valence_affinity = 1.337, 
                             arousal_affinity = 1.337, 
                             pleasantness_affinity = 1.337, 
                             engagement_affinity = 1.337, 
                             energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
@@ -159,32 +137,54 @@
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
                             key = 'C', ), 
+                        genre_predictions = [
+                            songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                                genre_type = '', 
+                                genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                                    genre_name = '', ), 
+                                probability = 1.337, )
+                            ], 
                         recording_party_entities = [
                             songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                    id = '', 
+                                    full_name = '', ), 
                                 contributor_types = [
                                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                         type_name = '', )
-                                    ], 
-                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                    id = '', 
-                                    full_name = '', ), )
+                                    ], )
                             ], 
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        isrc = '', ), 
+                        titles = [
+                            songtradr_api_client_python.models.title_dto.TitleDTO(
+                                title_text = '', )
+                            ], 
+                        isrc = '', 
+                        tags = [
+                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                    id = 56, 
+                                    name = '', 
+                                    categories = [
+                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                            category_name = '', )
+                                        ], ), )
+                            ], 
+                        spotify_id = '', ), 
                     error_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     error_message = '', ), 
                 url = ''
             )
         else :
             return FileWIthUrlDTO(
                 file = songtradr_api_client_python.models.file_dto.FileDTO(
@@ -199,51 +199,37 @@
                     fingerprint_status = 'processing', 
                     fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_status = 'processing', 
                     inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
-                        spotify_id = '', 
-                        genre_predictions = [
-                            songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                                genre_type = '', 
-                                genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                                    genre_name = '', ), 
-                                probability = 1.337, )
-                            ], 
-                        tags = [
-                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                    id = 56, 
-                                    categories = [
-                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                            category_name = '', )
-                                        ], 
-                                    name = '', ), )
-                            ], 
-                        titles = [
-                            songtradr_api_client_python.models.title_dto.TitleDTO(
-                                title_text = '', )
-                            ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            primary_mood_cluster_affinity = 1.337, 
-                            secondary_mood_cluster = 'aggressive', 
-                            secondary_mood_cluster_affinity = 1.337, 
-                            tertiary_mood_cluster = 'aggressive', 
-                            tertiary_mood_cluster_affinity = 1.337, 
-                            vocals_affinity = 1.337, 
-                            dominant_instrument_affinity = 1.337, 
-                            secondary_instrument = 'electric guitar', 
-                            secondary_instrument_affinity = 1.337, 
-                            tertiary_instrument = 'electric guitar', 
-                            tertiary_instrument_affinity = 1.337, 
-                            sound_generation_affinity = 1.337, 
-                            rhythm_affinity = 1.337, 
+                            arousal = 'very calm', 
+                            dominant_instrument = 'electric guitar', 
+                            energy = 'very quiet', 
+                            engagement = 'very unengaging', 
+                            groovyness = 'very steady', 
+                            harmony = 'very dissonant', 
+                            pleasantness = 'very unpleasant', 
+                            primary_mood_cluster = 'aggressive', 
+                            primary_sound_character = 'brassy', 
+                            rhythm = 'common time', 
+                            roughness = 'very clear', 
+                            scale = 'major key', 
+                            sound_generation = 'acoustic', 
+                            tempo = 'very slow', 
+                            texture = 'very thin', 
+                            timbre = 'very warm', 
+                            tonality = 'monotonous', 
+                            valence = 'very sad', 
+                            vocals = 'instrumental', 
+                            origin_decade = 'pre-1950s', 
+                            language_of_performance = 'en', 
                             primary_sound_character_affinity = 1.337, 
                             tonality_affinity = 1.337, 
                             bpm = 1.337, 
                             production_rating = 'low production quality', 
                             production_rating_affinity = 1.337, 
                             performance_rating = 'low performance quality', 
                             performance_rating_affinity = 1.337, 
@@ -267,38 +253,30 @@
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', 
-                            arousal = 'very calm', 
-                            dominant_instrument = 'electric guitar', 
-                            energy = 'very quiet', 
-                            engagement = 'very unengaging', 
-                            groovyness = 'very steady', 
-                            harmony = 'very dissonant', 
-                            pleasantness = 'very unpleasant', 
-                            primary_mood_cluster = 'aggressive', 
-                            language_of_performance = 'en', 
-                            primary_sound_character = 'brassy', 
-                            rhythm = 'common time', 
-                            roughness = 'very clear', 
-                            scale = 'major key', 
-                            sound_generation = 'acoustic', 
-                            tempo = 'very slow', 
-                            texture = 'very thin', 
-                            timbre = 'very warm', 
-                            tonality = 'monotonous', 
-                            valence = 'very sad', 
-                            vocals = 'instrumental', 
-                            origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            primary_mood_cluster_affinity = 1.337, 
+                            secondary_mood_cluster = 'aggressive', 
+                            secondary_mood_cluster_affinity = 1.337, 
+                            tertiary_mood_cluster = 'aggressive', 
+                            tertiary_mood_cluster_affinity = 1.337, 
+                            vocals_affinity = 1.337, 
+                            dominant_instrument_affinity = 1.337, 
+                            secondary_instrument = 'electric guitar', 
+                            secondary_instrument_affinity = 1.337, 
+                            tertiary_instrument = 'electric guitar', 
+                            tertiary_instrument_affinity = 1.337, 
+                            sound_generation_affinity = 1.337, 
+                            rhythm_affinity = 1.337, 
                             valence_affinity = 1.337, 
                             arousal_affinity = 1.337, 
                             pleasantness_affinity = 1.337, 
                             engagement_affinity = 1.337, 
                             energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
@@ -307,32 +285,54 @@
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
                             key = 'C', ), 
+                        genre_predictions = [
+                            songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                                genre_type = '', 
+                                genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                                    genre_name = '', ), 
+                                probability = 1.337, )
+                            ], 
                         recording_party_entities = [
                             songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                    id = '', 
+                                    full_name = '', ), 
                                 contributor_types = [
                                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                         type_name = '', )
-                                    ], 
-                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                    id = '', 
-                                    full_name = '', ), )
+                                    ], )
                             ], 
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        isrc = '', ), 
+                        titles = [
+                            songtradr_api_client_python.models.title_dto.TitleDTO(
+                                title_text = '', )
+                            ], 
+                        isrc = '', 
+                        tags = [
+                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                    id = 56, 
+                                    name = '', 
+                                    categories = [
+                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                            category_name = '', )
+                                        ], ), )
+                            ], 
+                        spotify_id = '', ), 
                     error_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     error_message = '', ),
                 url = '',
         )
         """
 
     def testFileWIthUrlDTO(self):
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_files_summary_dto.py` & `songtradr-api-client-python-1.12.22/test/test_files_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_forgot_password_dto.py` & `songtradr-api-client-python-1.12.22/test/test_forgot_password_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_genre_dto.py` & `songtradr-api-client-python-1.12.22/test/test_genre_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_genre_minimal_dto.py` & `songtradr-api-client-python-1.12.22/test/test_genre_minimal_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_genres_summary_dto.py` & `songtradr-api-client-python-1.12.22/test/test_genres_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_init_put_recording_audio_dto.py` & `songtradr-api-client-python-1.12.22/test/test_init_put_recording_audio_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_jwt_token_dto.py` & `songtradr-api-client-python-1.12.22/test/test_jwt_token_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_login_dto.py` & `songtradr-api-client-python-1.12.22/test/test_login_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_musical_features_dto.py` & `songtradr-api-client-python-1.12.22/test/test_musical_features_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,27 +36,35 @@
             optional params are included """
         # uncomment below to create an instance of `MusicalFeaturesDTO`
         """
         model = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO()  # noqa: E501
         if include_optional :
             return MusicalFeaturesDTO(
                 space = 'very compact', 
-                primary_mood_cluster_affinity = 1.337, 
-                secondary_mood_cluster = 'aggressive', 
-                secondary_mood_cluster_affinity = 1.337, 
-                tertiary_mood_cluster = 'aggressive', 
-                tertiary_mood_cluster_affinity = 1.337, 
-                vocals_affinity = 1.337, 
-                dominant_instrument_affinity = 1.337, 
-                secondary_instrument = 'electric guitar', 
-                secondary_instrument_affinity = 1.337, 
-                tertiary_instrument = 'electric guitar', 
-                tertiary_instrument_affinity = 1.337, 
-                sound_generation_affinity = 1.337, 
-                rhythm_affinity = 1.337, 
+                arousal = 'very calm', 
+                dominant_instrument = 'electric guitar', 
+                energy = 'very quiet', 
+                engagement = 'very unengaging', 
+                groovyness = 'very steady', 
+                harmony = 'very dissonant', 
+                pleasantness = 'very unpleasant', 
+                primary_mood_cluster = 'aggressive', 
+                primary_sound_character = 'brassy', 
+                rhythm = 'common time', 
+                roughness = 'very clear', 
+                scale = 'major key', 
+                sound_generation = 'acoustic', 
+                tempo = 'very slow', 
+                texture = 'very thin', 
+                timbre = 'very warm', 
+                tonality = 'monotonous', 
+                valence = 'very sad', 
+                vocals = 'instrumental', 
+                origin_decade = 'pre-1950s', 
+                language_of_performance = 'en', 
                 primary_sound_character_affinity = 1.337, 
                 tonality_affinity = 1.337, 
                 bpm = 1.337, 
                 production_rating = 'low production quality', 
                 production_rating_affinity = 1.337, 
                 performance_rating = 'low performance quality', 
                 performance_rating_affinity = 1.337, 
@@ -80,38 +88,30 @@
                 origin_decade_affinity = 1.337, 
                 language_of_performance_affinity = 1.337, 
                 curateability_affinity = 1.337, 
                 use_case_affinity = 1.337, 
                 industry_suitability = 'Automobiles and Parts', 
                 industry_suitability_affinity = 1.337, 
                 audience_region = 'Australia and New Zealand', 
-                arousal = 'very calm', 
-                dominant_instrument = 'electric guitar', 
-                energy = 'very quiet', 
-                engagement = 'very unengaging', 
-                groovyness = 'very steady', 
-                harmony = 'very dissonant', 
-                pleasantness = 'very unpleasant', 
-                primary_mood_cluster = 'aggressive', 
-                language_of_performance = 'en', 
-                primary_sound_character = 'brassy', 
-                rhythm = 'common time', 
-                roughness = 'very clear', 
-                scale = 'major key', 
-                sound_generation = 'acoustic', 
-                tempo = 'very slow', 
-                texture = 'very thin', 
-                timbre = 'very warm', 
-                tonality = 'monotonous', 
-                valence = 'very sad', 
-                vocals = 'instrumental', 
-                origin_decade = 'pre-1950s', 
                 curateability = 'curateable', 
                 use_case = 'background', 
                 channel_suitability = 'Spotify', 
+                primary_mood_cluster_affinity = 1.337, 
+                secondary_mood_cluster = 'aggressive', 
+                secondary_mood_cluster_affinity = 1.337, 
+                tertiary_mood_cluster = 'aggressive', 
+                tertiary_mood_cluster_affinity = 1.337, 
+                vocals_affinity = 1.337, 
+                dominant_instrument_affinity = 1.337, 
+                secondary_instrument = 'electric guitar', 
+                secondary_instrument_affinity = 1.337, 
+                tertiary_instrument = 'electric guitar', 
+                tertiary_instrument_affinity = 1.337, 
+                sound_generation_affinity = 1.337, 
+                rhythm_affinity = 1.337, 
                 valence_affinity = 1.337, 
                 arousal_affinity = 1.337, 
                 pleasantness_affinity = 1.337, 
                 engagement_affinity = 1.337, 
                 energy_affinity = 1.337, 
                 tempo_affinity = 1.337, 
                 scale_affinity = 1.337,
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_p_line_dto.py` & `songtradr-api-client-python-1.12.22/test/test_p_line_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_party_api.py` & `songtradr-api-client-python-1.12.22/test/test_party_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_party_large_dto.py` & `songtradr-api-client-python-1.12.22/test/test_party_large_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_party_small_dto.py` & `songtradr-api-client-python-1.12.22/test/test_party_small_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_playlist_api.py` & `songtradr-api-client-python-1.12.22/test/test_playlist_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_playlist_large_dto.py` & `songtradr-api-client-python-1.12.22/test/test_playlist_large_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -37,60 +37,48 @@
         # uncomment below to create an instance of `PlaylistLargeDTO`
         """
         model = songtradr_api_client_python.models.playlist_large_dto.PlaylistLargeDTO()  # noqa: E501
         if include_optional :
             return PlaylistLargeDTO(
                 name = '', 
                 state = 'active', 
+                description = '', 
+                usages = [
+                    songtradr_api_client_python.models.usage_dto.UsageDTO(
+                        name = '', )
+                    ], 
                 created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 updated = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                description = '', 
-                asset_url = '', 
-                pretzel_tier = '', 
-                usage = '', 
+                songtradr_playlist_guid = '', 
                 tracks = [
                     songtradr_api_client_python.models.recording_playlist_dto.RecordingPlaylistDTO(
                         recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
-                            spotify_id = '', 
-                            genre_predictions = [
-                                songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                                    genre_type = '', 
-                                    genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                                        genre_name = '', ), 
-                                    probability = 1.337, )
-                                ], 
-                            tags = [
-                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                        id = 56, 
-                                        categories = [
-                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                                category_name = '', )
-                                            ], 
-                                        name = '', ), )
-                                ], 
-                            titles = [
-                                songtradr_api_client_python.models.title_dto.TitleDTO(
-                                    title_text = '', )
-                                ], 
                             musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                                 space = 'very compact', 
-                                primary_mood_cluster_affinity = 1.337, 
-                                secondary_mood_cluster = 'aggressive', 
-                                secondary_mood_cluster_affinity = 1.337, 
-                                tertiary_mood_cluster = 'aggressive', 
-                                tertiary_mood_cluster_affinity = 1.337, 
-                                vocals_affinity = 1.337, 
-                                dominant_instrument_affinity = 1.337, 
-                                secondary_instrument = 'electric guitar', 
-                                secondary_instrument_affinity = 1.337, 
-                                tertiary_instrument = 'electric guitar', 
-                                tertiary_instrument_affinity = 1.337, 
-                                sound_generation_affinity = 1.337, 
-                                rhythm_affinity = 1.337, 
+                                arousal = 'very calm', 
+                                dominant_instrument = 'electric guitar', 
+                                energy = 'very quiet', 
+                                engagement = 'very unengaging', 
+                                groovyness = 'very steady', 
+                                harmony = 'very dissonant', 
+                                pleasantness = 'very unpleasant', 
+                                primary_mood_cluster = 'aggressive', 
+                                primary_sound_character = 'brassy', 
+                                rhythm = 'common time', 
+                                roughness = 'very clear', 
+                                scale = 'major key', 
+                                sound_generation = 'acoustic', 
+                                tempo = 'very slow', 
+                                texture = 'very thin', 
+                                timbre = 'very warm', 
+                                tonality = 'monotonous', 
+                                valence = 'very sad', 
+                                vocals = 'instrumental', 
+                                origin_decade = 'pre-1950s', 
+                                language_of_performance = 'en', 
                                 primary_sound_character_affinity = 1.337, 
                                 tonality_affinity = 1.337, 
                                 bpm = 1.337, 
                                 production_rating = 'low production quality', 
                                 production_rating_affinity = 1.337, 
                                 performance_rating = 'low performance quality', 
                                 performance_rating_affinity = 1.337, 
@@ -114,38 +102,30 @@
                                 origin_decade_affinity = 1.337, 
                                 language_of_performance_affinity = 1.337, 
                                 curateability_affinity = 1.337, 
                                 use_case_affinity = 1.337, 
                                 industry_suitability = 'Automobiles and Parts', 
                                 industry_suitability_affinity = 1.337, 
                                 audience_region = 'Australia and New Zealand', 
-                                arousal = 'very calm', 
-                                dominant_instrument = 'electric guitar', 
-                                energy = 'very quiet', 
-                                engagement = 'very unengaging', 
-                                groovyness = 'very steady', 
-                                harmony = 'very dissonant', 
-                                pleasantness = 'very unpleasant', 
-                                primary_mood_cluster = 'aggressive', 
-                                language_of_performance = 'en', 
-                                primary_sound_character = 'brassy', 
-                                rhythm = 'common time', 
-                                roughness = 'very clear', 
-                                scale = 'major key', 
-                                sound_generation = 'acoustic', 
-                                tempo = 'very slow', 
-                                texture = 'very thin', 
-                                timbre = 'very warm', 
-                                tonality = 'monotonous', 
-                                valence = 'very sad', 
-                                vocals = 'instrumental', 
-                                origin_decade = 'pre-1950s', 
                                 curateability = 'curateable', 
                                 use_case = 'background', 
                                 channel_suitability = 'Spotify', 
+                                primary_mood_cluster_affinity = 1.337, 
+                                secondary_mood_cluster = 'aggressive', 
+                                secondary_mood_cluster_affinity = 1.337, 
+                                tertiary_mood_cluster = 'aggressive', 
+                                tertiary_mood_cluster_affinity = 1.337, 
+                                vocals_affinity = 1.337, 
+                                dominant_instrument_affinity = 1.337, 
+                                secondary_instrument = 'electric guitar', 
+                                secondary_instrument_affinity = 1.337, 
+                                tertiary_instrument = 'electric guitar', 
+                                tertiary_instrument_affinity = 1.337, 
+                                sound_generation_affinity = 1.337, 
+                                rhythm_affinity = 1.337, 
                                 valence_affinity = 1.337, 
                                 arousal_affinity = 1.337, 
                                 pleasantness_affinity = 1.337, 
                                 engagement_affinity = 1.337, 
                                 energy_affinity = 1.337, 
                                 tempo_affinity = 1.337, 
                                 scale_affinity = 1.337, 
@@ -154,41 +134,61 @@
                                 harmony_affinity = 1.337, 
                                 texture_affinity = 1.337, 
                                 groovyness_affinity = 1.337, 
                                 space_affinity = 1.337, 
                                 key_affinity = 1.337, 
                                 channel_suitability_affinity = 1.337, 
                                 key = 'C', ), 
+                            genre_predictions = [
+                                songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                                    genre_type = '', 
+                                    genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                                        genre_name = '', ), 
+                                    probability = 1.337, )
+                                ], 
                             recording_party_entities = [
                                 songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                        id = '', 
+                                        full_name = '', ), 
                                     contributor_types = [
                                         songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                             type_name = '', )
-                                        ], 
-                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                        id = '', 
-                                        full_name = '', ), )
+                                        ], )
                                 ], 
                             genres = [
                                 songtradr_api_client_python.models.genre_dto.GenreDTO(
                                     id = 56, 
                                     name = '', )
                                 ], 
                             language_of_performance = '', 
                             release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            isrc = '', ), 
-                        songtradr_track_guid = '', 
+                            titles = [
+                                songtradr_api_client_python.models.title_dto.TitleDTO(
+                                    title_text = '', )
+                                ], 
+                            isrc = '', 
+                            tags = [
+                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                        id = 56, 
+                                        name = '', 
+                                        categories = [
+                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                                category_name = '', )
+                                            ], ), )
+                                ], 
+                            spotify_id = '', ), 
                         assigned_by_id = 56, 
-                        sequence = 56, )
+                        sequence = 56, 
+                        songtradr_track_guid = '', )
                     ], 
-                songtradr_playlist_guid = '', 
-                usages = [
-                    songtradr_api_client_python.models.usage_dto.UsageDTO(
-                        name = '', )
-                    ]
+                asset_url = '', 
+                pretzel_tier = '', 
+                usage = ''
             )
         else :
             return PlaylistLargeDTO(
                 name = '',
         )
         """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_product_medium_dto.py` & `songtradr-api-client-python-1.12.22/test/test_product_medium_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,39 +36,39 @@
             optional params are included """
         # uncomment below to create an instance of `ProductMediumDTO`
         """
         model = songtradr_api_client_python.models.product_medium_dto.ProductMediumDTO()  # noqa: E501
         if include_optional :
             return ProductMediumDTO(
                 duration = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                parties = [
-                    songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
-                        contributor_types = [
-                            songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                type_name = '', )
-                            ], 
-                        party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                            id = '', 
-                            full_name = '', ), )
-                    ], 
-                grid = '', 
-                release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
                     year = 56, 
                     text = '', ), 
-                titles = [
-                    songtradr_api_client_python.models.title_dto.TitleDTO(
-                        title_text = '', )
-                    ], 
                 genres = [
                     songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                         genre_name = '', )
                     ], 
-                gtin = ''
+                titles = [
+                    songtradr_api_client_python.models.title_dto.TitleDTO(
+                        title_text = '', )
+                    ], 
+                gtin = '', 
+                grid = '', 
+                release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                parties = [
+                    songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
+                        party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                            id = '', 
+                            full_name = '', ), 
+                        contributor_types = [
+                            songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                type_name = '', )
+                            ], )
+                    ]
             )
         else :
             return ProductMediumDTO(
         )
         """
 
     def testProductMediumDTO(self):
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_product_party_dto.py` & `songtradr-api-client-python-1.12.22/test/test_product_party_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -35,21 +35,21 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `ProductPartyDTO`
         """
         model = songtradr_api_client_python.models.product_party_dto.ProductPartyDTO()  # noqa: E501
         if include_optional :
             return ProductPartyDTO(
+                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                    id = '', 
+                    full_name = '', ), 
                 contributor_types = [
                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                         type_name = '', )
-                    ], 
-                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                    id = '', 
-                    full_name = '', )
+                    ]
             )
         else :
             return ProductPartyDTO(
                 party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                     id = '', 
                     full_name = '', ),
         )
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_api.py` & `songtradr-api-client-python-1.12.22/test/test_recording_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_for_similarity_search_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_for_similarity_search_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -37,48 +37,48 @@
         # uncomment below to create an instance of `RecordingForSimilaritySearchDTO`
         """
         model = songtradr_api_client_python.models.recording_for_similarity_search_dto.RecordingForSimilaritySearchDTO()  # noqa: E501
         if include_optional :
             return RecordingForSimilaritySearchDTO(
                 recording = songtradr_api_client_python.models.recording_small_dto.RecordingSmallDTO(
                     duration = 56, 
-                    titles = [
-                        songtradr_api_client_python.models.title_dto.TitleDTO(
-                            title_text = '', )
-                        ], 
                     parties = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                id = '', 
+                                full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                     type_name = '', )
-                                ], 
-                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                id = '', 
-                                full_name = '', ), )
+                                ], )
+                        ], 
+                    titles = [
+                        songtradr_api_client_python.models.title_dto.TitleDTO(
+                            title_text = '', )
                         ], 
                     isrc = '', ), 
                 score = 1.337
             )
         else :
             return RecordingForSimilaritySearchDTO(
                 recording = songtradr_api_client_python.models.recording_small_dto.RecordingSmallDTO(
                     duration = 56, 
-                    titles = [
-                        songtradr_api_client_python.models.title_dto.TitleDTO(
-                            title_text = '', )
-                        ], 
                     parties = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                id = '', 
+                                full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                     type_name = '', )
-                                ], 
-                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                id = '', 
-                                full_name = '', ), )
+                                ], )
+                        ], 
+                    titles = [
+                        songtradr_api_client_python.models.title_dto.TitleDTO(
+                            title_text = '', )
                         ], 
                     isrc = '', ),
                 score = 1.337,
         )
         """
 
     def testRecordingForSimilaritySearchDTO(self):
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_genre_prediction_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_genre_prediction_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_large_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_large_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,86 +36,69 @@
             optional params are included """
         # uncomment below to create an instance of `RecordingLargeDTO`
         """
         model = songtradr_api_client_python.models.recording_large_dto.RecordingLargeDTO()  # noqa: E501
         if include_optional :
             return RecordingLargeDTO(
                 duration = 56, 
-                spotify_id = '', 
-                genre_predictions = [
-                    songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                        genre_type = '', 
-                        genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                            genre_name = '', ), 
-                        probability = 1.337, )
-                    ], 
-                pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
-                    year = 56, 
-                    text = '', ), 
-                tags = [
-                    songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                        tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                            id = 56, 
-                            categories = [
-                                songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                    category_name = '', )
-                                ], 
-                            name = '', ), )
-                    ], 
-                titles = [
-                    songtradr_api_client_python.models.title_dto.TitleDTO(
-                        title_text = '', )
-                    ], 
                 tracks = [
                     songtradr_api_client_python.models.track_to_medium_product_dto.TrackToMediumProductDTO(
                         track_no = '', 
                         set_no = '', 
                         product = songtradr_api_client_python.models.product_medium_dto.ProductMediumDTO(
                             duration = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            parties = [
-                                songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
-                                    contributor_types = [
-                                        songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                            type_name = '', )
-                                        ], 
-                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                        id = '', 
-                                        full_name = '', ), )
-                                ], 
-                            grid = '', 
-                            release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                             pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
                                 year = 56, 
                                 text = '', ), 
-                            titles = [
-                                songtradr_api_client_python.models.title_dto.TitleDTO(
-                                    title_text = '', )
-                                ], 
                             genres = [
                                 songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                                     genre_name = '', )
                                 ], 
-                            gtin = '', ), )
+                            titles = [
+                                songtradr_api_client_python.models.title_dto.TitleDTO(
+                                    title_text = '', )
+                                ], 
+                            gtin = '', 
+                            grid = '', 
+                            release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            parties = [
+                                songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
+                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                        id = '', 
+                                        full_name = '', ), 
+                                    contributor_types = [
+                                        songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                            type_name = '', )
+                                        ], )
+                                ], ), )
                     ], 
                 musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                     space = 'very compact', 
-                    primary_mood_cluster_affinity = 1.337, 
-                    secondary_mood_cluster = 'aggressive', 
-                    secondary_mood_cluster_affinity = 1.337, 
-                    tertiary_mood_cluster = 'aggressive', 
-                    tertiary_mood_cluster_affinity = 1.337, 
-                    vocals_affinity = 1.337, 
-                    dominant_instrument_affinity = 1.337, 
-                    secondary_instrument = 'electric guitar', 
-                    secondary_instrument_affinity = 1.337, 
-                    tertiary_instrument = 'electric guitar', 
-                    tertiary_instrument_affinity = 1.337, 
-                    sound_generation_affinity = 1.337, 
-                    rhythm_affinity = 1.337, 
+                    arousal = 'very calm', 
+                    dominant_instrument = 'electric guitar', 
+                    energy = 'very quiet', 
+                    engagement = 'very unengaging', 
+                    groovyness = 'very steady', 
+                    harmony = 'very dissonant', 
+                    pleasantness = 'very unpleasant', 
+                    primary_mood_cluster = 'aggressive', 
+                    primary_sound_character = 'brassy', 
+                    rhythm = 'common time', 
+                    roughness = 'very clear', 
+                    scale = 'major key', 
+                    sound_generation = 'acoustic', 
+                    tempo = 'very slow', 
+                    texture = 'very thin', 
+                    timbre = 'very warm', 
+                    tonality = 'monotonous', 
+                    valence = 'very sad', 
+                    vocals = 'instrumental', 
+                    origin_decade = 'pre-1950s', 
+                    language_of_performance = 'en', 
                     primary_sound_character_affinity = 1.337, 
                     tonality_affinity = 1.337, 
                     bpm = 1.337, 
                     production_rating = 'low production quality', 
                     production_rating_affinity = 1.337, 
                     performance_rating = 'low performance quality', 
                     performance_rating_affinity = 1.337, 
@@ -139,38 +122,30 @@
                     origin_decade_affinity = 1.337, 
                     language_of_performance_affinity = 1.337, 
                     curateability_affinity = 1.337, 
                     use_case_affinity = 1.337, 
                     industry_suitability = 'Automobiles and Parts', 
                     industry_suitability_affinity = 1.337, 
                     audience_region = 'Australia and New Zealand', 
-                    arousal = 'very calm', 
-                    dominant_instrument = 'electric guitar', 
-                    energy = 'very quiet', 
-                    engagement = 'very unengaging', 
-                    groovyness = 'very steady', 
-                    harmony = 'very dissonant', 
-                    pleasantness = 'very unpleasant', 
-                    primary_mood_cluster = 'aggressive', 
-                    language_of_performance = 'en', 
-                    primary_sound_character = 'brassy', 
-                    rhythm = 'common time', 
-                    roughness = 'very clear', 
-                    scale = 'major key', 
-                    sound_generation = 'acoustic', 
-                    tempo = 'very slow', 
-                    texture = 'very thin', 
-                    timbre = 'very warm', 
-                    tonality = 'monotonous', 
-                    valence = 'very sad', 
-                    vocals = 'instrumental', 
-                    origin_decade = 'pre-1950s', 
                     curateability = 'curateable', 
                     use_case = 'background', 
                     channel_suitability = 'Spotify', 
+                    primary_mood_cluster_affinity = 1.337, 
+                    secondary_mood_cluster = 'aggressive', 
+                    secondary_mood_cluster_affinity = 1.337, 
+                    tertiary_mood_cluster = 'aggressive', 
+                    tertiary_mood_cluster_affinity = 1.337, 
+                    vocals_affinity = 1.337, 
+                    dominant_instrument_affinity = 1.337, 
+                    secondary_instrument = 'electric guitar', 
+                    secondary_instrument_affinity = 1.337, 
+                    tertiary_instrument = 'electric guitar', 
+                    tertiary_instrument_affinity = 1.337, 
+                    sound_generation_affinity = 1.337, 
+                    rhythm_affinity = 1.337, 
                     valence_affinity = 1.337, 
                     arousal_affinity = 1.337, 
                     pleasantness_affinity = 1.337, 
                     engagement_affinity = 1.337, 
                     energy_affinity = 1.337, 
                     tempo_affinity = 1.337, 
                     scale_affinity = 1.337, 
@@ -179,31 +154,56 @@
                     harmony_affinity = 1.337, 
                     texture_affinity = 1.337, 
                     groovyness_affinity = 1.337, 
                     space_affinity = 1.337, 
                     key_affinity = 1.337, 
                     channel_suitability_affinity = 1.337, 
                     key = 'C', ), 
+                pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
+                    year = 56, 
+                    text = '', ), 
+                genre_predictions = [
+                    songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                        genre_type = '', 
+                        genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                            genre_name = '', ), 
+                        probability = 1.337, )
+                    ], 
                 parties = [
                     songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                        party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                            id = '', 
+                            full_name = '', ), 
                         contributor_types = [
                             songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                 type_name = '', )
-                            ], 
-                        party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                            id = '', 
-                            full_name = '', ), )
+                            ], )
                     ], 
                 genres = [
                     songtradr_api_client_python.models.genre_dto.GenreDTO(
                         id = 56, 
                         name = '', )
                     ], 
                 language_of_performance = '', 
-                isrc = ''
+                titles = [
+                    songtradr_api_client_python.models.title_dto.TitleDTO(
+                        title_text = '', )
+                    ], 
+                isrc = '', 
+                tags = [
+                    songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                        tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                            id = 56, 
+                            name = '', 
+                            categories = [
+                                songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                    category_name = '', )
+                                ], ), )
+                    ], 
+                spotify_id = ''
             )
         else :
             return RecordingLargeDTO(
                 isrc = '',
         )
         """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_list_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_list_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -37,51 +37,37 @@
         # uncomment below to create an instance of `RecordingListDTO`
         """
         model = songtradr_api_client_python.models.recording_list_dto.RecordingListDTO()  # noqa: E501
         if include_optional :
             return RecordingListDTO(
                 recordings = [
                     songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
-                        spotify_id = '', 
-                        genre_predictions = [
-                            songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                                genre_type = '', 
-                                genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                                    genre_name = '', ), 
-                                probability = 1.337, )
-                            ], 
-                        tags = [
-                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                    id = 56, 
-                                    categories = [
-                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                            category_name = '', )
-                                        ], 
-                                    name = '', ), )
-                            ], 
-                        titles = [
-                            songtradr_api_client_python.models.title_dto.TitleDTO(
-                                title_text = '', )
-                            ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            primary_mood_cluster_affinity = 1.337, 
-                            secondary_mood_cluster = 'aggressive', 
-                            secondary_mood_cluster_affinity = 1.337, 
-                            tertiary_mood_cluster = 'aggressive', 
-                            tertiary_mood_cluster_affinity = 1.337, 
-                            vocals_affinity = 1.337, 
-                            dominant_instrument_affinity = 1.337, 
-                            secondary_instrument = 'electric guitar', 
-                            secondary_instrument_affinity = 1.337, 
-                            tertiary_instrument = 'electric guitar', 
-                            tertiary_instrument_affinity = 1.337, 
-                            sound_generation_affinity = 1.337, 
-                            rhythm_affinity = 1.337, 
+                            arousal = 'very calm', 
+                            dominant_instrument = 'electric guitar', 
+                            energy = 'very quiet', 
+                            engagement = 'very unengaging', 
+                            groovyness = 'very steady', 
+                            harmony = 'very dissonant', 
+                            pleasantness = 'very unpleasant', 
+                            primary_mood_cluster = 'aggressive', 
+                            primary_sound_character = 'brassy', 
+                            rhythm = 'common time', 
+                            roughness = 'very clear', 
+                            scale = 'major key', 
+                            sound_generation = 'acoustic', 
+                            tempo = 'very slow', 
+                            texture = 'very thin', 
+                            timbre = 'very warm', 
+                            tonality = 'monotonous', 
+                            valence = 'very sad', 
+                            vocals = 'instrumental', 
+                            origin_decade = 'pre-1950s', 
+                            language_of_performance = 'en', 
                             primary_sound_character_affinity = 1.337, 
                             tonality_affinity = 1.337, 
                             bpm = 1.337, 
                             production_rating = 'low production quality', 
                             production_rating_affinity = 1.337, 
                             performance_rating = 'low performance quality', 
                             performance_rating_affinity = 1.337, 
@@ -105,38 +91,30 @@
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', 
-                            arousal = 'very calm', 
-                            dominant_instrument = 'electric guitar', 
-                            energy = 'very quiet', 
-                            engagement = 'very unengaging', 
-                            groovyness = 'very steady', 
-                            harmony = 'very dissonant', 
-                            pleasantness = 'very unpleasant', 
-                            primary_mood_cluster = 'aggressive', 
-                            language_of_performance = 'en', 
-                            primary_sound_character = 'brassy', 
-                            rhythm = 'common time', 
-                            roughness = 'very clear', 
-                            scale = 'major key', 
-                            sound_generation = 'acoustic', 
-                            tempo = 'very slow', 
-                            texture = 'very thin', 
-                            timbre = 'very warm', 
-                            tonality = 'monotonous', 
-                            valence = 'very sad', 
-                            vocals = 'instrumental', 
-                            origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            primary_mood_cluster_affinity = 1.337, 
+                            secondary_mood_cluster = 'aggressive', 
+                            secondary_mood_cluster_affinity = 1.337, 
+                            tertiary_mood_cluster = 'aggressive', 
+                            tertiary_mood_cluster_affinity = 1.337, 
+                            vocals_affinity = 1.337, 
+                            dominant_instrument_affinity = 1.337, 
+                            secondary_instrument = 'electric guitar', 
+                            secondary_instrument_affinity = 1.337, 
+                            tertiary_instrument = 'electric guitar', 
+                            tertiary_instrument_affinity = 1.337, 
+                            sound_generation_affinity = 1.337, 
+                            rhythm_affinity = 1.337, 
                             valence_affinity = 1.337, 
                             arousal_affinity = 1.337, 
                             pleasantness_affinity = 1.337, 
                             engagement_affinity = 1.337, 
                             energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
@@ -145,78 +123,86 @@
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
                             key = 'C', ), 
+                        genre_predictions = [
+                            songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                                genre_type = '', 
+                                genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                                    genre_name = '', ), 
+                                probability = 1.337, )
+                            ], 
                         recording_party_entities = [
                             songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                    id = '', 
+                                    full_name = '', ), 
                                 contributor_types = [
                                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                         type_name = '', )
-                                    ], 
-                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                    id = '', 
-                                    full_name = '', ), )
+                                    ], )
                             ], 
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        isrc = '', )
-                    ], 
-                has_next_page = True, 
-                current_page_number = 56, 
-                total_results = 56
-            )
-        else :
-            return RecordingListDTO(
-                recordings = [
-                    songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
-                        spotify_id = '', 
-                        genre_predictions = [
-                            songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                                genre_type = '', 
-                                genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                                    genre_name = '', ), 
-                                probability = 1.337, )
+                        titles = [
+                            songtradr_api_client_python.models.title_dto.TitleDTO(
+                                title_text = '', )
                             ], 
+                        isrc = '', 
                         tags = [
                             songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                 tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                     id = 56, 
+                                    name = '', 
                                     categories = [
                                         songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
                                             category_name = '', )
-                                        ], 
-                                    name = '', ), )
-                            ], 
-                        titles = [
-                            songtradr_api_client_python.models.title_dto.TitleDTO(
-                                title_text = '', )
+                                        ], ), )
                             ], 
+                        spotify_id = '', )
+                    ], 
+                has_next_page = True, 
+                current_page_number = 56, 
+                total_results = 56
+            )
+        else :
+            return RecordingListDTO(
+                recordings = [
+                    songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            primary_mood_cluster_affinity = 1.337, 
-                            secondary_mood_cluster = 'aggressive', 
-                            secondary_mood_cluster_affinity = 1.337, 
-                            tertiary_mood_cluster = 'aggressive', 
-                            tertiary_mood_cluster_affinity = 1.337, 
-                            vocals_affinity = 1.337, 
-                            dominant_instrument_affinity = 1.337, 
-                            secondary_instrument = 'electric guitar', 
-                            secondary_instrument_affinity = 1.337, 
-                            tertiary_instrument = 'electric guitar', 
-                            tertiary_instrument_affinity = 1.337, 
-                            sound_generation_affinity = 1.337, 
-                            rhythm_affinity = 1.337, 
+                            arousal = 'very calm', 
+                            dominant_instrument = 'electric guitar', 
+                            energy = 'very quiet', 
+                            engagement = 'very unengaging', 
+                            groovyness = 'very steady', 
+                            harmony = 'very dissonant', 
+                            pleasantness = 'very unpleasant', 
+                            primary_mood_cluster = 'aggressive', 
+                            primary_sound_character = 'brassy', 
+                            rhythm = 'common time', 
+                            roughness = 'very clear', 
+                            scale = 'major key', 
+                            sound_generation = 'acoustic', 
+                            tempo = 'very slow', 
+                            texture = 'very thin', 
+                            timbre = 'very warm', 
+                            tonality = 'monotonous', 
+                            valence = 'very sad', 
+                            vocals = 'instrumental', 
+                            origin_decade = 'pre-1950s', 
+                            language_of_performance = 'en', 
                             primary_sound_character_affinity = 1.337, 
                             tonality_affinity = 1.337, 
                             bpm = 1.337, 
                             production_rating = 'low production quality', 
                             production_rating_affinity = 1.337, 
                             performance_rating = 'low performance quality', 
                             performance_rating_affinity = 1.337, 
@@ -240,38 +226,30 @@
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', 
-                            arousal = 'very calm', 
-                            dominant_instrument = 'electric guitar', 
-                            energy = 'very quiet', 
-                            engagement = 'very unengaging', 
-                            groovyness = 'very steady', 
-                            harmony = 'very dissonant', 
-                            pleasantness = 'very unpleasant', 
-                            primary_mood_cluster = 'aggressive', 
-                            language_of_performance = 'en', 
-                            primary_sound_character = 'brassy', 
-                            rhythm = 'common time', 
-                            roughness = 'very clear', 
-                            scale = 'major key', 
-                            sound_generation = 'acoustic', 
-                            tempo = 'very slow', 
-                            texture = 'very thin', 
-                            timbre = 'very warm', 
-                            tonality = 'monotonous', 
-                            valence = 'very sad', 
-                            vocals = 'instrumental', 
-                            origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            primary_mood_cluster_affinity = 1.337, 
+                            secondary_mood_cluster = 'aggressive', 
+                            secondary_mood_cluster_affinity = 1.337, 
+                            tertiary_mood_cluster = 'aggressive', 
+                            tertiary_mood_cluster_affinity = 1.337, 
+                            vocals_affinity = 1.337, 
+                            dominant_instrument_affinity = 1.337, 
+                            secondary_instrument = 'electric guitar', 
+                            secondary_instrument_affinity = 1.337, 
+                            tertiary_instrument = 'electric guitar', 
+                            tertiary_instrument_affinity = 1.337, 
+                            sound_generation_affinity = 1.337, 
+                            rhythm_affinity = 1.337, 
                             valence_affinity = 1.337, 
                             arousal_affinity = 1.337, 
                             pleasantness_affinity = 1.337, 
                             engagement_affinity = 1.337, 
                             energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
@@ -280,32 +258,54 @@
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
                             key = 'C', ), 
+                        genre_predictions = [
+                            songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                                genre_type = '', 
+                                genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                                    genre_name = '', ), 
+                                probability = 1.337, )
+                            ], 
                         recording_party_entities = [
                             songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                    id = '', 
+                                    full_name = '', ), 
                                 contributor_types = [
                                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                         type_name = '', )
-                                    ], 
-                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                    id = '', 
-                                    full_name = '', ), )
+                                    ], )
                             ], 
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        isrc = '', )
+                        titles = [
+                            songtradr_api_client_python.models.title_dto.TitleDTO(
+                                title_text = '', )
+                            ], 
+                        isrc = '', 
+                        tags = [
+                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                    id = 56, 
+                                    name = '', 
+                                    categories = [
+                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                            category_name = '', )
+                                        ], ), )
+                            ], 
+                        spotify_id = '', )
                     ],
                 has_next_page = True,
                 current_page_number = 56,
                 total_results = 56,
         )
         """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_medium_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_medium_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -35,51 +35,37 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `RecordingMediumDTO`
         """
         model = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO()  # noqa: E501
         if include_optional :
             return RecordingMediumDTO(
-                spotify_id = '', 
-                genre_predictions = [
-                    songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                        genre_type = '', 
-                        genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                            genre_name = '', ), 
-                        probability = 1.337, )
-                    ], 
-                tags = [
-                    songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                        tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                            id = 56, 
-                            categories = [
-                                songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                    category_name = '', )
-                                ], 
-                            name = '', ), )
-                    ], 
-                titles = [
-                    songtradr_api_client_python.models.title_dto.TitleDTO(
-                        title_text = '', )
-                    ], 
                 musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                     space = 'very compact', 
-                    primary_mood_cluster_affinity = 1.337, 
-                    secondary_mood_cluster = 'aggressive', 
-                    secondary_mood_cluster_affinity = 1.337, 
-                    tertiary_mood_cluster = 'aggressive', 
-                    tertiary_mood_cluster_affinity = 1.337, 
-                    vocals_affinity = 1.337, 
-                    dominant_instrument_affinity = 1.337, 
-                    secondary_instrument = 'electric guitar', 
-                    secondary_instrument_affinity = 1.337, 
-                    tertiary_instrument = 'electric guitar', 
-                    tertiary_instrument_affinity = 1.337, 
-                    sound_generation_affinity = 1.337, 
-                    rhythm_affinity = 1.337, 
+                    arousal = 'very calm', 
+                    dominant_instrument = 'electric guitar', 
+                    energy = 'very quiet', 
+                    engagement = 'very unengaging', 
+                    groovyness = 'very steady', 
+                    harmony = 'very dissonant', 
+                    pleasantness = 'very unpleasant', 
+                    primary_mood_cluster = 'aggressive', 
+                    primary_sound_character = 'brassy', 
+                    rhythm = 'common time', 
+                    roughness = 'very clear', 
+                    scale = 'major key', 
+                    sound_generation = 'acoustic', 
+                    tempo = 'very slow', 
+                    texture = 'very thin', 
+                    timbre = 'very warm', 
+                    tonality = 'monotonous', 
+                    valence = 'very sad', 
+                    vocals = 'instrumental', 
+                    origin_decade = 'pre-1950s', 
+                    language_of_performance = 'en', 
                     primary_sound_character_affinity = 1.337, 
                     tonality_affinity = 1.337, 
                     bpm = 1.337, 
                     production_rating = 'low production quality', 
                     production_rating_affinity = 1.337, 
                     performance_rating = 'low performance quality', 
                     performance_rating_affinity = 1.337, 
@@ -103,38 +89,30 @@
                     origin_decade_affinity = 1.337, 
                     language_of_performance_affinity = 1.337, 
                     curateability_affinity = 1.337, 
                     use_case_affinity = 1.337, 
                     industry_suitability = 'Automobiles and Parts', 
                     industry_suitability_affinity = 1.337, 
                     audience_region = 'Australia and New Zealand', 
-                    arousal = 'very calm', 
-                    dominant_instrument = 'electric guitar', 
-                    energy = 'very quiet', 
-                    engagement = 'very unengaging', 
-                    groovyness = 'very steady', 
-                    harmony = 'very dissonant', 
-                    pleasantness = 'very unpleasant', 
-                    primary_mood_cluster = 'aggressive', 
-                    language_of_performance = 'en', 
-                    primary_sound_character = 'brassy', 
-                    rhythm = 'common time', 
-                    roughness = 'very clear', 
-                    scale = 'major key', 
-                    sound_generation = 'acoustic', 
-                    tempo = 'very slow', 
-                    texture = 'very thin', 
-                    timbre = 'very warm', 
-                    tonality = 'monotonous', 
-                    valence = 'very sad', 
-                    vocals = 'instrumental', 
-                    origin_decade = 'pre-1950s', 
                     curateability = 'curateable', 
                     use_case = 'background', 
                     channel_suitability = 'Spotify', 
+                    primary_mood_cluster_affinity = 1.337, 
+                    secondary_mood_cluster = 'aggressive', 
+                    secondary_mood_cluster_affinity = 1.337, 
+                    tertiary_mood_cluster = 'aggressive', 
+                    tertiary_mood_cluster_affinity = 1.337, 
+                    vocals_affinity = 1.337, 
+                    dominant_instrument_affinity = 1.337, 
+                    secondary_instrument = 'electric guitar', 
+                    secondary_instrument_affinity = 1.337, 
+                    tertiary_instrument = 'electric guitar', 
+                    tertiary_instrument_affinity = 1.337, 
+                    sound_generation_affinity = 1.337, 
+                    rhythm_affinity = 1.337, 
                     valence_affinity = 1.337, 
                     arousal_affinity = 1.337, 
                     pleasantness_affinity = 1.337, 
                     engagement_affinity = 1.337, 
                     energy_affinity = 1.337, 
                     tempo_affinity = 1.337, 
                     scale_affinity = 1.337, 
@@ -143,32 +121,54 @@
                     harmony_affinity = 1.337, 
                     texture_affinity = 1.337, 
                     groovyness_affinity = 1.337, 
                     space_affinity = 1.337, 
                     key_affinity = 1.337, 
                     channel_suitability_affinity = 1.337, 
                     key = 'C', ), 
+                genre_predictions = [
+                    songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                        genre_type = '', 
+                        genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                            genre_name = '', ), 
+                        probability = 1.337, )
+                    ], 
                 recording_party_entities = [
                     songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                        party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                            id = '', 
+                            full_name = '', ), 
                         contributor_types = [
                             songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                 type_name = '', )
-                            ], 
-                        party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                            id = '', 
-                            full_name = '', ), )
+                            ], )
                     ], 
                 genres = [
                     songtradr_api_client_python.models.genre_dto.GenreDTO(
                         id = 56, 
                         name = '', )
                     ], 
                 language_of_performance = '', 
                 release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                isrc = ''
+                titles = [
+                    songtradr_api_client_python.models.title_dto.TitleDTO(
+                        title_text = '', )
+                    ], 
+                isrc = '', 
+                tags = [
+                    songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                        tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                            id = 56, 
+                            name = '', 
+                            categories = [
+                                songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                    category_name = '', )
+                                ], ), )
+                    ], 
+                spotify_id = ''
             )
         else :
             return RecordingMediumDTO(
                 isrc = '',
         )
         """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_minimal_with_musical_features_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_minimal_with_musical_features_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -38,27 +38,35 @@
         """
         model = songtradr_api_client_python.models.recording_minimal_with_musical_features_dto.RecordingMinimalWithMusicalFeaturesDTO()  # noqa: E501
         if include_optional :
             return RecordingMinimalWithMusicalFeaturesDTO(
                 musical_features = [
                     songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                         space = 'very compact', 
-                        primary_mood_cluster_affinity = 1.337, 
-                        secondary_mood_cluster = 'aggressive', 
-                        secondary_mood_cluster_affinity = 1.337, 
-                        tertiary_mood_cluster = 'aggressive', 
-                        tertiary_mood_cluster_affinity = 1.337, 
-                        vocals_affinity = 1.337, 
-                        dominant_instrument_affinity = 1.337, 
-                        secondary_instrument = 'electric guitar', 
-                        secondary_instrument_affinity = 1.337, 
-                        tertiary_instrument = 'electric guitar', 
-                        tertiary_instrument_affinity = 1.337, 
-                        sound_generation_affinity = 1.337, 
-                        rhythm_affinity = 1.337, 
+                        arousal = 'very calm', 
+                        dominant_instrument = 'electric guitar', 
+                        energy = 'very quiet', 
+                        engagement = 'very unengaging', 
+                        groovyness = 'very steady', 
+                        harmony = 'very dissonant', 
+                        pleasantness = 'very unpleasant', 
+                        primary_mood_cluster = 'aggressive', 
+                        primary_sound_character = 'brassy', 
+                        rhythm = 'common time', 
+                        roughness = 'very clear', 
+                        scale = 'major key', 
+                        sound_generation = 'acoustic', 
+                        tempo = 'very slow', 
+                        texture = 'very thin', 
+                        timbre = 'very warm', 
+                        tonality = 'monotonous', 
+                        valence = 'very sad', 
+                        vocals = 'instrumental', 
+                        origin_decade = 'pre-1950s', 
+                        language_of_performance = 'en', 
                         primary_sound_character_affinity = 1.337, 
                         tonality_affinity = 1.337, 
                         bpm = 1.337, 
                         production_rating = 'low production quality', 
                         production_rating_affinity = 1.337, 
                         performance_rating = 'low performance quality', 
                         performance_rating_affinity = 1.337, 
@@ -82,38 +90,30 @@
                         origin_decade_affinity = 1.337, 
                         language_of_performance_affinity = 1.337, 
                         curateability_affinity = 1.337, 
                         use_case_affinity = 1.337, 
                         industry_suitability = 'Automobiles and Parts', 
                         industry_suitability_affinity = 1.337, 
                         audience_region = 'Australia and New Zealand', 
-                        arousal = 'very calm', 
-                        dominant_instrument = 'electric guitar', 
-                        energy = 'very quiet', 
-                        engagement = 'very unengaging', 
-                        groovyness = 'very steady', 
-                        harmony = 'very dissonant', 
-                        pleasantness = 'very unpleasant', 
-                        primary_mood_cluster = 'aggressive', 
-                        language_of_performance = 'en', 
-                        primary_sound_character = 'brassy', 
-                        rhythm = 'common time', 
-                        roughness = 'very clear', 
-                        scale = 'major key', 
-                        sound_generation = 'acoustic', 
-                        tempo = 'very slow', 
-                        texture = 'very thin', 
-                        timbre = 'very warm', 
-                        tonality = 'monotonous', 
-                        valence = 'very sad', 
-                        vocals = 'instrumental', 
-                        origin_decade = 'pre-1950s', 
                         curateability = 'curateable', 
                         use_case = 'background', 
                         channel_suitability = 'Spotify', 
+                        primary_mood_cluster_affinity = 1.337, 
+                        secondary_mood_cluster = 'aggressive', 
+                        secondary_mood_cluster_affinity = 1.337, 
+                        tertiary_mood_cluster = 'aggressive', 
+                        tertiary_mood_cluster_affinity = 1.337, 
+                        vocals_affinity = 1.337, 
+                        dominant_instrument_affinity = 1.337, 
+                        secondary_instrument = 'electric guitar', 
+                        secondary_instrument_affinity = 1.337, 
+                        tertiary_instrument = 'electric guitar', 
+                        tertiary_instrument_affinity = 1.337, 
+                        sound_generation_affinity = 1.337, 
+                        rhythm_affinity = 1.337, 
                         valence_affinity = 1.337, 
                         arousal_affinity = 1.337, 
                         pleasantness_affinity = 1.337, 
                         engagement_affinity = 1.337, 
                         energy_affinity = 1.337, 
                         tempo_affinity = 1.337, 
                         scale_affinity = 1.337,
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_minimal_with_taggrams_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_minimal_with_taggrams_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_minimal_with_tagstrengths_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_minimal_with_tagstrengths_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_party_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_party_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -35,21 +35,21 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `RecordingPartyDTO`
         """
         model = songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO()  # noqa: E501
         if include_optional :
             return RecordingPartyDTO(
+                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                    id = '', 
+                    full_name = '', ), 
                 contributor_types = [
                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                         type_name = '', )
-                    ], 
-                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                    id = '', 
-                    full_name = '', )
+                    ]
             )
         else :
             return RecordingPartyDTO(
                 party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                     id = '', 
                     full_name = '', ),
         )
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_playlist_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_playlist_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,51 +36,37 @@
             optional params are included """
         # uncomment below to create an instance of `RecordingPlaylistDTO`
         """
         model = songtradr_api_client_python.models.recording_playlist_dto.RecordingPlaylistDTO()  # noqa: E501
         if include_optional :
             return RecordingPlaylistDTO(
                 recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
-                    spotify_id = '', 
-                    genre_predictions = [
-                        songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
-                            genre_type = '', 
-                            genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
-                                genre_name = '', ), 
-                            probability = 1.337, )
-                        ], 
-                    tags = [
-                        songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                            tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                id = 56, 
-                                categories = [
-                                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                        category_name = '', )
-                                    ], 
-                                name = '', ), )
-                        ], 
-                    titles = [
-                        songtradr_api_client_python.models.title_dto.TitleDTO(
-                            title_text = '', )
-                        ], 
                     musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                         space = 'very compact', 
-                        primary_mood_cluster_affinity = 1.337, 
-                        secondary_mood_cluster = 'aggressive', 
-                        secondary_mood_cluster_affinity = 1.337, 
-                        tertiary_mood_cluster = 'aggressive', 
-                        tertiary_mood_cluster_affinity = 1.337, 
-                        vocals_affinity = 1.337, 
-                        dominant_instrument_affinity = 1.337, 
-                        secondary_instrument = 'electric guitar', 
-                        secondary_instrument_affinity = 1.337, 
-                        tertiary_instrument = 'electric guitar', 
-                        tertiary_instrument_affinity = 1.337, 
-                        sound_generation_affinity = 1.337, 
-                        rhythm_affinity = 1.337, 
+                        arousal = 'very calm', 
+                        dominant_instrument = 'electric guitar', 
+                        energy = 'very quiet', 
+                        engagement = 'very unengaging', 
+                        groovyness = 'very steady', 
+                        harmony = 'very dissonant', 
+                        pleasantness = 'very unpleasant', 
+                        primary_mood_cluster = 'aggressive', 
+                        primary_sound_character = 'brassy', 
+                        rhythm = 'common time', 
+                        roughness = 'very clear', 
+                        scale = 'major key', 
+                        sound_generation = 'acoustic', 
+                        tempo = 'very slow', 
+                        texture = 'very thin', 
+                        timbre = 'very warm', 
+                        tonality = 'monotonous', 
+                        valence = 'very sad', 
+                        vocals = 'instrumental', 
+                        origin_decade = 'pre-1950s', 
+                        language_of_performance = 'en', 
                         primary_sound_character_affinity = 1.337, 
                         tonality_affinity = 1.337, 
                         bpm = 1.337, 
                         production_rating = 'low production quality', 
                         production_rating_affinity = 1.337, 
                         performance_rating = 'low performance quality', 
                         performance_rating_affinity = 1.337, 
@@ -104,38 +90,30 @@
                         origin_decade_affinity = 1.337, 
                         language_of_performance_affinity = 1.337, 
                         curateability_affinity = 1.337, 
                         use_case_affinity = 1.337, 
                         industry_suitability = 'Automobiles and Parts', 
                         industry_suitability_affinity = 1.337, 
                         audience_region = 'Australia and New Zealand', 
-                        arousal = 'very calm', 
-                        dominant_instrument = 'electric guitar', 
-                        energy = 'very quiet', 
-                        engagement = 'very unengaging', 
-                        groovyness = 'very steady', 
-                        harmony = 'very dissonant', 
-                        pleasantness = 'very unpleasant', 
-                        primary_mood_cluster = 'aggressive', 
-                        language_of_performance = 'en', 
-                        primary_sound_character = 'brassy', 
-                        rhythm = 'common time', 
-                        roughness = 'very clear', 
-                        scale = 'major key', 
-                        sound_generation = 'acoustic', 
-                        tempo = 'very slow', 
-                        texture = 'very thin', 
-                        timbre = 'very warm', 
-                        tonality = 'monotonous', 
-                        valence = 'very sad', 
-                        vocals = 'instrumental', 
-                        origin_decade = 'pre-1950s', 
                         curateability = 'curateable', 
                         use_case = 'background', 
                         channel_suitability = 'Spotify', 
+                        primary_mood_cluster_affinity = 1.337, 
+                        secondary_mood_cluster = 'aggressive', 
+                        secondary_mood_cluster_affinity = 1.337, 
+                        tertiary_mood_cluster = 'aggressive', 
+                        tertiary_mood_cluster_affinity = 1.337, 
+                        vocals_affinity = 1.337, 
+                        dominant_instrument_affinity = 1.337, 
+                        secondary_instrument = 'electric guitar', 
+                        secondary_instrument_affinity = 1.337, 
+                        tertiary_instrument = 'electric guitar', 
+                        tertiary_instrument_affinity = 1.337, 
+                        sound_generation_affinity = 1.337, 
+                        rhythm_affinity = 1.337, 
                         valence_affinity = 1.337, 
                         arousal_affinity = 1.337, 
                         pleasantness_affinity = 1.337, 
                         engagement_affinity = 1.337, 
                         energy_affinity = 1.337, 
                         tempo_affinity = 1.337, 
                         scale_affinity = 1.337, 
@@ -144,35 +122,57 @@
                         harmony_affinity = 1.337, 
                         texture_affinity = 1.337, 
                         groovyness_affinity = 1.337, 
                         space_affinity = 1.337, 
                         key_affinity = 1.337, 
                         channel_suitability_affinity = 1.337, 
                         key = 'C', ), 
+                    genre_predictions = [
+                        songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
+                            genre_type = '', 
+                            genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
+                                genre_name = '', ), 
+                            probability = 1.337, )
+                        ], 
                     recording_party_entities = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                id = '', 
+                                full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                     type_name = '', )
-                                ], 
-                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                id = '', 
-                                full_name = '', ), )
+                                ], )
                         ], 
                     genres = [
                         songtradr_api_client_python.models.genre_dto.GenreDTO(
                             id = 56, 
                             name = '', )
                         ], 
                     language_of_performance = '', 
                     release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    isrc = '', ), 
-                songtradr_track_guid = '', 
+                    titles = [
+                        songtradr_api_client_python.models.title_dto.TitleDTO(
+                            title_text = '', )
+                        ], 
+                    isrc = '', 
+                    tags = [
+                        songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                            tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                id = 56, 
+                                name = '', 
+                                categories = [
+                                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                        category_name = '', )
+                                    ], ), )
+                        ], 
+                    spotify_id = '', ), 
                 assigned_by_id = 56, 
-                sequence = 56
+                sequence = 56, 
+                songtradr_track_guid = ''
             )
         else :
             return RecordingPlaylistDTO(
         )
         """
 
     def testRecordingPlaylistDTO(self):
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_small_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,27 +36,27 @@
             optional params are included """
         # uncomment below to create an instance of `RecordingSmallDTO`
         """
         model = songtradr_api_client_python.models.recording_small_dto.RecordingSmallDTO()  # noqa: E501
         if include_optional :
             return RecordingSmallDTO(
                 duration = 56, 
-                titles = [
-                    songtradr_api_client_python.models.title_dto.TitleDTO(
-                        title_text = '', )
-                    ], 
                 parties = [
                     songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                        party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                            id = '', 
+                            full_name = '', ), 
                         contributor_types = [
                             songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                 type_name = '', )
-                            ], 
-                        party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                            id = '', 
-                            full_name = '', ), )
+                            ], )
+                    ], 
+                titles = [
+                    songtradr_api_client_python.models.title_dto.TitleDTO(
+                        title_text = '', )
                     ], 
                 isrc = ''
             )
         else :
             return RecordingSmallDTO(
                 isrc = '',
         )
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_recording_tag_small_dto.py` & `songtradr-api-client-python-1.12.22/test/test_recording_tag_small_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -37,29 +37,29 @@
         # uncomment below to create an instance of `RecordingTagSmallDTO`
         """
         model = songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO()  # noqa: E501
         if include_optional :
             return RecordingTagSmallDTO(
                 tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                     id = 56, 
+                    name = '', 
                     categories = [
                         songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
                             category_name = '', )
-                        ], 
-                    name = '', )
+                        ], )
             )
         else :
             return RecordingTagSmallDTO(
                 tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                     id = 56, 
+                    name = '', 
                     categories = [
                         songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
                             category_name = '', )
-                        ], 
-                    name = '', ),
+                        ], ),
         )
         """
 
     def testRecordingTagSmallDTO(self):
         """Test RecordingTagSmallDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_save_file_recording_dto.py` & `songtradr-api-client-python-1.12.22/test/test_save_file_recording_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_save_playlist_dto.py` & `songtradr-api-client-python-1.12.22/test/test_save_playlist_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_save_recording_genre_dto.py` & `songtradr-api-client-python-1.12.22/test/test_save_recording_genre_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_save_recording_party_dto.py` & `songtradr-api-client-python-1.12.22/test/test_save_recording_party_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_save_recording_playlist_dto.py` & `songtradr-api-client-python-1.12.22/test/test_save_recording_playlist_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_save_recording_tag_dto.py` & `songtradr-api-client-python-1.12.22/test/test_save_recording_tag_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_save_referrer_dto.py` & `songtradr-api-client-python-1.12.22/test/test_save_referrer_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_save_taggrams_dto.py` & `songtradr-api-client-python-1.12.22/test/test_save_taggrams_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_save_user_dto.py` & `songtradr-api-client-python-1.12.22/test/test_save_user_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_search_filter_values_dto.py` & `songtradr-api-client-python-1.12.22/test/test_search_filter_values_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_search_recording_granular_abstraction_dto.py` & `songtradr-api-client-python-1.12.22/test/test_search_recording_granular_abstraction_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_search_recording_granular_dto.py` & `songtradr-api-client-python-1.12.22/test/test_search_recording_granular_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_sign_up_dto.py` & `songtradr-api-client-python-1.12.22/test/test_sign_up_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_tag_dto.py` & `songtradr-api-client-python-1.12.22/test/test_tag_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,19 +36,19 @@
             optional params are included """
         # uncomment below to create an instance of `TagDTO`
         """
         model = songtradr_api_client_python.models.tag_dto.TagDTO()  # noqa: E501
         if include_optional :
             return TagDTO(
                 id = 56, 
+                name = '', 
                 categories = [
                     songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
                         category_name = '', )
-                    ], 
-                name = ''
+                    ]
             )
         else :
             return TagDTO(
                 id = 56,
                 name = '',
         )
         """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_tag_small_dto.py` & `songtradr-api-client-python-1.12.22/test/test_tag_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_taggram_dto.py` & `songtradr-api-client-python-1.12.22/test/test_taggram_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_tags_summary_dto.py` & `songtradr-api-client-python-1.12.22/test/test_tags_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_tagstrength_dto.py` & `songtradr-api-client-python-1.12.22/test/test_tagstrength_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_title_dto.py` & `songtradr-api-client-python-1.12.22/test/test_title_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_token_request.py` & `songtradr-api-client-python-1.12.22/test/test_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_track_to_medium_product_dto.py` & `songtradr-api-client-python-1.12.22/test/test_track_to_medium_product_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -39,70 +39,70 @@
         model = songtradr_api_client_python.models.track_to_medium_product_dto.TrackToMediumProductDTO()  # noqa: E501
         if include_optional :
             return TrackToMediumProductDTO(
                 track_no = '', 
                 set_no = '', 
                 product = songtradr_api_client_python.models.product_medium_dto.ProductMediumDTO(
                     duration = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    parties = [
-                        songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
-                            contributor_types = [
-                                songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                    type_name = '', )
-                                ], 
-                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                id = '', 
-                                full_name = '', ), )
-                        ], 
-                    grid = '', 
-                    release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
                         year = 56, 
                         text = '', ), 
-                    titles = [
-                        songtradr_api_client_python.models.title_dto.TitleDTO(
-                            title_text = '', )
-                        ], 
                     genres = [
                         songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                             genre_name = '', )
                         ], 
-                    gtin = '', )
+                    titles = [
+                        songtradr_api_client_python.models.title_dto.TitleDTO(
+                            title_text = '', )
+                        ], 
+                    gtin = '', 
+                    grid = '', 
+                    release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    parties = [
+                        songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
+                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                id = '', 
+                                full_name = '', ), 
+                            contributor_types = [
+                                songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                    type_name = '', )
+                                ], )
+                        ], )
             )
         else :
             return TrackToMediumProductDTO(
                 track_no = '',
                 product = songtradr_api_client_python.models.product_medium_dto.ProductMediumDTO(
                     duration = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    parties = [
-                        songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
-                            contributor_types = [
-                                songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                    type_name = '', )
-                                ], 
-                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                id = '', 
-                                full_name = '', ), )
-                        ], 
-                    grid = '', 
-                    release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
                         year = 56, 
                         text = '', ), 
-                    titles = [
-                        songtradr_api_client_python.models.title_dto.TitleDTO(
-                            title_text = '', )
-                        ], 
                     genres = [
                         songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                             genre_name = '', )
                         ], 
-                    gtin = '', ),
+                    titles = [
+                        songtradr_api_client_python.models.title_dto.TitleDTO(
+                            title_text = '', )
+                        ], 
+                    gtin = '', 
+                    grid = '', 
+                    release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    parties = [
+                        songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
+                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                id = '', 
+                                full_name = '', ), 
+                            contributor_types = [
+                                songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                    type_name = '', )
+                                ], )
+                        ], ),
         )
         """
 
     def testTrackToMediumProductDTO(self):
         """Test TrackToMediumProductDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_update_password_dto.py` & `songtradr-api-client-python-1.12.22/test/test_update_password_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_usage_dto.py` & `songtradr-api-client-python-1.12.22/test/test_usage_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_user_api.py` & `songtradr-api-client-python-1.12.22/test/test_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.21/test/test_user_dto.py` & `songtradr-api-client-python-1.12.22/test/test_user_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.21
+    The version of the OpenAPI document: 1.12.22
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

