# Comparing `tmp/hsms-0.1.3.tar.gz` & `tmp/hsms-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsms-0.1.3.tar", last modified: Wed Mar  1 19:18:56 2023, max compression
+gzip compressed data, was "hsms-0.2.0.tar", last modified: Wed Jun 14 22:31:50 2023, max compression
```

## Comparing `hsms-0.1.3.tar` & `hsms-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,61 @@
--rw-r--r--   0        0        0     1279 1985-10-26 08:20:00.000000 hsms-0.1.3/PKG-INFO
--rw-r--r--   0        0        0      941 1985-10-26 08:20:00.000000 hsms-0.1.3/README.md
--rw-r--r--   0        0        0     1158 1985-10-26 08:20:00.000000 hsms-0.1.3/SConstruct
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/__init__.py
--rw-r--r--   0        0        0      182 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/atoms/__init__.py
--rw-r--r--   0        0        0      460 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/atoms/ints.py
--rw-r--r--   0        0        0      151 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/atoms/sized_bytes.py
--rw-r--r--   0        0        0     2366 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/bls12_381/BLSPublicKey.py
--rw-r--r--   0        0        0     3224 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/bls12_381/BLSSecretExponent.py
--rw-r--r--   0        0        0     1758 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/bls12_381/BLSSignature.py
--rw-r--r--   0        0        0      151 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/bls12_381/__init__.py
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/cmds/__init__.py
--rwxr-xr-x   0        0        0      953 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/cmds/hsm_dump_sb.py
--rw-r--r--   0        0        0     3509 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/cmds/hsm_test_spend.py
--rw-r--r--   0        0        0      301 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/cmds/hsmgen.py
--rwxr-xr-x   0        0        0     1979 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/cmds/hsmmerge.py
--rw-r--r--   0        0        0      259 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/cmds/hsmpk.py
--rwxr-xr-x   0        0        0     6296 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/cmds/hsms.py
--rwxr-xr-x   0        0        0     4268 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/cmds/hsmwizard.py
--rwxr-xr-x   0        0        0     2323 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/cmds/qrint.py
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/consensus/__init__.py
--rw-r--r--   0        0        0      493 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/consensus/conditions.py
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/contrib/__init__.py
--rw-r--r--   0        0        0     5189 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/contrib/bech32m.py
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/debug/__init__.py
--rw-r--r--   0        0        0     8367 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/debug/debug_spend_bundle.py
--rw-r--r--   0        0        0     1864 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/make_unsigned_tx.py
--rw-r--r--   0        0        0       88 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/meta/__init__.py
--rw-r--r--   0        0        0      437 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/meta/bin_methods.py
--rw-r--r--   0        0        0      320 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/meta/hexbytes.py
--rw-r--r--   0        0        0     1012 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/meta/make_sized_bytes.py
--rw-r--r--   0        0        0     1864 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/meta/streamable.py
--rw-r--r--   0        0        0      440 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/meta/struct_stream.py
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/process/__init__.py
--rw-r--r--   0        0        0     5859 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/process/sign.py
--rw-r--r--   0        0        0     1456 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/process/signing_hints.py
--rw-r--r--   0        0        0     2320 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/process/unsigned_spend.py
--rw-r--r--   0        0        0      123 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/puzzles/calculate_synthetic_public_key.cl
--rw-r--r--   0        0        0     1114 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/puzzles/condition_codes.clvm
--rw-r--r--   0        0        0      783 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/puzzles/conlang.py
--rw-r--r--   0        0        0     1491 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/puzzles/load_clvm.py
--rw-r--r--   0        0        0       56 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/puzzles/p2_conditions.cl
--rw-r--r--   0        0        0      667 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/puzzles/p2_conditions.py
--rw-r--r--   0        0        0     3237 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/puzzles/p2_delegated_puzzle_or_hidden_puzzle.cl
--rw-r--r--   0        0        0     5784 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py
--rw-r--r--   0        0        0      227 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/streamables/__init__.py
--rw-r--r--   0        0        0      948 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/streamables/coin.py
--rw-r--r--   0        0        0     1332 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/streamables/coin_spend.py
--rw-r--r--   0        0        0     5662 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/streamables/program.py
--rw-r--r--   0        0        0     1384 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/streamables/spend_bundle.py
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/util/__init__.py
--rw-r--r--   0        0        0      746 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/util/bech32.py
--rw-r--r--   0        0        0     2231 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/util/byte_chunks.py
--rw-r--r--   0        0        0     2237 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/util/clvm_serialization.py
--rw-r--r--   0        0        0     5486 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/util/qrint_encoding.py
--rw-r--r--   0        0        0      190 1985-10-26 08:20:00.000000 hsms-0.1.3/hsms/util/std_hash.py
--rw-r--r--   0        0        0     1049 1985-10-26 08:20:00.000000 hsms-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1249 1985-10-26 08:20:00.000000 hsms-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      941 1985-10-26 08:20:00.000000 hsms-0.2.0/README.md
+-rw-r--r--   0        0        0     1158 1985-10-26 08:20:00.000000 hsms-0.2.0/SConstruct
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/__init__.py
+-rw-r--r--   0        0        0      182 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/atoms/__init__.py
+-rw-r--r--   0        0        0      460 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/atoms/ints.py
+-rw-r--r--   0        0        0      151 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/atoms/sized_bytes.py
+-rw-r--r--   0        0        0      198 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/bls12_381/__init__.py
+-rw-r--r--   0        0        0     2769 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/bls12_381/bls_public_key.py
+-rw-r--r--   0        0        0     3436 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/bls12_381/bls_secret_exponent.py
+-rw-r--r--   0        0        0     1904 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/bls12_381/bls_signature.py
+-rw-r--r--   0        0        0      438 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/bls12_381/secret_key_utils.py
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/clvm/__init__.py
+-rw-r--r--   0        0        0     2617 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/clvm/disasm.py
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/__init__.py
+-rwxr-xr-x   0        0        0      953 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/hsm_dump_sb.py
+-rw-r--r--   0        0        0     3529 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/hsm_test_spend.py
+-rw-r--r--   0        0        0      301 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/hsmgen.py
+-rwxr-xr-x   0        0        0     1992 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/hsmmerge.py
+-rw-r--r--   0        0        0      259 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/hsmpk.py
+-rwxr-xr-x   0        0        0     6347 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/hsms.py
+-rwxr-xr-x   0        0        0     4331 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/hsmwizard.py
+-rw-r--r--   0        0        0     3050 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/poser_gen.py
+-rw-r--r--   0        0        0     1947 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/poser_verify.py
+-rwxr-xr-x   0        0        0     2599 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/cmds/qrint.py
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/consensus/__init__.py
+-rw-r--r--   0        0        0      484 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/consensus/conditions.py
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/contrib/__init__.py
+-rw-r--r--   0        0        0     5189 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/contrib/bech32m.py
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/debug/__init__.py
+-rw-r--r--   0        0        0     8489 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/debug/debug_spend_bundle.py
+-rw-r--r--   0        0        0     1883 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/make_unsigned_tx.py
+-rw-r--r--   0        0        0       88 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/meta/__init__.py
+-rw-r--r--   0        0        0      441 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/meta/bin_methods.py
+-rw-r--r--   0        0        0      320 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/meta/hexbytes.py
+-rw-r--r--   0        0        0     1012 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/meta/make_sized_bytes.py
+-rw-r--r--   0        0        0     1864 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/meta/streamable.py
+-rw-r--r--   0        0        0      444 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/meta/struct_stream.py
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/process/__init__.py
+-rw-r--r--   0        0        0     5817 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/process/sign.py
+-rw-r--r--   0        0        0     1456 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/process/signing_hints.py
+-rw-r--r--   0        0        0     2340 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/process/unsigned_spend.py
+-rw-r--r--   0        0        0      123 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/puzzles/calculate_synthetic_public_key.cl
+-rw-r--r--   0        0        0     1114 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/puzzles/condition_codes.clvm
+-rw-r--r--   0        0        0      785 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/puzzles/conlang.py
+-rw-r--r--   0        0        0     1482 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/puzzles/load_clvm.py
+-rw-r--r--   0        0        0       56 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/puzzles/p2_conditions.cl
+-rw-r--r--   0        0        0      687 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/puzzles/p2_conditions.py
+-rw-r--r--   0        0        0     3237 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/puzzles/p2_delegated_puzzle_or_hidden_puzzle.cl
+-rw-r--r--   0        0        0     5682 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py
+-rw-r--r--   0        0        0      190 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/streamables/__init__.py
+-rw-r--r--   0        0        0      863 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/streamables/coin.py
+-rw-r--r--   0        0        0     1280 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/streamables/coin_spend.py
+-rw-r--r--   0        0        0     1384 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/streamables/spend_bundle.py
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/util/__init__.py
+-rw-r--r--   0        0        0      746 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/util/bech32.py
+-rw-r--r--   0        0        0     2231 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/util/byte_chunks.py
+-rw-r--r--   0        0        0     2152 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/util/clvm_serialization.py
+-rw-r--r--   0        0        0     5486 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/util/qrint_encoding.py
+-rw-r--r--   0        0        0      190 1985-10-26 08:20:00.000000 hsms-0.2.0/hsms/util/std_hash.py
+-rw-r--r--   0        0        0     1121 1985-10-26 08:20:00.000000 hsms-0.2.0/pyproject.toml
```

### Comparing `hsms-0.1.3/PKG-INFO` & `hsms-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: hsms
-Version: 0.1.3
+Version: 0.2.0
 Summary: Hardware security module simulator for chia bls12_381 signatures
 License: Apache-2.0
 Requires-Dist: blspy==1.0.16
 Requires-Dist: segno==1.4.1
