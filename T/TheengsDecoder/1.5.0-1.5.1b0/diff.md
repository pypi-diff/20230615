# Comparing `tmp/TheengsDecoder-1.5.0.tar.gz` & `tmp/TheengsDecoder-1.5.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TheengsDecoder-1.5.0.tar", last modified: Fri Jun  9 00:04:46 2023, max compression
+gzip compressed data, was "TheengsDecoder-1.5.1b0.tar", last modified: Thu Jun 15 14:46:04 2023, max compression
```

## Comparing `TheengsDecoder-1.5.0.tar` & `TheengsDecoder-1.5.1b0.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.259791 TheengsDecoder-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-06-09 00:04:46.259791 TheengsDecoder-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.235791 TheengsDecoder-1.5.0/TheengsDecoder/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/TheengsDecoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/TheengsDecoder/_decoder.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.239791 TheengsDecoder-1.5.0/TheengsDecoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-06-09 00:04:46.000000 TheengsDecoder-1.5.0/TheengsDecoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11521 2023-06-09 00:04:46.000000 TheengsDecoder-1.5.0/TheengsDecoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 00:04:46.000000 TheengsDecoder-1.5.0/TheengsDecoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-09 00:04:46.000000 TheengsDecoder-1.5.0/TheengsDecoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 00:04:46.259791 TheengsDecoder-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-09 00:04:43.000000 TheengsDecoder-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.239791 TheengsDecoder-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.239791 TheengsDecoder-1.5.0/src/arduino_json/
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-09 00:04:31.000000 TheengsDecoder-1.5.0/src/arduino_json/.git
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/.mbedignore
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/ArduinoJson.h
--rw-r--r--   0 runner    (1001) docker     (122)    40084 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)    10845 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      871 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (122)    32515 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/banner.svg
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/component.mk
--rw-r--r--   0 runner    (1001) docker     (122)      932 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/keywords.txt
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/library.json
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/library.properties
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.239791 TheengsDecoder-1.5.0/src/arduino_json/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.239791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2413 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5393 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5295 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3810 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Collection/
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7657 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Configuration.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/
--rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStringReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3108 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/
--rw-r--r--   0 runner    (1001) docker     (122)     4061 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9071 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    18680 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Latch.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Memory/
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4855 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Misc/
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Misc/Visitable.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/
--rw-r--r--   0 runner    (1001) docker     (122)    15856 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5241 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/ieee754.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Namespace.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/Float.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.247791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/
--rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1001 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/Pair.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.247791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/
--rw-r--r--   0 runner    (1001) docker     (122)      526 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/assert.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      370 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/ctype.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/integer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/math.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.247791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      889 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/conditional.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/declval.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      423 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/enable_if.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/integral_constant.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_array.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_const.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      992 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_floating_point.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_pointer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_same.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_void.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_const.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_cv.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_reference.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/type_identity.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/DummyWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      686 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/measure.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      616 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/StoragePolicy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/String.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/Converter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9517 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5651 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10885 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantTag.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/compatibility.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/version.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson.h
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2157 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    29875 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/decoder.h
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/decoder_c.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.259791 TheengsDecoder-1.5.0/src/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/ABN03_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/ABTemp_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/APPLE_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/Amphiro_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2595 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BC08_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BM1IN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BM2_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BM3IN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BM4IN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2962 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BPARASITE_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BWBSDOO_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGD1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3733 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGDK2_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2319 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGDN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     6179 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGG1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGH1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGP1W_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGPR1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/GAEN_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4840 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/H5055_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/H5072_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/H5074_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/H5102_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/H5106_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2273 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/HHCCJCY01HHCC_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/HHCCJCY10_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/HHCCPOT002_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/IBS_THBP01B_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/IBT_2X_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/IBT_4XS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3854 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/IBT_6XS_SOLIS6_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/JHT_F525_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/JQJCY01YM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/KKM_K6P_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/KKM_K9_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/LYWSD02_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/LYWSD03MMC_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/LYWSDCGQ_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3892 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/MBXPRO_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/MS_CDP_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/MUE4094RT_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/Miband_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/Mokobeacon_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4604 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/Mopeka_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/PH10_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     8958 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/RDL52832_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/RuuviTag_RAWv1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/RuuviTag_RAWv2_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBBT_002C_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBCS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBCU_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3468 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBMS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBMT_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBOT_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBS1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SCD4X_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SHT4X_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/ServiceData_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/Skale_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SmartDry_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/T201_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/T301_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2445 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/TPMS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/TPTH_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4690 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/ThermoBeacon_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/XMTZC04HM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/XMTZC05HM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/common_props.h
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/iBeacon_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/iNodeEM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/tracker_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     6645 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.708307 TheengsDecoder-1.5.1b0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-06-15 14:46:04.708307 TheengsDecoder-1.5.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.684306 TheengsDecoder-1.5.1b0/TheengsDecoder/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/TheengsDecoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/TheengsDecoder/_decoder.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.684306 TheengsDecoder-1.5.1b0/TheengsDecoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-06-15 14:46:04.000000 TheengsDecoder-1.5.1b0/TheengsDecoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11521 2023-06-15 14:46:04.000000 TheengsDecoder-1.5.1b0/TheengsDecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 14:46:04.000000 TheengsDecoder-1.5.1b0/TheengsDecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-15 14:46:04.000000 TheengsDecoder-1.5.1b0/TheengsDecoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 14:46:04.708307 TheengsDecoder-1.5.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-06-15 14:46:02.000000 TheengsDecoder-1.5.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.684306 TheengsDecoder-1.5.1b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.688306 TheengsDecoder-1.5.1b0/src/arduino_json/
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/arduino_json/.git
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/.mbedignore
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/ArduinoJson.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40084 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10845 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      871 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    32515 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/banner.svg
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/component.mk
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/keywords.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/library.json
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/library.properties
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.688306 TheengsDecoder-1.5.1b0/src/arduino_json/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.688306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.688306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2413 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5393 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5295 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3810 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.688306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Collection/
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7657 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Configuration.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.688306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/
+-rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.688306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStringReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3108 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.692306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Document/
+-rw-r--r--   0 runner    (1001) docker     (122)     4061 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9071 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.692306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    18680 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/Latch.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.692306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Memory/
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4855 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.692306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Misc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Misc/Visitable.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.692306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/MsgPack/
+-rw-r--r--   0 runner    (1001) docker     (122)    15856 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5241 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/MsgPack/ieee754.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Namespace.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.692306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/Float.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.692306 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/
+-rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1001 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/Pair.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.696307 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/assert.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/ctype.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/integer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/math.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.696307 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      889 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.696307 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/conditional.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/declval.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      423 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/enable_if.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/integral_constant.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_array.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_const.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      992 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_floating_point.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_pointer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_same.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_void.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_const.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_cv.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_reference.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/type_identity.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.696307 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.700307 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/DummyWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      686 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/measure.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.700307 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/StringStorage/
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.700307 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.700307 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/StoragePolicy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/String.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.700307 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/Converter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9517 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5651 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10885 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantTag.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/compatibility.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/version.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2157 2023-06-15 14:45:54.000000 TheengsDecoder-1.5.1b0/src/arduino_json/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    30936 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/decoder_c.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:46:04.708307 TheengsDecoder-1.5.1b0/src/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/ABN03_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/ABTemp_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/APPLE_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/Amphiro_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2595 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/BC08_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/BM1IN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/BM2_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/BM3IN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/BM4IN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3244 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/BPARASITE_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/BWBSDOO_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/CGD1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/CGDK2_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2319 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/CGDN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6783 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/CGG1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/CGH1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/CGP1W_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/CGPR1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/GAEN_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4840 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/H5055_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/H5072_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/H5074_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/H5102_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/H5106_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/HHCCJCY01HHCC_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/HHCCJCY10_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1526 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/HHCCPOT002_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2461 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/IBS_THBP01B_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3838 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/IBT_2X_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/IBT_4XS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4144 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/IBT_6XS_SOLIS6_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/JHT_F525_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/JQJCY01YM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/KKM_K6P_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/KKM_K9_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/LYWSD02_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3162 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/LYWSD03MMC_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1921 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/LYWSDCGQ_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3892 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/MBXPRO_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/MS_CDP_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/MUE4094RT_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/Miband_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/Mokobeacon_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4604 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/Mopeka_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/PH10_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8958 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/RDL52832_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/RuuviTag_RAWv1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4746 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/RuuviTag_RAWv2_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/SBBT_002C_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/SBCS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/SBCU_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3468 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/SBMS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/SBMT_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/SBOT_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/SBS1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/SCD4X_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/SHT4X_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/ServiceData_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/Skale_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/SmartDry_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/T201_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/T301_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/TPMS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/TPTH_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/ThermoBeacon_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/XMTZC04HM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/XMTZC05HM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/common_props.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/iBeacon_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/iNodeEM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices/tracker_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6645 2023-06-15 14:45:52.000000 TheengsDecoder-1.5.1b0/src/devices.h
```

### Comparing `TheengsDecoder-1.5.0/CMakeLists.txt` & `TheengsDecoder-1.5.1b0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/LICENSE.txt` & `TheengsDecoder-1.5.1b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/PKG-INFO` & `TheengsDecoder-1.5.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheengsDecoder
-Version: 1.5.0
+Version: 1.5.1b0
 Summary: A message decoder for the Internet of Things
 Author: Theengs
 License:  GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Theengs Decoder project aims to provide an efficient, portable and lightweight library for BLE Internet of Things messages decoding.
```

### Comparing `TheengsDecoder-1.5.0/README.md` & `TheengsDecoder-1.5.1b0/README.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/TheengsDecoder/_decoder.cpp` & `TheengsDecoder-1.5.1b0/TheengsDecoder/_decoder.cpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/TheengsDecoder.egg-info/PKG-INFO` & `TheengsDecoder-1.5.1b0/TheengsDecoder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheengsDecoder
-Version: 1.5.0
+Version: 1.5.1b0
 Summary: A message decoder for the Internet of Things
 Author: Theengs
 License:  GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Theengs Decoder project aims to provide an efficient, portable and lightweight library for BLE Internet of Things messages decoding.
```

### Comparing `TheengsDecoder-1.5.0/TheengsDecoder.egg-info/SOURCES.txt` & `TheengsDecoder-1.5.1b0/TheengsDecoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/setup.py` & `TheengsDecoder-1.5.1b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if version.parse(get_cmake_version()) < version.parse("3.4"):
         setup_requires.append("cmake")
 except SKBuildError:
     setup_requires.append("cmake")
 
 setup(
     name="TheengsDecoder",
-    version="v1.5.0",
+    version="v1.5.1beta",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="A message decoder for the Internet of Things",
     author='Theengs',
     license=" GPL-3.0 License",
     packages=['TheengsDecoder'],
     setup_requires=setup_requires,
```

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/CHANGELOG.md` & `TheengsDecoder-1.5.1b0/src/arduino_json/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/CMakeLists.txt` & `TheengsDecoder-1.5.1b0/src/arduino_json/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/LICENSE.md` & `TheengsDecoder-1.5.1b0/src/arduino_json/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/README.md` & `TheengsDecoder-1.5.1b0/src/arduino_json/README.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/SUPPORT.md` & `TheengsDecoder-1.5.1b0/src/arduino_json/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/appveyor.yml` & `TheengsDecoder-1.5.1b0/src/arduino_json/appveyor.yml`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/banner.svg` & `TheengsDecoder-1.5.1b0/src/arduino_json/banner.svg`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/keywords.txt` & `TheengsDecoder-1.5.1b0/src/arduino_json/keywords.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/library.json` & `TheengsDecoder-1.5.1b0/src/arduino_json/library.json`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/library.properties` & `TheengsDecoder-1.5.1b0/src/arduino_json/library.properties`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Configuration.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Configuration.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Latch.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/Latch.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Namespace.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Namespace.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/Pair.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Object/Pair.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/String.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/String.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/compatibility.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson/compatibility.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson.hpp` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/ArduinoJson.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/arduino_json/src/CMakeLists.txt` & `TheengsDecoder-1.5.1b0/src/arduino_json/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/decoder.cpp` & `TheengsDecoder-1.5.1b0/src/decoder.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -785,14 +785,43 @@
             if (strstr((const char*)decoder[1], MFG_DATA)) {
               src = mfg_data;
             }
 
             std::string value(src + decoder[2].as<int>(), decoder[3].as<int>());
             jsondata[sanitizeJsonKey(kv.key().c_str())] = value;
             success = i_main;
+          } else if (strstr((const char*)decoder[0], "mac_from_hex_data") != nullptr) {
+            const char* src = svc_data;
+            if (strstr((const char*)decoder[1], MFG_DATA)) {
+              src = mfg_data;
+            }
+
+            std::string value(src + decoder[2].as<int>(), 12);
+
+            // reverse MAC
+            if (strstr((const char*)decoder[0], "revmac_from_hex_data") != nullptr) {
+              const char* mac_string = nullptr;
+              mac_string = value.c_str();
+              char* reverse_mac_string = (char*)malloc(strlen(mac_string) + 1);
+              reverse_hex_data(mac_string, reverse_mac_string, 12);
+              value = reverse_mac_string;
+            }
+
+            // upper case MAC
+            for (int x = 0; x <= 12; x++) {
+              value[x] = toupper(value[x]);
+            }
+
+            // add colons
+            for (int x = 2; x <= 14; x += 3) {
+              value.insert(x, 1, ':');
+            }
+
+            jsondata[sanitizeJsonKey(kv.key().c_str())] = value;
+            success = i_main;
           }
         }
       }
       return success;
     }
   }
   return success;
```

### Comparing `TheengsDecoder-1.5.0/src/decoder.h` & `TheengsDecoder-1.5.1b0/src/decoder.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/decoder_c.cpp` & `TheengsDecoder-1.5.1b0/src/decoder_c.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 */
 
 #include <stdio.h>
 #include <string.h>
 
 #include "decoder.h"
-#include "shared/theengs.h"
+#if (SKBUILD)
+#  include "shared/theengs.h"
+#endif
 
 // Utility function local to the bridge's implementation
 TheengsDecoder* AsDecoder(void* decoder) { return reinterpret_cast<TheengsDecoder*>(decoder); }
 
 void* Theengs_NewDecoder() {
   auto decoder = new TheengsDecoder();
   return decoder;
```

### Comparing `TheengsDecoder-1.5.0/src/devices/ABN03_json.h` & `TheengsDecoder-1.5.1b0/src/devices/CGDN1_json.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-const char* _ABN03_json = "{\"brand\":\"April Brother\",\"model\":\"N03\",\"model_id\":\"ABN03\",\"tag\":\"0208\",\"condition\":[\"servicedata\",\"=\",30,\"index\",0,\"ab03\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,4,true,true],\"post_proc\":[\"/\",8]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",22,4,true,false],\"post_proc\":[\"/\",2]},\"lux\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",26,4,true,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,2,false,false]}}}";
-/* R""""(
+const char* _CGDN1_json = "{\"brand\":\"Qingping\",\"model\":\"Air Monitor Lite\",\"model_id\":\"CGDN1\",\"tag\":\"0f\",\"condition\":[\"servicedata\",\"=\",48,\"index\",2,\"0e\",\"|\",\"servicedata\",\"=\",48,\"index\",2,\"24\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true,false],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"pm25\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,true,false]},\"pm10\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",36,4,true,false]},\"co2\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",44,4,true,false]}}}";
+/*R""""(
 {
-   "brand":"April Brother",
-   "model":"N03",
-   "model_id":"ABN03",
-   "tag":"0208",
-   "condition":["servicedata", "=", 30, "index", 0, "ab03"],
+   "brand":"Qingping",
+   "model":"Air Monitor Lite",
+   "model_id":"CGDN1",
+   "tag":"0f",
+   "condition":["servicedata", "=", 48, "index", 2, "0e", "|", "servicedata", "=", 48, "index", 2, "24", "&", "uuid", "index", 0, "fdcd"],
    "properties":{
       "tempc":{
-         "decoder":["value_from_hex_data", "servicedata", 18, 4, true, true],
-         "post_proc":["/", 8]
+         "decoder":["value_from_hex_data", "servicedata", 20, 4, true, false],
+         "post_proc":["/", 10]
       },
       "hum":{
-         "decoder":["value_from_hex_data", "servicedata", 22, 4, true, false],
-         "post_proc":["/", 2]
+         "decoder":["value_from_hex_data", "servicedata", 24, 4, true, false],
+         "post_proc":["/", 10]
+      },
+      "pm25":{
+         "decoder":["value_from_hex_data", "servicedata", 32, 4, true, false]
       },
-      "lux":{
-         "decoder":["value_from_hex_data", "servicedata", 26, 4, true, false]
+      "pm10":{
+         "decoder":["value_from_hex_data", "servicedata", 36, 4, true, false]
       },
-      "batt":{
-         "decoder":["value_from_hex_data", "servicedata", 16, 2, false, false]
+      "co2":{
+         "decoder":["value_from_hex_data", "servicedata", 44, 4, true, false]
       }
    }
 })"""";*/
 
