# Comparing `tmp/drift_protocol-0.4.0-py3-none-any.whl.zip` & `tmp/drift_protocol-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 12243 bytes, number of entries: 14
--rw-r--r--  2.0 unx      285 b- defN 23-May-17 14:53 drift_protocol/__init__.py
--rw-r--r--  2.0 unx       96 b- defN 23-May-17 14:53 drift_protocol/common/__init__.py
--rw-r--r--  2.0 unx     2580 b- defN 23-May-17 14:53 drift_protocol/common/data_payload_pb2.py
--rw-r--r--  2.0 unx     8282 b- defN 23-May-17 14:53 drift_protocol/common/drift_package_pb2.py
--rw-r--r--  2.0 unx     4542 b- defN 23-May-17 14:53 drift_protocol/common/status_code_pb2.py
--rw-r--r--  2.0 unx       29 b- defN 23-May-17 14:53 drift_protocol/meta/__init__.py
--rw-r--r--  2.0 unx    24799 b- defN 23-May-17 14:53 drift_protocol/meta/meta_info_pb2.py
--rw-r--r--  2.0 unx       79 b- defN 23-May-17 14:53 drift_protocol/trigger_service/__init__.py
--rw-r--r--  2.0 unx     3454 b- defN 23-May-17 14:53 drift_protocol/trigger_service/interval_trigger_message_pb2.py
--rw-r--r--  2.0 unx     2622 b- defN 23-May-17 14:53 drift_protocol/trigger_service/trigger_message_pb2.py
--rw-r--r--  2.0 unx     1807 b- defN 23-May-17 14:53 drift_protocol-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 14:53 drift_protocol-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-May-17 14:53 drift_protocol-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1296 b- defN 23-May-17 14:53 drift_protocol-0.4.0.dist-info/RECORD
-14 files, 49978 bytes uncompressed, 10033 bytes compressed:  79.9%
+Zip file size: 13069 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      285 b- defN 23-Jun-15 10:24 drift_protocol/__init__.py
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-15 10:24 drift_protocol/common/__init__.py
+-rw-r--r--  2.0 unx     2580 b- defN 23-Jun-15 10:24 drift_protocol/common/data_payload_pb2.py
+-rw-r--r--  2.0 unx     8282 b- defN 23-Jun-15 10:24 drift_protocol/common/drift_package_pb2.py
+-rw-r--r--  2.0 unx     4542 b- defN 23-Jun-15 10:24 drift_protocol/common/status_code_pb2.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jun-15 10:24 drift_protocol/meta/__init__.py
+-rw-r--r--  2.0 unx    35609 b- defN 23-Jun-15 10:24 drift_protocol/meta/meta_info_pb2.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-15 10:24 drift_protocol/trigger_service/__init__.py
+-rw-r--r--  2.0 unx     3454 b- defN 23-Jun-15 10:24 drift_protocol/trigger_service/interval_trigger_message_pb2.py
+-rw-r--r--  2.0 unx     2622 b- defN 23-Jun-15 10:24 drift_protocol/trigger_service/trigger_message_pb2.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-Jun-15 10:24 drift_protocol-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 10:24 drift_protocol-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-15 10:24 drift_protocol-0.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1296 b- defN 23-Jun-15 10:24 drift_protocol-0.5.0.dist-info/RECORD
+14 files, 60788 bytes uncompressed, 10859 bytes compressed:  82.1%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: drift_protocol/trigger_service/interval_trigger_message_pb2.py
 Comment: 
 
 Filename: drift_protocol/trigger_service/trigger_message_pb2.py
 Comment: 
 
-Filename: drift_protocol-0.4.0.dist-info/METADATA
+Filename: drift_protocol-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: drift_protocol-0.4.0.dist-info/WHEEL
+Filename: drift_protocol-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: drift_protocol-0.4.0.dist-info/top_level.txt
+Filename: drift_protocol-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: drift_protocol-0.4.0.dist-info/RECORD
+Filename: drift_protocol-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drift_protocol/__init__.py

```diff
@@ -1,8 +1,8 @@
 """ Auto-generated file for package with generated protobuf bindings
 """
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 import google.protobuf as protobuf
 
 if protobuf.__version__ < '3.12.4':
     raise RuntimeError(f'Version of protobuf PIP package must be >=3.12.4. However you have {protobuf.__version__}')
```