-Requires-Dist: clvm==0.9.7
-Requires-Dist: clvm_tools==0.4.6
+Requires-Dist: clvm_rs==0.2.5
 Requires-Dist: clvm_tools_rs==0.1.30
 Description-Content-Type: text/markdown
 
 
 HSMS: hardware security module software/simulator
 
 This project is intended to run on an air-gapped computer to sign chia spends using bls12_381 keys.
```

### Comparing `hsms-0.1.3/README.md` & `hsms-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/SConstruct` & `hsms-0.2.0/SConstruct`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/hsms/bls12_381/BLSPublicKey.py` & `hsms-0.2.0/hsms/bls12_381/bls_public_key.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,51 @@
-from typing import List
+from typing import BinaryIO, List
 
 import blspy
 
-from hsms.atoms import hexbytes
-from hsms.util.bech32 import bech32_decode, bech32_encode, Encoding
+from ..atoms import hexbytes
+from ..util.bech32 import bech32_decode, bech32_encode, Encoding
 
-BECH32M_PREFIX = "bls1238"
+from .secret_key_utils import public_key_from_int
+
+BECH32M_PUBLIC_KEY_PREFIX = "bls1238"
 
 
 class BLSPublicKey:
     def __init__(self, g1: blspy.G1Element):
         assert isinstance(g1, blspy.G1Element)
         self._g1 = g1
 
     @classmethod
     def from_bytes(cls, blob):
         bls_public_hd_key = blspy.G1Element.from_bytes(blob)
         return BLSPublicKey(bls_public_hd_key)
 
     @classmethod
+    def parse(cls, f: BinaryIO):
+        return cls.from_bytes(f.read(48))
+
+    @classmethod
     def generator(cls):
         return BLSPublicKey(blspy.G1Element.generator())
 
     @classmethod
     def zero(cls):
         return cls(blspy.G1Element())
 
+    def stream(self, f: BinaryIO) -> None:
+        f.write(bytes(self._g1))
+
     def __add__(self, other):
         return BLSPublicKey(self._g1 + other._g1)
 
     def __mul__(self, other):
+        if self == self.generator():
+            # this would be subject to timing attacks
+            return BLSPublicKey(public_key_from_int(other))
         if other == 0:
             return self.zero()
         if other == 1:
             return self
         parity = other & 1
         v = self.__mul__(other >> 1)
         v += v
@@ -41,15 +53,15 @@
             v += self
         return v
 
     def __rmul__(self, other):
         return self.__mul__(other)
 
     def __eq__(self, other):
-        return bytes(self) == bytes(other)
+        return self._g1 == other._g1
 
     def __bytes__(self) -> bytes:
         return hexbytes(self._g1)
 
     def child(self, index: int) -> "BLSPublicKey":
         return BLSPublicKey(
             blspy.AugSchemeMPL.derive_child_pk_unhardened(self._g1, index)
@@ -61,24 +73,24 @@
             r = self.child(index)
         return r
 
     def fingerprint(self):
         return self._g1.get_fingerprint()
 
     def as_bech32m(self):
-        return bech32_encode(BECH32M_PREFIX, bytes(self), Encoding.BECH32M)
+        return bech32_encode(BECH32M_PUBLIC_KEY_PREFIX, bytes(self), Encoding.BECH32M)
 
     @classmethod
     def from_bech32m(cls, text: str) -> "BLSPublicKey":
         r = bech32_decode(text, max_length=91)
         if r is not None:
             prefix, base8_data, encoding = r
             if (
                 encoding == Encoding.BECH32M
-                and prefix == BECH32M_PREFIX
+                and prefix == BECH32M_PUBLIC_KEY_PREFIX
                 and len(base8_data) == 49
             ):
                 return cls.from_bytes(base8_data[:48])
         raise ValueError("not bls12_381 bech32m pubkey")
 
     def __hash__(self):
         return bytes(self).__hash__()
```

### Comparing `hsms-0.1.3/hsms/bls12_381/BLSSecretExponent.py` & `hsms-0.2.0/hsms/bls12_381/bls_secret_exponent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-from typing import List, Optional
+from typing import BinaryIO, List, Optional
 
 import blspy
 
-from hsms.atoms import bytes32
+from ..atoms import bytes32
+from ..util.std_hash import std_hash
+from ..util.bech32 import bech32_decode, bech32_encode, Encoding
 