-const char* _ABN03_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"lux\":{\"unit\":\"lx\",\"name\":\"illuminance\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"}}}";
+const char* _CGDN1_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"pm25\":{\"unit\":\"μg/m³\",\"name\":\"PM2.5\"},\"pm10\":{\"unit\":\"μg/m³\",\"name\":\"PM10\"},\"co2\":{\"unit\":\"ppm\",\"name\":\"carbon dioxide\"}}}";
 /*R""""(
 {
    "properties":{
       "tempc":{
          "unit":"°C",
          "name":"temperature"
       },
       "hum":{
          "unit":"%",
          "name":"humidity"
       },
-      "lux":{
-         "unit":"lx",
-         "name":"illuminance"
-      },
-      "batt":{
-         "unit":"%",
-         "name":"battery"
+      "pm25":{
+         "unit":"μg/m³",
+         "name":"PM2.5"
+      },
+      "pm10":{
+         "unit":"μg/m³",
+         "name":"PM10"
+      },
+      "co2":{
+         "unit":"ppm",
+         "name":"carbon dioxide"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/ABTemp_json.h` & `TheengsDecoder-1.5.1b0/src/devices/ABTemp_json.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _ABTemp_json = "{\"brand\":\"April Brother\",\"model\":\"ABTemp\",\"model_id\":\"ABTemp\",\"tag\":\"0608\",\"condition\":[\"manufacturerdata\",\"=\",50,\"index\",0,\"4c000215b5b182c7eab14988aa99b5c1517008d9\"],\"properties\":{\"mfid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",0,4]},\"uuid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",8,32]},\"major\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",40,4,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",44,2,false]},\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",46,2,false]},\"txpower\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",48,2,false]}}}";
+const char* _ABTemp_json = "{\"brand\":\"April Brother\",\"model\":\"ABTemp\",\"model_id\":\"ABTemp\",\"tag\":\"0608\",\"condition\":[\"manufacturerdata\",\"=\",50,\"index\",0,\"4c000215b5b182c7eab14988aa99b5c1517008d9\"],\"properties\":{\"mfid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",0,4]},\"uuid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",8,32]},\"major\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",40,4,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",44,2,false]},\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",46,2,false]},\"txpower\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",48,2,false]},\"mac\":{\"condition\":[\"servicedata\",\"=\",22],\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",0]}}}";
 /*R""""(
 {
    "brand":"April Brother",
    "model":"ABTemp",
    "model_id":"ABTemp",
    "tag":"0608",
    "condition":["manufacturerdata", "=", 50, "index", 0, "4c000215b5b182c7eab14988aa99b5c1517008d9"],
@@ -20,19 +20,23 @@
          "decoder":["value_from_hex_data", "manufacturerdata", 44, 2, false]
       },
       "tempc":{
          "decoder":["value_from_hex_data", "manufacturerdata", 46, 2, false]
       },
       "txpower":{
          "decoder":["value_from_hex_data","manufacturerdata", 48, 2, false]
+      },
+      "mac":{
+         "condition":["servicedata", "=", 22],
+         "decoder":["revmac_from_hex_data", "servicedata", 0]
       }
    }
 })"""";*/
 
-const char* _ABTemp_json_props = "{\"properties\":{\"mfid\":{\"unit\":\"hex\",\"name\":\"manufacturer id\"},\"uuid\":{\"unit\":\"hex\",\"name\":\"service uuid\"},\"major\":{\"unit\":\"hex\",\"name\":\"major value\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"txpower\":{\"unit\":\"dBm\",\"name\":\"tx power @ 1 m\"}}}";
+const char* _ABTemp_json_props = "{\"properties\":{\"mfid\":{\"unit\":\"hex\",\"name\":\"manufacturer id\"},\"uuid\":{\"unit\":\"hex\",\"name\":\"service uuid\"},\"major\":{\"unit\":\"hex\",\"name\":\"major value\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"txpower\":{\"unit\":\"dBm\",\"name\":\"tx power @ 1 m\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "mfid":{
          "unit":"hex",
          "name":"manufacturer id"
       },
@@ -51,10 +55,14 @@
       "tempc":{
          "unit":"°C",
          "name":"temperature"
       },
       "txpower":{
          "unit":"dBm",
          "name":"tx power @ 1 m"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/APPLE_json.h` & `TheengsDecoder-1.5.1b0/src/devices/APPLE_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/Amphiro_json.h` & `TheengsDecoder-1.5.1b0/src/devices/Amphiro_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/BC08_json.h` & `TheengsDecoder-1.5.1b0/src/devices/BC08_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/BM1IN1_json.h` & `TheengsDecoder-1.5.1b0/src/devices/BM1IN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/BM2_json.h` & `TheengsDecoder-1.5.1b0/src/devices/BM2_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/BM3IN1_json.h` & `TheengsDecoder-1.5.1b0/src/devices/BM3IN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/BM4IN1_json.h` & `TheengsDecoder-1.5.1b0/src/devices/BM4IN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/BPARASITE_json.h` & `TheengsDecoder-1.5.1b0/src/devices/BPARASITE_json.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _BPARASITE_json = "{\"brand\":\"rbaron\",\"model\":\"b-parasite\",\"model_id\":\"BPv1.0-1.2\",\"tag\":\"0904\",\"condition\":[\"servicedata\",\">=\",32,\"index\",0,\"1\",\"|\",\"servicedata\",\">=\",32,\"index\",0,\"2\",\"&\",\"uuid\",\"index\",0,\"181a\"],\"properties\":{\"tempc\":{\"condition\":[\"servicedata\",0,\"1\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",8,4,false,true],\"post_proc\":[\"/\",1000]},\"_tempc\":{\"condition\":[\"servicedata\",0,\"2\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",8,4,false,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,false,false],\"post_proc\":[\"/\",655.35]},\"moi\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,4,false,false],\"post_proc\":[\"/\",655.35]},\"lux\":{\"condition\":[\"servicedata\",1,\"bit\",0,1],\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,false,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",4,4,false,false],\"post_proc\":[\"/\",1000]}}}";
+const char* _BPARASITE_json = "{\"brand\":\"rbaron\",\"model\":\"b-parasite\",\"model_id\":\"BPv1.0-1.2\",\"tag\":\"0904\",\"condition\":[\"servicedata\",\">=\",32,\"index\",0,\"1\",\"|\",\"servicedata\",\">=\",32,\"index\",0,\"2\",\"&\",\"uuid\",\"index\",0,\"181a\"],\"properties\":{\"tempc\":{\"condition\":[\"servicedata\",0,\"1\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",8,4,false,true],\"post_proc\":[\"/\",1000]},\"_tempc\":{\"condition\":[\"servicedata\",0,\"2\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",8,4,false,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,false,false],\"post_proc\":[\"/\",655.35]},\"moi\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,4,false,false],\"post_proc\":[\"/\",655.35]},\"lux\":{\"condition\":[\"servicedata\",1,\"bit\",0,1],\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,false,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",4,4,false,false],\"post_proc\":[\"/\",1000]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"servicedata\",20]}}}";
 
 /* R""""(
 {
    "brand":"rbaron",
    "model":"b-parasite",
    "model_id":"BPv1.0-1.2",
    "tag":"0904",
@@ -29,19 +29,22 @@
       "lux":{
          "condition":["servicedata", 1, "bit", 0, 1],
          "decoder":["value_from_hex_data", "servicedata", 32, 4, false, false]
       },
       "volt":{
          "decoder":["value_from_hex_data", "servicedata", 4, 4, false, false],
           "post_proc":["/", 1000]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "servicedata", 20]
       }
    }
 })"""";*/
 
-const char* _BPARASITE_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"moi\":{\"unit\":\"%\",\"name\":\"moisture\"},\"lux\":{\"unit\":\"lx\",\"name\":\"illuminance\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"}}}";
+const char* _BPARASITE_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"moi\":{\"unit\":\"%\",\"name\":\"moisture\"},\"lux\":{\"unit\":\"lx\",\"name\":\"illuminance\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "tempc":{
          "unit":"°C",
          "name":"temperature"
       },
@@ -56,10 +59,14 @@
       "lux":{
          "unit":"lx",
          "name":"illuminance"
       },
       "volt":{
          "unit":"V",
          "name":"voltage"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/BWBSDOO_json.h` & `TheengsDecoder-1.5.1b0/src/devices/BWBSDOO_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/CGD1_json.h` & `TheengsDecoder-1.5.1b0/src/devices/CGD1_json.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "common_props.h"
 
-const char* _CGD1_json = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"Alarm Clock\",\"model_id\":\"CGC1/CGD1\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",34,\"index\",2,\"0c\",\"|\",\"servicedata\",\"=\",34,\"index\",2,\"1e\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true,true],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,2,false,false],\"post_proc\":[\"&\",127]}}}";
+const char* _CGD1_json = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"Alarm Clock\",\"model_id\":\"CGC1/CGD1\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",34,\"index\",2,\"0c\",\"|\",\"servicedata\",\"=\",34,\"index\",2,\"1e\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true,true],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,2,false,false],\"post_proc\":[\"&\",127]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",4]}}}";
 
 /*R""""(
 {
    "brand":"ClearGrass/Qingping",
    "model":"Alarm Clock",
    "model_id":"CGC1/CGD1",
    "tag":"01",
@@ -17,12 +17,15 @@
       "hum":{
          "decoder":["value_from_hex_data", "servicedata", 24, 4, true, false],
          "post_proc":["/", 10]
       },
       "batt":{
          "decoder":["value_from_hex_data", "servicedata", 32, 2, false, false],
          "post_proc":["&", 127]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 4]
       }
    }
 })"""";*/
 
 const char* _CGD1_json_props = _common_BTH_props;
```

### Comparing `TheengsDecoder-1.5.0/src/devices/CGDK2_json.h` & `TheengsDecoder-1.5.1b0/src/devices/CGDK2_json.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "common_props.h"
 
-const char* _CGDK2_json_STOCK = "{\"brand\":\"Qingping\",\"model\":\"TH Lite\",\"model_id\":\"CGDK2\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",34,\"index\",2,\"10\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,4,true,false],\"post_proc\":[\"/\",10]}}}";
+const char* _CGDK2_json_STOCK = "{\"brand\":\"Qingping\",\"model\":\"TH Lite\",\"model_id\":\"CGDK2\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",34,\"index\",2,\"10\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",4]}}}";
 /*R""""(
 {
    "brand":"Qingping",
    "model":"TH Lite",
    "model_id":"CGDK2",
    "tag":"01",
    "condition":["servicedata", "=", 34, "index", 2, "10", "&", "uuid", "index", 0, "fdcd"],
@@ -12,20 +12,23 @@
       "tempc":{
          "decoder":["value_from_hex_data", "servicedata", 20, 4, true],
          "post_proc":["/", 10]
       },
       "hum":{
          "decoder":["value_from_hex_data", "servicedata", 24, 4, true, false],
          "post_proc":["/", 10]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 4]
       }
    }
 })"""";*/
 
 // ATC1441
-const char* _CGDK2_json_ATC1441 = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"TH Lite\",\"model_id\":\"CGDK2_ATC1441\",\"tag\":\"0102\",\"condition\":[\"servicedata\",\"=\",26,\"&\",\"uuid\",\"index\",0,\"181a\",\"&\",\"name\",\"index\",0,\"CGDK\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,false],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,2,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,2,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,false],\"post_proc\":[\"/\",1000]}}}";
+const char* _CGDK2_json_ATC1441 = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"TH Lite\",\"model_id\":\"CGDK2_ATC1441\",\"tag\":\"0102\",\"condition\":[\"servicedata\",\"=\",26,\"&\",\"uuid\",\"index\",0,\"181a\",\"&\",\"name\",\"index\",0,\"CGDK\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,false],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,2,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,2,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,false],\"post_proc\":[\"/\",1000]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"servicedata\",0]}}}";
 /* R""""(
 {
    "brand":"ClearGrass/Qingping",
    "model":"TH Lite",
    "model_id":"CGDK2_ATC1441",
    "tag":"0102",
    "condition":["servicedata", "=", 26, "&", "uuid", "index", 0, "181a", "&", "name", "index", 0, "CGDK"],
@@ -39,20 +42,23 @@
       },
       "batt":{
          "decoder":["value_from_hex_data", "servicedata", 18, 2, false]
       },
       "volt":{
          "decoder":["value_from_hex_data", "servicedata", 20, 4, false],
          "post_proc":["/", 1000]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "servicedata", 0]
       }
    }
 })"""";*/
 
 // PVVX
-const char* _CGDK2_json_PVVX = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"TH Lite\",\"model_id\":\"CGDK2_PVVX\",\"tag\":\"0102\",\"condition\":[\"servicedata\",\"=\",30,\"&\",\"uuid\",\"index\",0,\"181a\",\"&\",\"name\",\"index\",0,\"CGDK\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,4,true],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,2,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true],\"post_proc\":[\"/\",1000]}}}";
+const char* _CGDK2_json_PVVX = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"TH Lite\",\"model_id\":\"CGDK2_PVVX\",\"tag\":\"0102\",\"condition\":[\"servicedata\",\"=\",30,\"&\",\"uuid\",\"index\",0,\"181a\",\"&\",\"name\",\"index\",0,\"CGDK\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,4,true],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,2,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true],\"post_proc\":[\"/\",1000]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",0]}}}";
 /* R""""(
 {
    "brand":"ClearGrass/Qingping",
    "model":"TH Lite",
    "model_id":"CGDK2_PVVX",
    "tag":"0102",
    "condition":["servicedata", "=", 30, "&", "uuid", "index", 0, "181a", "&", "name", "index", 0, "CGDK"],
@@ -67,12 +73,15 @@
       },
       "batt":{
          "decoder":["value_from_hex_data", "servicedata", 24, 2, false]
       },
       "volt":{
          "decoder":["value_from_hex_data", "servicedata", 20, 4, true],
          "post_proc":["/", 1000]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 0]
       }
    }
 })"""";*/
 
 const char* _CGDK2_json_props = _common_BVTH_props;
```

### Comparing `TheengsDecoder-1.5.0/src/devices/CGDN1_json.h` & `TheengsDecoder-1.5.1b0/src/devices/HHCCJCY10_json.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,54 @@
-const char* _CGDN1_json = "{\"brand\":\"Qingping\",\"model\":\"Air Monitor Lite\",\"model_id\":\"CGDN1\",\"tag\":\"0f\",\"condition\":[\"servicedata\",\"=\",48,\"index\",2,\"0e\",\"|\",\"servicedata\",\"=\",48,\"index\",2,\"24\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true,false],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"pm25\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,true,false]},\"pm10\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",36,4,true,false]},\"co2\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",44,4,true,false]}}}";
+const char* _HHCCJCY10_json = "{\"brand\":\"Xiaomi/VegTrug\",\"model\":\"MiFlora\",\"model_id\":\"HHCCJCY10\",\"tag\":\"09\",\"condition\":[\"servicedata\",\"=\",18,\"&\",\"uuid\",\"index\",0,\"fd50\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",2,4,false,true],\"post_proc\":[\"/\",10]},\"moi\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",0,2,false,false]},\"lux\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",6,6,false,false]},\"fer\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",14,4,false,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,2,false,false]}}}";
 /*R""""(
 {
-   "brand":"Qingping",
-   "model":"Air Monitor Lite",
-   "model_id":"CGDN1",
-   "tag":"0f",
-   "condition":["servicedata", "=", 48, "index", 2, "0e", "|", "servicedata", "=", 48, "index", 2, "24", "&", "uuid", "index", 0, "fdcd"],
+   "brand":"Xiaomi/VegTrug",
+   "model":"MiFlora",
+   "model_id":"HHCCJCY10",
+   "tag":"09",
+   "condition":["servicedata", "=", 18, "&", "uuid", "index", 0, "fd50"],
    "properties":{
       "tempc":{
-         "decoder":["value_from_hex_data", "servicedata", 20, 4, true, false],
+         "decoder":["value_from_hex_data", "servicedata", 2, 4, false, true],
          "post_proc":["/", 10]
       },
-      "hum":{
-         "decoder":["value_from_hex_data", "servicedata", 24, 4, true, false],
-         "post_proc":["/", 10]
+      "moi":{
+         "decoder":["value_from_hex_data", "servicedata", 0, 2, false, false]
       },
-      "pm25":{
-         "decoder":["value_from_hex_data", "servicedata", 32, 4, true, false]
+      "lux":{
+         "decoder":["value_from_hex_data", "servicedata", 6, 6, false, false]
       },
-      "pm10":{
-         "decoder":["value_from_hex_data", "servicedata", 36, 4, true, false]
+      "fer":{
+         "decoder":["value_from_hex_data", "servicedata", 14, 4, false, false]
       },
-      "co2":{
-         "decoder":["value_from_hex_data", "servicedata", 44, 4, true, false]
+      "batt":{
+         "decoder":["value_from_hex_data", "servicedata", 12, 2, false, false]
       }
    }
 })"""";*/
 