## drift_protocol/common/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
+from .status_code_pb2 import *
 from .drift_package_pb2 import *
 from .data_payload_pb2 import *
-from .status_code_pb2 import *
```

## drift_protocol/meta/meta_info_pb2.py

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='drift_protocol/meta/meta_info.proto',
   package='drift.proto.meta',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n#drift_protocol/meta/meta_info.proto\x12\x10\x64rift.proto.meta\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\'drift_protocol/common/status_code.proto\"\xb7\x03\n\x08MetaInfo\x12\x31\n\x04type\x18\x01 \x01(\x0e\x32#.drift.proto.meta.MetaInfo.DataType\x12<\n\x10time_series_info\x18\x02 \x01(\x0b\x32 .drift.proto.meta.TimeSeriesInfoH\x00\x12\x31\n\nimage_info\x18\x03 \x01(\x0b\x32\x1b.drift.proto.meta.ImageInfoH\x00\x12\x39\n\x0bscalar_info\x18\x04 \x01(\x0b\x32\".drift.proto.meta.ScalarValuesInfoH\x00\x12/\n\ttext_info\x18\x05 \x01(\x0b\x32\x1a.drift.proto.meta.TextInfoH\x00\x12\x39\n\x0e\x61lignment_info\x18\x06 \x01(\x0b\x32\x1f.drift.proto.meta.AlignmentInfoH\x00\"X\n\x08\x44\x61taType\x12\x0f\n\x0bTIME_SERIES\x10\x00\x12\t\n\x05IMAGE\x10\x01\x12\x11\n\rSCALAR_VALUES\x10\x02\x12\x08\n\x04TEXT\x10\x03\x12\x13\n\x0f\x41LIGNED_PACKAGE\x10\x04\x42\x06\n\x04info\"\xcc\x01\n\x0eTimeSeriesInfo\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0estop_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04size\x18\x03 \x01(\x04\x12\r\n\x05\x66irst\x18\x04 \x01(\x02\x12\x0c\n\x04last\x18\x05 \x01(\x02\x12\x0b\n\x03min\x18\x06 \x01(\x02\x12\x0b\n\x03max\x18\x07 \x01(\x02\x12\x0c\n\x04mean\x18\x08 \x01(\x02\"\x96\x01\n\tImageInfo\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.drift.proto.meta.ImageInfo.ImageType\x12\r\n\x05width\x18\x02 \x01(\x04\x12\x0e\n\x06height\x18\x03 \x01(\x04\x12\x16\n\x0e\x63hannel_layout\x18\x04 \x01(\t\"\x1d\n\tImageType\x12\x06\n\x02WB\x10\x00\x12\x08\n\x04JPEG\x10\x01\"\xa4\x01\n\x10ScalarValuesInfo\x12\x42\n\tvariables\x18\x01 \x03(\x0b\x32/.drift.proto.meta.ScalarValuesInfo.VariableInfo\x1aL\n\x0cVariableInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.drift.proto.common.StatusCode\"\x1d\n\x08TextInfo\x12\x11\n\tmime_type\x18\x01 \x01(\t\"\x96\x01\n\rAlignmentInfo\x12=\n\x08packages\x18\x01 \x03(\x0b\x32+.drift.proto.meta.AlignmentInfo.PackageInfo\x1a\x46\n\x0bPackageInfo\x12\r\n\x05topic\x18\x01 \x01(\t\x12(\n\x04meta\x18\x02 \x01(\x0b\x32\x1a.drift.proto.meta.MetaInfob\x06proto3'
+  serialized_pb=b'\n#drift_protocol/meta/meta_info.proto\x12\x10\x64rift.proto.meta\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\'drift_protocol/common/status_code.proto\"\xd6\x03\n\x11WaveletBufferInfo\x12\x13\n\x0b\x61\x62i_version\x18\x01 \x01(\r\x12\x14\n\x0cwavelet_type\x18\x02 \x01(\r\x12\x1b\n\x13\x64\x65\x63omposition_steps\x18\x03 \x01(\r\x12\x19\n\x11\x66loat_compression\x18\x04 \x01(\r\x12G\n\x0cno_denoising\x18\x0f \x01(\x0b\x32/.drift.proto.meta.WaveletBufferInfo.NoDenoisingH\x00\x12U\n\x13threshold_denoising\x18\x10 \x01(\x0b\x32\x36.drift.proto.meta.WaveletBufferInfo.ThresholdDenoisingH\x00\x12Q\n\x11partial_denoising\x18\x11 \x01(\x0b\x32\x34.drift.proto.meta.WaveletBufferInfo.PartialDenoisingH\x00\x1a\r\n\x0bNoDenoising\x1a*\n\x12ThresholdDenoising\x12\t\n\x01\x61\x18\x01 \x01(\x02\x12\t\n\x01\x62\x18\x02 \x01(\x02\x1a#\n\x10PartialDenoising\x12\x0f\n\x07partial\x18\x01 \x01(\x02\x42\x0b\n\tdenoising\"\xf9\x03\n\x08MetaInfo\x12\x31\n\x04type\x18\x01 \x01(\x0e\x32#.drift.proto.meta.MetaInfo.DataType\x12<\n\x10time_series_info\x18\x02 \x01(\x0b\x32 .drift.proto.meta.TimeSeriesInfoH\x00\x12\x31\n\nimage_info\x18\x03 \x01(\x0b\x32\x1b.drift.proto.meta.ImageInfoH\x00\x12\x39\n\x0bscalar_info\x18\x04 \x01(\x0b\x32\".drift.proto.meta.ScalarValuesInfoH\x00\x12/\n\ttext_info\x18\x05 \x01(\x0b\x32\x1a.drift.proto.meta.TextInfoH\x00\x12\x39\n\x0e\x61lignment_info\x18\x06 \x01(\x0b\x32\x1f.drift.proto.meta.AlignmentInfoH\x00\x12@\n\x13wavelet_buffer_info\x18\x07 \x01(\x0b\x32#.drift.proto.meta.WaveletBufferInfo\"X\n\x08\x44\x61taType\x12\x0f\n\x0bTIME_SERIES\x10\x00\x12\t\n\x05IMAGE\x10\x01\x12\x11\n\rSCALAR_VALUES\x10\x02\x12\x08\n\x04TEXT\x10\x03\x12\x13\n\x0f\x41LIGNED_PACKAGE\x10\x04\x42\x06\n\x04info\"\xcc\x01\n\x0eTimeSeriesInfo\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0estop_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04size\x18\x03 \x01(\x04\x12\r\n\x05\x66irst\x18\x04 \x01(\x02\x12\x0c\n\x04last\x18\x05 \x01(\x02\x12\x0b\n\x03min\x18\x06 \x01(\x02\x12\x0b\n\x03max\x18\x07 \x01(\x02\x12\x0c\n\x04mean\x18\x08 \x01(\x02\"\x96\x01\n\tImageInfo\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.drift.proto.meta.ImageInfo.ImageType\x12\r\n\x05width\x18\x02 \x01(\x04\x12\x0e\n\x06height\x18\x03 \x01(\x04\x12\x16\n\x0e\x63hannel_layout\x18\x04 \x01(\t\"\x1d\n\tImageType\x12\x06\n\x02WB\x10\x00\x12\x08\n\x04JPEG\x10\x01\"\xa4\x01\n\x10ScalarValuesInfo\x12\x42\n\tvariables\x18\x01 \x03(\x0b\x32/.drift.proto.meta.ScalarValuesInfo.VariableInfo\x1aL\n\x0cVariableInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.drift.proto.common.StatusCode\"\x1d\n\x08TextInfo\x12\x11\n\tmime_type\x18\x01 \x01(\t\"\x96\x01\n\rAlignmentInfo\x12=\n\x08packages\x18\x01 \x03(\x0b\x32+.drift.proto.meta.AlignmentInfo.PackageInfo\x1a\x46\n\x0bPackageInfo\x12\r\n\x05topic\x18\x01 \x01(\t\x12(\n\x04meta\x18\x02 \x01(\x0b\x32\x1a.drift.proto.meta.MetaInfob\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,drift__protocol_dot_common_dot_status__code__pb2.DESCRIPTOR,])
 
 
 
 _METAINFO_DATATYPE = _descriptor.EnumDescriptor(
   name='DataType',
@@ -58,16 +58,16 @@
       name='ALIGNED_PACKAGE', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=475,
-  serialized_end=563,
+  serialized_start=1014,
+  serialized_end=1102,
 )
 _sym_db.RegisterEnumDescriptor(_METAINFO_DATATYPE)
 
 _IMAGEINFO_IMAGETYPE = _descriptor.EnumDescriptor(
   name='ImageType',
   full_name='drift.proto.meta.ImageInfo.ImageType',
   filename=None,
@@ -83,20 +83,192 @@
       name='JPEG', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=902,
-  serialized_end=931,
+  serialized_start=1441,
+  serialized_end=1470,
 )
 _sym_db.RegisterEnumDescriptor(_IMAGEINFO_IMAGETYPE)
 
 
+_WAVELETBUFFERINFO_NODENOISING = _descriptor.Descriptor(
+  name='NoDenoising',
+  full_name='drift.proto.meta.WaveletBufferInfo.NoDenoising',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=495,
+  serialized_end=508,
+)
+
+_WAVELETBUFFERINFO_THRESHOLDDENOISING = _descriptor.Descriptor(
+  name='ThresholdDenoising',
+  full_name='drift.proto.meta.WaveletBufferInfo.ThresholdDenoising',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='a', full_name='drift.proto.meta.WaveletBufferInfo.ThresholdDenoising.a', index=0,
+      number=1, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='b', full_name='drift.proto.meta.WaveletBufferInfo.ThresholdDenoising.b', index=1,
+      number=2, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=510,
+  serialized_end=552,
+)
+
+_WAVELETBUFFERINFO_PARTIALDENOISING = _descriptor.Descriptor(
+  name='PartialDenoising',
+  full_name='drift.proto.meta.WaveletBufferInfo.PartialDenoising',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='partial', full_name='drift.proto.meta.WaveletBufferInfo.PartialDenoising.partial', index=0,
+      number=1, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=554,
+  serialized_end=589,
+)
+
+_WAVELETBUFFERINFO = _descriptor.Descriptor(
+  name='WaveletBufferInfo',
+  full_name='drift.proto.meta.WaveletBufferInfo',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='abi_version', full_name='drift.proto.meta.WaveletBufferInfo.abi_version', index=0,
+      number=1, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='wavelet_type', full_name='drift.proto.meta.WaveletBufferInfo.wavelet_type', index=1,
+      number=2, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='decomposition_steps', full_name='drift.proto.meta.WaveletBufferInfo.decomposition_steps', index=2,
+      number=3, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='float_compression', full_name='drift.proto.meta.WaveletBufferInfo.float_compression', index=3,
+      number=4, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='no_denoising', full_name='drift.proto.meta.WaveletBufferInfo.no_denoising', index=4,
+      number=15, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='threshold_denoising', full_name='drift.proto.meta.WaveletBufferInfo.threshold_denoising', index=5,
+      number=16, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='partial_denoising', full_name='drift.proto.meta.WaveletBufferInfo.partial_denoising', index=6,
+      number=17, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_WAVELETBUFFERINFO_NODENOISING, _WAVELETBUFFERINFO_THRESHOLDDENOISING, _WAVELETBUFFERINFO_PARTIALDENOISING, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='denoising', full_name='drift.proto.meta.WaveletBufferInfo.denoising',
+      index=0, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
+  ],
+  serialized_start=132,
+  serialized_end=602,
+)
+
+
 _METAINFO = _descriptor.Descriptor(
   name='MetaInfo',
   full_name='drift.proto.meta.MetaInfo',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -139,14 +311,21 @@
     _descriptor.FieldDescriptor(
       name='alignment_info', full_name='drift.proto.meta.MetaInfo.alignment_info', index=5,
       number=6, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='wavelet_buffer_info', full_name='drift.proto.meta.MetaInfo.wavelet_buffer_info', index=6,
+      number=7, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
     _METAINFO_DATATYPE,
   ],
@@ -157,16 +336,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='info', full_name='drift.proto.meta.MetaInfo.info',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=132,
-  serialized_end=571,
+  serialized_start=605,
+  serialized_end=1110,
 )
 
 
 _TIMESERIESINFO = _descriptor.Descriptor(
   name='TimeSeriesInfo',
   full_name='drift.proto.meta.TimeSeriesInfo',
   filename=None,
@@ -238,16 +417,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=574,
-  serialized_end=778,
+  serialized_start=1113,
+  serialized_end=1317,
 )
 
 
 _IMAGEINFO = _descriptor.Descriptor(
   name='ImageInfo',
   full_name='drift.proto.meta.ImageInfo',
   filename=None,
@@ -292,16 +471,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=781,
-  serialized_end=931,
+  serialized_start=1320,
+  serialized_end=1470,
 )
 
 
 _SCALARVALUESINFO_VARIABLEINFO = _descriptor.Descriptor(
   name='VariableInfo',
   full_name='drift.proto.meta.ScalarValuesInfo.VariableInfo',
   filename=None,
@@ -331,16 +510,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1022,
-  serialized_end=1098,
+  serialized_start=1561,
+  serialized_end=1637,
 )
 
 _SCALARVALUESINFO = _descriptor.Descriptor(
   name='ScalarValuesInfo',
   full_name='drift.proto.meta.ScalarValuesInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -362,16 +541,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=934,
-  serialized_end=1098,
+  serialized_start=1473,
+  serialized_end=1637,
 )
 
 
 _TEXTINFO = _descriptor.Descriptor(
   name='TextInfo',
   full_name='drift.proto.meta.TextInfo',
   filename=None,
@@ -394,16 +573,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1100,
-  serialized_end=1129,
+  serialized_start=1639,
+  serialized_end=1668,
 )
 
 
 _ALIGNMENTINFO_PACKAGEINFO = _descriptor.Descriptor(
   name='PackageInfo',
   full_name='drift.proto.meta.AlignmentInfo.PackageInfo',
   filename=None,
@@ -433,16 +612,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1212,
-  serialized_end=1282,
+  serialized_start=1751,
+  serialized_end=1821,
 )
 
 _ALIGNMENTINFO = _descriptor.Descriptor(
   name='AlignmentInfo',
   full_name='drift.proto.meta.AlignmentInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -464,24 +643,40 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1132,
-  serialized_end=1282,
+  serialized_start=1671,
+  serialized_end=1821,
 )
 
+_WAVELETBUFFERINFO_NODENOISING.containing_type = _WAVELETBUFFERINFO
+_WAVELETBUFFERINFO_THRESHOLDDENOISING.containing_type = _WAVELETBUFFERINFO
+_WAVELETBUFFERINFO_PARTIALDENOISING.containing_type = _WAVELETBUFFERINFO
+_WAVELETBUFFERINFO.fields_by_name['no_denoising'].message_type = _WAVELETBUFFERINFO_NODENOISING
+_WAVELETBUFFERINFO.fields_by_name['threshold_denoising'].message_type = _WAVELETBUFFERINFO_THRESHOLDDENOISING
+_WAVELETBUFFERINFO.fields_by_name['partial_denoising'].message_type = _WAVELETBUFFERINFO_PARTIALDENOISING
+_WAVELETBUFFERINFO.oneofs_by_name['denoising'].fields.append(
+  _WAVELETBUFFERINFO.fields_by_name['no_denoising'])
+_WAVELETBUFFERINFO.fields_by_name['no_denoising'].containing_oneof = _WAVELETBUFFERINFO.oneofs_by_name['denoising']
+_WAVELETBUFFERINFO.oneofs_by_name['denoising'].fields.append(
+  _WAVELETBUFFERINFO.fields_by_name['threshold_denoising'])
+_WAVELETBUFFERINFO.fields_by_name['threshold_denoising'].containing_oneof = _WAVELETBUFFERINFO.oneofs_by_name['denoising']
+_WAVELETBUFFERINFO.oneofs_by_name['denoising'].fields.append(
+  _WAVELETBUFFERINFO.fields_by_name['partial_denoising'])
+_WAVELETBUFFERINFO.fields_by_name['partial_denoising'].containing_oneof = _WAVELETBUFFERINFO.oneofs_by_name['denoising']
 _METAINFO.fields_by_name['type'].enum_type = _METAINFO_DATATYPE
 _METAINFO.fields_by_name['time_series_info'].message_type = _TIMESERIESINFO
 _METAINFO.fields_by_name['image_info'].message_type = _IMAGEINFO
 _METAINFO.fields_by_name['scalar_info'].message_type = _SCALARVALUESINFO
 _METAINFO.fields_by_name['text_info'].message_type = _TEXTINFO
 _METAINFO.fields_by_name['alignment_info'].message_type = _ALIGNMENTINFO
+_METAINFO.fields_by_name['wavelet_buffer_info'].message_type = _WAVELETBUFFERINFO
 _METAINFO_DATATYPE.containing_type = _METAINFO
 _METAINFO.oneofs_by_name['info'].fields.append(
   _METAINFO.fields_by_name['time_series_info'])
 _METAINFO.fields_by_name['time_series_info'].containing_oneof = _METAINFO.oneofs_by_name['info']
 _METAINFO.oneofs_by_name['info'].fields.append(
   _METAINFO.fields_by_name['image_info'])
 _METAINFO.fields_by_name['image_info'].containing_oneof = _METAINFO.oneofs_by_name['info']
@@ -500,22 +695,54 @@
 _IMAGEINFO_IMAGETYPE.containing_type = _IMAGEINFO
 _SCALARVALUESINFO_VARIABLEINFO.fields_by_name['status'].enum_type = drift__protocol_dot_common_dot_status__code__pb2._STATUSCODE
 _SCALARVALUESINFO_VARIABLEINFO.containing_type = _SCALARVALUESINFO
 _SCALARVALUESINFO.fields_by_name['variables'].message_type = _SCALARVALUESINFO_VARIABLEINFO
 _ALIGNMENTINFO_PACKAGEINFO.fields_by_name['meta'].message_type = _METAINFO
 _ALIGNMENTINFO_PACKAGEINFO.containing_type = _ALIGNMENTINFO
 _ALIGNMENTINFO.fields_by_name['packages'].message_type = _ALIGNMENTINFO_PACKAGEINFO
+DESCRIPTOR.message_types_by_name['WaveletBufferInfo'] = _WAVELETBUFFERINFO
 DESCRIPTOR.message_types_by_name['MetaInfo'] = _METAINFO
 DESCRIPTOR.message_types_by_name['TimeSeriesInfo'] = _TIMESERIESINFO
 DESCRIPTOR.message_types_by_name['ImageInfo'] = _IMAGEINFO
 DESCRIPTOR.message_types_by_name['ScalarValuesInfo'] = _SCALARVALUESINFO
 DESCRIPTOR.message_types_by_name['TextInfo'] = _TEXTINFO
 DESCRIPTOR.message_types_by_name['AlignmentInfo'] = _ALIGNMENTINFO
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
+WaveletBufferInfo = _reflection.GeneratedProtocolMessageType('WaveletBufferInfo', (_message.Message,), {
+
+  'NoDenoising' : _reflection.GeneratedProtocolMessageType('NoDenoising', (_message.Message,), {
+    'DESCRIPTOR' : _WAVELETBUFFERINFO_NODENOISING,
+    '__module__' : 'drift_protocol.meta.meta_info_pb2'
+    # @@protoc_insertion_point(class_scope:drift.proto.meta.WaveletBufferInfo.NoDenoising)
+    })
+  ,
+
+  'ThresholdDenoising' : _reflection.GeneratedProtocolMessageType('ThresholdDenoising', (_message.Message,), {
+    'DESCRIPTOR' : _WAVELETBUFFERINFO_THRESHOLDDENOISING,
+    '__module__' : 'drift_protocol.meta.meta_info_pb2'
+    # @@protoc_insertion_point(class_scope:drift.proto.meta.WaveletBufferInfo.ThresholdDenoising)
+    })
+  ,
+
+  'PartialDenoising' : _reflection.GeneratedProtocolMessageType('PartialDenoising', (_message.Message,), {
+    'DESCRIPTOR' : _WAVELETBUFFERINFO_PARTIALDENOISING,
+    '__module__' : 'drift_protocol.meta.meta_info_pb2'
+    # @@protoc_insertion_point(class_scope:drift.proto.meta.WaveletBufferInfo.PartialDenoising)
+    })
+  ,
+  'DESCRIPTOR' : _WAVELETBUFFERINFO,
+  '__module__' : 'drift_protocol.meta.meta_info_pb2'
+  # @@protoc_insertion_point(class_scope:drift.proto.meta.WaveletBufferInfo)
+  })
+_sym_db.RegisterMessage(WaveletBufferInfo)
+_sym_db.RegisterMessage(WaveletBufferInfo.NoDenoising)
+_sym_db.RegisterMessage(WaveletBufferInfo.ThresholdDenoising)
+_sym_db.RegisterMessage(WaveletBufferInfo.PartialDenoising)
+
 MetaInfo = _reflection.GeneratedProtocolMessageType('MetaInfo', (_message.Message,), {
   'DESCRIPTOR' : _METAINFO,
   '__module__' : 'drift_protocol.meta.meta_info_pb2'
   # @@protoc_insertion_point(class_scope:drift.proto.meta.MetaInfo)
   })
 _sym_db.RegisterMessage(MetaInfo)
```