-from hsms.util.std_hash import std_hash
-from hsms.util.bech32 import bech32_decode, bech32_encode, Encoding
+from .bls_public_key import BLSPublicKey
+from .bls_signature import BLSSignature
+from .secret_key_utils import private_key_from_int
 
-from .BLSSignature import BLSSignature
-from .BLSPublicKey import BLSPublicKey
 
-
-BECH32M_PREFIX = "se"
-
-GROUP_ORDER = (
-    52435875175126190479447740508185965837690552500527637822603658699938581184513
-)
+BECH32M_SECRET_EXPONENT_PREFIX = "se"
 
 
 class BLSSecretExponent:
     def __init__(self, sk: blspy.PrivateKey):
         self._sk = sk
 
     @classmethod
     def from_seed(cls, blob: bytes) -> "BLSSecretExponent":
         secret_exponent = int.from_bytes(std_hash(blob), "big")
         return cls.from_int(secret_exponent)
 
     @classmethod
     def from_int(cls, secret_exponent) -> "BLSSecretExponent":
-        secret_exponent %= GROUP_ORDER
-        blob = secret_exponent.to_bytes(32, "big")
-        return cls.from_bytes(blob)
+        return cls(private_key_from_int(secret_exponent))
 
     @classmethod
     def from_bytes(cls, blob) -> "BLSSecretExponent":
         return cls(blspy.PrivateKey.from_bytes(blob))
 
+    @classmethod
+    def parse(cls, f: BinaryIO):
+        return cls.from_bytes(f.read(32))
+
+    def stream(self, f: BinaryIO) -> None:
+        f.write(bytes(self._sk))
+
     def fingerprint(self) -> int:
         return self._sk.get_g1().get_fingerprint()
 
     def sign(
         self, message_hash: bytes32, final_public_key: Optional[BLSPublicKey] = None
     ) -> BLSSignature:
         if final_public_key:
@@ -66,24 +67,26 @@
     def child_for_path(self, path: List[int]) -> "BLSSecretExponent":
         r = self
         for index in path:
             r = self.child(index)
         return r
 
     def as_bech32m(self):
-        return bech32_encode(BECH32M_PREFIX, bytes(self), Encoding.BECH32M)
+        return bech32_encode(
+            BECH32M_SECRET_EXPONENT_PREFIX, bytes(self), Encoding.BECH32M
+        )
 
     @classmethod
     def from_bech32m(cls, text: str) -> "BLSSecretExponent":
         r = bech32_decode(text)
         if r is not None:
             prefix, base8_data, encoding = r
             if (
                 encoding == Encoding.BECH32M
-                and prefix == BECH32M_PREFIX
+                and prefix == BECH32M_SECRET_EXPONENT_PREFIX
                 and len(base8_data) == 33
             ):
                 return cls.from_bytes(base8_data[:32])
         raise ValueError("not secret exponent")
 
     @classmethod
     def zero(cls) -> "BLSSecretExponent":
@@ -92,15 +95,17 @@
     def __add__(self, other):
         return self.from_int(int(self) + int(other))
 
     def __int__(self):
         return self.secret_exponent()
 
     def __eq__(self, other):
-        return int(self) == int(other)
+        if isinstance(other, int):
+            other = BLSSecretExponent.from_int(other)
+        return self._sk == other._sk
 
     def __bytes__(self):
         return bytes(self._sk)
 
     def __str__(self):
         return "<prv for:%s>" % self.public_key()
```

### Comparing `hsms-0.1.3/hsms/bls12_381/BLSSignature.py` & `hsms-0.2.0/hsms/bls12_381/bls_signature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,59 @@
-from typing import Iterator, List, Tuple
+from dataclasses import dataclass
+from typing import BinaryIO, Iterator, List, Tuple
 
 import blspy
 
-from hsms.meta import streamable
+from ..atoms import bytes32, bytes96
 
-from hsms.streamables import bytes32, bytes96
-
-from .BLSPublicKey import BLSPublicKey
+from .bls_public_key import BLSPublicKey
 
 ZERO96 = bytes96([0] * 96)
 
 
-@streamable
 class BLSSignature:
     """
-    This wraps the blspy version and resolves a couple edge cases around aggregation and validation.
+    This wraps the blspy version and resolves a couple edge cases
+    around aggregation and validation.
     """
 
-    @streamable
+    @dataclass
     class aggsig_pair:
         public_key: BLSPublicKey
         message_hash: bytes32
 
     def __init__(self, g2: blspy.G2Element):
         assert isinstance(g2, blspy.G2Element)
         self._g2 = g2
 
     @classmethod
     def from_bytes(cls, blob):
         bls_public_hd_key = blspy.G2Element.from_bytes(blob)
         return cls(bls_public_hd_key)
 
     @classmethod
+    def parse(cls, f: BinaryIO):
+        return cls.from_bytes(bytes96.parse(f))
+
+    @classmethod
     def generator(cls):
         return cls(blspy.G2Element.generator())
 
     @classmethod
     def zero(cls):
         return cls(blspy.G2Element())
 
+    def stream(self, f):
+        f.write(bytes(self._g2))
+
     def __add__(self, other):
         return self.__class__(self._g2 + other._g2)
 
     def __eq__(self, other):
-        return bytes(self) == bytes(other)
+        return self._g2 == other._g2
 
     def __bytes__(self) -> bytes:
         return bytes(self._g2)
 
     def __str__(self):
         return bytes(self._g2).hex()
```

### Comparing `hsms-0.1.3/hsms/cmds/hsm_dump_sb.py` & `hsms-0.2.0/hsms/cmds/hsm_dump_sb.py`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/hsms/cmds/hsm_test_spend.py` & `hsms-0.2.0/hsms/cmds/hsm_test_spend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import argparse
 import hashlib
 import zlib
 
+from clvm_rs import Program
+
 from hsms.bls12_381 import BLSPublicKey
 
 from hsms.process.signing_hints import SumHint, PathHint
 
 from hsms.puzzles.p2_delegated_puzzle_or_hidden_puzzle import (
     DEFAULT_HIDDEN_PUZZLE,
     puzzle_for_public_key_and_hidden_puzzle,
     solution_for_conditions,
     calculate_synthetic_offset,
 )
-from hsms.streamables import Coin, CoinSpend, Program
+from hsms.streamables import Coin, CoinSpend
 from hsms.process.unsigned_spend import UnsignedSpend
 from hsms.puzzles.conlang import CREATE_COIN
 from hsms.util.byte_chunks import (
     create_chunks_for_blob,
     optimal_chunk_size_for_max_chunk_size,
 )
 from hsms.util.qrint_encoding import b2a_qrint
```

### Comparing `hsms-0.1.3/hsms/cmds/hsmmerge.py` & `hsms-0.2.0/hsms/cmds/hsmmerge.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from typing import List
 
 import argparse
 