-const char* _CGDN1_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"pm25\":{\"unit\":\"μg/m³\",\"name\":\"PM2.5\"},\"pm10\":{\"unit\":\"μg/m³\",\"name\":\"PM10\"},\"co2\":{\"unit\":\"ppm\",\"name\":\"carbon dioxide\"}}}";
+const char* _HHCCJCY10_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"moi\":{\"unit\":\"%\",\"name\":\"moisture\"},\"lux\":{\"unit\":\"lx\",\"name\":\"illuminance\"},\"fer\":{\"unit\":\"µS/cm\",\"name\":\"fertility\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"}}}";
 /*R""""(
 {
    "properties":{
       "tempc":{
          "unit":"°C",
          "name":"temperature"
       },
-      "hum":{
+      "moi":{
          "unit":"%",
-         "name":"humidity"
+         "name":"moisture"
+      },
+      "lux":{
+         "unit":"lx",
+         "name":"illuminance"
       },
-      "pm25":{
-         "unit":"μg/m³",
-         "name":"PM2.5"
-      },
-      "pm10":{
-         "unit":"μg/m³",
-         "name":"PM10"
-      },
-      "co2":{
-         "unit":"ppm",
-         "name":"carbon dioxide"
+      "fer":{
+         "unit":"µS/cm",
+         "name":"fertility"
+      },
+      "batt":{
+         "unit":"%",
+         "name":"battery"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/CGG1_json.h` & `TheengsDecoder-1.5.1b0/src/devices/CGG1_json.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "common_props.h"
 
-const char* _CGG1_json_STOCK = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"Round TH\",\"model_id\":\"CGG1\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",34,\"index\",2,\"07\",\"|\",\"servicedata\",\"=\",34,\"index\",2,\"16\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,4,true],\"post_proc\":[\"/\",10]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,2,false]}}}";
+const char* _CGG1_json_STOCK = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"Round TH\",\"model_id\":\"CGG1\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",34,\"index\",2,\"07\",\"|\",\"servicedata\",\"=\",34,\"index\",2,\"16\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,4,true],\"post_proc\":[\"/\",10]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,2,false]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",4]}}}";
 /* R""""(
 {
    "brand":"ClearGrass/Qingping",
    "model":"Round TH",
    "model_id":"CGG1",
    "tag":"01",
    "condition":["servicedata", "=", 34, "index", 2, "07", "|", "servicedata", "=", 34, "index", 2, "16", "&", "uuid", "index", 0, "fdcd"],
@@ -15,20 +15,23 @@
       },
       "hum":{
          "decoder":["value_from_hex_data", "servicedata", 24, 4, true],
          "post_proc":["/", 10]
       },
       "batt":{
          "decoder":["value_from_hex_data", "servicedata", 32, 2, false]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 4]
       }
    }
 })"""";*/
 
 // ATC1441
-const char* _CGG1_json_ATC1441 = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"Round TH\",\"model_id\":\"CGG1_ATC1441\",\"tag\":\"0102\",\"condition\":[\"servicedata\",\"=\",26,\"&\",\"uuid\",\"index\",0,\"181a\",\"&\",\"name\",\"index\",0,\"CGG\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,false],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,2,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,2,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,false],\"post_proc\":[\"/\",1000]}}}";
+const char* _CGG1_json_ATC1441 = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"Round TH\",\"model_id\":\"CGG1_ATC1441\",\"tag\":\"0102\",\"condition\":[\"servicedata\",\"=\",26,\"&\",\"uuid\",\"index\",0,\"181a\",\"&\",\"name\",\"index\",0,\"CGG\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,false],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,2,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,2,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,false],\"post_proc\":[\"/\",1000]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"servicedata\",0]}}}";
 /* R""""(
 {
    "brand":"ClearGrass/Qingping",
    "model":"Round TH",
    "model_id":"CGG1_ATC1441",
    "tag":"0102",
    "condition":["servicedata", "=", 26, "&", "uuid", "index", 0, "181a", "&", "name", "index", 0, "CGG"],
@@ -42,20 +45,23 @@
       },
       "batt":{
          "decoder":["value_from_hex_data", "servicedata", 18, 2, false]
       },
       "volt":{
          "decoder":["value_from_hex_data", "servicedata", 20, 4, false],
          "post_proc":["/", 1000]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "servicedata", 0]
       }
    }
 })"""";*/
 
 // PVVX
-const char* _CGG1_json_PVVX = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"Round TH\",\"model_id\":\"CGG1_PVVX\",\"tag\":\"0102\",\"condition\":[\"servicedata\",\"=\",30,\"&\",\"uuid\",\"index\",0,\"181a\",\"&\",\"name\",\"index\",0,\"CGG\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,4,true],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,2,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true],\"post_proc\":[\"/\",1000]}}}";
+const char* _CGG1_json_PVVX = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"Round TH\",\"model_id\":\"CGG1_PVVX\",\"tag\":\"0102\",\"condition\":[\"servicedata\",\"=\",30,\"&\",\"uuid\",\"index\",0,\"181a\",\"&\",\"name\",\"index\",0,\"CGG\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,4,true],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,2,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true],\"post_proc\":[\"/\",1000]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",0]}}}";
 /* R""""(
 {
    "brand":"ClearGrass/Qingping",
    "model":"Round TH",
    "model_id":"CGG1_PVVX",
    "tag":"0102",
    "condition":["servicedata", "=", 30, "&", "uuid", "index", 0, "181a", "&", "name", "index", 0, "CGG"],
@@ -70,19 +76,22 @@
       },
       "batt":{
          "decoder":["value_from_hex_data", "servicedata", 24, 2, false]
       },
       "volt":{
          "decoder":["value_from_hex_data", "servicedata", 20, 4, true],
          "post_proc":["/", 1000]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 0]
       }
    }
 })"""";*/
 
-const char* _CGG1_json_STOCK_2 = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"Round TH\",\"model_id\":\"CGG1\",\"tag\":\"0102\",\"condition\":[\"servicedata\",\"=\",30,\"|\",\"servicedata\",\"=\",32,\"|\",\"servicedata\",\"=\",36,\"&\",\"name\",\"index\",0,\"Qingping Temp & RH\",\"|\",\"name\",\"index\",0,\"ClearGrass Temp & RH\",\"&\",\"uuid\",\"index\",0,\"fe95\"],\"properties\":{\"tempc\":{\"condition\":[\"servicedata\",\">=\",32,\"&\",\"servicedata\",23,\"!\",\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"condition\":[\"servicedata\",\"=\",36,\"&\",\"servicedata\",23,\"!\",\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,true],\"post_proc\":[\"/\",10]},\"_hum\":{\"condition\":[\"servicedata\",\"=\",32,\"&\",\"servicedata\",23,\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true],\"post_proc\":[\"/\",10]},\"batt\":{\"condition\":[\"servicedata\",\"=\",30],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,2,false]}}}";
+const char* _CGG1_json_STOCK_2 = "{\"brand\":\"ClearGrass/Qingping\",\"model\":\"Round TH\",\"model_id\":\"CGG1\",\"tag\":\"0102\",\"condition\":[\"servicedata\",\"=\",30,\"|\",\"servicedata\",\"=\",32,\"|\",\"servicedata\",\"=\",36,\"&\",\"name\",\"index\",0,\"Qingping Temp & RH\",\"|\",\"name\",\"index\",0,\"ClearGrass Temp & RH\",\"&\",\"uuid\",\"index\",0,\"fe95\"],\"properties\":{\"tempc\":{\"condition\":[\"servicedata\",\">=\",32,\"&\",\"servicedata\",23,\"!\",\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"condition\":[\"servicedata\",\"=\",36,\"&\",\"servicedata\",23,\"!\",\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,true],\"post_proc\":[\"/\",10]},\"_hum\":{\"condition\":[\"servicedata\",\"=\",32,\"&\",\"servicedata\",23,\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true],\"post_proc\":[\"/\",10]},\"batt\":{\"condition\":[\"servicedata\",\"=\",30],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,2,false]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",10]}}}";
 /*
 R""""(
 {
    "brand":"ClearGrass/Qingping",
    "model":"Round TH",
    "model_id":"CGG1",
    "tag":"0102",
@@ -102,12 +111,15 @@
          "condition":["servicedata", "=", 32, "&", "servicedata", 23, "6"],
          "decoder":["value_from_hex_data", "servicedata", 28, 4, true],
          "post_proc":["/", 10]
       },
       "batt":{
          "condition":["servicedata", "=", 30],
          "decoder":["value_from_hex_data", "servicedata", 28, 2, false]      
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 10]
       }
    }
 })"""";*/
 
 const char* _CGG1_json_props = _common_BVTH_props;
```

### Comparing `TheengsDecoder-1.5.0/src/devices/CGH1_json.h` & `TheengsDecoder-1.5.1b0/src/devices/CGH1_json.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _CGH1_json = "{\"brand\":\"Qingping\",\"model\":\"Contact Sensor\",\"model_id\":\"CGH1\",\"tag\":\"0404\",\"condition\":[\"servicedata\",\"=\",34,\"index\",2,\"04\",\"|\",\"servicedata\",\"=\",28,\"index\",2,\"04\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"open\":{\"condition\":[\"servicedata\",\"=\",28],\"decoder\":[\"bit_static_value\",\"servicedata\",21,0,true,false]},\"_open\":{\"condition\":[\"servicedata\",\"=\",34],\"decoder\":[\"bit_static_value\",\"servicedata\",33,0,true,false]}}}";
+const char* _CGH1_json = "{\"brand\":\"Qingping\",\"model\":\"Contact Sensor\",\"model_id\":\"CGH1\",\"tag\":\"0404\",\"condition\":[\"servicedata\",\"=\",34,\"index\",2,\"04\",\"|\",\"servicedata\",\"=\",28,\"index\",2,\"04\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"open\":{\"condition\":[\"servicedata\",\"=\",28],\"decoder\":[\"bit_static_value\",\"servicedata\",21,0,true,false]},\"_open\":{\"condition\":[\"servicedata\",\"=\",34],\"decoder\":[\"bit_static_value\",\"servicedata\",33,0,true,false]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",4]}}}";
 /*R""""(
 {
    "brand":"Qingping",
    "model":"Contact Sensor",
    "model_id":"CGH1",
    "tag":"0404",
    "condition":["servicedata", "=", 34, "index", 2, "04", "|", "servicedata", "=", 28, "index", 2, "04", "&", "uuid", "index", 0, "fdcd"],
@@ -10,21 +10,28 @@
       "open":{
          "condition":["servicedata", "=", 28],
          "decoder":["bit_static_value", "servicedata", 21, 0, true, false]
       },
       "_open":{
          "condition":["servicedata", "=", 34],
          "decoder":["bit_static_value", "servicedata", 33, 0, true, false]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 4]
       }
    }
 })"""";*/
 
-const char* _CGH1_json_props = "{\"properties\":{\"open\":{\"unit\":\"status\",\"name\":\"door\"}}}";
+const char* _CGH1_json_props = "{\"properties\":{\"open\":{\"unit\":\"status\",\"name\":\"door\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "open":{
          "unit":"status",
          "name":"door"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/CGP1W_json.h` & `TheengsDecoder-1.5.1b0/src/devices/CGP1W_json.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _CGP1W_json = "{\"brand\":\"ClearGrass\",\"model\":\"Weather Station\",\"model_id\":\"CGP1W\",\"tag\":\"02\",\"condition\":[\"servicedata\",\"=\",42,\"index\",2,\"09\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"pres\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,true,false],\"post_proc\":[\"/\",10]}}}";
+const char* _CGP1W_json = "{\"brand\":\"ClearGrass\",\"model\":\"Weather Station\",\"model_id\":\"CGP1W\",\"tag\":\"02\",\"condition\":[\"servicedata\",\"=\",42,\"index\",2,\"09\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"pres\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,true,false],\"post_proc\":[\"/\",10]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",4]}}}";
 /*R""""(
 {
    "brand":"ClearGrass",
    "model":"Weather Station",
    "model_id":"CGP1W",
    "tag":"02",
    "condition":["servicedata", "=", 42, "index", 2, "09", "&", "uuid", "index", 0, "fdcd"],
@@ -14,29 +14,36 @@
       "hum":{
          "decoder":["value_from_hex_data", "servicedata", 24, 4, true, false],
          "post_proc":["/", 10]
       },
       "pres":{
          "decoder":["value_from_hex_data", "servicedata", 32, 4, true, false],
          "post_proc":["/", 10]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 4]
       }
    }
 })"""";*/
 
-const char* _CGP1W_json_props = "{\"properties\":{\"pres\":{\"unit\":\"hPa\",\"name\":\"pressure\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"}}}";
+const char* _CGP1W_json_props = "{\"properties\":{\"pres\":{\"unit\":\"hPa\",\"name\":\"pressure\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "pres":{
          "unit":"hPa",
          "name":"pressure"
       },
       "tempc":{
          "unit":"°C",
          "name":"temperature"
       },
       "hum":{
          "unit":"%",
          "name":"humidity"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/CGPR1_json.h` & `TheengsDecoder-1.5.1b0/src/devices/CGPR1_json.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _CGPR1_json = "{\"brand\":\"Qingping\",\"model\":\"Motion & Light\",\"model_id\":\"CGPR1\",\"tag\":\"0404\",\"condition\":[\"servicedata\",\"=\",28,\"index\",2,\"12\",\"|\",\"servicedata\",\"=\",34,\"index\",2,\"12\",\"|\",\"servicedata\",\"=\",40,\"index\",2,\"12\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"lux\":{\"condition\":[\"servicedata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,true,false]},\"_lux\":{\"condition\":[\"servicedata\",\"=\",34],\"decoder\":[\"value_from_hex_data\",\"servicedata\",22,4,true,false]},\"pres\":{\"condition\":[\"servicedata\",\"=\",34],\"decoder\":[\"bit_static_value\",\"servicedata\",21,0,false,true]},\"_pres\":{\"condition\":[\"servicedata\",\"=\",28],\"decoder\":[\"bit_static_value\",\"servicedata\",21,0,false,true]},\"batt\":{\"condition\":[\"servicedata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,2,false,false]}}}";
+const char* _CGPR1_json = "{\"brand\":\"Qingping\",\"model\":\"Motion & Light\",\"model_id\":\"CGPR1\",\"tag\":\"0404\",\"condition\":[\"servicedata\",\"=\",28,\"index\",2,\"12\",\"|\",\"servicedata\",\"=\",34,\"index\",2,\"12\",\"|\",\"servicedata\",\"=\",40,\"index\",2,\"12\",\"&\",\"uuid\",\"index\",0,\"fdcd\"],\"properties\":{\"lux\":{\"condition\":[\"servicedata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,true,false]},\"_lux\":{\"condition\":[\"servicedata\",\"=\",34],\"decoder\":[\"value_from_hex_data\",\"servicedata\",22,4,true,false]},\"pres\":{\"condition\":[\"servicedata\",\"=\",34],\"decoder\":[\"bit_static_value\",\"servicedata\",21,0,false,true]},\"_pres\":{\"condition\":[\"servicedata\",\"=\",28],\"decoder\":[\"bit_static_value\",\"servicedata\",21,0,false,true]},\"batt\":{\"condition\":[\"servicedata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,2,false,false]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",4]}}}";
 /*
 R""""(
 {
    "brand":"Qingping",
    "model":"Motion & Light",
    "model_id":"CGPR1",
    "tag":"0404",
@@ -23,29 +23,36 @@
       "_pres":{
          "condition":["servicedata", "=", 28],
          "decoder":["bit_static_value", "servicedata", 21, 0, false, true]
       },
       "batt":{
          "condition":["servicedata", "=", 40],
          "decoder":["value_from_hex_data", "servicedata", 20, 2, false, false]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 4]
       }
    }
 })"""";*/
 
-const char* _CGPR1_json_props = "{\"properties\":{\"lux\":{\"unit\":\"lx\",\"name\":\"illuminance\"},\"pres\":{\"unit\":\"status\",\"name\":\"presence\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"}}}";
+const char* _CGPR1_json_props = "{\"properties\":{\"lux\":{\"unit\":\"lx\",\"name\":\"illuminance\"},\"pres\":{\"unit\":\"status\",\"name\":\"presence\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "lux":{
          "unit":"lx",
          "name":"illuminance"
       },
       "pres":{
          "unit":"status",
          "name":"presence"
       },
       "batt":{
          "unit":"%",
          "name":"battery"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/GAEN_json.h` & `TheengsDecoder-1.5.1b0/src/devices/GAEN_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/H5055_json.h` & `TheengsDecoder-1.5.1b0/src/devices/H5055_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/H5072_json.h` & `TheengsDecoder-1.5.1b0/src/devices/H5072_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/H5074_json.h` & `TheengsDecoder-1.5.1b0/src/devices/H5074_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/H5102_json.h` & `TheengsDecoder-1.5.1b0/src/devices/H5102_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/H5106_json.h` & `TheengsDecoder-1.5.1b0/src/devices/H5106_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/HHCCJCY01HHCC_json.h` & `TheengsDecoder-1.5.1b0/src/devices/HHCCJCY01HHCC_json.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _HHCCJCY01HHCC_json = "{\"brand\":\"Xiaomi/VegTrug\",\"model\":\"MiFlora\",\"model_id\":\"HHCCJCY01HHCC\",\"tag\":\"09\",\"condition\":[\"servicedata\",\"index\",4,\"9800\",\"|\",\"servicedata\",\"index\",4,\"bc03\",\"&\",\"uuid\",\"index\",0,\"fe95\"],\"properties\":{\"tempc\":{\"condition\":[\"servicedata\",24,\"0410\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,4,true],\"post_proc\":[\"/\",10]},\"moi\":{\"condition\":[\"servicedata\",24,\"0810\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,2,false]},\"lux\":{\"condition\":[\"servicedata\",24,\"0710\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,6,true]},\"fer\":{\"condition\":[\"servicedata\",24,\"0910\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,4,true]}}}";
+const char* _HHCCJCY01HHCC_json = "{\"brand\":\"Xiaomi/VegTrug\",\"model\":\"MiFlora\",\"model_id\":\"HHCCJCY01HHCC\",\"tag\":\"09\",\"condition\":[\"servicedata\",\"index\",4,\"9800\",\"|\",\"servicedata\",\"index\",4,\"bc03\",\"&\",\"uuid\",\"index\",0,\"fe95\"],\"properties\":{\"tempc\":{\"condition\":[\"servicedata\",24,\"0410\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,4,true],\"post_proc\":[\"/\",10]},\"moi\":{\"condition\":[\"servicedata\",24,\"0810\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,2,false]},\"lux\":{\"condition\":[\"servicedata\",24,\"0710\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,6,true]},\"fer\":{\"condition\":[\"servicedata\",24,\"0910\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,4,true]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",10]}}}";
 /*R""""(
 {
    "brand":"Xiaomi/VegTrug",
    "model":"MiFlora",
    "model_id":"HHCCJCY01HHCC",
    "tag":"09",
    "condition":["servicedata", "index", 4, "9800", "|", "servicedata", "index", 4, "bc03", "&", "uuid", "index", 0, "fe95"],
@@ -19,19 +19,22 @@
       "lux":{
          "condition":["servicedata", 24, "0710"],
          "decoder":["value_from_hex_data", "servicedata", 30, 6, true]
       },
       "fer":{
          "condition":["servicedata", 24, "0910"],
          "decoder":["value_from_hex_data", "servicedata", 30, 4, true]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 10]
       }
    }
 })"""";*/
 
