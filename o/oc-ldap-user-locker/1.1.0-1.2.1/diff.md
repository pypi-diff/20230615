# Comparing `tmp/oc_ldap_user_locker-1.1.0-py3-none-any.whl.zip` & `tmp/oc_ldap_user_locker-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12049 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-May-31 06:55 oc_ldap_user_locker/__init__.py
--rw-r--r--  2.0 unx      528 b- defN 23-May-31 06:55 oc_ldap_user_locker/__main__.py
--rw-r--r--  2.0 unx    15442 b- defN 23-May-31 06:55 oc_ldap_user_locker/locker.py
--rw-r--r--  2.0 unx     5441 b- defN 23-May-31 06:55 oc_ldap_user_locker/mailer.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-31 06:55 oc_ldap_user_locker-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      274 b- defN 23-May-31 06:55 oc_ldap_user_locker-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 06:55 oc_ldap_user_locker-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-May-31 06:55 oc_ldap_user_locker-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      791 b- defN 23-May-31 06:55 oc_ldap_user_locker-1.1.0.dist-info/RECORD
-9 files, 33945 bytes uncompressed, 10665 bytes compressed:  68.6%
+Zip file size: 12074 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 08:10 oc_ldap_user_locker/__init__.py
+-rw-r--r--  2.0 unx      528 b- defN 23-Jun-15 08:10 oc_ldap_user_locker/__main__.py
+-rw-r--r--  2.0 unx    15564 b- defN 23-Jun-15 08:10 oc_ldap_user_locker/locker.py
+-rw-r--r--  2.0 unx     5441 b- defN 23-Jun-15 08:10 oc_ldap_user_locker/mailer.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-15 08:10 oc_ldap_user_locker-1.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      274 b- defN 23-Jun-15 08:10 oc_ldap_user_locker-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 08:10 oc_ldap_user_locker-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-15 08:10 oc_ldap_user_locker-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      791 b- defN 23-Jun-15 08:10 oc_ldap_user_locker-1.2.1.dist-info/RECORD
+9 files, 34067 bytes uncompressed, 10690 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: oc_ldap_user_locker/locker.py
 Comment: 
 
 Filename: oc_ldap_user_locker/mailer.py
 Comment: 
 
-Filename: oc_ldap_user_locker-1.1.0.dist-info/LICENSE
+Filename: oc_ldap_user_locker-1.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: oc_ldap_user_locker-1.1.0.dist-info/METADATA
+Filename: oc_ldap_user_locker-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: oc_ldap_user_locker-1.1.0.dist-info/WHEEL
+Filename: oc_ldap_user_locker-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: oc_ldap_user_locker-1.1.0.dist-info/top_level.txt
+Filename: oc_ldap_user_locker-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: oc_ldap_user_locker-1.1.0.dist-info/RECORD
+Filename: oc_ldap_user_locker-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oc_ldap_user_locker/locker.py

```diff
@@ -143,64 +143,65 @@
         return _result
 
     def _check_user_conf(self, user_rec, conf):
         """
         Check user configuration is suitable for our case
         :param OcLdapRecord user_rec: LDAP record for user account
         :param dict conf: user configuration
-        :return bool:
+        :return int: number of attributes matched, or None if configuration is not applicable
         """
 
         # if no 'condition_attributes' specified - it is our case
         if not conf.get('condition_attributes'):
-            return True
+            return 0
 
         # search for attribute otherwise
         # all of attributes are to be matched
         # we have to raise an exception if one of mandatory values is not specified
+        _matched_attributes = 0
         for _attrib in conf['condition_attributes'].keys():
             logging.debug("Comparing attribute: '%s'" % _attrib)
             _vals_from_rec = user_rec.get_attribute(_attrib)
             _match_conf = conf['condition_attributes'][_attrib]
 
             if not self._compare_attribute(_vals_from_rec, _match_conf):
                 logging.debug("Failed on attribute: '%s'" % _attrib)
-                return False
+                return None
 
-        return True
+            _matched_attributes += 1
+
+        return _matched_attributes
 
     def _find_valid_conf(self, user_rec):
         """
         Parse users configuration and find valid days
         :param OcLdapRecord user_rec: LDAP record for user account
         :return int:
         """
         logging.debug("Started configuration analysis for %s" % user_rec.get_attribute('cn'))
         _users_conf = self.config.get("users")
         _conf_f = None
 
         # analyse all cases one-by-one
+        _matched_attributes = None
+
         for _conf in _users_conf:
-            _applicable = self._check_user_conf(user_rec, _conf)
+            _matched_attributes_c = self._check_user_conf(user_rec, _conf)
 
-            if not _applicable:
+            if _matched_attributes_c is None:
                 # this configuration can not be applied
                 continue
 
-            if _conf_f is None:
+            # NOTE: checking '_matched_attributes' for 'None' is a sort of paranoia since
+            #       it should never happen
+            if _conf_f is None or _matched_attributes_c > _matched_attributes:
                 # we found at least one suitable configration:
                 _conf_f = _conf
-                continue
+                _matched_attributes = _matched_attributes_c
             
-            # select one with minimum valid days
-            # the default value is not applicable for this parameter, so we have to raise an exception
-            # for case it is not specified or has wrong type
-            if _conf_f['days_valid'] > _conf['days_valid']:
-                _conf_f = _conf
-
         return _conf_f
 
     def _process_single_user(self, ldap_c, user_dn):
         """
         Process single user record
         :param OCLDAPUSERCAT ldap_c: ldap client instance
         :param str user_dn: user record distinct name (DN)
```

## Comparing `oc_ldap_user_locker-1.1.0.dist-info/LICENSE` & `oc_ldap_user_locker-1.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `oc_ldap_user_locker-1.1.0.dist-info/RECORD` & `oc_ldap_user_locker-1.2.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 oc_ldap_user_locker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oc_ldap_user_locker/__main__.py,sha256=rg29B6Ou1-_XqIdqt0AFuRSBYAt96KmoELjydZvmPQc,528
-oc_ldap_user_locker/locker.py,sha256=ZaX00EpVnF_nM2co7SpNpgH0J1F3Cj3z5a6dx3GWCJ8,15442
+oc_ldap_user_locker/locker.py,sha256=bY0dmau6DHmX3USAJ8LoutonacmzZZGyjdOdq3BvOtY,15564
 oc_ldap_user_locker/mailer.py,sha256=qDAdc4Eetxuj0g8xhzuc_Qk7KX_VhfPWJkEw7g5XsSc,5441
-oc_ldap_user_locker-1.1.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-oc_ldap_user_locker-1.1.0.dist-info/METADATA,sha256=Kcikg_1f86LE8-Z-j6eX9MNsGj_wAA0Ghu-6vM3wwPk,274
-oc_ldap_user_locker-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-oc_ldap_user_locker-1.1.0.dist-info/top_level.txt,sha256=VgvLdN22xrjMzdP18fGULsr4ergDZbPZBI4GHD62ep0,20
-oc_ldap_user_locker-1.1.0.dist-info/RECORD,,
+oc_ldap_user_locker-1.2.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+oc_ldap_user_locker-1.2.1.dist-info/METADATA,sha256=Fy0bAU8n2zXbsNRBODC_X4fwyJQFBgfkYtN73Q7xE7g,274
+oc_ldap_user_locker-1.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+oc_ldap_user_locker-1.2.1.dist-info/top_level.txt,sha256=VgvLdN22xrjMzdP18fGULsr4ergDZbPZBI4GHD62ep0,20
+oc_ldap_user_locker-1.2.1.dist-info/RECORD,,
```