-from hsms.bls12_381.BLSSecretExponent import BLSSignature
+from hsms.bls12_381 import BLSSignature
 from hsms.process.unsigned_spend import UnsignedSpend
 from hsms.process.sign import generate_synthetic_offset_signatures
 from hsms.streamables import bytes96, SpendBundle
 from hsms.util.qrint_encoding import a2b_qrint
 
 
 def create_spend_bundle(unsigned_spend: UnsignedSpend, signatures: List[BLSSignature]):
@@ -39,26 +39,28 @@
     ]
     spend_bundle = create_spend_bundle(unsigned_spend, signatures)
     print(bytes(spend_bundle).hex())
 
 
 def create_parser():
     parser = argparse.ArgumentParser(
-        description="Create a signed `SpendBundle` from `UnsignedSpends` and signatures."
+        description=(
+            "Create a signed `SpendBundle` from `UnsignedSpends` " "and signatures."
+        )
     )
     parser.add_argument(
         "unsigned_spend",
         metavar="path-to-unsigned-spend-as-hex",
         help="file containing hex-encoded `UnsignedSpends`",
     )
     parser.add_argument(
         "signature",
-        metavar="hex-encoded-signature",
+        metavar="qrint-encoded-signature",
         nargs="+",
-        help="hex-encoded signature",
+        help="qrint-encoded signature",
     )
     return parser
 
 
 def main():
     parser = create_parser()
     args = parser.parse_args()
```

### Comparing `hsms-0.1.3/hsms/cmds/hsms.py` & `hsms-0.2.0/hsms/cmds/hsms.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 import argparse
 import io
 import readline  # noqa: this allows long lines on stdin
 import subprocess
 import sys
 import zlib
 
+from clvm_rs import Program
+
 import segno
 
-from hsms.bls12_381.BLSSecretExponent import BLSSecretExponent, BLSSignature
+from hsms.bls12_381 import BLSSecretExponent, BLSSignature
 from hsms.consensus.conditions import conditions_by_opcode
 from hsms.process.sign import conditions_for_coin_spend, sign
 from hsms.process.unsigned_spend import UnsignedSpend
 from hsms.puzzles import conlang
-from hsms.streamables import bytes32, Program
+from hsms.streamables import bytes32
 from hsms.util.bech32 import bech32_encode
 from hsms.util.byte_chunks import ChunkAssembler
 from hsms.util.qrint_encoding import a2b_qrint, b2a_qrint
 
 
-XCH_PER_MOJO = Decimal(1e12)
+XCH_PER_MOJO = Decimal("1e12")
 
 
 def unsigned_spend_from_blob(blob: bytes) -> UnsignedSpend:
     try:
         uncompressed_blob = zlib.decompress(blob)
         program = Program.from_bytes(uncompressed_blob)
         return UnsignedSpend.from_program(program)
@@ -171,16 +173,19 @@
     )
     parser.add_argument(
         # "-f",
         "private_key_file",
         metavar="path-to-private-keys",
         action="append",
         default=[],
-        help="file containing bech32m-encoded secret exponents. If file name ends with .gpg, "
-        '"gpg -d" will be invoked automatically. File is read one line at a time.',
+        help=(
+            "file containing bech32m-encoded secret exponents. "
+            """If file name ends with .gpg, "gpg -d" will be invoked """
+            "automatically. File is read one line at a time."
+        ),
         type=argparse.FileType("r"),
     )
     return parser
 
 
 def main():
     parser = create_parser()
```

### Comparing `hsms-0.1.3/hsms/cmds/hsmwizard.py` & `hsms-0.2.0/hsms/cmds/hsmwizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,18 @@
 def create_parser():
     parser = argparse.ArgumentParser(
         description="Wizard to look for USB mount point and key file and launch hsms"
     )
     parser.add_argument(
         "-d",
         "--device-to-mount",
-        help="path, usually to something in `/dev/disk/` to ensure exists before attempting to mount",
+        help=(
+            "path, usually to something in `/dev/disk/` "
+            "to ensure exists before attempting to mount"
+        ),
     )
     parser.add_argument(
         "-r",
         "--mount-command-read-only",
         help="command to mount disk read-only",
         default="/usr/bin/sudo mount -o ro {device_to_mount} {mount_path}",
     )
@@ -122,15 +125,16 @@
                     1, f"failed to remount device {args.device_to_mount} read/write"
                 )
             cmd = f"/usr/bin/touch {wallet_path}.tmp && /bin/rm {wallet_path}.tmp"
             r = os.system(cmd)
             if r != 0:
                 parser.exit(
                     1,
-                    f"could not create temporary file `{wallet_path}.tmp`, drive permissions may be wrong",
+                    f"could not create temporary file `{wallet_path}.tmp`, "
+                    f"drive permissions may be wrong",
                 )
         generate_secret(wallet_path)
     print()
     input("hit return to power off> ")
     os.system("poweroff")
```

### Comparing `hsms-0.1.3/hsms/cmds/qrint.py` & `hsms-0.2.0/hsms/cmds/qrint.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from hsms.process.sign import generate_synthetic_offset_signatures
 from hsms.streamables import SpendBundle
 from hsms.util.qrint_encoding import a2b_qrint, b2a_qrint
 
 
 def create_spend_bundle(unsigned_spend, signatures):
-
     extra_signatures = generate_synthetic_offset_signatures(unsigned_spend)
 
     # now let's try adding them all together and creating a `SpendBundle`
 
     all_signatures = signatures + [sig_info.signature for sig_info in extra_signatures]
     total_signature = sum(all_signatures, start=all_signatures[0].zero())
 
@@ -25,24 +24,30 @@
         with open(p) as f:
             text = f.read().strip()
     except Exception:
         text = p
     return text
 
 
-def decode(path):
+def decode(path, hex_output):
     if path.endswith(".qri") and len(path) > 4:
         new_path = path[:-4]
     else:
-        new_path = path + ".bin"
+        new_path = path + (".hex" if hex_output else ".bin")
     if os.path.exists(new_path):
         raise ValueError(f"{new_path} already exists")
 
     blob = open(path).read().strip()
     decoded = a2b_qrint(blob)
+
+    if hex_output:
+        with open(new_path, "w") as f:
+            f.write(decoded.hex())
+        return
+
     with open(new_path, "wb") as f:
         f.write(decoded)
 
 
 def encode(path):
     new_path = path + ".qri"
     if os.path.exists(new_path):
@@ -59,28 +64,31 @@
         blob = f.read()
 
     is_qrint = (
         all(c in b"0123456789" for c in blob.strip()) and not args.encode_to_qrint
     )
 
     if is_qrint:
-        return decode(args.path)
+        return decode(args.path, args.hex_output)
     else:
         return encode(args.path)
 
 
 def create_parser():
     parser = argparse.ArgumentParser(description="Convert binary to/from qrint format.")
     parser.add_argument(
         "-e",
         "--encode-to-qrint",
         action="store_true",
         help="force conversion from binary to qrint",
     )
     parser.add_argument(
+        "-H", "--hex-output", action="store_true", help="force convert to hex"
+    )
+    parser.add_argument(
         "path",
         metavar="path-to-binary-or-qrint-file",
         help="file containing qrint or binary (context-sensitive)",
     )
     return parser