-const char* _HHCCJCY01HHCC_json_props = "{\"properties\":{\"lux\":{\"unit\":\"lx\",\"name\":\"illuminance\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"fer\":{\"unit\":\"µS/cm\",\"name\":\"fertility\"},\"moi\":{\"unit\":\"%\",\"name\":\"moisture\"}}}";
+const char* _HHCCJCY01HHCC_json_props = "{\"properties\":{\"lux\":{\"unit\":\"lx\",\"name\":\"illuminance\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"fer\":{\"unit\":\"µS/cm\",\"name\":\"fertility\"},\"moi\":{\"unit\":\"%\",\"name\":\"moisture\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "lux":{
          "unit":"lx",
          "name":"illuminance"
       },
@@ -42,10 +45,14 @@
       "fer":{
          "unit":"µS/cm",
          "name":"fertility"
       },
       "moi":{
          "unit":"%",
          "name":"moisture"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/HHCCJCY10_json.h` & `TheengsDecoder-1.5.1b0/src/devices/LYWSD02_json.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,32 @@
-const char* _HHCCJCY10_json = "{\"brand\":\"Xiaomi/VegTrug\",\"model\":\"MiFlora\",\"model_id\":\"HHCCJCY10\",\"tag\":\"09\",\"condition\":[\"servicedata\",\"=\",18,\"&\",\"uuid\",\"index\",0,\"fd50\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",2,4,false,true],\"post_proc\":[\"/\",10]},\"moi\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",0,2,false,false]},\"lux\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",6,6,false,false]},\"fer\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",14,4,false,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,2,false,false]}}}";
-/*R""""(
+#include "common_props.h"
+
+const char* _LYWSD02_json = "{\"brand\":\"Xiaomi/Mijia\",\"model\":\"e-ink Clock\",\"model_id\":\"LYWSD02\",\"tag\":\"01\",\"condition\":[\"uuid\",\"index\",0,\"fe95\",\"&\",\"servicedata\",\"index\",4,\"5b04\"],\"properties\":{\"tempc\":{\"condition\":[\"servicedata\",24,\"0410\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"condition\":[\"servicedata\",24,\"0610\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,4,true,false],\"post_proc\":[\"/\",10]},\"batt\":{\"condition\":[\"servicedata\",24,\"0a10\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,2,false,false]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",10]}}}";
+/* R""""(
 {
-   "brand":"Xiaomi/VegTrug",
-   "model":"MiFlora",
-   "model_id":"HHCCJCY10",
-   "tag":"09",
-   "condition":["servicedata", "=", 18, "&", "uuid", "index", 0, "fd50"],
+   "brand":"Xiaomi/Mijia",
+   "model":"e-ink Clock",
+   "model_id":"LYWSD02",
+   "tag":"01",
+   "condition":["uuid", "index", 0, "fe95", "&", "servicedata", "index", 4, "5b04"],
    "properties":{
       "tempc":{
-         "decoder":["value_from_hex_data", "servicedata", 2, 4, false, true],
+         "condition":["servicedata", 24, "0410"],
+         "decoder":["value_from_hex_data", "servicedata", 30, 4, true],
          "post_proc":["/", 10]
       },
-      "moi":{
-         "decoder":["value_from_hex_data", "servicedata", 0, 2, false, false]
-      },
-      "lux":{
-         "decoder":["value_from_hex_data", "servicedata", 6, 6, false, false]
-      },
-      "fer":{
-         "decoder":["value_from_hex_data", "servicedata", 14, 4, false, false]
+      "hum":{
+         "condition":["servicedata", 24, "0610"],
+         "decoder":["value_from_hex_data", "servicedata", 30, 4, true, false],
+         "post_proc":["/", 10]
       },
       "batt":{
-         "decoder":["value_from_hex_data", "servicedata", 12, 2, false, false]
-      }
-   }
-})"""";*/
-
-const char* _HHCCJCY10_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"moi\":{\"unit\":\"%\",\"name\":\"moisture\"},\"lux\":{\"unit\":\"lx\",\"name\":\"illuminance\"},\"fer\":{\"unit\":\"µS/cm\",\"name\":\"fertility\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"}}}";
-/*R""""(
-{
-   "properties":{
-      "tempc":{
-         "unit":"°C",
-         "name":"temperature"
-      },
-      "moi":{
-         "unit":"%",
-         "name":"moisture"
+         "condition":["servicedata", 24, "0a10"],
+         "decoder":["value_from_hex_data", "servicedata", 30, 2, false, false]
       },
-      "lux":{
-         "unit":"lx",
-         "name":"illuminance"
-      },
-      "fer":{
-         "unit":"µS/cm",
-         "name":"fertility"
-      },
-      "batt":{
-         "unit":"%",
-         "name":"battery"
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 10]
       }
    }
 })"""";*/
+
+const char* _LYWSD02_json_props = _common_BTH_props;
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `TheengsDecoder-1.5.0/src/devices/HHCCPOT002_json.h` & `TheengsDecoder-1.5.1b0/src/devices/SBS1_json.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,40 @@
-const char* _HHCCPOT002_json = "{\"brand\":\"Xiaomi\",\"model\":\"RoPot\",\"model_id\":\"HHCCPOT002\",\"tag\":\"09\",\"condition\":[\"servicedata\",\"index\",2,\"205d01\"],\"properties\":{\"moi\":{\"condition\":[\"servicedata\",25,\"8\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,2,false]},\"fer\":{\"condition\":[\"servicedata\",25,\"9\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,4,true]}}}";
+const char* _SBS1_json = "{\"brand\":\"SwitchBot\",\"model\":\"Bot\",\"model_id\":\"X1\",\"tag\":\"0e02\",\"condition\":[\"uuid\",\"index\",0,\"0d00\",\"|\",\"uuid\",\"index\",0,\"fd3d\",\"&\",\"servicedata\",\"=\",6,\"index\",0,\"48\"],\"properties\":{\"mode\":{\"decoder\":[\"bit_static_value\",\"servicedata\",2,3,\"onestate\",\"on/off\"]},\"state\":{\"decoder\":[\"bit_static_value\",\"servicedata\",2,2,\"on\",\"off\"]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",4,2,false,false],\"post_proc\":[\"&\",127]}}}";
 /*R""""(
 {
-   "brand":"Xiaomi",
-   "model":"RoPot",
-   "model_id":"HHCCPOT002",
-   "tag":"09",
-   "condition":["servicedata", "index", 2, "205d01"],
+   "brand":"SwitchBot",
+   "model":"Bot",
+   "model_id":"X1",
+   "tag":"0e02",
+   "condition":["uuid", "index", 0, "0d00", "|", "uuid", "index", 0, "fd3d", "&", "servicedata", "=", 6, "index", 0, "48"],
    "properties":{
-      "moi":{
-         "condition":["servicedata", 25, "8"],
-         "decoder":["value_from_hex_data", "servicedata", 30, 2, false]
+      "mode":{
+         "decoder":["bit_static_value", "servicedata", 2, 3, "onestate", "on/off"]
       },
-      "fer":{
-         "condition":["servicedata", 25, "9"],
-         "decoder":["value_from_hex_data", "servicedata", 30, 4, true]
+      "state":{
+         "decoder":["bit_static_value", "servicedata", 2, 2, "on", "off"]
+      },
+      "batt":{
+         "decoder":["value_from_hex_data", "servicedata", 4, 2, false, false],
+         "post_proc":["&", 127]
       }
    }
 })"""";*/
 
-const char* _HHCCPOT002_json_props = "{\"properties\":{\"moi\":{\"unit\":\"%\",\"name\":\"moisture\"},\"fer\":{\"unit\":\"µS/cm\",\"name\":\"fertility\"}}}";
+const char* _SBS1_json_props = "{\"properties\":{\"mode\":{\"unit\":\"string\",\"name\":\"mode\"},\"state\":{\"unit\":\"string\",\"name\":\"state\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"}}}";
 /*R""""(
 {
    "properties":{
-      "moi":{
-         "unit":"%",
-         "name":"moisture"
+      "mode":{
+         "unit":"string",
+         "name":"mode"
+      },
+      "state":{
+         "unit":"string",
+         "name":"state"
       },
-      "fer":{
-         "unit":"µS/cm",
-         "name":"fertility"
+      "batt":{
+         "unit":"%",
+         "name":"battery"
       }
    }
-})"""";*/
+})"""";*/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `TheengsDecoder-1.5.0/src/devices/IBS_THBP01B_json.h` & `TheengsDecoder-1.5.1b0/src/devices/IBS_THBP01B_json.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _IBS_THBP01B_json = "{\"brand\":\"Inkbird\",\"model\":\"T(H) Sensor\",\"model_id\":\"IBS-TH1/TH2/P01B\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"sps\",\"|\",\"name\",\"index\",0,\"tps\",\"&\",\"manufacturerdata\",\"=\",18],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",0,4,true],\"post_proc\":[\"/\",100]},\"extprobe\":{\"condition\":[\"manufacturerdata\",9,\"!\",\"0\"],\"decoder\":[\"static_value\",true]},\"hum\":{\"condition\":[\"manufacturerdata\",4,\"!\",\"ffff\",\"&\",\"manufacturerdata\",4,\"!\",\"0000\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",4,4,true,false],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",14,2,false,false]}}}";
+const char* _IBS_THBP01B_json = "{\"brand\":\"Inkbird\",\"model\":\"T(H) Sensor\",\"model_id\":\"IBS-TH1/TH2/P01B\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"sps\",\"|\",\"name\",\"index\",0,\"tps\",\"&\",\"manufacturerdata\",\"=\",18],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",0,4,true],\"post_proc\":[\"/\",100]},\"extprobe\":{\"condition\":[\"manufacturerdata\",9,\"!\",\"0\"],\"decoder\":[\"static_value\",true]},\"hum\":{\"condition\":[\"manufacturerdata\",4,\"!\",\"ffff\",\"&\",\"manufacturerdata\",4,\"!\",\"0000\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",4,4,true,false],\"post_proc\":[\"/\",100]},\"batt\":{\"condition\":[\"manufacturerdata\",14,\"!\",\"f\",\"&\",\"manufacturerdata\",14,\"!\",\"e\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",14,2,false,false]}}}";
 /*R""""(
 {
    "brand":"Inkbird",
    "model":"T(H) Sensor",
    "model_id":"IBS-TH1/TH2/P01B",
    "tag":"0103",
    "condition":["name", "index", 0, "sps", "|", "name", "index", 0, "tps", "&", "manufacturerdata", "=", 18],
@@ -17,14 +17,15 @@
       },
       "hum":{
          "condition":["manufacturerdata", 4, "!", "ffff", "&", "manufacturerdata", 4, "!", "0000"],
          "decoder":["value_from_hex_data", "manufacturerdata", 4, 4, true, false],
          "post_proc":["/", 100]
       },
       "batt":{
+         "condition":["manufacturerdata", 14, "!", "f", "&", "manufacturerdata", 14, "!", "e"],
          "decoder":["value_from_hex_data", "manufacturerdata", 14, 2, false, false]
       }
    }
 })"""";*/
 
 const char* _IBS_THBP01B_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"extprobe\":{\"unit\":\"status\",\"name\":\"external probe connected\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"}}}";
 /*R""""(
```

### Comparing `TheengsDecoder-1.5.0/src/devices/IBT_2X_json.h` & `TheengsDecoder-1.5.1b0/src/devices/IBT_2X_json.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _IBT_2X_json_2XS = "{\"brand\":\"Inkbird\",\"model\":\"iBBQ\",\"model_id\":\"IBT-2X(S)\",\"tag\":\"0301\",\"condition\":[\"manufacturerdata\",\"=\",28,\"index\",0,\"00000000\",\"&\",\"manufacturerdata\",\"mac@index\",8],\"conditionnomac\":[\"name\",\"index\",0,\"iBBQ\",\"|\",\"name\",\"index\",0,\"xBBQ\",\"&\",\"manufacturerdata\",\"=\",28,\"index\",0,\"00000000\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",22,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true,false],\"post_proc\":[\"/\",10]},\"tempc2\":{\"condition\":[\"manufacturerdata\",26,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,true,false],\"post_proc\":[\"/\",10]}}}";
+const char* _IBT_2X_json_2XS = "{\"brand\":\"Inkbird\",\"model\":\"iBBQ\",\"model_id\":\"IBT-2X(S)\",\"tag\":\"0301\",\"condition\":[\"manufacturerdata\",\"=\",28,\"index\",0,\"00000000\",\"&\",\"manufacturerdata\",\"mac@index\",8],\"conditionnomac\":[\"name\",\"index\",0,\"iBBQ\",\"|\",\"name\",\"index\",0,\"xBBQ\",\"&\",\"manufacturerdata\",\"=\",28,\"index\",0,\"00000000\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",22,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true,false],\"post_proc\":[\"/\",10]},\"tempc2\":{\"condition\":[\"manufacturerdata\",26,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"manufacturerdata\",8]}}}";
 /*R""""(
 {
    "brand":"Inkbird",
    "model":"iBBQ",
    "model_id":"IBT-2X(S)",
    "tag":"0301",
    "condition":["manufacturerdata", "=", 28, "index", 0, "00000000", "&", "manufacturerdata", "mac@index", 8],
@@ -13,19 +13,22 @@
          "decoder":["value_from_hex_data", "manufacturerdata", 20, 4, true, false],
          "post_proc":["/", 10]
       },
       "tempc2":{
          "condition":["manufacturerdata", 26, "!", "ff"],
          "decoder":["value_from_hex_data", "manufacturerdata", 24, 4, true, false],
          "post_proc":["/", 10]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "manufacturerdata", 8]
       }
    }
 })"""";*/
 
-const char* _IBT_2X_json_2X = "{\"brand\":\"Inkbird\",\"model\":\"iBBQ\",\"model_id\":\"IBT-2X(S)\",\"tag\":\"0301\",\"condition\":[\"manufacturerdata\",\"=\",28,\"index\",0,\"01000000\",\"&\",\"manufacturerdata\",\"revmac@index\",8],\"conditionnomac\":[\"name\",\"index\",0,\"iBBQ\",\"|\",\"name\",\"index\",0,\"xBBQ\",\"&\",\"manufacturerdata\",\"=\",28,\"index\",0,\"01000000\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",22,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true,false],\"post_proc\":[\"/\",10]},\"tempc2\":{\"condition\":[\"manufacturerdata\",26,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,true,false],\"post_proc\":[\"/\",10]}}}";
+const char* _IBT_2X_json_2X = "{\"brand\":\"Inkbird\",\"model\":\"iBBQ\",\"model_id\":\"IBT-2X(S)\",\"tag\":\"0301\",\"condition\":[\"manufacturerdata\",\"=\",28,\"index\",0,\"01000000\",\"&\",\"manufacturerdata\",\"revmac@index\",8],\"conditionnomac\":[\"name\",\"index\",0,\"iBBQ\",\"|\",\"name\",\"index\",0,\"xBBQ\",\"&\",\"manufacturerdata\",\"=\",28,\"index\",0,\"01000000\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",22,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true,false],\"post_proc\":[\"/\",10]},\"tempc2\":{\"condition\":[\"manufacturerdata\",26,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"manufacturerdata\",8]}}}";
 /*R""""(
 {
    "brand":"Inkbird",
    "model":"iBBQ",
    "model_id":"IBT-2X(S)",
    "tag":"0301",
    "condition":["manufacturerdata", "=", 28, "index", 0, "01000000", "&", "manufacturerdata", "revmac@index", 8],
@@ -36,25 +39,32 @@
          "decoder":["value_from_hex_data", "manufacturerdata", 20, 4, true, false],
          "post_proc":["/", 10]
       },
       "tempc2":{
          "condition":["manufacturerdata", 26, "!", "ff"],
          "decoder":["value_from_hex_data", "manufacturerdata", 24, 4, true, false],
          "post_proc":["/", 10]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "manufacturerdata", 8]
       }
    }
 })"""";*/
 