## Comparing `drift_protocol-0.4.0.dist-info/METADATA` & `drift_protocol-0.5.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drift-protocol
-Version: 0.4.0
+Version: 0.5.0
 Summary: Protobuf Libraries to encode message in Drift infrastructure
 Home-page: https://github.com/panda-official/DriftProtocol/
 Author: PANDA, GmbH
 Author-email: info@panda.technology
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

## Comparing `drift_protocol-0.4.0.dist-info/RECORD` & `drift_protocol-0.5.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-drift_protocol/__init__.py,sha256=wO6ilg3tO-Y1IXZ2HPfiGn1lc-Oj8NFABf_bvmlGCOg,285
-drift_protocol/common/__init__.py,sha256=5h0oJrSznVY4PQHVPf3-nsV5-A_UKFawOS8x0JCShAw,96
+drift_protocol/__init__.py,sha256=ccagWV-db3mD1SSONq-0Z7LAPlATdHqK09moSyKKzcY,285
+drift_protocol/common/__init__.py,sha256=KjFbGwPza4S-JtLUcce8ZuQaMwe0f-Wi17uAfBuhdF8,96
 drift_protocol/common/data_payload_pb2.py,sha256=JRVWR043i9CKok3Lo_twtyKMgLiPLYpysVCqrYR17nU,2580
 drift_protocol/common/drift_package_pb2.py,sha256=Lgf7_HNKqGzA_3dtCALDlAlLJ1h7oCwhVyXtBilQb5M,8282
 drift_protocol/common/status_code_pb2.py,sha256=P2qnFsTCcx7hugviaA2yV5nM2PWKEMyjgVzVRoJawOo,4542
 drift_protocol/meta/__init__.py,sha256=qu7lcUVJvYebLqo4tSmTX66klkF9333pFiqjZaTaPQA,29