```

### Comparing `hsms-0.1.3/hsms/contrib/bech32m.py` & `hsms-0.2.0/hsms/contrib/bech32m.py`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/hsms/debug/debug_spend_bundle.py` & `hsms-0.2.0/hsms/debug/debug_spend_bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from typing import List
 
-from clvm import KEYWORD_FROM_ATOM
-from clvm_tools.binutils import disassemble as bu_disassemble
+from clvm_rs import Program
 
 from hsms.bls12_381 import BLSSignature
+from hsms.clvm.disasm import disassemble as bu_disassemble, KEYWORD_FROM_ATOM
 from hsms.consensus.conditions import conditions_by_opcode
 from hsms.process.sign import generate_verify_pairs
 from hsms.puzzles import conlang
-from hsms.streamables import Coin, Program
+from hsms.streamables import Coin
 from hsms.util.std_hash import std_hash
 
 KFA = {bytes([getattr(conlang, k)]): k for k in dir(conlang) if k[0] in "ACR"}
 
-
 AGG_SIG_ME_ADDITIONAL_DATA = bytes.fromhex(
     "ccd5bb71183532bff220ba46c268991a3ff07eb358e8255a65c30a2dce0e5fbb"
 )
 
 
 # information needed to spend a cc
 # if we ever support more genesis conditions, like a re-issuable coin,
 # we may need also to save the `genesis_coin_mod` or its hash
 
 
 def disassemble(sexp):
     """
-    This version of `disassemble` also disassembles condition opcodes like `ASSERT_ANNOUNCEMENT_CONSUMED`.
+    This version of `disassemble` also disassembles condition opcodes like
+    `ASSERT_ANNOUNCEMENT_CONSUMED`.
     """
     kfa = dict(KEYWORD_FROM_ATOM)
-    kfa.update((Program.to(k).as_atom(), v) for k, v in KFA.items())
+    kfa.update((Program.to(k).atom, v) for k, v in KFA.items())
     return bu_disassemble(sexp, kfa)
 
 
 def coin_as_program(coin: Coin) -> Program:
     """
     Convenience function for when putting `coin_info` into a solution.
     """
@@ -43,16 +43,16 @@
     return disassemble(coin_as_program(coin))
 
 
 def debug_spend_bundle(
     spend_bundle, agg_sig_additional_data=AGG_SIG_ME_ADDITIONAL_DATA
 ) -> None:
     """
-    Print a lot of useful information about a `SpendBundle` that might help with debugging
-    its clvm.
+    Print a lot of useful information about a `SpendBundle` that might help with
+    debugging its clvm.
     """
 
     pks = []
     msgs = []
 
     created_coin_announcements: List[List[bytes]] = []
     asserted_coin_announcements = []
@@ -65,38 +65,41 @@
         puzzle_reveal = Program.from_bytes(bytes(coin_spend.puzzle_reveal))
         solution = Program.from_bytes(bytes(coin_spend.solution))
         coin_name = coin.name()
 
         if puzzle_reveal.tree_hash() != coin_spend.coin.puzzle_hash:
             print("*** BAD PUZZLE REVEAL")
             print(
-                f"{puzzle_reveal.tree_hash().hex()} vs {coin_spend.coin.puzzle_hash.hex()}"
+                f"{puzzle_reveal.tree_hash().hex()} vs"
+                f" {coin_spend.coin.puzzle_hash.hex()}"
             )
             print("*" * 80)
             continue
 
         print(f"consuming coin {dump_coin(coin)}")
         print(f"  with id {coin_name}")
         print()
         print(
-            f"\nbrun -y main.sym '{bu_disassemble(puzzle_reveal)}' '{bu_disassemble(solution)}'"
+            f"\nbrun -y main.sym '{bu_disassemble(puzzle_reveal)}'"
+            f" '{bu_disassemble(solution)}'"
         )
-        r = puzzle_reveal.run(solution)
+        cost, r = puzzle_reveal.run_with_cost(solution, max_cost=1<<34)
         conditions = conditions_by_opcode(r)
         error = None
         if error:
             print(f"*** error {error}")
         elif conditions is not None:
             for public_key, m in generate_verify_pairs(
                 coin_spend, agg_sig_additional_data
             ):
                 pks.append(public_key)
                 msgs.append(m)
             print()
             print(disassemble(r))
+            print(f"cost = {cost}")
             print()
             if conditions and len(conditions) > 0:
                 print("grouped conditions:")
                 for condition_programs in conditions.values():
                     print()
                     for c in condition_programs:
                         print(f"  {disassemble(Program.to(c))}")
@@ -186,35 +189,35 @@
         )
 
         print()
         print()
         print(f"zero_coin_set = {sorted(zero_coin_set)}")
         print()
         if created_coin_announcement_pairs or asserted_coin_announcements:
-            print(
-                f"created  coin announcements = {sorted([_[-1] for _ in created_coin_announcement_pairs])}"
-            )
+            sa = sorted([_[-1] for _ in created_coin_announcement_pairs])
+            print(f"created  coin announcements = {sa}")
             print()
             print(
                 f"asserted coin announcements = {sorted(asserted_coin_announcements)}"
             )
             print()
             print(f"symdiff of coin announcements = {sorted(eor_coin_announcements)}")
             print()
         if created_puzzle_announcement_pairs or asserted_puzzle_announcements:
-            print(
-                f"created  puzzle announcements = {sorted([_[-1] for _ in created_puzzle_announcement_pairs])}"
-            )
+            sa = sorted([_[-1] for _ in created_puzzle_announcement_pairs])
+            print(f"created  puzzle announcements = {sa}")
             print()
             print(
-                f"asserted puzzle announcements = {sorted(asserted_puzzle_announcements)}"
+                f"asserted puzzle announcements ="
+                f" {sorted(asserted_puzzle_announcements)}"
             )
             print()
             print(
-                f"symdiff of puzzle announcements = {sorted(eor_puzzle_announcements)}"
+                f"symdiff of puzzle announcements ="
+                f" {sorted(eor_puzzle_announcements)}"
             )
             print()
     print()
     print("=" * 80)
     print()
     signature = BLSSignature.from_bytes(spend_bundle.aggregated_signature)
     validates = signature.verify(list(zip(pks, msgs)))
```

### Comparing `hsms-0.1.3/hsms/make_unsigned_tx.py` & `hsms-0.2.0/hsms/make_unsigned_tx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import hashlib
 
-from hsms.atoms.hexbytes import hexbytes
-from hsms.streamables import Coin, CoinSpend, Program
+from clvm_rs import Program
+
+from hsms.meta.hexbytes import hexbytes
 from hsms.multisig.pst import PartiallySignedTransaction
+from hsms.streamables import Coin, CoinSpend
 
 from clvm_tools.binutils import assemble
 
 
 PAY_TO_AGGSIG_ME_PROG = """(q (50
      0x8ba79a9ccd362086d552a6f56da7fe612959b0dd372350ad798c77c2170de2163a00e499928cc40547a7a8a5e2cde6be
      0x4bf5122f344554c53bde2ebb8cd2b7e3d1600ad631c385a5d7cce23c7785459a))"""