-const char* _IBT_2X_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc2\":{\"unit\":\"°C\",\"name\":\"temperature\"}}}";
+const char* _IBT_2X_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc2\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "tempc":{
          "unit":"°C",
          "name":"temperature"
       },
       "tempc2":{
          "unit":"°C",
          "name":"temperature"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/IBT_4XS_json.h` & `TheengsDecoder-1.5.1b0/src/devices/IBT_4XS_json.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _IBT_4XS_json = "{\"brand\":\"Inkbird\",\"model\":\"iBBQ\",\"model_id\":\"IBT-4X(S/C)\",\"tag\":\"0301\",\"condition\":[\"manufacturerdata\",\"=\",36,\"index\",0,\"00000000\",\"&\",\"manufacturerdata\",\"mac@index\",8],\"conditionnomac\":[\"name\",\"index\",0,\"iBBQ\",\"&\",\"manufacturerdata\",\"=\",36,\"index\",0,\"00000000\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",22,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true,false],\"post_proc\":[\"/\",10]},\"tempc2\":{\"condition\":[\"manufacturerdata\",26,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"tempc3\":{\"condition\":[\"manufacturerdata\",30,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",28,4,true,false],\"post_proc\":[\"/\",10]},\"tempc4\":{\"condition\":[\"manufacturerdata\",34,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,4,true,false],\"post_proc\":[\"/\",10]}}}";
+const char* _IBT_4XS_json = "{\"brand\":\"Inkbird\",\"model\":\"iBBQ\",\"model_id\":\"IBT-4X(S/C)\",\"tag\":\"0301\",\"condition\":[\"manufacturerdata\",\"=\",36,\"index\",0,\"00000000\",\"&\",\"manufacturerdata\",\"mac@index\",8],\"conditionnomac\":[\"name\",\"index\",0,\"iBBQ\",\"&\",\"manufacturerdata\",\"=\",36,\"index\",0,\"00000000\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",22,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true,false],\"post_proc\":[\"/\",10]},\"tempc2\":{\"condition\":[\"manufacturerdata\",26,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"tempc3\":{\"condition\":[\"manufacturerdata\",30,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",28,4,true,false],\"post_proc\":[\"/\",10]},\"tempc4\":{\"condition\":[\"manufacturerdata\",34,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,4,true,false],\"post_proc\":[\"/\",10]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"manufacturerdata\",8]}}}";
 /*R""""(
 {
    "brand":"Inkbird",
    "model":"iBBQ",
    "model_id":"IBT-4X(S/C)",
    "tag":"0301",
    "condition":["manufacturerdata", "=" ,36 ,"index", 0, "00000000", "&", "manufacturerdata", "mac@index", 8],
@@ -23,19 +23,22 @@
          "decoder":["value_from_hex_data", "manufacturerdata", 28, 4, true, false],
          "post_proc":["/", 10]
       },
       "tempc4":{
          "condition":["manufacturerdata", 34, "!", "ff"],
          "decoder":["value_from_hex_data", "manufacturerdata", 32, 4, true, false],
          "post_proc":["/", 10]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "manufacturerdata", 8]
       }
    }
 })"""";*/
 
-const char* _IBT_4XS_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc2\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc3\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc4\":{\"unit\":\"°C\",\"name\":\"temperature\"}}}";
+const char* _IBT_4XS_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc2\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc3\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc4\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "tempc":{
          "unit":"°C",
          "name":"temperature"
       },
@@ -46,10 +49,14 @@
       "tempc3":{
          "unit":"°C",
          "name":"temperature"
       },
       "tempc4":{
          "unit":"°C",
          "name":"temperature"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/IBT_6XS_SOLIS6_json.h` & `TheengsDecoder-1.5.1b0/src/devices/IBT_6XS_SOLIS6_json.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _IBT_6XS_SOLIS6_json = "{\"brand\":\"Inkbird/Tenergy\",\"model\":\"iBBQ/SOLIS6\",\"model_id\":\"IBT-6XS/SOLIS-6\",\"tag\":\"0301\",\"condition\":[\"manufacturerdata\",\"=\",44,\"index\",0,\"00000000\",\"&\",\"manufacturerdata\",\"mac@index\",8],\"conditionnomac\":[\"name\",\"index\",0,\"iBBQ\",\"&\",\"manufacturerdata\",\"=\",44,\"index\",0,\"00000000\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",22,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true,false],\"post_proc\":[\"/\",10]},\"tempc2\":{\"condition\":[\"manufacturerdata\",26,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"tempc3\":{\"condition\":[\"manufacturerdata\",30,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",28,4,true,false],\"post_proc\":[\"/\",10]},\"tempc4\":{\"condition\":[\"manufacturerdata\",34,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,4,true,false],\"post_proc\":[\"/\",10]},\"tempc5\":{\"condition\":[\"manufacturerdata\",38,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",36,4,true,false],\"post_proc\":[\"/\",10]},\"tempc6\":{\"condition\":[\"manufacturerdata\",42,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",40,4,true,false],\"post_proc\":[\"/\",10]}}}";
+const char* _IBT_6XS_SOLIS6_json = "{\"brand\":\"Inkbird/Tenergy\",\"model\":\"iBBQ/SOLIS6\",\"model_id\":\"IBT-6XS/SOLIS-6\",\"tag\":\"0301\",\"condition\":[\"manufacturerdata\",\"=\",44,\"index\",0,\"00000000\",\"&\",\"manufacturerdata\",\"mac@index\",8],\"conditionnomac\":[\"name\",\"index\",0,\"iBBQ\",\"&\",\"manufacturerdata\",\"=\",44,\"index\",0,\"00000000\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",22,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true,false],\"post_proc\":[\"/\",10]},\"tempc2\":{\"condition\":[\"manufacturerdata\",26,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,true,false],\"post_proc\":[\"/\",10]},\"tempc3\":{\"condition\":[\"manufacturerdata\",30,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",28,4,true,false],\"post_proc\":[\"/\",10]},\"tempc4\":{\"condition\":[\"manufacturerdata\",34,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,4,true,false],\"post_proc\":[\"/\",10]},\"tempc5\":{\"condition\":[\"manufacturerdata\",38,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",36,4,true,false],\"post_proc\":[\"/\",10]},\"tempc6\":{\"condition\":[\"manufacturerdata\",42,\"!\",\"ff\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",40,4,true,false],\"post_proc\":[\"/\",10]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"manufacturerdata\",8]}}}";
 /*R""""(
 {
    "brand":"Inkbird/Tenergy",
    "model":"iBBQ/SOLIS6",
    "model_id":"IBT-6XS/SOLIS-6",
    "tag":"0301",
    "condition":["manufacturerdata", "=", 44, "index", 0, "00000000", "&", "manufacturerdata", "mac@index", 8],
@@ -33,19 +33,22 @@
          "decoder":["value_from_hex_data", "manufacturerdata", 36, 4, true, false],
          "post_proc":["/", 10]
       },
       "tempc6":{
          "condition":["manufacturerdata", 42, "!", "ff"],
          "decoder":["value_from_hex_data", "manufacturerdata", 40, 4, true, false],
          "post_proc":["/", 10]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "manufacturerdata", 8]
       }
    }
 })"""";*/
 
-const char* _IBT_6XS_SOLIS6_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc2\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc3\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc4\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc5\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc6\":{\"unit\":\"°C\",\"name\":\"temperature\"}}}";
+const char* _IBT_6XS_SOLIS6_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc2\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc3\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc4\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc5\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"tempc6\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "tempc":{
          "unit":"°C",
          "name":"temperature"
       },
@@ -64,10 +67,14 @@
       "tempc5":{
          "unit":"°C",
          "name":"temperature"
       },
       "tempc6":{
          "unit":"°C",
          "name":"temperature"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/JHT_F525_json.h` & `TheengsDecoder-1.5.1b0/src/devices/JHT_F525_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/JQJCY01YM_json.h` & `TheengsDecoder-1.5.1b0/src/devices/JQJCY01YM_json.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _JQJCY01YM_json = "{\"brand\":\"Xiaomi\",\"model\":\"Formaldehyde detector\",\"model_id\":\"JQJCY01YM\",\"tag\":\"0f\",\"condition\":[\"servicedata\",\"index\",2,\"20df02\"],\"properties\":{\"for\":{\"condition\":[\"servicedata\",23,\"0\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true],\"post_proc\":[\"/\",100]},\"hum\":{\"condition\":[\"servicedata\",23,\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true,false],\"post_proc\":[\"/\",10]},\"tempc\":{\"condition\":[\"servicedata\",23,\"4\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true,false],\"post_proc\":[\"/\",10]},\"batt\":{\"condition\":[\"servicedata\",23,\"a\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,2,false,false]}}}";
+const char* _JQJCY01YM_json = "{\"brand\":\"Xiaomi\",\"model\":\"Formaldehyde detector\",\"model_id\":\"JQJCY01YM\",\"tag\":\"0f\",\"condition\":[\"servicedata\",\"index\",2,\"20df02\"],\"properties\":{\"for\":{\"condition\":[\"servicedata\",23,\"0\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true],\"post_proc\":[\"/\",100]},\"hum\":{\"condition\":[\"servicedata\",23,\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true,false],\"post_proc\":[\"/\",10]},\"tempc\":{\"condition\":[\"servicedata\",23,\"4\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true,false],\"post_proc\":[\"/\",10]},\"batt\":{\"condition\":[\"servicedata\",23,\"a\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,2,false,false]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",10]}}}";
 /*R""""(
 {
    "brand":"Xiaomi",
    "model":"Formaldehyde detector",
    "model_id":"JQJCY01YM",
    "tag":"0f",
    "condition":["servicedata", "index", 2, "20df02"],
@@ -21,19 +21,22 @@
          "condition":["servicedata", 23, "4"],
          "decoder":["value_from_hex_data", "servicedata", 28, 4, true, false],
          "post_proc":["/", 10]
       },
       "batt":{
          "condition":["servicedata", 23, "a"],
          "decoder":["value_from_hex_data", "servicedata", 28, 2, false, false]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 10]
       }
    }
 })"""";*/
 
-const char* _JQJCY01YM_json_props = "{\"properties\":{\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"for\":{\"unit\":\"mg/m³\",\"name\":\"formaldehyde\"}}}";
+const char* _JQJCY01YM_json_props = "{\"properties\":{\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"for\":{\"unit\":\"mg/m³\",\"name\":\"formaldehyde\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "batt":{
          "unit":"%",
          "name":"battery"
       },
@@ -44,10 +47,14 @@
       "hum":{
          "unit":"%",
          "name":"humidity"
       },
       "for":{
          "unit":"mg/m³",
          "name":"formaldehyde"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/KKM_K6P_json.h` & `TheengsDecoder-1.5.1b0/src/devices/KKM_K6P_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/KKM_K9_json.h` & `TheengsDecoder-1.5.1b0/src/devices/KKM_K9_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/LYWSD02_json.h` & `TheengsDecoder-1.5.1b0/src/devices/ABN03_json.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,55 @@
-#include "common_props.h"
-
-const char* _LYWSD02_json = "{\"brand\":\"Xiaomi/Mijia\",\"model\":\"e-ink Clock\",\"model_id\":\"LYWSD02\",\"tag\":\"01\",\"condition\":[\"uuid\",\"index\",0,\"fe95\",\"&\",\"servicedata\",\"index\",4,\"5b04\"],\"properties\":{\"tempc\":{\"condition\":[\"servicedata\",24,\"0410\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"condition\":[\"servicedata\",24,\"0610\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,4,true,false],\"post_proc\":[\"/\",10]},\"batt\":{\"condition\":[\"servicedata\",24,\"0a10\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",30,2,false,false]}}}";
+const char* _ABN03_json = "{\"brand\":\"April Brother\",\"model\":\"N03\",\"model_id\":\"ABN03\",\"tag\":\"0208\",\"condition\":[\"servicedata\",\"=\",30,\"index\",0,\"ab03\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,4,true,true],\"post_proc\":[\"/\",8]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",22,4,true,false],\"post_proc\":[\"/\",2]},\"lux\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",26,4,true,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,2,false,false]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"servicedata\",4]}}}";
 /* R""""(
 {
-   "brand":"Xiaomi/Mijia",
-   "model":"e-ink Clock",
-   "model_id":"LYWSD02",
-   "tag":"01",
-   "condition":["uuid", "index", 0, "fe95", "&", "servicedata", "index", 4, "5b04"],
+   "brand":"April Brother",
+   "model":"N03",
+   "model_id":"ABN03",
+   "tag":"0208",
+   "condition":["servicedata", "=", 30, "index", 0, "ab03"],
    "properties":{
       "tempc":{
-         "condition":["servicedata", 24, "0410"],
-         "decoder":["value_from_hex_data", "servicedata", 30, 4, true],
-         "post_proc":["/", 10]
+         "decoder":["value_from_hex_data", "servicedata", 18, 4, true, true],
+         "post_proc":["/", 8]
       },
       "hum":{
-         "condition":["servicedata", 24, "0610"],
-         "decoder":["value_from_hex_data", "servicedata", 30, 4, true, false],
-         "post_proc":["/", 10]
+         "decoder":["value_from_hex_data", "servicedata", 22, 4, true, false],
+         "post_proc":["/", 2]
+      },
+      "lux":{
+         "decoder":["value_from_hex_data", "servicedata", 26, 4, true, false]
       },
       "batt":{
-         "condition":["servicedata", 24, "0a10"],
-         "decoder":["value_from_hex_data", "servicedata", 30, 2, false, false]
+         "decoder":["value_from_hex_data", "servicedata", 16, 2, false, false]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "servicedata", 4]
       }
    }
 })"""";*/
 
-const char* _LYWSD02_json_props = _common_BTH_props;
+const char* _ABN03_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"lux\":{\"unit\":\"lx\",\"name\":\"illuminance\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
+/*R""""(
+{
+   "properties":{
+      "tempc":{
+         "unit":"°C",
+         "name":"temperature"
+      },
+      "hum":{
+         "unit":"%",
+         "name":"humidity"
+      },
+      "lux":{
+         "unit":"lx",
+         "name":"illuminance"
+      },
+      "batt":{
+         "unit":"%",
+         "name":"battery"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
+      }
+   }
+})"""";*/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TheengsDecoder-1.5.0/src/devices/LYWSD03MMC_json.h` & `TheengsDecoder-1.5.1b0/src/devices/LYWSD03MMC_json.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "common_props.h"
 
-const char* _LYWSD03MMC_json_ATC = "{\"brand\":\"Xiaomi\",\"model\":\"TH Sensor\",\"model_id\":\"LYWSD03MMC/MJWSD05MMC_ATC\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",26,\"index\",0,\"a4c138\",\"&\",\"uuid\",\"index\",0,\"181a\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,false,true],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,2,false,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,2,false,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,false,false],\"post_proc\":[\"/\",1000]}}}";
+const char* _LYWSD03MMC_json_ATC = "{\"brand\":\"Xiaomi\",\"model\":\"TH Sensor\",\"model_id\":\"LYWSD03MMC/MJWSD05MMC_ATC\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",26,\"index\",0,\"a4c138\",\"&\",\"uuid\",\"index\",0,\"181a\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,false,true],\"post_proc\":[\"/\",10]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,2,false,false]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,2,false,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,false,false],\"post_proc\":[\"/\",1000]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"servicedata\",0]}}}";
 /* R""""(
 {
    "brand":"Xiaomi",
    "model":"TH Sensor",
    "model_id":"LYWSD03MMC/MJWSD05MMC_ATC",
    "tag":"01",
    "condition":["servicedata", "=", 26, "index", 0 , "a4c138", "&", "uuid", "index", 0, "181a"],
@@ -18,19 +18,22 @@
       },
       "batt":{
          "decoder":["value_from_hex_data", "servicedata", 18, 2, false, false]
       },
       "volt":{
          "decoder":["value_from_hex_data", "servicedata", 20, 4, false, false],
          "post_proc":["/", 1000]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "servicedata", 0]
       }
    }
 })"""";*/
 
-const char* _LYWSD03MMC_json_PVVX = "{\"brand\":\"Xiaomi\",\"model\":\"TH Sensor\",\"model_id\":\"LYWSD03MMC/MJWSD05MMC_PVVX\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",30,\"index\",6,\"38c1a4\",\"&\",\"uuid\",\"index\",0,\"181a\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,true,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,4,true,false],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,2,false,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true,false],\"post_proc\":[\"/\",1000]}}}";
+const char* _LYWSD03MMC_json_PVVX = "{\"brand\":\"Xiaomi\",\"model\":\"TH Sensor\",\"model_id\":\"LYWSD03MMC/MJWSD05MMC_PVVX\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",30,\"index\",6,\"38c1a4\",\"&\",\"uuid\",\"index\",0,\"181a\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,4,true,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,4,true,false],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",24,2,false,false]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",20,4,true,false],\"post_proc\":[\"/\",1000]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",0]}}}";
 /* R""""(
 {
    "brand":"Xiaomi",
    "model":"TH Sensor",
    "model_id":"LYWSD03MMC/MJWSD05MMC_PVVX",
    "tag":"01",
    "condition":["servicedata", "=", 30, "index", 6 , "38c1a4", "&", "uuid", "index", 0, "181a"],
@@ -45,12 +48,15 @@
       },
       "batt":{
          "decoder":["value_from_hex_data", "servicedata", 24, 2, false, false]
       },
       "volt":{
          "decoder":["value_from_hex_data", "servicedata", 20, 4, true, false],
          "post_proc":["/", 1000]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 0]
       }
    }
 })"""";*/
 
 const char* _LYWSD03MMC_json_props = _common_BVTH_props;