-drift_protocol/meta/meta_info_pb2.py,sha256=Rki1STfRa8hFqOkZITb9MSpvpoxStv2Vq7H1tJA-CV4,24799
+drift_protocol/meta/meta_info_pb2.py,sha256=kIP2wZLwQtx3DZ2fGs6tnig5NIhOnRAcW2g7ba6_3Us,35609
 drift_protocol/trigger_service/__init__.py,sha256=BqR5M-dhiYxaAeEpZWnNxiq1OM9tTZ951mCt4XcM054,79
 drift_protocol/trigger_service/interval_trigger_message_pb2.py,sha256=93LNGo2Uf3s47bZ5mcBV6HlOcDbjEaxIHo1JhOl_GQk,3454
 drift_protocol/trigger_service/trigger_message_pb2.py,sha256=wbPLot0W6_msZifQGulaElWaqp05eb9hPPbw35CZW2U,2622
-drift_protocol-0.4.0.dist-info/METADATA,sha256=vBZVHv3KlaxgheUg_zmhvLOKUZ5RXxmb0QCiiLZXt4s,1807
-drift_protocol-0.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-drift_protocol-0.4.0.dist-info/top_level.txt,sha256=DbRiBVI9rCZ4d5UjXFR8gRrV-dJuSoWEsiNhNA8wcns,15
-drift_protocol-0.4.0.dist-info/RECORD,,
+drift_protocol-0.5.0.dist-info/METADATA,sha256=ItDKjlKfjthxwVvpCr_lQ_jVBbllZ3HwXhrPk0yjCmE,1807
+drift_protocol-0.5.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+drift_protocol-0.5.0.dist-info/top_level.txt,sha256=DbRiBVI9rCZ4d5UjXFR8gRrV-dJuSoWEsiNhNA8wcns,15
+drift_protocol-0.5.0.dist-info/RECORD,,
```