```

### Comparing `hsms-0.1.3/hsms/meta/make_sized_bytes.py` & `hsms-0.2.0/hsms/meta/make_sized_bytes.py`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/hsms/meta/streamable.py` & `hsms-0.2.0/hsms/meta/streamable.py`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/hsms/process/sign.py` & `hsms-0.2.0/hsms/process/sign.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from dataclasses import dataclass
 from typing import Dict, Iterable, List, Optional, Tuple
 from weakref import WeakKeyDictionary
 
+from clvm_rs import Program
+
 from hsms.atoms import hexbytes
 from hsms.bls12_381 import BLSPublicKey, BLSSecretExponent
 from hsms.consensus.conditions import conditions_by_opcode
-from hsms.streamables import bytes32, CoinSpend, Program
+from hsms.streamables import bytes32, CoinSpend
 from hsms.puzzles.conlang import AGG_SIG_ME, AGG_SIG_UNSAFE
 
 from .signing_hints import SumHint, SumHints, PathHint, PathHints
 from .unsigned_spend import SignatureInfo, UnsignedSpend
 
 
 @dataclass
@@ -20,17 +22,17 @@
 
 
 CONDITIONS_FOR_COIN_SPEND: Dict[CoinSpend, Program] = WeakKeyDictionary()
 
 
 def conditions_for_coin_spend(coin_spend: CoinSpend) -> Program:
     if coin_spend not in CONDITIONS_FOR_COIN_SPEND:
-        CONDITIONS_FOR_COIN_SPEND[coin_spend] = coin_spend.puzzle_reveal.run(
-            coin_spend.solution
-        )
+        CONDITIONS_FOR_COIN_SPEND[coin_spend] = coin_spend.puzzle_reveal.run_with_cost(
+            coin_spend.solution, max_cost=1<<32
+        )[1]
     return CONDITIONS_FOR_COIN_SPEND[coin_spend]
 
 
 def build_sum_hints_lookup(sum_hints: List[SumHint]) -> SumHints:
     return {_.final_public_key(): _ for _ in sum_hints}
 
 
@@ -119,23 +121,21 @@
 def verify_pairs_for_conditions(
     conditions: Program, agg_sig_me_message_suffix: bytes
 ) -> Iterable[Tuple[BLSPublicKey, bytes]]:
     d = conditions_by_opcode(conditions)
 
     agg_sig_me_conditions = d.get(AGG_SIG_ME, [])
     for condition in agg_sig_me_conditions:
-        condition_list = list(condition.as_atom_list())
-        yield BLSPublicKey.from_bytes(condition_list[1]), hexbytes(
-            condition_list[2] + agg_sig_me_message_suffix
+        yield BLSPublicKey.from_bytes(condition.at("rf").atom), hexbytes(
+            condition.at("rrf").atom + agg_sig_me_message_suffix
         )
 
     agg_sig_unsafe_conditions = d.get(AGG_SIG_UNSAFE, [])
     for condition in agg_sig_unsafe_conditions:
-        condition_list = list(condition.as_atom_list())
-        yield BLSPublicKey.from_bytes(condition_list[1]), hexbytes(condition[2])
+        yield BLSPublicKey.from_bytes(condition.at("rf"), hexbytes(condition.at("rrf")))
 
 
 def secret_key_for_public_key(
     secrets: List[BLSSecretExponent], path, root_public_key, public_key
 ) -> Optional[BLSSecretExponent]:
     for secret in secrets:
         if secret.public_key() == root_public_key:
```

### Comparing `hsms-0.1.3/hsms/process/signing_hints.py` & `hsms-0.2.0/hsms/process/signing_hints.py`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/hsms/process/unsigned_spend.py` & `hsms-0.2.0/hsms/process/unsigned_spend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import zlib
 
 from dataclasses import dataclass
 from typing import List
 
+from clvm_rs import Program
+
 from hsms.bls12_381 import BLSPublicKey, BLSSignature
 from hsms.process.signing_hints import SumHint, PathHint
-from hsms.streamables import bytes32, CoinSpend, Program
+from hsms.streamables import bytes32, CoinSpend
 from hsms.util.byte_chunks import assemble_chunks, create_chunks_for_blob
 from hsms.util.clvm_serialization import (
     transform_dict,
     transform_dict_by_key,
     clvm_to_list,
 )
```

### Comparing `hsms-0.1.3/hsms/puzzles/condition_codes.clvm` & `hsms-0.2.0/hsms/puzzles/condition_codes.clvm`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/hsms/puzzles/conlang.py` & `hsms-0.2.0/hsms/puzzles/conlang.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 AGG_SIG_UNSAFE = 49
 AGG_SIG_ME = 50
 
-# the conditions below reserve coin amounts and have to be accounted for in output totals
+# the conditions below reserve coin amounts and
+# have to be accounted for in output totals
 
 CREATE_COIN = 51
 RESERVE_FEE = 52
 
 # the conditions below deal with announcements, for inter-coin communication
 
 # coin announcements
```

### Comparing `hsms-0.1.3/hsms/puzzles/load_clvm.py` & `hsms-0.2.0/hsms/puzzles/load_clvm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 
 import pkg_resources
+from clvm_rs import Program
 from clvm_tools_rs import compile_clvm
-from hsms.streamables import Program
 
 
 def load_clvm(clvm_filename, package_or_requirement=__name__) -> Program:
     """
     This function takes a .clvm file in the given package and compiles it to a
     .clvm.hex file if the .hex file is missing or older than the .clvm file, then
     returns the contents of the .hex file as a `Program`.
```

### Comparing `hsms-0.1.3/hsms/puzzles/p2_conditions.py` & `hsms-0.2.0/hsms/puzzles/p2_conditions.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 in bitcoin.
 
 This is a pretty useless most of the time. But some (most?) solutions
 require a delegated puzzle program, so in those cases, this is just what
 the doctor ordered.
 """
 
-from hsms.streamables import Program
+from clvm_rs import Program
 
 from .load_clvm import load_clvm
 
 MOD = load_clvm("p2_conditions.cl")
 
 
 def puzzle_for_conditions(conditions) -> Program:
-    return MOD.run([conditions])
+    return MOD.run_with_cost([conditions], max_cost=1<<32)[1]
 
 
 def solution_for_conditions(conditions) -> Program:
     return Program.to([puzzle_for_conditions(conditions), 0])
```

### Comparing `hsms-0.1.3/hsms/puzzles/p2_delegated_puzzle_or_hidden_puzzle.cl` & `hsms-0.2.0/hsms/puzzles/p2_delegated_puzzle_or_hidden_puzzle.cl`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/hsms/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py` & `hsms-0.2.0/hsms/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Pay to delegated puzzle or hidden puzzle
 
 In this puzzle program, the solution must choose either a hidden puzzle or a
 delegated puzzle on a given public key.
 
-The given public key is morphed by adding an offset from the hash of the hidden puzzle
-and itself, giving a new so-called "synthetic" public key which has the hidden puzzle
-hidden inside of it.
+The given public key is morphed by adding an offset from the hash of the hidden
+puzzle and itself, giving a new so-called "synthetic" public key which has the
+hidden puzzle hidden inside of it.
 
-If the hidden puzzle path is taken, the hidden puzzle and original public key will be revealed
-which proves that it was hidden there in the first place.
+If the hidden puzzle path is taken, the hidden puzzle and original public key
+will be revealed which proves that it was hidden there in the first place.
 
 This roughly corresponds to bitcoin's taproot.
 
 Note:
 
 p2_delegated_puzzle_or_hidden_puzzle is essentially the "standard coin" in chia.
 DEFAULT_HIDDEN_PUZZLE_HASH from this puzzle is used with
@@ -26,45 +26,47 @@
 
 - The user's wallet contains a primary sk/pk pair which are used to derive to one
   level a set of auxiliary sk/pk pairs which are used for specific coins. These
   can be used for signing in AGG_SIG_ME, but the standard coin uses a key further
   derived from one of these via calculate_synthetic_secret_key as described in
   https://chialisp.com/docs/standard_transaction. Therefore, when a wallet needs
   to find a secret key for signing based on a public key, it needs to try repeating
-  this derivation as well and see if the BLSPublicKey (pk) associated with any of the
-  derived secret keys matches the pk requested by the coin.
+  this derivation as well and see if the BLSPublicKey (pk) associated with any of
+  the derived secret keys matches the pk requested by the coin.
 
 - Python code previously appeared which was written like:
 
     delegated_puzzle_solution = Program.to((1, condition_args))
     solutions = Program.to([[], delegated_puzzle_solution, []])
 
   In context, delegated_puzzle_solution here is any *chialisp program*, here one
   simply quoting a list of conditions, and the following argument is the arguments
   to this program, which here are unused. Secondly, the actual arguments to the
   p2_delegated_puzzle_or_hidden_puzzle are given. The first argument determines
   whether a hidden or revealed puzzle is used. If the puzzle is hidden, then what
   is required is a signature given a specific synthetic key since the key cannot be
   derived inline without the puzzle. In that case, the first argument is this key.
-  In most cases, the puzzle will be revealed, and this argument will be the nil object,
-  () (represented here by an empty python list).
+  In most cases, the puzzle will be revealed, and this argument will be the nil
+  object, () (represented here by an empty python list).
 
   The second and third arguments are a chialisp program and its corresponding
   arguments, which will be run inside the standard coin puzzle. This interacts with
-  sign_coin_spend in that the AGG_SIG_ME condition added by the inner puzzle asks the
-  surrounding system to provide a signature over the provided program with a synthetic
-  key whose derivation is within. Any wallets which intend to use standard coins in
-  this way must try to resolve a public key to a secret key via this derivation.
+  sign_coin_spend in that the AGG_SIG_ME condition added by the inner puzzle asks
+  the surrounding system to provide a signature over the provided program with a 
+  synthetic key whose derivation is within. Any wallets which intend to use
+  standard coins in this way must try to resolve a public key to a secret key
+  via this derivation.
 """
 
 import hashlib
 
-from hsms.bls12_381 import BLSPublicKey, BLSSecretExponent
+from clvm_rs import Program
 
-from hsms.streamables import bytes32, Program
+from hsms.bls12_381 import BLSPublicKey, BLSSecretExponent
+from hsms.streamables import bytes32
 
 from .load_clvm import load_clvm
 from .p2_conditions import puzzle_for_conditions
 
 DEFAULT_HIDDEN_PUZZLE = Program.from_bytes(
     bytes.fromhex("ff0980")
 )  # this puzzle `(=)` always fails
@@ -84,16 +86,18 @@
     assert offset == int(Program.to(blob))
     return BLSSecretExponent.from_int(offset)
 
 
 def calculate_synthetic_public_key(
     public_key: BLSPublicKey, hidden_puzzle_hash: bytes32
 ) -> BLSPublicKey:
-    r = SYNTHETIC_MOD.run([bytes(public_key), hidden_puzzle_hash])
-    return BLSPublicKey.from_bytes(r.as_atom())
+    _cost, r = SYNTHETIC_MOD.run_with_cost(
+        [bytes(public_key), hidden_puzzle_hash], max_cost=1 << 32
+    )
+    return BLSPublicKey.from_bytes(r.atom)
 
 
 def calculate_synthetic_secret_key(
     secret_key: BLSSecretExponent, hidden_puzzle_hash: bytes32
 ) -> BLSSecretExponent:
     public_key = secret_key.public_key()
     synthetic_offset = calculate_synthetic_offset(public_key, hidden_puzzle_hash)
@@ -118,20 +122,14 @@
     public_key: BLSPublicKey, hidden_puzzle: Program
 ) -> Program:
     return puzzle_for_public_key_and_hidden_puzzle_hash(
         public_key, hidden_puzzle.tree_hash()
     )
 
 
-def puzzle_for_pk(public_key: BLSPublicKey) -> Program:
-    return puzzle_for_public_key_and_hidden_puzzle_hash(
-        public_key, DEFAULT_HIDDEN_PUZZLE_HASH
-    )
-
-
 def solution_for_delegated_puzzle(
     delegated_puzzle: Program, solution: Program
 ) -> Program:
     return Program.to([[], delegated_puzzle, solution])
 
 
 def solution_for_hidden_puzzle(
```

### Comparing `hsms-0.1.3/hsms/streamables/coin_spend.py` & `hsms-0.2.0/hsms/streamables/coin_spend.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-from dataclasses import dataclass
+from clvm_rs import Program
 
 from .coin import Coin
-from .program import Program
 
-from hsms.atoms import bytes32, uint64
 from hsms.meta import streamable
 from hsms.util.clvm_serialization import transform_as_struct
 
 
-@dataclass(frozen=True)
 @streamable
 class CoinSpend:
     """
-    This is a rather disparate data structure that validates coin transfers. It's generally populated
-    with data from different sources, since burned coins are identified by name, so it is built up
-    more often that it is streamed.
+    This is a rather disparate data structure that validates coin transfers. It's
+    generally populated with data from different sources, since burned coins are
+    identified by name, so it is built up more often that it is streamed.
     """
 
     coin: Coin
     puzzle_reveal: Program
     solution: Program
 
     def as_program(self):
@@ -35,11 +32,15 @@
             lambda x: x,
             lambda x: Program.to(x).as_int(),
             lambda x: x,
         )
         puzzle_reveal = Program.to(puzzle_reveal)
         solution = Program.to(solution)
         return cls(
-            Coin(bytes32(parent_coin_info), puzzle_reveal.tree_hash(), uint64(amount)),
+            Coin(
+                parent_coin_info,
+                puzzle_reveal.tree_hash(),
+                amount,
+            ),
             puzzle_reveal,
             solution,
         )