```

### Comparing `TheengsDecoder-1.5.0/src/devices/LYWSDCGQ_json.h` & `TheengsDecoder-1.5.1b0/src/devices/LYWSDCGQ_json.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "common_props.h"
 
-const char* _LYWSDCGQ_json = "{\"brand\":\"Xiaomi\",\"model\":\"Mi Jia round\",\"model_id\":\"LYWSDCGQ\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"index\",2,\"20aa01\"],\"properties\":{\"batt\":{\"condition\":[\"servicedata\",23,\"a\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,2,false,false]},\"tempc\":{\"condition\":[\"servicedata\",23,\"d\",\"|\",\"servicedata\",23,\"4\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"condition\":[\"servicedata\",23,\"d\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,true,false],\"post_proc\":[\"/\",10]},\"_hum\":{\"condition\":[\"servicedata\",23,\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true,false],\"post_proc\":[\"/\",10]}}}";
+const char* _LYWSDCGQ_json = "{\"brand\":\"Xiaomi\",\"model\":\"Mi Jia round\",\"model_id\":\"LYWSDCGQ\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"index\",2,\"20aa01\"],\"properties\":{\"batt\":{\"condition\":[\"servicedata\",23,\"a\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,2,false,false]},\"tempc\":{\"condition\":[\"servicedata\",23,\"d\",\"|\",\"servicedata\",23,\"4\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true],\"post_proc\":[\"/\",10]},\"hum\":{\"condition\":[\"servicedata\",23,\"d\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",32,4,true,false],\"post_proc\":[\"/\",10]},\"_hum\":{\"condition\":[\"servicedata\",23,\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",28,4,true,false],\"post_proc\":[\"/\",10]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"servicedata\",10]}}}";
 /*R""""(
 {
    "brand":"Xiaomi",
    "model":"Mi Jia round",
    "model_id":"LYWSDCGQ",
    "tag":"01",
    "condition":["servicedata", "index", 2, "20aa01"],
@@ -23,12 +23,15 @@
          "decoder":["value_from_hex_data", "servicedata", 32, 4, true, false],
          "post_proc":["/", 10]
       },
       "_hum":{
          "condition":["servicedata", 23, "6"],
          "decoder":["value_from_hex_data", "servicedata", 28, 4, true, false],
          "post_proc":["/", 10]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "servicedata", 10]
       }
    }
 })"""";*/
 
 const char* _LYWSDCGQ_json_props = _common_BTH_props;
```

### Comparing `TheengsDecoder-1.5.0/src/devices/MBXPRO_json.h` & `TheengsDecoder-1.5.1b0/src/devices/MBXPRO_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/MS_CDP_json.h` & `TheengsDecoder-1.5.1b0/src/devices/MS_CDP_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/MUE4094RT_json.h` & `TheengsDecoder-1.5.1b0/src/devices/MUE4094RT_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/Miband_json.h` & `TheengsDecoder-1.5.1b0/src/devices/Miband_json.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _Miband_json = "{\"brand\":\"Xiaomi/Amazfit\",\"model\":\"Mi Band/Smart Watch\",\"model_id\":\"MB/SW\",\"tag\":\"0b0a\",\"condition\":[\"manufacturerdata\",\"=\",52,\"index\",0,\"5701\",\"&\",\"manufacturerdata\",\"mac@index\",40],\"conditionnomac\":[\"uuid\",\"contain\",\"fee0\"],\"properties\":{\"steps\":{\"condition\":[\"servicedata\",\"=\",8],\"decoder\":[\"value_from_hex_data\",\"servicedata\",0,4,true,false]},\"act_bpm\":{\"condition\":[\"manufacturerdata\",0,\"570102\",\"&\",\"manufacturerdata\",10,\"!\",\"f\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",10,2,false,false]},\"device\":{\"decoder\":[\"static_value\",\"Xiaomi/Amazfit Tracker\"]}}}";
+const char* _Miband_json = "{\"brand\":\"Xiaomi/Amazfit\",\"model\":\"Mi Band/Smart Watch\",\"model_id\":\"MB/SW\",\"tag\":\"0b0a\",\"condition\":[\"manufacturerdata\",\"=\",52,\"index\",0,\"5701\",\"&\",\"manufacturerdata\",\"mac@index\",40],\"conditionnomac\":[\"uuid\",\"contain\",\"fee0\"],\"properties\":{\"steps\":{\"condition\":[\"servicedata\",\"=\",8],\"decoder\":[\"value_from_hex_data\",\"servicedata\",0,4,true,false]},\"act_bpm\":{\"condition\":[\"manufacturerdata\",0,\"570102\",\"&\",\"manufacturerdata\",10,\"!\",\"f\"],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",10,2,false,false]},\"device\":{\"decoder\":[\"static_value\",\"Xiaomi/Amazfit Tracker\"]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"manufacturerdata\",40]}}}";
 /*R""""(
 {
    "brand":"Xiaomi/Amazfit",
    "model":"Mi Band/Smart Watch",
    "model_id":"MB/SW",
    "tag":"0b0a",
    "condition":["manufacturerdata", "=", 52, "index", 0, "5701", "&", "manufacturerdata", "mac@index", 40],
@@ -14,29 +14,36 @@
       },
       "act_bpm":{
          "condition":["manufacturerdata", 0, "570102", "&", "manufacturerdata", 10, "!", "f"],
          "decoder":["value_from_hex_data", "manufacturerdata", 10, 2, false, false]
       },
       "device":{
          "decoder":["static_value", "Xiaomi/Amazfit Tracker"]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "manufacturerdata", 40]
       }
    }
 })"""";*/
 
-const char* _Miband_json_props = "{\"properties\":{\"steps\":{\"unit\":\"int\",\"name\":\"step-count\"},\"act_bpm\":{\"unit\":\"bpm\",\"name\":\"activity heart rate\"},\"device\":{\"unit\":\"string\",\"name\":\"tracker device\"}}}";
+const char* _Miband_json_props = "{\"properties\":{\"steps\":{\"unit\":\"int\",\"name\":\"step-count\"},\"act_bpm\":{\"unit\":\"bpm\",\"name\":\"activity heart rate\"},\"device\":{\"unit\":\"string\",\"name\":\"tracker device\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "steps":{
          "unit":"int",
          "name":"step-count"
       },
       "act_bpm":{
          "unit":"bpm",
          "name":"activity heart rate"
       },
       "device":{
          "unit":"string",
          "name":"tracker device"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/Mokobeacon_json.h` & `TheengsDecoder-1.5.1b0/src/devices/Mokobeacon_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/Mopeka_json.h` & `TheengsDecoder-1.5.1b0/src/devices/Mopeka_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/PH10_json.h` & `TheengsDecoder-1.5.1b0/src/devices/PH10_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/RDL52832_json.h` & `TheengsDecoder-1.5.1b0/src/devices/RDL52832_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/RuuviTag_RAWv1_json.h` & `TheengsDecoder-1.5.1b0/src/devices/RuuviTag_RAWv1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/RuuviTag_RAWv2_json.h` & `TheengsDecoder-1.5.1b0/src/devices/RuuviTag_RAWv2_json.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _RuuviTag_RAWv2_json = "{\"brand\":\"Ruuvi\",\"model\":\"RuuviTag\",\"model_id\":\"RuuviTag_RAWv2\",\"tag\":\"0708\",\"condition\":[\"manufacturerdata\",\"=\",52,\"index\",0,\"990405\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,4,false,true],\"post_proc\":[\"/\",200]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",10,4,false,false],\"post_proc\":[\"/\",400]},\"pres\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",14,4,false,false],\"post_proc\":[\"+\",50000,\"/\",100]},\"accx\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",18,4,false,true],\"post_proc\":[\"/\",10000,\"*\",9.80665]},\"accy\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",22,4,false,true],\"post_proc\":[\"/\",10000,\"*\",9.80665]},\"accz\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",26,4,false,true],\"post_proc\":[\"/\",10000,\"*\",9.80665]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",30,4,false,false],\"post_proc\":[\">\",5,\"+\",1600,\"/\",1000]},\"tx\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",30,4,false,false],\"post_proc\":[\"%\",32,\"*\",2,\"-\",40]},\"mov\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",34,2,false,false]},\"seq\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",36,4,false,false]}}}";
+const char* _RuuviTag_RAWv2_json = "{\"brand\":\"Ruuvi\",\"model\":\"RuuviTag\",\"model_id\":\"RuuviTag_RAWv2\",\"tag\":\"0708\",\"condition\":[\"manufacturerdata\",\"=\",52,\"index\",0,\"990405\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,4,false,true],\"post_proc\":[\"/\",200]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",10,4,false,false],\"post_proc\":[\"/\",400]},\"pres\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",14,4,false,false],\"post_proc\":[\"+\",50000,\"/\",100]},\"accx\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",18,4,false,true],\"post_proc\":[\"/\",10000,\"*\",9.80665]},\"accy\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",22,4,false,true],\"post_proc\":[\"/\",10000,\"*\",9.80665]},\"accz\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",26,4,false,true],\"post_proc\":[\"/\",10000,\"*\",9.80665]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",30,4,false,false],\"post_proc\":[\">\",5,\"+\",1600,\"/\",1000]},\"tx\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",30,4,false,false],\"post_proc\":[\"%\",32,\"*\",2,\"-\",40]},\"mov\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",34,2,false,false]},\"seq\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",36,4,false,false]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"manufacturerdata\",40]}}}";
 /*R""""(
 {
    "brand":"Ruuvi",
    "model":"RuuviTag",
    "model_id":"RuuviTag_RAWv2",
    "tag":"0708",
    "condition":["manufacturerdata", "=", 52, "index", 0, "990405"],
@@ -40,19 +40,22 @@
          "post_proc":["%", 32, "*", 2, "-", 40]
       },
       "mov":{
          "decoder":["value_from_hex_data", "manufacturerdata", 34, 2, false, false]
       },
       "seq":{
          "decoder":["value_from_hex_data", "manufacturerdata", 36, 4, false, false]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "manufacturerdata", 40]
       }
    }
 })"""";*/
 
-const char* _RuuviTag_RAWv2_json_props = "{\"properties\":{\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"pres\":{\"unit\":\"hPa\",\"name\":\"pressure\"},\"accx\":{\"unit\":\"m/s²\",\"name\":\"acceleration x\"},\"accy\":{\"unit\":\"m/s²\",\"name\":\"acceleration y\"},\"accz\":{\"unit\":\"m/s²\",\"name\":\"acceleration z\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"},\"tx\":{\"unit\":\"dBm\",\"name\":\"tx power\"},\"mov\":{\"unit\":\"int\",\"name\":\"movement counter\"},\"seq\":{\"unit\":\"int\",\"name\":\"measurement sequence number\"}}}";
+const char* _RuuviTag_RAWv2_json_props = "{\"properties\":{\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"pres\":{\"unit\":\"hPa\",\"name\":\"pressure\"},\"accx\":{\"unit\":\"m/s²\",\"name\":\"acceleration x\"},\"accy\":{\"unit\":\"m/s²\",\"name\":\"acceleration y\"},\"accz\":{\"unit\":\"m/s²\",\"name\":\"acceleration z\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"},\"tx\":{\"unit\":\"dBm\",\"name\":\"tx power\"},\"mov\":{\"unit\":\"int\",\"name\":\"movement counter\"},\"seq\":{\"unit\":\"int\",\"name\":\"measurement sequence number\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "hum":{
          "unit":"%",
          "name":"humidity"
       },
@@ -87,10 +90,14 @@
       "mov":{
          "unit":"int",
          "name":"movement counter"
       },
       "seq":{
          "unit":"int",
          "name":"measurement sequence number"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/SBBT_002C_json.h` & `TheengsDecoder-1.5.1b0/src/devices/SBBT_002C_json.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _SBBT_002C_json = "{\"brand\":\"Shelly\",\"model\":\"ShellyBLU Button1\",\"model_id\":\"SBBT-002C\",\"tag\":\"1106\",\"condition\":[\"servicedata\",\"=\",14,\"index\",0,\"40\",\"|\",\"servicedata\",\"=\",14,\"index\",0,\"44\",\"&\",\"uuid\",\"index\",0,\"fcd2\",\"&\",\"name\",\"index\",0,\"SBBT-002C\"],\"properties\":{\"packet\":{\"condition\":[\"servicedata\",2,\"00\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",4,2,false,false]},\"batt\":{\"condition\":[\"servicedata\",6,\"01\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",8,2,false,false]},\"press\":{\"condition\":[\"servicedata\",10,\"3a\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,2,false,false]}}}";
+const char* _SBBT_002C_json = "{\"brand\":\"Shelly\",\"model\":\"ShellyBLU Button1\",\"model_id\":\"SBBT-002C\",\"tag\":\"1106\",\"condition\":[\"servicedata\",\"=\",14,\"index\",0,\"40\",\"|\",\"servicedata\",\"=\",14,\"index\",0,\"44\",\"&\",\"uuid\",\"index\",0,\"fcd2\",\"&\",\"name\",\"index\",0,\"SBBT-002C\"],\"properties\":{\"packet\":{\"condition\":[\"servicedata\",2,\"00\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",4,2,false,false]},\"batt\":{\"condition\":[\"servicedata\",6,\"01\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",8,2,false,false]},\"press\":{\"condition\":[\"servicedata\",10,\"3a\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,2,false,false]},\"mac\":{\"condition\":[\"manufacturerdata\",\"=\",30],\"decoder\":[\"revmac_from_hex_data\",\"manufacturerdata\",18]}}}";
 /*R""""(
 {
    "brand":"Shelly",
    "model":"ShellyBLU Button1",
    "model_id":"SBBT-002C",
    "tag":"1106",
    "condition":["servicedata", "=", 14, "index", 0, "40", "|", "servicedata", "=", 14, "index", 0, "44", "&", "uuid", "index", 0, "fcd2", "&", "name", "index", 0, "SBBT-002C"],
@@ -14,29 +14,37 @@
       "batt":{
          "condition":["servicedata", 6, "01"],
          "decoder":["value_from_hex_data", "servicedata", 8, 2, false, false]
       },
       "press":{
          "condition":["servicedata", 10, "3a"],
          "decoder":["value_from_hex_data", "servicedata", 12, 2, false, false]
+      },
+      "mac":{
+         "condition":["manufacturerdata", "=", 30],
+         "decoder":["revmac_from_hex_data", "manufacturerdata", 18]
       }
    }
 })"""";*/
 
-const char* _SBBT_002C_json_props = "{\"properties\":{\"packet\":{\"unit\":\"int\",\"name\":\"packet id\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"press\":{\"unit\":\"int\",\"name\":\"press type\"}}}";
+const char* _SBBT_002C_json_props = "{\"properties\":{\"packet\":{\"unit\":\"int\",\"name\":\"packet id\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"press\":{\"unit\":\"int\",\"name\":\"press type\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "packet":{
          "unit":"int",
          "name":"packet id"
       },
       "batt":{
          "unit":"%",
          "name":"battery"
       },
       "press":{
          "unit":"int",
          "name":"press type"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/SBCS_json.h` & `TheengsDecoder-1.5.1b0/src/devices/SBCS_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/SBCU_json.h` & `TheengsDecoder-1.5.1b0/src/devices/SBCU_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/SBMS_json.h` & `TheengsDecoder-1.5.1b0/src/devices/SBMS_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/SBMT_json.h` & `TheengsDecoder-1.5.1b0/src/devices/SBMT_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/SBOT_json.h` & `TheengsDecoder-1.5.1b0/src/devices/SBOT_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/SBS1_json.h` & `TheengsDecoder-1.5.1b0/src/devices/XMTZC04HM_json.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-const char* _SBS1_json = "{\"brand\":\"SwitchBot\",\"model\":\"Bot\",\"model_id\":\"X1\",\"tag\":\"0e02\",\"condition\":[\"uuid\",\"index\",0,\"0d00\",\"|\",\"uuid\",\"index\",0,\"fd3d\",\"&\",\"servicedata\",\"=\",6,\"index\",0,\"48\"],\"properties\":{\"mode\":{\"decoder\":[\"bit_static_value\",\"servicedata\",2,3,\"onestate\",\"on/off\"]},\"state\":{\"decoder\":[\"bit_static_value\",\"servicedata\",2,2,\"on\",\"off\"]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",4,2,false,false],\"post_proc\":[\"&\",127]}}}";
