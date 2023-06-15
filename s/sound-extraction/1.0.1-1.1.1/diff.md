# Comparing `tmp/sound-extraction-1.0.1.tar.gz` & `tmp/sound-extraction-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sound-extraction-1.0.1.tar", last modified: Mon Jun 12 18:18:52 2023, max compression
+gzip compressed data, was "dist\sound-extraction-1.1.1.tar", last modified: Thu Jun 15 13:17:19 2023, max compression
```

## Comparing `sound-extraction-1.0.1.tar` & `sound-extraction-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:18:52.978063 sound-extraction-1.0.1/
--rw-rw-rw-   0        0        0     1087 2023-06-12 17:14:00.000000 sound-extraction-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      964 2023-06-12 18:18:52.977094 sound-extraction-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4889 2023-06-06 18:56:03.000000 sound-extraction-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 18:18:52.978063 sound-extraction-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1524 2023-06-12 18:17:23.000000 sound-extraction-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:18:52.949159 sound-extraction-1.0.1/sound-extraction/
-drwxrwxrwx   0        0        0        0 2023-06-12 18:18:52.975071 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/
--rw-rw-rw-   0        0        0      964 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      153 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 13:17:19.981634 sound-extraction-1.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-06-12 17:14:00.000000 sound-extraction-1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     6223 2023-06-15 13:17:19.979171 sound-extraction-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5717 2023-06-15 02:45:40.000000 sound-extraction-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:17:19.983633 sound-extraction-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1131 2023-06-15 13:17:07.000000 sound-extraction-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:17:19.968667 sound-extraction-1.1.1/sound_extraction.egg-info/
+-rw-rw-rw-   0        0        0     6223 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      153 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 13:17:19.973654 sound-extraction-1.1.1/src/
+-rw-rw-rw-   0        0        0    17950 2023-06-15 02:35:01.000000 sound-extraction-1.1.1/src/sound_extraction.py
```

### Comparing `sound-extraction-1.0.1/LICENSE.txt` & `sound-extraction-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sound-extraction-1.0.1/README.md` & `sound-extraction-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 # Audio-File Extraction
 
 ## About
 
 Use this tool to segment (i.e., clip or slice), copy, and extract short-duration recordings, from long-duration WAV or FLAC files. Segmenting audio files into smaller parts can make recordings compatible for certain analytical workflows and allow for easier manipulation and sharing. Segment and extracting recordings based on a list of recording start times (date times) and a desired duration. This allows for applications such as the extraction of stratified audio samples, among others.
 
+## Downloading the package from PyPI
+
+    pip install sound-extraction
+
+After downloading the package from PyPI, you can use the following command to run the program:
+
+    sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"
+
+Users can follow the same arguments and commands mentioned below to run the program. [Here](#usage)
+
+- If you want to run the program from the source files then follow the steps below:
+
 ## Setup (Windows)
 
 Download Audio-File Extraction Files: [Sound-File Extraction](https://drive.google.com/file/d/1HX9Cz0I7uKsIPuhHCdB1lfCmbtFY_YxJ/view?usp=share_link)
 
     python -m venv venv
     venv\Scripts\Activate
     pip install -r requirements.txt
@@ -44,15 +56,15 @@
 
 Arguments and commands used are required to get the slicing of larger audio files into smaller audio files of your choice.
 
 Here's a complete list of all command line arguments:
 
     -r, Path to original audio files (required). Need to make sure all the audio files are stored in a folder.
     -o, Path to output folder (required). Program will create a folder for you with current time, name of site and extraction of duration to the specified path.
-    -c, Path to your list of recordings to be extracted. This must be a CSV file where all the sample recording names to be extracted, stored in a column named "sampleFile".
+    -c, Path to the CSV file with the following requirements: Header should include "sample file" and "categories" columns. The "sample file" column should be in the format 20220608_170343, and the "categories" column should contain categories such as "Nocturnal", etc.
     -s, Prefix or the recording name, or ID, etc. This will be used to name the extracted audio files.
     -d, Duration of the extracted audio file. Change the duration of the extracted audio files, if required. Default is 3 minutes.
     -span, Span of the audio file. Extracted audio files will not span to 3 minutes if the original file is shorter.
     -e, Extension of the audio file (.wav or .flac). If your original audio files are flac then you need to use ".wav". Default is flac.
     -slice, Slice the audio file in smaller segments/chunks. Default is 10 seconds.
 
 We can see the arguments list by using the following command:
@@ -73,8 +85,14 @@
 
 2. This program will send the error message to the Sentry server to improve the user performace and to keep track of the errors which will be handled by myself.
 
 ## Important Notes
 
 1. Try to have your original audio files in subfolder of root directory and once you provide path of root folder then code will search for all the files in all subfolders as well as in root folder.
 
-2. Original files should be in the format `20220611T202300.wav` or `20220611T202300.flac`. Sample files in CSV should be in the format `20220611_202300.wav` or `20220611_202300.flac`.
+2. Original files should be in the format `20220611T202300.wav` or `20220611T202300.flac`. Sample files in CSV should be in the format `20220611_202300.wav` or `20220611_202300.flac` under the heading `sampleFile`. For instance,
+
+   ![Sample Image](data/image.png)
+
+## Changelog
+
+1. All the version changes are mentioned in the [CHANGELOG.md](https://github.com/prayagnshah/Sound-Extraction/blob/main/CHANGELOG.md) file.
```