```

### Comparing `hsms-0.1.3/hsms/streamables/spend_bundle.py` & `hsms-0.2.0/hsms/streamables/spend_bundle.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 from .coin_spend import CoinSpend
 
 
 @dataclass(frozen=True)
 class SpendBundle:
     """
-    This is a list of coins being spent along with their solution programs, and a single
-    aggregated signature. This is the object that most closely corresponds to a bitcoin
-    transaction (although because of non-interactive signature aggregation, the boundaries
-    between transactions are more flexible than in bitcoin).
+    This is a list of coins being spent along with their solution programs, and a
+    single aggregated signature. This is the object that most closely corresponds to
+    a bitcoin transaction (although because of non-interactive signature aggregation,
+    the boundaries between transactions are more flexible than in bitcoin).
     """
 
     coin_spends: List[CoinSpend]
     aggregated_signature: bytes96
 
     def __add__(self, other: "SpendBundle") -> "SpendBundle":
         return self.__class__(
```

### Comparing `hsms-0.1.3/hsms/util/bech32.py` & `hsms-0.2.0/hsms/util/bech32.py`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/hsms/util/byte_chunks.py` & `hsms-0.2.0/hsms/util/byte_chunks.py`

 * *Files identical despite different names*

### Comparing `hsms-0.1.3/hsms/util/clvm_serialization.py` & `hsms-0.2.0/hsms/util/clvm_serialization.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any, Callable, Dict, List, Tuple, TypeVar
 
-from clvm.casts import int_from_bytes
-from clvm.CLVMObject import CLVMObject
+from clvm_rs import Program
 
 
 K = TypeVar("K")
 T = TypeVar("T")
 V = TypeVar("V")
 
 
@@ -21,60 +20,60 @@
         print(ex)
         breakpoint()
     d = dict(r)
     return d
 
 
 def transform_by_key(
-    key: CLVMObject,
-    value: CLVMObject,
-    transformation_lookup: Dict[str, Callable[[CLVMObject], Any]],
+    key: Program,
+    value: Program,
+    transformation_lookup: Dict[str, Callable[[Program], Any]],
 ) -> Tuple[str, Any]:
     """
     Use this if the key is utf-8 and the value decoding depends on the key.
     """
     key_str = key.atom.decode()
     f = transformation_lookup.get(key_str, lambda x: x)
     final_value = f(value)
     return (key_str, final_value)
 
 
 def transform_dict_by_key(
-    transformation_lookup: Dict[str, Callable[[CLVMObject], Any]]
+    transformation_lookup: Dict[str, Callable[[Program], Any]]
 ) -> Any:
     return lambda k, v: transform_by_key(k, v, transformation_lookup)
 
 
-def transform_as_struct(items: CLVMObject, *struct_transformers) -> Tuple[Any, ...]:
+def transform_as_struct(items: Program, *struct_transformers) -> Tuple[Any, ...]:
     r = []
     for f in struct_transformers:
         r.append(f(items.pair[0]))
         items = items.pair[1]
     return tuple(r)
 
 
 def clvm_to_list(
-    item_list: CLVMObject, item_transformation_f: Callable[[CLVMObject], T]
+    item_list: Program, item_transformation_f: Callable[[Program], T]
 ) -> List[T]:
     r = []
     while item_list.pair:
         this_item, item_list = item_list.pair
         r.append(item_transformation_f(this_item))
     return r
 
 
 def clvm_list_of_bytes_to_list(
-    items: CLVMObject, from_bytes_f: Callable[[bytes], T]
+    items: Program, from_bytes_f: Callable[[bytes], T]
 ) -> List[T]:
     return clvm_to_list(items, lambda obj: from_bytes_f(obj.atom))
 
 
-def clvm_to_list_of_ints(items: CLVMObject) -> List[int]:
-    return clvm_to_list(items, lambda obj: int_from_bytes(obj.atom))
+def clvm_to_list_of_ints(items: Program) -> List[int]:
+    return clvm_to_list(items, lambda obj: Program.to(obj).as_int())
 
 
 def clvm_list_to_dict(
-    items: CLVMObject,
-    from_clvm_f_to_kv: Callable[[CLVMObject, CLVMObject], Tuple[K, V]],
+    items: Program,
+    from_clvm_f_to_kv: Callable[[Program, Program], Tuple[K, V]],
 ) -> Dict[K, V]:
     r = clvm_to_list(items, lambda obj: from_clvm_f_to_kv(obj.pair[0], obj.pair[1]))
     return dict(r)
```

### Comparing `hsms-0.1.3/hsms/util/qrint_encoding.py` & `hsms-0.2.0/hsms/util/qrint_encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This file implements the `qrint` encoding of binary data to a string of decimal digits.
 
 QR codes support different encoding modes, and generation tools typically choose them
-automatically. There is a binary QR code encoding, but it doesn't work well with hand-scanners
-since they act like keyboards, and most bytes can't be typed. So we need to encode the
-data in a keyboard-friends subset of ASCII.
+automatically. There is a binary QR code encoding, but it doesn't work well with
+hand-scanners since they act like keyboards, and most bytes can't be typed. So we need
+to encode the data in a keyboard-friends subset of ASCII.
 
 According to Wikipedia, the candidates are
 
 - Kanji/Kana
 - alphanumeric (0-9, A-Z, space plus 8 punctuation marks)
 - binary (all 8-bit values)
 - numeric (digits 0-9)
```

### Comparing `hsms-0.1.3/pyproject.toml` & `hsms-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "hsms"
 description = "Hardware security module simulator for chia bls12_381 signatures"
 authors = ["Richard Kiss <him@richardkiss.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/chia-network/hsms.git"
 readme = "README.md"
 src_root = "."
-dependencies = ["blspy==1.0.16", "segno==1.4.1", "clvm==0.9.7", "clvm_tools==0.4.6", "clvm_tools_rs==0.1.30"]
+dependencies = ["blspy==1.0.16", "segno==1.4.1", "clvm_rs==0.2.5", "clvm_tools_rs==0.1.30"]
 packages = ["hsms"]
 # version is defined with `setuptools_scm`. See `SConstruct` file.
 
 [tool.enscons.optional_dependencies]
 test = ["nose", "coverage"]
 dev = ["flake8>=4.0.1", "black>=22.6"]
 
@@ -19,13 +19,15 @@
   "hsms = hsms.cmds.hsms:main",
   "hsmpk = hsms.cmds.hsmpk:main",
   "hsmgen = hsms.cmds.hsmgen:main",
   "hsmmerge = hsms.cmds.hsmmerge:main",
   "hsm_test_spend = hsms.cmds.hsm_test_spend:main",
   "hsm_dump_sb = hsms.cmds.hsm_dump_sb:main",
   "qrint = hsms.cmds.qrint:main",
-  "hsmwizard = hsms.cmds.hsmwizard:main"
+  "hsmwizard = hsms.cmds.hsmwizard:main",
+  "poser_gen = hsms.cmds.poser_gen:main",
+  "poser_verify = hsms.cmds.poser_verify:main"
 ]
 
 [build-system]
 requires = ["pytoml>=0.1", "enscons", "setuptools_scm>=6.2"]
 build-backend = "enscons.api"
```