+const char* _XMTZC04HM_json = "{\"brand\":\"Xiaomi\",\"model\":\"Mi Smart Scale\",\"model_id\":\"XMTZC01HM/XMTZC04HM\",\"tag\":\"05\",\"condition\":[\"servicedata\",\"index\",0,\"2\",\"|\",\"servicedata\",\"index\",0,\"a\",\"|\",\"servicedata\",\"index\",0,\"6\",\"|\",\"servicedata\",\"index\",0,\"e\",\"&\",\"uuid\",\"contain\",\"181d\"],\"properties\":{\"weighing_mode\":{\"decoder\":[\"bit_static_value\",\"servicedata\",0,2,\"person\",\"object\"]},\"unit\":{\"decoder\":[\"bit_static_value\",\"servicedata\",1,0,\"kg\",\"lb\"]},\"weight\":{\"condition\":[\"servicedata\",1,\"2\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",2,4,true,false],\"post_proc\":[\"/\",200]},\"_weight\":{\"condition\":[\"servicedata\",1,\"3\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",2,4,true,false],\"post_proc\":[\"/\",100]}}}";
 /*R""""(
 {
-   "brand":"SwitchBot",
-   "model":"Bot",
-   "model_id":"X1",
-   "tag":"0e02",
-   "condition":["uuid", "index", 0, "0d00", "|", "uuid", "index", 0, "fd3d", "&", "servicedata", "=", 6, "index", 0, "48"],
+   "brand":"Xiaomi",
+   "model":"Mi Smart Scale",
+   "model_id":"XMTZC01HM/XMTZC04HM",
+   "tag":"05",
+   "condition":["servicedata", "index", 0, "2", "|", "servicedata", "index", 0, "a", "|", "servicedata", "index", 0, "6", "|", "servicedata", "index", 0, "e", "&", "uuid", "contain", "181d"],
    "properties":{
-      "mode":{
-         "decoder":["bit_static_value", "servicedata", 2, 3, "onestate", "on/off"]
+      "weighing_mode":{
+         "decoder":["bit_static_value", "servicedata", 0, 2, "person", "object"]
       },
-      "state":{
-         "decoder":["bit_static_value", "servicedata", 2, 2, "on", "off"]
+      "unit":{
+         "decoder":["bit_static_value", "servicedata", 1, 0, "kg", "lb"]
       },
-      "batt":{
-         "decoder":["value_from_hex_data", "servicedata", 4, 2, false, false],
-         "post_proc":["&", 127]
+      "weight":{
+         "condition":["servicedata", 1, "2"],
+         "decoder":["value_from_hex_data", "servicedata", 2, 4, true, false],
+         "post_proc":["/", 200]
+      },
+      "_weight":{
+         "condition":["servicedata", 1, "3"],
+         "decoder":["value_from_hex_data", "servicedata", 2, 4, true, false],
+         "post_proc":["/", 100]
       }
    }
 })"""";*/
 
-const char* _SBS1_json_props = "{\"properties\":{\"mode\":{\"unit\":\"string\",\"name\":\"mode\"},\"state\":{\"unit\":\"string\",\"name\":\"state\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"}}}";
+const char* _XMTZC04HM_json_props = "{\"properties\":{\"weighing_mode\":{\"unit\":\"string\",\"name\":\"weighing_mode\"},\"weight\":{\"unit\":\"kg\",\"name\":\"weight\"}}}";
 /*R""""(
 {
    "properties":{
-      "mode":{
-         "unit":"string",
-         "name":"mode"
-      },
-      "state":{
+      "weighing_mode":{
          "unit":"string",
-         "name":"state"
+         "name":"weighing_mode"
       },
-      "batt":{
-         "unit":"%",
-         "name":"battery"
+      "weight":{
+         "unit":"kg",
+         "name":"weight"
       }
    }
-})"""";*/
+})"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/SCD4X_json.h` & `TheengsDecoder-1.5.1b0/src/devices/SCD4X_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/SHT4X_json.h` & `TheengsDecoder-1.5.1b0/src/devices/SHT4X_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/ServiceData_json.h` & `TheengsDecoder-1.5.1b0/src/devices/ServiceData_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/Skale_json.h` & `TheengsDecoder-1.5.1b0/src/devices/Skale_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/SmartDry_json.h` & `TheengsDecoder-1.5.1b0/src/devices/SmartDry_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/T201_json.h` & `TheengsDecoder-1.5.1b0/src/devices/T201_json.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "common_props.h"
 
-const char* _T201_json = "{\"brand\":\"Oria\",\"model\":\"TH Sensor\",\"model_id\":\"T201\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"T201\",\"&\",\"manufacturerdata\",\">=\",38],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,false,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",28,4,false,false],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,2,false,false]}}}";
+const char* _T201_json = "{\"brand\":\"Oria\",\"model\":\"TH Sensor\",\"model_id\":\"T201\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"T201\",\"&\",\"manufacturerdata\",\">=\",38],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,false,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",28,4,false,false],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,2,false,false]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"manufacturerdata\",8]}}}";
 /*R""""(
 {
    "brand":"Oria",
    "model":"TH Sensor",
    "model_id":"T201",
    "tag":"0103",
    "condition":["name", "index", 0, "T201", "&", "manufacturerdata", ">=", 38],
@@ -15,12 +15,15 @@
       },
       "hum":{
          "decoder":["value_from_hex_data", "manufacturerdata", 28, 4, false, false],
          "post_proc":["/", 100]
       },
       "batt":{
          "decoder":["value_from_hex_data", "manufacturerdata", 32, 2, false, false]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "manufacturerdata", 8]
       }
    }
 })"""";*/
 
 const char* _T201_json_props = _common_BTH_props;
```

### Comparing `TheengsDecoder-1.5.0/src/devices/T301_json.h` & `TheengsDecoder-1.5.1b0/src/devices/T301_json.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "common_props.h"
 
-const char* _T301_json = "{\"brand\":\"Oria\",\"model\":\"TH Sensor\",\"model_id\":\"T301\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"T301\",\"&\",\"manufacturerdata\",\"=\",38],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,false,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",28,4,false,false],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,2,false,false]}}}";
+const char* _T301_json = "{\"brand\":\"Oria\",\"model\":\"TH Sensor\",\"model_id\":\"T301\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"T301\",\"&\",\"manufacturerdata\",\"=\",38],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,false,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",28,4,false,false],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,2,false,false]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"manufacturerdata\",8]}}}";
 /*R""""(
 {
    "brand":"Oria",
    "model":"TH Sensor",
    "model_id":"T301",
    "tag":"0103",
    "condition":["name", "index", 0, "T301", "&", "manufacturerdata", "=", 38],
@@ -15,12 +15,15 @@
       },
       "hum":{
          "decoder":["value_from_hex_data", "manufacturerdata", 28, 4, false, false],
          "post_proc":["/", 100]
       },
       "batt":{
          "decoder":["value_from_hex_data", "manufacturerdata", 32, 2, false, false]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "manufacturerdata", 8]
       }
    }
 })"""";*/
 
 const char* _T301_json_props = _common_BTH_props;
```

### Comparing `TheengsDecoder-1.5.0/src/devices/TPMS_json.h` & `TheengsDecoder-1.5.1b0/src/devices/TPMS_json.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _TPMS_json = "{\"brand\":\"GENERIC\",\"model\":\"TPMS\",\"model_id\":\"TPMS\",\"tag\":\"0a01\",\"condition\":[\"manufacturerdata\",\"=\",36,\"index\",0,\"000\",\"&\",\"manufacturerdata\",\"mac@index\",4],\"conditionnomac\":[\"manufacturerdata\",\"=\",36,\"&\",\"name\",\"index\",0,\"TPMS\"],\"properties\":{\"count\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",5,1,false],\"post_proc\":[\"+\",1]},\"pres\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",16,8,true],\"post_proc\":[\"/\",100000]},\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,8,true],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,2,true]},\"alarm\":{\"decoder\":[\"bit_static_value\",\"manufacturerdata\",35,0,false,true]}}}";
+const char* _TPMS_json = "{\"brand\":\"GENERIC\",\"model\":\"TPMS\",\"model_id\":\"TPMS\",\"tag\":\"0a01\",\"condition\":[\"manufacturerdata\",\"=\",36,\"index\",0,\"000\",\"&\",\"manufacturerdata\",\"mac@index\",4],\"conditionnomac\":[\"manufacturerdata\",\"=\",36,\"&\",\"name\",\"index\",0,\"TPMS\"],\"properties\":{\"count\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",5,1,false],\"post_proc\":[\"+\",1]},\"pres\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",16,8,true],\"post_proc\":[\"/\",100000]},\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,8,true],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,2,true]},\"alarm\":{\"decoder\":[\"bit_static_value\",\"manufacturerdata\",35,0,false,true]},\"mac\":{\"decoder\":[\"mac_from_hex_data\",\"manufacturerdata\",4]}}}";
 /*R""""(
 {
    "brand":"GENERIC",
    "model":"TPMS",
    "model_id":"TPMS",
    "tag":"0a01",
    "condition":["manufacturerdata", "=", 36, "index", 0, "000", "&", "manufacturerdata", "mac@index", 4],
@@ -21,19 +21,22 @@
          "post_proc":["/", 100]
       },
       "batt":{
          "decoder":["value_from_hex_data", "manufacturerdata", 32, 2, true]
       },
       "alarm":{
          "decoder":["bit_static_value", "manufacturerdata", 35, 0, false, true]
+      },
+      "mac":{
+         "decoder":["mac_from_hex_data", "manufacturerdata", 4]
       }
    }
 })"""";*/
 
-const char* _TPMS_json_props = "{\"properties\":{\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"pres\":{\"unit\":\"bar\",\"name\":\"pressure\"},\"count\":{\"unit\":\"int\",\"name\":\"count\"},\"alarm\":{\"unit\":\"status\",\"name\":\"alarm\"}}}";
+const char* _TPMS_json_props = "{\"properties\":{\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"pres\":{\"unit\":\"bar\",\"name\":\"pressure\"},\"count\":{\"unit\":\"int\",\"name\":\"count\"},\"alarm\":{\"unit\":\"status\",\"name\":\"alarm\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "batt":{
          "unit":"%",
          "name":"battery"
       },
@@ -48,10 +51,14 @@
       "count":{
          "unit":"int",
          "name":"count"
       },
       "alarm":{
          "unit":"status",
          "name":"alarm"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/TPTH_json.h` & `TheengsDecoder-1.5.1b0/src/devices/TPTH_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices/ThermoBeacon_json.h` & `TheengsDecoder-1.5.1b0/src/devices/ThermoBeacon_json.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _ThermoBeacon_json = "{\"brand\":\"GENERIC\",\"model\":\"ThermoBeacon\",\"model_id\":\"WS02/WS08\",\"tag\":\"0101\",\"condition\":[\"manufacturerdata\",\"index\",0,\"1000\",\"|\",\"manufacturerdata\",\"index\",0,\"1100\",\"|\",\"manufacturerdata\",\"index\",0,\"1500\",\"|\",\"manufacturerdata\",\"index\",0,\"1800\",\"|\",\"manufacturerdata\",\"index\",0,\"1b00\",\"&\",\"manufacturerdata\",\">=\",40],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,true],\"post_proc\":[\"/\",16]},\"hum\":{\"condition\":[\"manufacturerdata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",28,4,true],\"post_proc\":[\"/\",16]},\"volt\":{\"condition\":[\"manufacturerdata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true],\"post_proc\":[\"/\",1000]},\"time\":{\"condition\":[\"manufacturerdata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,8,true,false]},\"tempc_max\":{\"condition\":[\"manufacturerdata\",\"=\",44],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true],\"post_proc\":[\"/\",16]},\"time_max\":{\"condition\":[\"manufacturerdata\",\"=\",44],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,8,true,false]},\"tempc_min\":{\"condition\":[\"manufacturerdata\",\"=\",44],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,4,true],\"post_proc\":[\"/\",16]},\"time_min\":{\"condition\":[\"manufacturerdata\",\"=\",44],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",36,8,true,false]}}}";
+const char* _ThermoBeacon_json = "{\"brand\":\"GENERIC\",\"model\":\"ThermoBeacon\",\"model_id\":\"WS02/WS08\",\"tag\":\"0101\",\"condition\":[\"manufacturerdata\",\"index\",0,\"1000\",\"|\",\"manufacturerdata\",\"index\",0,\"1100\",\"|\",\"manufacturerdata\",\"index\",0,\"1500\",\"|\",\"manufacturerdata\",\"index\",0,\"1800\",\"|\",\"manufacturerdata\",\"index\",0,\"1b00\",\"&\",\"manufacturerdata\",\">=\",40],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,4,true],\"post_proc\":[\"/\",16]},\"hum\":{\"condition\":[\"manufacturerdata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",28,4,true],\"post_proc\":[\"/\",16]},\"volt\":{\"condition\":[\"manufacturerdata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true],\"post_proc\":[\"/\",1000]},\"time\":{\"condition\":[\"manufacturerdata\",\"=\",40],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,8,true,false]},\"tempc_max\":{\"condition\":[\"manufacturerdata\",\"=\",44],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,4,true],\"post_proc\":[\"/\",16]},\"time_max\":{\"condition\":[\"manufacturerdata\",\"=\",44],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,8,true,false]},\"tempc_min\":{\"condition\":[\"manufacturerdata\",\"=\",44],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,4,true],\"post_proc\":[\"/\",16]},\"time_min\":{\"condition\":[\"manufacturerdata\",\"=\",44],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",36,8,true,false]},\"mac\":{\"decoder\":[\"revmac_from_hex_data\",\"manufacturerdata\",8]}}}";
 /*R""""(
 {
    "brand":"GENERIC",
    "model":"ThermoBeacon",
    "model_id":"WS02/WS08",
    "tag":"0101",
    "condition":["manufacturerdata", "index", 0, "1000", "|", "manufacturerdata", "index", 0, "1100", "|", "manufacturerdata", "index", 0, "1500", "|", "manufacturerdata", "index", 0, "1800", "|", "manufacturerdata", "index", 0, "1b00", "&", "manufacturerdata", ">=", 40],
@@ -39,19 +39,22 @@
          "condition":["manufacturerdata", "=", 44],
          "decoder":["value_from_hex_data", "manufacturerdata", 32, 4, true],
          "post_proc":["/", 16]
       },
       "time_min":{
          "condition":["manufacturerdata", "=", 44],
          "decoder":["value_from_hex_data", "manufacturerdata", 36, 8, true, false]
+      },
+      "mac":{
+         "decoder":["revmac_from_hex_data", "manufacturerdata", 8]
       }
    }
 })"""";*/
 
-const char* _ThermoBeacon_json_props = "{\"properties\":{\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"time\":{\"unit\":\"int\",\"name\":\"timestamp\"},\"tempc_max\":{\"unit\":\"°C\",\"name\":\"maximum temperature\"},\"time_max\":{\"unit\":\"int\",\"name\":\"maximum temperature timestamp\"},\"tempc_min\":{\"unit\":\"°C\",\"name\":\"minimum temperature\"},\"time_min\":{\"unit\":\"int\",\"name\":\"minimum temperature timestamp\"}}}";
+const char* _ThermoBeacon_json_props = "{\"properties\":{\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"time\":{\"unit\":\"int\",\"name\":\"timestamp\"},\"tempc_max\":{\"unit\":\"°C\",\"name\":\"maximum temperature\"},\"time_max\":{\"unit\":\"int\",\"name\":\"maximum temperature timestamp\"},\"tempc_min\":{\"unit\":\"°C\",\"name\":\"minimum temperature\"},\"time_min\":{\"unit\":\"int\",\"name\":\"minimum temperature timestamp\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "volt":{
          "unit":"V",
          "name":"voltage"
       },
@@ -78,10 +81,14 @@
       "tempc_min":{
          "unit":"°C",
          "name":"minimum temperature"
       },
       "time_min":{
          "unit":"int",
          "name":"minimum temperature timestamp"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.5.0/src/devices/XMTZC04HM_json.h` & `TheengsDecoder-1.5.1b0/src/devices/XMTZC05HM_json.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,50 @@
-const char* _XMTZC04HM_json = "{\"brand\":\"Xiaomi\",\"model\":\"Mi Smart Scale\",\"model_id\":\"XMTZC01HM/XMTZC04HM\",\"tag\":\"05\",\"condition\":[\"servicedata\",\"index\",0,\"2\",\"|\",\"servicedata\",\"index\",0,\"a\",\"|\",\"servicedata\",\"index\",0,\"6\",\"|\",\"servicedata\",\"index\",0,\"e\",\"&\",\"uuid\",\"contain\",\"181d\"],\"properties\":{\"weighing_mode\":{\"decoder\":[\"bit_static_value\",\"servicedata\",0,2,\"person\",\"object\"]},\"unit\":{\"decoder\":[\"bit_static_value\",\"servicedata\",1,0,\"kg\",\"lb\"]},\"weight\":{\"condition\":[\"servicedata\",1,\"2\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",2,4,true,false],\"post_proc\":[\"/\",200]},\"_weight\":{\"condition\":[\"servicedata\",1,\"3\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",2,4,true,false],\"post_proc\":[\"/\",100]}}}";
+const char* _XMTZC05HM_json = "{\"brand\":\"Xiaomi\",\"model\":\"Mi Body Composition Scale\",\"model_id\":\"XMTZC02HM/XMTZC05HM\",\"tag\":\"05\",\"condition\":[\"servicedata\",\"index\",2,\"2\",\"|\",\"servicedata\",\"index\",2,\"a\",\"&\",\"uuid\",\"contain\",\"181b\"],\"properties\":{\"weighing_mode\":{\"decoder\":[\"bit_static_value\",\"servicedata\",1,2,\"person\",\"object\"]},\"unit\":{\"decoder\":[\"bit_static_value\",\"servicedata\",1,0,\"kg\",\"lb\"]},\"weight\":{\"condition\":[\"servicedata\",1,\"bit\",0,0],\"decoder\":[\"value_from_hex_data\",\"servicedata\",22,4,true,false],\"post_proc\":[\"/\",200]},\"_weight\":{\"condition\":[\"servicedata\",1,\"bit\",0,1],\"decoder\":[\"value_from_hex_data\",\"servicedata\",22,4,true,false],\"post_proc\":[\"/\",100]},\"impedance\":{\"condition\":[\"servicedata\",3,\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,4,true,false]}}}";
 /*R""""(
 {
    "brand":"Xiaomi",
-   "model":"Mi Smart Scale",
-   "model_id":"XMTZC01HM/XMTZC04HM",
+   "model":"Mi Body Composition Scale",
+   "model_id":"XMTZC02HM/XMTZC05HM",
    "tag":"05",
-   "condition":["servicedata", "index", 0, "2", "|", "servicedata", "index", 0, "a", "|", "servicedata", "index", 0, "6", "|", "servicedata", "index", 0, "e", "&", "uuid", "contain", "181d"],
+   "condition":["servicedata", "index", 2, "2", "|", "servicedata", "index", 2, "a", "&", "uuid", "contain", "181b"],
    "properties":{
       "weighing_mode":{
-         "decoder":["bit_static_value", "servicedata", 0, 2, "person", "object"]
+         "decoder":["bit_static_value", "servicedata", 1, 2, "person", "object"]
       },
       "unit":{
          "decoder":["bit_static_value", "servicedata", 1, 0, "kg", "lb"]
       },
       "weight":{
-         "condition":["servicedata", 1, "2"],
-         "decoder":["value_from_hex_data", "servicedata", 2, 4, true, false],
+         "condition":["servicedata", 1, "bit", 0, 0],
+         "decoder":["value_from_hex_data", "servicedata", 22, 4, true, false],
          "post_proc":["/", 200]
       },
       "_weight":{
-         "condition":["servicedata", 1, "3"],
-         "decoder":["value_from_hex_data", "servicedata", 2, 4, true, false],
+         "condition":["servicedata", 1, "bit", 0, 1],
+         "decoder":["value_from_hex_data", "servicedata", 22, 4, true, false],
          "post_proc":["/", 100]
+      },
+      "impedance":{
+         "condition":["servicedata", 3, "6"],
+         "decoder":["value_from_hex_data", "servicedata", 18, 4, true, false]
       }
    }
 })"""";*/
 
