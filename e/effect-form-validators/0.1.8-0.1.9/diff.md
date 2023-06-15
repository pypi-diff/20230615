# Comparing `tmp/effect-form-validators-0.1.8.tar.gz` & `tmp/effect-form-validators-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "effect-form-validators-0.1.8.tar", last modified: Wed May 25 16:01:32 2022, max compression
+gzip compressed data, was "effect-form-validators-0.1.9.tar", last modified: Fri May 27 11:29:56 2022, max compression
```

## Comparing `effect-form-validators-0.1.8.tar` & `effect-form-validators-0.1.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.130923 effect-form-validators-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      106 2022-04-23 01:20:28.000000 effect-form-validators-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-04-23 01:20:28.000000 effect-form-validators-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.120896 effect-form-validators-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.123892 effect-form-validators-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1492 2022-05-07 02:31:07.000000 effect-form-validators-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1822 2022-05-25 16:01:07.000000 effect-form-validators-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)      133 2022-05-04 04:19:24.000000 effect-form-validators-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-04-22 18:40:44.000000 effect-form-validators-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)     1647 2022-05-25 16:01:32.131044 effect-form-validators-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      800 2022-04-23 10:56:15.000000 effect-form-validators-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-04-23 01:20:28.000000 effect-form-validators-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.124638 effect-form-validators-0.1.8/effect_form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      185 2022-05-04 04:19:24.000000 effect-form-validators-0.1.8/effect_form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-05-04 04:19:24.000000 effect-form-validators-0.1.8/effect_form_validators/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.125903 effect-form-validators-0.1.8/effect_form_validators/effect_prn/
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-05-11 02:34:27.000000 effect-form-validators-0.1.8/effect_form_validators/effect_prn/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2236 2022-05-25 16:01:07.000000 effect-form-validators-0.1.8/effect_form_validators/effect_prn/hospitalization_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.126392 effect-form-validators-0.1.8/effect_form_validators/effect_screening/
--rw-r--r--   0 erikvw     (501) staff       (20)       76 2022-05-25 16:01:07.000000 effect-form-validators-0.1.8/effect_form_validators/effect_screening/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6648 2022-05-25 16:01:07.000000 effect-form-validators-0.1.8/effect_form_validators/effect_screening/subject_screening_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.129331 effect-form-validators-0.1.8/effect_form_validators/effect_subject/
--rw-r--r--   0 erikvw     (501) staff       (20)     1226 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5031 2022-05-07 02:31:07.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/arv_history_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-05-05 09:45:55.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/arv_treatment_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      299 2022-05-04 04:19:24.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/blood_culture_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3756 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/chest_xray_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      248 2022-05-04 04:19:24.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/clinical_note_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1349 2022-05-04 04:19:24.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/diagnosis_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      874 2022-05-05 09:45:55.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/histopathology_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1464 2022-05-07 02:31:07.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/lp_csf_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      255 2022-05-04 04:19:24.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/medication_adherence_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2652 2022-05-05 09:45:55.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/medication_history_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1434 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/mental_status_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3125 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/patient_treatment_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7154 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/signs_and_symptoms_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2245 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/study_medication_baseline_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1860 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/study_medication_followup_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7813 2022-05-07 02:31:07.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/subject_visit_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      640 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/effect_subject/vital_signs_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.129634 effect-form-validators-0.1.8/effect_form_validators/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-04 00:09:11.000000 effect-form-validators-0.1.8/effect_form_validators/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.129856 effect-form-validators-0.1.8/effect_form_validators/tests/effect_prn/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:07.000000 effect-form-validators-0.1.8/effect_form_validators/tests/effect_prn/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    20873 2022-05-25 16:01:07.000000 effect-form-validators-0.1.8/effect_form_validators/tests/effect_prn/test_hospitalisation.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.130119 effect-form-validators-0.1.8/effect_form_validators/tests/effect_screening/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:07.000000 effect-form-validators-0.1.8/effect_form_validators/tests/effect_screening/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2648 2022-05-25 16:01:07.000000 effect-form-validators-0.1.8/effect_form_validators/tests/effect_screening/test_subject_screening.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.130812 effect-form-validators-0.1.8/effect_form_validators/tests/effect_subject/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:07.000000 effect-form-validators-0.1.8/effect_form_validators/tests/effect_subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8378 2022-05-25 16:01:07.000000 effect-form-validators-0.1.8/effect_form_validators/tests/effect_subject/test_chest_xray.py
--rw-r--r--   0 erikvw     (501) staff       (20)    26371 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/tests/effect_subject/test_patient_treatment.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10747 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/tests/effect_subject/test_signs_and_symptoms.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7711 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/tests/effect_subject/test_vital_signs.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3133 2022-05-25 16:01:23.000000 effect-form-validators-0.1.8/effect_form_validators/tests/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      158 2022-05-04 04:19:24.000000 effect-form-validators-0.1.8/effect_form_validators/tests/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-05-07 02:26:03.000000 effect-form-validators-0.1.8/effect_form_validators/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 16:01:32.125492 effect-form-validators-0.1.8/effect_form_validators.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1647 2022-05-25 16:01:31.000000 effect-form-validators-0.1.8/effect_form_validators.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2682 2022-05-25 16:01:32.000000 effect-form-validators-0.1.8/effect_form_validators.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-25 16:01:31.000000 effect-form-validators-0.1.8/effect_form_validators.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-04-25 15:55:26.000000 effect-form-validators-0.1.8/effect_form_validators.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       23 2022-05-25 16:01:32.000000 effect-form-validators-0.1.8/effect_form_validators.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1709 2022-05-07 02:31:07.000000 effect-form-validators-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-04-23 01:20:28.000000 effect-form-validators-0.1.8/requirements.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     3242 2022-05-23 15:08:50.000000 effect-form-validators-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1170 2022-05-25 16:01:32.131385 effect-form-validators-0.1.8/setup.cfg
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.964582 effect-form-validators-0.1.9/
+-rw-r--r--   0 jw         (502) staff       (20)      106 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/.coveragerc
+-rw-r--r--   0 jw         (502) staff       (20)      436 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/.editorconfig
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.925984 effect-form-validators-0.1.9/.github/
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.933038 effect-form-validators-0.1.9/.github/workflows/
+-rw-r--r--   0 jw         (502) staff       (20)     1492 2022-05-05 20:14:52.000000 effect-form-validators-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 jw         (502) staff       (20)     1822 2022-05-24 17:17:07.000000 effect-form-validators-0.1.9/.gitignore
+-rw-r--r--   0 jw         (502) staff       (20)      133 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/CHANGES
+-rw-r--r--   0 jw         (502) staff       (20)    35149 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/LICENSE
+-rw-r--r--   0 jw         (502) staff       (20)     1647 2022-05-27 11:29:56.965564 effect-form-validators-0.1.9/PKG-INFO
+-rw-r--r--   0 jw         (502) staff       (20)      800 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/README.rst
+-rw-r--r--   0 jw         (502) staff       (20)      162 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/codecov.yml
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.934391 effect-form-validators-0.1.9/effect_form_validators/
+-rw-r--r--   0 jw         (502) staff       (20)      185 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/effect_form_validators/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)      169 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/effect_form_validators/apps.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.938273 effect-form-validators-0.1.9/effect_form_validators/effect_prn/
+-rw-r--r--   0 jw         (502) staff       (20)       73 2022-05-11 01:46:03.000000 effect-form-validators-0.1.9/effect_form_validators/effect_prn/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)     2236 2022-05-24 11:58:40.000000 effect-form-validators-0.1.9/effect_form_validators/effect_prn/hospitalization_form_validator.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.941234 effect-form-validators-0.1.9/effect_form_validators/effect_screening/
+-rw-r--r--   0 jw         (502) staff       (20)       76 2022-05-24 11:58:40.000000 effect-form-validators-0.1.9/effect_form_validators/effect_screening/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)     8336 2022-05-27 11:29:45.000000 effect-form-validators-0.1.9/effect_form_validators/effect_screening/subject_screening_form_validator.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.956301 effect-form-validators-0.1.9/effect_form_validators/effect_subject/
+-rw-r--r--   0 jw         (502) staff       (20)     1226 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)     5031 2022-05-05 20:14:52.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/arv_history_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)      118 2022-05-05 09:52:29.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/arv_treatment_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)      299 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/blood_culture_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)     3756 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/chest_xray_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)      248 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/clinical_note_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)     1349 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/diagnosis_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)      874 2022-05-05 09:52:29.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/histopathology_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)     1464 2022-05-05 17:49:27.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/lp_csf_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)      255 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/medication_adherence_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)     2652 2022-05-05 09:52:29.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/medication_history_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)     1434 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/mental_status_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)     3125 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/patient_treatment_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)     7154 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/signs_and_symptoms_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)     2245 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/study_medication_baseline_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)     1860 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/study_medication_followup_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)     7813 2022-05-05 22:12:50.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/subject_visit_form_validator.py
+-rw-r--r--   0 jw         (502) staff       (20)      640 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/effect_subject/vital_signs_form_validator.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.958021 effect-form-validators-0.1.9/effect_form_validators/tests/
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-05-20 15:33:59.000000 effect-form-validators-0.1.9/effect_form_validators/tests/__init__.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.958900 effect-form-validators-0.1.9/effect_form_validators/tests/effect_prn/
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-05-24 11:58:40.000000 effect-form-validators-0.1.9/effect_form_validators/tests/effect_prn/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)    20873 2022-05-24 11:58:40.000000 effect-form-validators-0.1.9/effect_form_validators/tests/effect_prn/test_hospitalisation.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.960050 effect-form-validators-0.1.9/effect_form_validators/tests/effect_screening/
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-05-24 11:58:40.000000 effect-form-validators-0.1.9/effect_form_validators/tests/effect_screening/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)    11121 2022-05-27 11:29:45.000000 effect-form-validators-0.1.9/effect_form_validators/tests/effect_screening/test_subject_screening.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.963420 effect-form-validators-0.1.9/effect_form_validators/tests/effect_subject/
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-05-24 11:58:40.000000 effect-form-validators-0.1.9/effect_form_validators/tests/effect_subject/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)     8378 2022-05-24 11:58:40.000000 effect-form-validators-0.1.9/effect_form_validators/tests/effect_subject/test_chest_xray.py
+-rw-r--r--   0 jw         (502) staff       (20)    26371 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/tests/effect_subject/test_patient_treatment.py
+-rw-r--r--   0 jw         (502) staff       (20)    10747 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/tests/effect_subject/test_signs_and_symptoms.py
+-rw-r--r--   0 jw         (502) staff       (20)     7711 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/tests/effect_subject/test_vital_signs.py
+-rw-r--r--   0 jw         (502) staff       (20)     3133 2022-05-27 11:24:12.000000 effect-form-validators-0.1.9/effect_form_validators/tests/mixins.py
+-rw-r--r--   0 jw         (502) staff       (20)      158 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/effect_form_validators/tests/models.py
+-rw-r--r--   0 jw         (502) staff       (20)      118 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/effect_form_validators/urls.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-05-27 11:29:56.936691 effect-form-validators-0.1.9/effect_form_validators.egg-info/
+-rw-r--r--   0 jw         (502) staff       (20)     1647 2022-05-27 11:29:56.000000 effect-form-validators-0.1.9/effect_form_validators.egg-info/PKG-INFO
+-rw-r--r--   0 jw         (502) staff       (20)     2682 2022-05-27 11:29:56.000000 effect-form-validators-0.1.9/effect_form_validators.egg-info/SOURCES.txt
+-rw-r--r--   0 jw         (502) staff       (20)        1 2022-05-27 11:29:56.000000 effect-form-validators-0.1.9/effect_form_validators.egg-info/dependency_links.txt
+-rw-r--r--   0 jw         (502) staff       (20)        1 2022-05-16 18:55:17.000000 effect-form-validators-0.1.9/effect_form_validators.egg-info/not-zip-safe
+-rw-r--r--   0 jw         (502) staff       (20)       23 2022-05-27 11:29:56.000000 effect-form-validators-0.1.9/effect_form_validators.egg-info/top_level.txt
+-rw-r--r--   0 jw         (502) staff       (20)     1709 2022-05-05 20:14:52.000000 effect-form-validators-0.1.9/pyproject.toml
+-rw-r--r--   0 jw         (502) staff       (20)        1 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/requirements.txt
+-rw-r--r--   0 jw         (502) staff       (20)     3242 2022-05-05 09:37:17.000000 effect-form-validators-0.1.9/runtests.py
+-rw-r--r--   0 jw         (502) staff       (20)     1170 2022-05-27 11:29:56.967008 effect-form-validators-0.1.9/setup.cfg
```

### Comparing `effect-form-validators-0.1.8/.github/workflows/build.yml` & `effect-form-validators-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/.gitignore` & `effect-form-validators-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/LICENSE` & `effect-form-validators-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/PKG-INFO` & `effect-form-validators-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effect-form-validators
-Version: 0.1.8
+Version: 0.1.9
 Summary: Form validation classes for the EFFECT trial
 Home-page: https://github.com/effect-trial/effect-form-validators
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django,edc,EFFECT,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `effect-form-validators-0.1.8/README.rst` & `effect-form-validators-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_prn/hospitalization_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_prn/hospitalization_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_screening/subject_screening_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_screening/subject_screening_form_validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,56 @@
 from django import forms
 from edc_consent.form_validators import ConsentFormValidatorMixin
 from edc_constants.constants import FEMALE, MALE, NO, OTHER, PENDING, POS, YES
 from edc_form_validators import FormValidator
+from edc_model import estimated_date_from_ago
+from edc_utils.forms import EstimatedDateFromAgoFormMixin
 
 
-class SubjectScreeningFormValidator(ConsentFormValidatorMixin, FormValidator):
+class SubjectScreeningFormValidator(
+    EstimatedDateFromAgoFormMixin, ConsentFormValidatorMixin, FormValidator
+):
     def clean(self) -> None:
         self.get_consent_for_period_or_raise(self.cleaned_data.get("report_datetime"))
         self.validate_age()
+        self.validate_hiv_dx()
         self.validate_cd4()
         self.validate_serum_crag()
         self.validate_lp_and_csf_crag()
         self.validate_cm_in_csf()
         self.validate_mg_ssx()
         self.validate_pregnancy()
         self.required_if(
             YES, field="unsuitable_for_study", field_required="reasons_unsuitable"
         )
 
+    def validate_hiv_dx(self):
+        self.not_required_if(
+            NO,
+            field="hiv_pos",
+            field_required="hiv_dx_ago",
+            inverse=False,
+        )
+        self.not_required_if(
+            NO,
+            field="hiv_pos",
+            field_required="hiv_dx_date",
+            inverse=False,
+        )
+        if self.cleaned_data.get("hiv_pos") == YES and not (
+            self.cleaned_data.get("hiv_dx_ago") or self.cleaned_data.get("hiv_dx_date")
+        ):
+            raise forms.ValidationError(
+                {"hiv_dx_date": "This field is required (or the above)."}
+            )
+
+        self.raise_if_both_ago_and_actual_date(
+            ago_field="hiv_dx_ago", date_field="hiv_dx_date", label="HIV diagnosis"
+        )
+
     def validate_cd4(self) -> None:
         if self.cleaned_data.get("cd4_date") and self.cleaned_data.get("report_datetime"):
             if (
                 self.cleaned_data.get("cd4_date")
                 > self.cleaned_data.get("report_datetime").date()
             ):
                 raise forms.ValidationError(
@@ -34,18 +63,27 @@
                 raise forms.ValidationError(
                     {
                         "cd4_date": (
                             "Invalid. Cannot be more than 21 days before the report date"
                         )
                     }
                 )
+            if self.cleaned_data.get("cd4_date") and self.provided_hiv_dx_date:
+                if self.provided_hiv_dx_date > self.cleaned_data.get("cd4_date"):
+                    raise forms.ValidationError(
+                        {
+                            "cd4_date": (
+                                "Invalid. "
+                                "Most recent CD4 count date cannot be before HIV diagnosis."
+                            )
+                        }
+                    )
 
     def validate_serum_crag(self) -> None:
-        """Assert serum CrAg date is:
-        - positive
+        """Assert serum CrAg is positive, and serum CrAg date is:
         - not before CD4 date
         - within 21 days of CD4
         - within 14 days of report
         """
         if self.cleaned_data.get("serum_crag_value") != POS:
             raise forms.ValidationError(
                 {
@@ -161,7 +199,13 @@
 
     def validate_mg_ssx(self) -> None:
         self.validate_other_specify(
             field="any_other_mg_ssx",
             other_specify_field="any_other_mg_ssx_other",
             other_stored_value=YES,
         )
+
+    @property
+    def provided_hiv_dx_date(self):
+        if self.cleaned_data.get("hiv_dx_ago"):
+            return estimated_date_from_ago(data=self.cleaned_data, ago_field="hiv_dx_ago")
+        return self.cleaned_data.get("hiv_dx_date")
```

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/__init__.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/__init__.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/arv_history_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/arv_history_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/chest_xray_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/chest_xray_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/diagnosis_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/diagnosis_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/histopathology_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/histopathology_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/lp_csf_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/lp_csf_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/medication_history_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/medication_history_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/mental_status_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/mental_status_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/patient_treatment_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/patient_treatment_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/signs_and_symptoms_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/signs_and_symptoms_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/study_medication_baseline_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/study_medication_baseline_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/study_medication_followup_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/study_medication_followup_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/subject_visit_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/subject_visit_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/effect_subject/vital_signs_form_validator.py` & `effect-form-validators-0.1.9/effect_form_validators/effect_subject/vital_signs_form_validator.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/tests/effect_prn/test_hospitalisation.py` & `effect-form-validators-0.1.9/effect_form_validators/tests/effect_prn/test_hospitalisation.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/tests/effect_subject/test_chest_xray.py` & `effect-form-validators-0.1.9/effect_form_validators/tests/effect_subject/test_chest_xray.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/tests/effect_subject/test_patient_treatment.py` & `effect-form-validators-0.1.9/effect_form_validators/tests/effect_subject/test_patient_treatment.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/tests/effect_subject/test_signs_and_symptoms.py` & `effect-form-validators-0.1.9/effect_form_validators/tests/effect_subject/test_signs_and_symptoms.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/tests/effect_subject/test_vital_signs.py` & `effect-form-validators-0.1.9/effect_form_validators/tests/effect_subject/test_vital_signs.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators/tests/mixins.py` & `effect-form-validators-0.1.9/effect_form_validators/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/effect_form_validators.egg-info/PKG-INFO` & `effect-form-validators-0.1.9/effect_form_validators.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effect-form-validators
-Version: 0.1.8
+Version: 0.1.9
 Summary: Form validation classes for the EFFECT trial
 Home-page: https://github.com/effect-trial/effect-form-validators
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django,edc,EFFECT,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `effect-form-validators-0.1.8/effect_form_validators.egg-info/SOURCES.txt` & `effect-form-validators-0.1.9/effect_form_validators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/pyproject.toml` & `effect-form-validators-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/runtests.py` & `effect-form-validators-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `effect-form-validators-0.1.8/setup.cfg` & `effect-form-validators-0.1.9/setup.cfg`

 * *Files identical despite different names*