-const char* _XMTZC04HM_json_props = "{\"properties\":{\"weighing_mode\":{\"unit\":\"string\",\"name\":\"weighing_mode\"},\"weight\":{\"unit\":\"kg\",\"name\":\"weight\"}}}";
+const char* _XMTZC05HM_json_props = "{\"properties\":{\"weighing_mode\":{\"unit\":\"string\",\"name\":\"weighing_mode\"},\"weight\":{\"unit\":\"kg\",\"name\":\"weight\"},\"impedance\":{\"unit\":\"Ω\",\"name\":\"impedance\"}}}";
 /*R""""(
 {
    "properties":{
       "weighing_mode":{
          "unit":"string",
          "name":"weighing_mode"
       },
       "weight":{
          "unit":"kg",
          "name":"weight"
+      },
+      "impedance":{
+         "unit":"Ω",
+         "name":"impedance"
       }
    }
-})"""";*/
+})"""";*/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TheengsDecoder-1.5.0/src/devices/XMTZC05HM_json.h` & `TheengsDecoder-1.5.1b0/src/devices/iBeacon_json.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,64 @@
-const char* _XMTZC05HM_json = "{\"brand\":\"Xiaomi\",\"model\":\"Mi Body Composition Scale\",\"model_id\":\"XMTZC02HM/XMTZC05HM\",\"tag\":\"05\",\"condition\":[\"servicedata\",\"index\",2,\"2\",\"|\",\"servicedata\",\"index\",2,\"a\",\"&\",\"uuid\",\"contain\",\"181b\"],\"properties\":{\"weighing_mode\":{\"decoder\":[\"bit_static_value\",\"servicedata\",1,2,\"person\",\"object\"]},\"unit\":{\"decoder\":[\"bit_static_value\",\"servicedata\",1,0,\"kg\",\"lb\"]},\"weight\":{\"condition\":[\"servicedata\",1,\"bit\",0,0],\"decoder\":[\"value_from_hex_data\",\"servicedata\",22,4,true,false],\"post_proc\":[\"/\",200]},\"_weight\":{\"condition\":[\"servicedata\",1,\"bit\",0,1],\"decoder\":[\"value_from_hex_data\",\"servicedata\",22,4,true,false],\"post_proc\":[\"/\",100]},\"impedance\":{\"condition\":[\"servicedata\",3,\"6\"],\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,4,true,false]}}}";
+const char* _ibeacon_json = "{\"brand\":\"GENERIC\",\"model\":\"iBeacon\",\"model_id\":\"IBEACON\",\"tag\":\"06\",\"condition\":[\"manufacturerdata\",\"=\",50,\"index\",0,\"4c00\"],\"properties\":{\"mfid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",0,4]},\"uuid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",8,32]},\"major\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",40,4,false]},\"minor\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",44,4,false]},\"txpower\":{\"condition\":[\"manufacturerdata\",48,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",48,2,false]},\"volt\":{\"condition\":[\"manufacturerdata\",48,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",48,2,false],\"post_proc\":[\"/\",10]}}}";
+
 /*R""""(
 {
-   "brand":"Xiaomi",
-   "model":"Mi Body Composition Scale",
-   "model_id":"XMTZC02HM/XMTZC05HM",
-   "tag":"05",
-   "condition":["servicedata", "index", 2, "2", "|", "servicedata", "index", 2, "a", "&", "uuid", "contain", "181b"],
+   "brand":"GENERIC",
+   "model":"iBeacon",
+   "model_id":"IBEACON",
+   "tag":"06",
+   "condition":["manufacturerdata", "=", 50, "index", 0, "4c00"],
    "properties":{
-      "weighing_mode":{
-         "decoder":["bit_static_value", "servicedata", 1, 2, "person", "object"]
+      "mfid":{
+         "decoder":["string_from_hex_data", "manufacturerdata", 0, 4]
+      },
+      "uuid":{
+         "decoder":["string_from_hex_data", "manufacturerdata", 8, 32]
       },
-      "unit":{
-         "decoder":["bit_static_value", "servicedata", 1, 0, "kg", "lb"]
+      "major":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 40, 4, false]
       },
-      "weight":{
-         "condition":["servicedata", 1, "bit", 0, 0],
-         "decoder":["value_from_hex_data", "servicedata", 22, 4, true, false],
-         "post_proc":["/", 200]
-      },
-      "_weight":{
-         "condition":["servicedata", 1, "bit", 0, 1],
-         "decoder":["value_from_hex_data", "servicedata", 22, 4, true, false],
-         "post_proc":["/", 100]
-      },
-      "impedance":{
-         "condition":["servicedata", 3, "6"],
-         "decoder":["value_from_hex_data", "servicedata", 18, 4, true, false]
+      "minor":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 44, 4, false]
+      },
+      "txpower":{
+         "condition":["manufacturerdata", 48, "bit", 3, 1],
+         "decoder":["value_from_hex_data","manufacturerdata", 48, 2, false]
+      },
+      "volt":{
+         "condition":["manufacturerdata", 48, "bit", 3, 0],
+         "decoder":["value_from_hex_data","manufacturerdata", 48, 2, false],
+         "post_proc":["/", 10]
       }
    }
 })"""";*/
 
-const char* _XMTZC05HM_json_props = "{\"properties\":{\"weighing_mode\":{\"unit\":\"string\",\"name\":\"weighing_mode\"},\"weight\":{\"unit\":\"kg\",\"name\":\"weight\"},\"impedance\":{\"unit\":\"Ω\",\"name\":\"impedance\"}}}";
+const char* _ibeacon_json_props = "{\"properties\":{\"mfid\":{\"unit\":\"hex\",\"name\":\"manufacturer id\"},\"uuid\":{\"unit\":\"hex\",\"name\":\"service uuid\"},\"major\":{\"unit\":\"hex\",\"name\":\"major value\"},\"minor\":{\"unit\":\"hex\",\"name\":\"minor value\"},\"txpower\":{\"unit\":\"dBm\",\"name\":\"tx power @ 1 m\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"}}}";
 /*R""""(
 {
    "properties":{
-      "weighing_mode":{
-         "unit":"string",
-         "name":"weighing_mode"
-      },
-      "weight":{
-         "unit":"kg",
-         "name":"weight"
-      },
-      "impedance":{
-         "unit":"Ω",
-         "name":"impedance"
+      "mfid":{
+         "unit":"hex",
+         "name":"manufacturer id"
+      },
+      "uuid":{
+         "unit":"hex",
+         "name":"service uuid"
+      },
+      "major":{
+         "unit":"hex",
+         "name":"major value"
+      },
+      "minor":{
+         "unit":"hex",
+         "name":"minor value"
+      },
+      "txpower":{
+         "unit":"dBm",
+         "name":"tx power @ 1 m"
+      },
+      "volt":{
+         "unit":"V",
+         "name":"voltage"
       }
    }
-})"""";*/
+})"""";*/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `TheengsDecoder-1.5.0/src/devices/common_props.h` & `TheengsDecoder-1.5.1b0/src/devices/common_props.h`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       "hum":{
          "unit":"%",
          "name":"humidity"
       }
    }
 })"""";*/
 
-const char* _common_BTH_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"}}}";
+const char* _common_BTH_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*
 R""""(
 {
    "properties":{
       "tempc":{
          "unit":"°C",
          "name":"temperature"
@@ -28,19 +28,23 @@
       "hum":{
          "unit":"%",
          "name":"humidity"
       },
       "batt":{
          "unit":"%",
          "name":"battery"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
 
-const char* _common_BVTH_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"}}}";
+const char* _common_BVTH_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"},\"mac\":{\"unit\":\"string\",\"name\":\"MAC address\"}}}";
 /*R""""(
 {
    "properties":{
       "tempc":{
          "unit":"°C",
          "name":"temperature"
       },
@@ -51,12 +55,16 @@
       "batt":{
          "unit":"%",
          "name":"battery"
       },
       "volt":{
          "unit":"V",
          "name":"voltage"
+      },
+      "mac":{
+         "unit":"string",
+         "name":"MAC address"
       }
    }
 })"""";*/
 
 #endif
```

### Comparing `TheengsDecoder-1.5.0/src/devices/iBeacon_json.h` & `TheengsDecoder-1.5.1b0/src/devices/iNodeEM_json.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,72 @@
-const char* _ibeacon_json = "{\"brand\":\"GENERIC\",\"model\":\"iBeacon\",\"model_id\":\"IBEACON\",\"tag\":\"06\",\"condition\":[\"manufacturerdata\",\"=\",50,\"index\",0,\"4c00\"],\"properties\":{\"mfid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",0,4]},\"uuid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",8,32]},\"major\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",40,4,false]},\"minor\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",44,4,false]},\"txpower\":{\"condition\":[\"manufacturerdata\",48,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",48,2,false]},\"volt\":{\"condition\":[\"manufacturerdata\",48,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",48,2,false],\"post_proc\":[\"/\",10]}}}";
-
+const char* _iNodeEM_json = "{\"brand\":\"iNode\",\"model\":\"Energy Meter\",\"model_id\":\"INEM\",\"tag\":\"0c01\",\"condition\":[\"manufacturerdata\",\"index\",0,\"90\",\"|\",\"manufacturerdata\",\"index\",0,\"92\",\"|\",\"manufacturerdata\",\"index\",0,\"94\",\"|\",\"manufacturerdata\",\"index\",0,\"96\",\"&\",\"manufacturerdata\",\"=\",26,\"index\",2,\"82\"],\"properties\":{\".cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",16,4,true,false],\"post_proc\":[\"&\",16383]},\"avg\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",4,4,true,false],\"post_proc\":[\"*\",60,\"/\",\".cal\"]},\"avgu\":{\"decoder\":[\"bit_static_value\",\"manufacturerdata\",18,0,\"kW\",\"m³\"]},\"sum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,4,true,false],\"post_proc\":[\"/\",\".cal\"]},\"sumu\":{\"decoder\":[\"bit_static_value\",\"manufacturerdata\",18,0,\"kWh\",\"m³\"]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,1,false,false],\"post_proc\":[\"-\",1,\"*\",10]},\"_batt\":{\"condition\":[\"manufacturerdata\",20,\"1\",\"|\",\"manufacturerdata\",20,\"c\",\"|\",\"manufacturerdata\",20,\"d\",\"|\",\"manufacturerdata\",20,\"e\",\"|\",\"manufacturerdata\",20,\"f\"],\"decoder\":[\"static_value\",\"100\"]},\"lowbatt\":{\"condition\":[\"manufacturerdata\",1,\"bit\",2,1],\"decoder\":[\"static_value\",true]}}}";
 /*R""""(
 {
-   "brand":"GENERIC",
-   "model":"iBeacon",
-   "model_id":"IBEACON",
-   "tag":"06",
-   "condition":["manufacturerdata", "=", 50, "index", 0, "4c00"],
+   "brand":"iNode",
+   "model":"Energy Meter",
+   "model_id":"INEM",
+   "tag":"0c01",
+   "condition":["manufacturerdata", "index", 0, "90", "|", "manufacturerdata", "index", 0, "92", "|", "manufacturerdata", "index", 0, "94", "|", "manufacturerdata", "index", 0, "96", "&", "manufacturerdata", "=", 26, "index", 2, "82"],
    "properties":{
-      "mfid":{
-         "decoder":["string_from_hex_data", "manufacturerdata", 0, 4]
-      },
-      "uuid":{
-         "decoder":["string_from_hex_data", "manufacturerdata", 8, 32]
-      },
-      "major":{
-         "decoder":["value_from_hex_data", "manufacturerdata", 40, 4, false]
-      },
-      "minor":{
-         "decoder":["value_from_hex_data", "manufacturerdata", 44, 4, false]
-      },
-      "txpower":{
-         "condition":["manufacturerdata", 48, "bit", 3, 1],
-         "decoder":["value_from_hex_data","manufacturerdata", 48, 2, false]
-      },
-      "volt":{
-         "condition":["manufacturerdata", 48, "bit", 3, 0],
-         "decoder":["value_from_hex_data","manufacturerdata", 48, 2, false],
-         "post_proc":["/", 10]
+      ".cal":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 16, 4, true, false],
+         "post_proc":["&", 16383]
+      },
+      "avg":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 4, 4, true, false],
+         "post_proc":[ "*", 60, "/", ".cal"]
+      },
+      "avgu":{
+         "decoder":["bit_static_value", "manufacturerdata", 18, 0, "kW", "m³"]
+      },
+      "sum":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 8, 4, true, false],
+         "post_proc":["/", ".cal"]
+      },
+      "sumu":{
+         "decoder":["bit_static_value", "manufacturerdata", 18, 0, "kWh", "m³"]
+      },
+      "batt":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 20, 1, false, false],
+         "post_proc":["-", 1, "*", 10]
+      },
+      "_batt":{
+         "condition":["manufacturerdata", 20, "1", "|", "manufacturerdata", 20, "c", "|", "manufacturerdata", 20, "d", "|", "manufacturerdata", 20, "e", "|", "manufacturerdata", 20, "f"],
+         "decoder":["static_value", "100"]
+      },
+      "lowbatt":{
+         "condition":["manufacturerdata", 1, "bit", 2, 1],
+         "decoder":["static_value", true]
       }
    }
 })"""";*/
 
-const char* _ibeacon_json_props = "{\"properties\":{\"mfid\":{\"unit\":\"hex\",\"name\":\"manufacturer id\"},\"uuid\":{\"unit\":\"hex\",\"name\":\"service uuid\"},\"major\":{\"unit\":\"hex\",\"name\":\"major value\"},\"minor\":{\"unit\":\"hex\",\"name\":\"minor value\"},\"txpower\":{\"unit\":\"dBm\",\"name\":\"tx power @ 1 m\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"}}}";
+const char* _iNodeEM_json_props = "{\"properties\":{\"avg\":{\"unit\":\"kW/m³\",\"name\":\"average\"},\"avgu\":{\"unit\":\"string\",\"name\":\"average unit\"},\"sum\":{\"unit\":\"kWh/m³\",\"name\":\"sum\"},\"sumu\":{\"unit\":\"string\",\"name\":\"sum unit\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"lowbatt\":{\"unit\":\"status\",\"name\":\"low battery\"}}}";
 /*R""""(
 {
    "properties":{
-      "mfid":{
-         "unit":"hex",
-         "name":"manufacturer id"
-      },
-      "uuid":{
-         "unit":"hex",
-         "name":"service uuid"
-      },
-      "major":{
-         "unit":"hex",
-         "name":"major value"
-      },
-      "minor":{
-         "unit":"hex",
-         "name":"minor value"
-      },
-      "txpower":{
-         "unit":"dBm",
-         "name":"tx power @ 1 m"
-      },
-      "volt":{
-         "unit":"V",
-         "name":"voltage"
+      "avg":{
+         "unit":"kW/m³",
+         "name":"average"
+      },
+      "avgu":{
+         "unit":"string",
+         "name":"average unit"
+      },
+      "sum":{
+         "unit":"kWh/m³",
+         "name":"sum"
+      },
+      "sumu":{
+         "unit":"string",
+         "name":"sum unit"
+      },
+      "batt":{
+         "unit":"%",
+         "name":"battery"
+      },
+      "lowbatt":{
+         "unit":"status",
+         "name":"low battery"
       }
    }
 })"""";*/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TheengsDecoder-1.5.0/src/devices/tracker_json.h` & `TheengsDecoder-1.5.1b0/src/devices/tracker_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.5.0/src/devices.h` & `TheengsDecoder-1.5.1b0/src/devices.h`

 * *Files identical despite different names*

