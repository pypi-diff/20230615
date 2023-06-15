# Comparing `tmp/ipaclient-4.8.9-py2.py3-none-any.whl.zip` & `tmp/ipaclient-4.9.12-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,248 +1,236 @@
-Zip file size: 601886 bytes, number of entries: 246
--rw-rw-r--  2.0 unx      766 b- defN 18-Sep-28 11:25 ipaclient/__init__.py
--rw-rw-r--  2.0 unx      276 b- defN 20-May-11 09:00 ipaclient/__main__.py
--rw-rw-r--  2.0 unx    17008 b- defN 20-Jun-26 14:32 ipaclient/csrgen.py
--rw-rw-r--  2.0 unx    11568 b- defN 20-Jun-26 14:32 ipaclient/csrgen_ffi.py
--rw-rw-r--  2.0 unx    23867 b- defN 20-Jun-26 14:32 ipaclient/discovery.py
--rw-rw-r--  2.0 unx     5431 b- defN 20-Jul-09 07:26 ipaclient/frontend.py
--rw-rw-r--  2.0 unx      229 b- defN 19-Apr-08 14:24 ipaclient/csrgen/profiles/caIPAserviceCert.json
--rw-rw-r--  2.0 unx      235 b- defN 19-Apr-08 14:24 ipaclient/csrgen/profiles/userCert.json
--rw-rw-r--  2.0 unx      215 b- defN 19-Dec-13 14:59 ipaclient/csrgen/rules/dataDNS.json
--rw-rw-r--  2.0 unx      121 b- defN 19-Dec-13 14:59 ipaclient/csrgen/rules/dataEmail.json
--rw-rw-r--  2.0 unx      212 b- defN 19-Dec-13 14:59 ipaclient/csrgen/rules/dataHostCN.json
--rw-rw-r--  2.0 unx      153 b- defN 19-Dec-13 14:59 ipaclient/csrgen/rules/dataSubjectBase.json
--rw-rw-r--  2.0 unx      114 b- defN 19-Dec-13 14:59 ipaclient/csrgen/rules/dataUsernameCN.json
--rw-rw-r--  2.0 unx      166 b- defN 19-Dec-13 14:59 ipaclient/csrgen/rules/syntaxSAN.json
--rw-rw-r--  2.0 unx      213 b- defN 19-Dec-13 14:59 ipaclient/csrgen/rules/syntaxSubject.json
--rw-rw-r--  2.0 unx      428 b- defN 19-Dec-13 14:59 ipaclient/csrgen/templates/openssl_base.tmpl
--rw-rw-r--  2.0 unx      890 b- defN 19-Apr-08 14:24 ipaclient/csrgen/templates/openssl_macros.tmpl
--rw-rw-r--  2.0 unx      123 b- defN 18-Sep-28 11:25 ipaclient/plugins/__init__.py
--rw-rw-r--  2.0 unx     1178 b- defN 20-May-11 09:00 ipaclient/plugins/automember.py
--rw-rw-r--  2.0 unx    10638 b- defN 20-May-11 09:00 ipaclient/plugins/automount.py
--rw-rw-r--  2.0 unx     2087 b- defN 20-May-11 09:00 ipaclient/plugins/ca.py
--rw-rw-r--  2.0 unx     7401 b- defN 20-May-11 09:00 ipaclient/plugins/cert.py
--rw-rw-r--  2.0 unx     1596 b- defN 20-May-11 09:00 ipaclient/plugins/certmap.py
--rw-rw-r--  2.0 unx     1499 b- defN 20-May-11 09:00 ipaclient/plugins/certprofile.py
--rw-rw-r--  2.0 unx     3627 b- defN 20-May-11 09:00 ipaclient/plugins/csrgen.py
--rw-rw-r--  2.0 unx    18526 b- defN 20-Jun-26 14:32 ipaclient/plugins/dns.py
--rw-rw-r--  2.0 unx     1509 b- defN 20-May-11 09:00 ipaclient/plugins/hbacrule.py
--rw-rw-r--  2.0 unx     2175 b- defN 20-May-11 09:00 ipaclient/plugins/hbactest.py
--rw-rw-r--  2.0 unx     1876 b- defN 20-May-11 09:00 ipaclient/plugins/host.py
--rw-rw-r--  2.0 unx     3404 b- defN 20-May-11 09:00 ipaclient/plugins/idrange.py
--rw-rw-r--  2.0 unx     1443 b- defN 19-Apr-26 10:54 ipaclient/plugins/internal.py
--rw-rw-r--  2.0 unx     1057 b- defN 20-May-11 09:00 ipaclient/plugins/location.py
--rw-rw-r--  2.0 unx     3040 b- defN 20-May-11 09:00 ipaclient/plugins/migration.py
--rw-rw-r--  2.0 unx      886 b- defN 20-May-11 09:00 ipaclient/plugins/misc.py
--rw-rw-r--  2.0 unx     6368 b- defN 20-Jul-09 07:26 ipaclient/plugins/otptoken.py
--rw-rw-r--  2.0 unx     6365 b- defN 20-May-11 09:00 ipaclient/plugins/otptoken_yubikey.py
--rw-rw-r--  2.0 unx      441 b- defN 20-May-11 09:00 ipaclient/plugins/passwd.py
--rw-rw-r--  2.0 unx      774 b- defN 20-May-11 09:00 ipaclient/plugins/permission.py
--rw-rw-r--  2.0 unx     1651 b- defN 20-May-11 09:00 ipaclient/plugins/rpcclient.py
--rw-rw-r--  2.0 unx      626 b- defN 20-May-11 09:00 ipaclient/plugins/server.py
--rw-rw-r--  2.0 unx     1948 b- defN 20-May-11 09:00 ipaclient/plugins/service.py
--rw-rw-r--  2.0 unx     2221 b- defN 20-May-11 09:00 ipaclient/plugins/sudorule.py
--rw-rw-r--  2.0 unx     1937 b- defN 20-May-11 09:00 ipaclient/plugins/topology.py
--rw-rw-r--  2.0 unx     1897 b- defN 20-May-11 09:00 ipaclient/plugins/trust.py
--rw-rw-r--  2.0 unx     2966 b- defN 20-May-11 09:00 ipaclient/plugins/user.py
--rw-rw-r--  2.0 unx    37158 b- defN 20-Jun-26 14:32 ipaclient/plugins/vault.py
--rw-rw-r--  2.0 unx     3991 b- defN 20-May-11 09:00 ipaclient/remote_plugins/__init__.py
--rw-rw-r--  2.0 unx     2324 b- defN 20-Jul-09 07:26 ipaclient/remote_plugins/compat.py
--rw-rw-r--  2.0 unx    19022 b- defN 20-Jun-29 07:42 ipaclient/remote_plugins/schema.py
--rw-rw-r--  2.0 unx      265 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/__init__.py
--rw-rw-r--  2.0 unx    25449 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/aci.py
--rw-rw-r--  2.0 unx    24427 b- defN 20-Jul-09 07:26 ipaclient/remote_plugins/2_114/automember.py
--rw-rw-r--  2.0 unx    35202 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/automount.py
--rw-rw-r--  2.0 unx     1806 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/batch.py
--rw-rw-r--  2.0 unx     9773 b- defN 20-Jun-26 14:32 ipaclient/remote_plugins/2_114/cert.py
--rw-rw-r--  2.0 unx    13684 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/config.py
--rw-rw-r--  2.0 unx    10698 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/delegation.py
--rw-rw-r--  2.0 unx   167818 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/dns.py
--rw-rw-r--  2.0 unx    26481 b- defN 20-Jul-09 07:26 ipaclient/remote_plugins/2_114/group.py
--rw-rw-r--  2.0 unx    35745 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/hbacrule.py
--rw-rw-r--  2.0 unx    11491 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/hbacsvc.py
--rw-rw-r--  2.0 unx    14599 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/hbacsvcgroup.py
--rw-rw-r--  2.0 unx     9123 b- defN 20-Jul-09 07:26 ipaclient/remote_plugins/2_114/hbactest.py
--rw-rw-r--  2.0 unx    45438 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/host.py
--rw-rw-r--  2.0 unx    20339 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/hostgroup.py
--rw-rw-r--  2.0 unx    19509 b- defN 20-Aug-10 06:17 ipaclient/remote_plugins/2_114/idrange.py
--rw-rw-r--  2.0 unx    39044 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/idviews.py
--rw-rw-r--  2.0 unx     2019 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/internal.py
--rw-rw-r--  2.0 unx     1537 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/join.py
--rw-rw-r--  2.0 unx     7559 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/krbtpolicy.py
--rw-rw-r--  2.0 unx    10437 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/migration.py
--rw-rw-r--  2.0 unx     2753 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/misc.py
--rw-rw-r--  2.0 unx    24339 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/netgroup.py
--rw-rw-r--  2.0 unx     6184 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/otpconfig.py
--rw-rw-r--  2.0 unx    25992 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/otptoken.py
--rw-rw-r--  2.0 unx      690 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/otptoken_yubikey.py
--rw-rw-r--  2.0 unx     2431 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/passwd.py
--rw-rw-r--  2.0 unx    31931 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/permission.py
--rw-rw-r--  2.0 unx     1675 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/ping.py
--rw-rw-r--  2.0 unx     1198 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/pkinit.py
--rw-rw-r--  2.0 unx    17885 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/privilege.py
--rw-rw-r--  2.0 unx    27438 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/pwpolicy.py
--rw-rw-r--  2.0 unx    15257 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/radiusproxy.py
--rw-rw-r--  2.0 unx     5425 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/realmdomains.py
--rw-rw-r--  2.0 unx    20693 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/role.py
--rw-rw-r--  2.0 unx     9336 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/selfservice.py
--rw-rw-r--  2.0 unx    25184 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/selinuxusermap.py
--rw-rw-r--  2.0 unx    32359 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/service.py
--rw-rw-r--  2.0 unx    25143 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/session.py
--rw-rw-r--  2.0 unx    10873 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/sudocmd.py
--rw-rw-r--  2.0 unx    14955 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/sudocmdgroup.py
--rw-rw-r--  2.0 unx    50213 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/sudorule.py
--rw-rw-r--  2.0 unx    35406 b- defN 20-Jul-09 07:26 ipaclient/remote_plugins/2_114/trust.py
--rw-rw-r--  2.0 unx    46927 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_114/user.py
--rw-rw-r--  2.0 unx      265 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/__init__.py
--rw-rw-r--  2.0 unx    25449 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/aci.py
--rw-rw-r--  2.0 unx    24427 b- defN 20-Jul-09 07:26 ipaclient/remote_plugins/2_156/automember.py
--rw-rw-r--  2.0 unx    35304 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/automount.py
--rw-rw-r--  2.0 unx     1806 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/batch.py
--rw-rw-r--  2.0 unx    31324 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/caacl.py
--rw-rw-r--  2.0 unx     9940 b- defN 20-Jun-26 14:32 ipaclient/remote_plugins/2_156/cert.py
--rw-rw-r--  2.0 unx    12590 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/certprofile.py
--rw-rw-r--  2.0 unx    13698 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/config.py
--rw-rw-r--  2.0 unx    10698 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/delegation.py
--rw-rw-r--  2.0 unx   161194 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/dns.py
--rw-rw-r--  2.0 unx     1199 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/domainlevel.py
--rw-rw-r--  2.0 unx    26515 b- defN 20-Jul-09 07:26 ipaclient/remote_plugins/2_156/group.py
--rw-rw-r--  2.0 unx    35779 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/hbacrule.py
--rw-rw-r--  2.0 unx    11525 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/hbacsvc.py
--rw-rw-r--  2.0 unx    14633 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/hbacsvcgroup.py
--rw-rw-r--  2.0 unx     9123 b- defN 20-Jul-09 07:26 ipaclient/remote_plugins/2_156/hbactest.py
--rw-rw-r--  2.0 unx    48912 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/host.py
--rw-rw-r--  2.0 unx    20373 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/hostgroup.py
--rw-rw-r--  2.0 unx    20053 b- defN 20-Aug-10 06:17 ipaclient/remote_plugins/2_156/idrange.py
--rw-rw-r--  2.0 unx    42287 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/idviews.py
--rw-rw-r--  2.0 unx     2019 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/internal.py
--rw-rw-r--  2.0 unx     1537 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/join.py
--rw-rw-r--  2.0 unx     7559 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/krbtpolicy.py
--rw-rw-r--  2.0 unx    11089 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/migration.py
--rw-rw-r--  2.0 unx     2753 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/misc.py
--rw-rw-r--  2.0 unx    24373 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/netgroup.py
--rw-rw-r--  2.0 unx     6184 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/otpconfig.py
--rw-rw-r--  2.0 unx    26027 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/otptoken.py
--rw-rw-r--  2.0 unx      690 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/otptoken_yubikey.py
--rw-rw-r--  2.0 unx     2431 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/passwd.py
--rw-rw-r--  2.0 unx    34289 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/permission.py
--rw-rw-r--  2.0 unx     1675 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/ping.py
--rw-rw-r--  2.0 unx     1198 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/pkinit.py
--rw-rw-r--  2.0 unx    17919 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/privilege.py
--rw-rw-r--  2.0 unx    27506 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/pwpolicy.py
--rw-rw-r--  2.0 unx    15291 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/radiusproxy.py
--rw-rw-r--  2.0 unx     5425 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/realmdomains.py
--rw-rw-r--  2.0 unx    20727 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/role.py
--rw-rw-r--  2.0 unx     9336 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/selfservice.py
--rw-rw-r--  2.0 unx    25218 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/selinuxusermap.py
--rw-rw-r--  2.0 unx     6296 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/server.py
--rw-rw-r--  2.0 unx    35920 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/service.py
--rw-rw-r--  2.0 unx    25495 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/servicedelegation.py
--rw-rw-r--  2.0 unx      678 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/session.py
--rw-rw-r--  2.0 unx    43617 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/stageuser.py
--rw-rw-r--  2.0 unx    10907 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/sudocmd.py
--rw-rw-r--  2.0 unx    14989 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/sudocmdgroup.py
--rw-rw-r--  2.0 unx    50247 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/sudorule.py
--rw-rw-r--  2.0 unx    32297 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/topology.py
--rw-rw-r--  2.0 unx    35970 b- defN 20-Jul-09 07:26 ipaclient/remote_plugins/2_156/trust.py
--rw-rw-r--  2.0 unx    55185 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/user.py
--rw-rw-r--  2.0 unx    45219 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_156/vault.py
--rw-rw-r--  2.0 unx      265 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/__init__.py
--rw-rw-r--  2.0 unx    25449 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/aci.py
--rw-rw-r--  2.0 unx    24426 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/automember.py
--rw-rw-r--  2.0 unx    35304 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/automount.py
--rw-rw-r--  2.0 unx     1806 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/batch.py
--rw-rw-r--  2.0 unx    31324 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/caacl.py
--rw-rw-r--  2.0 unx     9940 b- defN 20-Jun-26 14:32 ipaclient/remote_plugins/2_164/cert.py
--rw-rw-r--  2.0 unx    12590 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/certprofile.py
--rw-rw-r--  2.0 unx    13738 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/config.py
--rw-rw-r--  2.0 unx    10698 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/delegation.py
--rw-rw-r--  2.0 unx   161863 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/dns.py
--rw-rw-r--  2.0 unx     1161 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/domainlevel.py
--rw-rw-r--  2.0 unx    26514 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/group.py
--rw-rw-r--  2.0 unx    35779 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/hbacrule.py
--rw-rw-r--  2.0 unx    11525 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/hbacsvc.py
--rw-rw-r--  2.0 unx    14633 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/hbacsvcgroup.py
--rw-rw-r--  2.0 unx     9122 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/hbactest.py
--rw-rw-r--  2.0 unx    48912 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/host.py
--rw-rw-r--  2.0 unx    20373 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/hostgroup.py
--rw-rw-r--  2.0 unx    20053 b- defN 20-Aug-10 06:17 ipaclient/remote_plugins/2_164/idrange.py
--rw-rw-r--  2.0 unx    42287 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/idviews.py
--rw-rw-r--  2.0 unx     2019 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/internal.py
--rw-rw-r--  2.0 unx     1490 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/join.py
--rw-rw-r--  2.0 unx     7559 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/krbtpolicy.py
--rw-rw-r--  2.0 unx    11089 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/migration.py
--rw-rw-r--  2.0 unx     2753 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/misc.py
--rw-rw-r--  2.0 unx    24373 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/netgroup.py
--rw-rw-r--  2.0 unx     6184 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/otpconfig.py
--rw-rw-r--  2.0 unx    26027 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/otptoken.py
--rw-rw-r--  2.0 unx      690 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/otptoken_yubikey.py
--rw-rw-r--  2.0 unx     2428 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/passwd.py
--rw-rw-r--  2.0 unx    34289 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/permission.py
--rw-rw-r--  2.0 unx     1675 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/ping.py
--rw-rw-r--  2.0 unx     1198 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/pkinit.py
--rw-rw-r--  2.0 unx    17919 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/privilege.py
--rw-rw-r--  2.0 unx    27506 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/pwpolicy.py
--rw-rw-r--  2.0 unx    15291 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/radiusproxy.py
--rw-rw-r--  2.0 unx     5425 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/realmdomains.py
--rw-rw-r--  2.0 unx    20727 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/role.py
--rw-rw-r--  2.0 unx     9336 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/selfservice.py
--rw-rw-r--  2.0 unx    25218 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/selinuxusermap.py
--rw-rw-r--  2.0 unx     8308 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/server.py
--rw-rw-r--  2.0 unx    35920 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/service.py
--rw-rw-r--  2.0 unx    25495 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/servicedelegation.py
--rw-rw-r--  2.0 unx      678 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/session.py
--rw-rw-r--  2.0 unx    46972 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/stageuser.py
--rw-rw-r--  2.0 unx    10907 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/sudocmd.py
--rw-rw-r--  2.0 unx    14989 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/sudocmdgroup.py
--rw-rw-r--  2.0 unx    50247 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/sudorule.py
--rw-rw-r--  2.0 unx    33854 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/topology.py
--rw-rw-r--  2.0 unx    35969 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/trust.py
--rw-rw-r--  2.0 unx    58614 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/user.py
--rw-rw-r--  2.0 unx    45219 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_164/vault.py
--rw-rw-r--  2.0 unx      264 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/__init__.py
--rw-rw-r--  2.0 unx    25387 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/aci.py
--rw-rw-r--  2.0 unx    22254 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/automember.py
--rw-rw-r--  2.0 unx    34860 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/automount.py
--rw-rw-r--  2.0 unx     1778 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/batch.py
--rw-rw-r--  2.0 unx     5126 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/cert.py
--rw-rw-r--  2.0 unx    13121 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/config.py
--rw-rw-r--  2.0 unx    10719 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/delegation.py
--rw-rw-r--  2.0 unx   162895 b- defN 20-Apr-29 12:15 ipaclient/remote_plugins/2_49/dns.py
--rw-rw-r--  2.0 unx    10381 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/entitle.py
--rw-rw-r--  2.0 unx    24815 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/group.py
--rw-rw-r--  2.0 unx    33334 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/hbacrule.py
--rw-rw-r--  2.0 unx    10742 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/hbacsvc.py
--rw-rw-r--  2.0 unx    13533 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/hbacsvcgroup.py
--rw-rw-r--  2.0 unx     6574 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/hbactest.py
--rw-rw-r--  2.0 unx    30139 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/host.py
--rw-rw-r--  2.0 unx    19153 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/hostgroup.py
--rw-rw-r--  2.0 unx    18929 b- defN 20-Aug-10 06:17 ipaclient/remote_plugins/2_49/idrange.py
--rw-rw-r--  2.0 unx     1994 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/internal.py
--rw-rw-r--  2.0 unx     1537 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/join.py
--rw-rw-r--  2.0 unx     7610 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/krbtpolicy.py
--rw-rw-r--  2.0 unx    10395 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/migration.py
--rw-rw-r--  2.0 unx     2753 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/misc.py
--rw-rw-r--  2.0 unx    23320 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/netgroup.py
--rw-rw-r--  2.0 unx     2263 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/passwd.py
--rw-rw-r--  2.0 unx    21798 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/permission.py
--rw-rw-r--  2.0 unx     1648 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/ping.py
--rw-rw-r--  2.0 unx     1170 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/pkinit.py
--rw-rw-r--  2.0 unx    16284 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/privilege.py
--rw-rw-r--  2.0 unx    27724 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/pwpolicy.py
--rw-rw-r--  2.0 unx    18589 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/role.py
--rw-rw-r--  2.0 unx     9297 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/selfservice.py
--rw-rw-r--  2.0 unx    23713 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/selinuxusermap.py
--rw-rw-r--  2.0 unx    18039 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/service.py
--rw-rw-r--  2.0 unx    25115 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/session.py
--rw-rw-r--  2.0 unx    10124 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/sudocmd.py
--rw-rw-r--  2.0 unx    13741 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/sudocmdgroup.py
--rw-rw-r--  2.0 unx    44052 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/sudorule.py
--rw-rw-r--  2.0 unx    20233 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/trust.py
--rw-rw-r--  2.0 unx    39108 b- defN 20-Apr-29 12:16 ipaclient/remote_plugins/2_49/user.py
--rw-rw-r--  2.0 unx    35147 b- defN 20-Aug-20 10:51 ipaclient-4.8.9.dist-info/COPYING
--rw-rw-r--  2.0 unx     1686 b- defN 20-Aug-20 10:51 ipaclient-4.8.9.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 20-Aug-20 10:51 ipaclient-4.8.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx       49 b- defN 20-Aug-20 10:51 ipaclient-4.8.9.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 20-Aug-20 10:51 ipaclient-4.8.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    23710 b- defN 20-Aug-20 10:51 ipaclient-4.8.9.dist-info/RECORD
-246 files, 4350889 bytes uncompressed, 563900 bytes compressed:  87.1%
+Zip file size: 590560 bytes, number of entries: 234
+-rw-r--r--  2.0 unx      766 b- defN 20-Sep-30 13:07 ipaclient/__init__.py
+-rw-r--r--  2.0 unx      276 b- defN 20-Sep-30 13:07 ipaclient/__main__.py
+-rw-r--r--  2.0 unx    23867 b- defN 23-Apr-18 05:46 ipaclient/discovery.py
+-rw-r--r--  2.0 unx     5623 b- defN 23-Jun-15 05:40 ipaclient/frontend.py
+-rw-r--r--  2.0 unx      123 b- defN 20-Sep-30 13:07 ipaclient/plugins/__init__.py
+-rw-r--r--  2.0 unx     1496 b- defN 23-May-31 07:34 ipaclient/plugins/automember.py
+-rw-r--r--  2.0 unx    10793 b- defN 23-Jun-15 05:40 ipaclient/plugins/automount.py
+-rw-r--r--  2.0 unx     4095 b- defN 23-Jun-07 16:59 ipaclient/plugins/baseuser.py
+-rw-r--r--  2.0 unx     2087 b- defN 23-Jan-19 08:00 ipaclient/plugins/ca.py
+-rw-r--r--  2.0 unx     4516 b- defN 23-Apr-18 05:46 ipaclient/plugins/cert.py
+-rw-r--r--  2.0 unx     1596 b- defN 23-Jan-19 08:00 ipaclient/plugins/certmap.py
+-rw-r--r--  2.0 unx     1499 b- defN 20-Sep-30 13:07 ipaclient/plugins/certprofile.py
+-rw-r--r--  2.0 unx    18526 b- defN 23-Apr-18 05:46 ipaclient/plugins/dns.py
+-rw-r--r--  2.0 unx     1509 b- defN 20-Sep-30 13:07 ipaclient/plugins/hbacrule.py
+-rw-r--r--  2.0 unx     2175 b- defN 20-Sep-30 13:07 ipaclient/plugins/hbactest.py
+-rw-r--r--  2.0 unx     1876 b- defN 20-Sep-30 13:07 ipaclient/plugins/host.py
+-rw-r--r--  2.0 unx     3404 b- defN 20-Sep-30 13:07 ipaclient/plugins/idrange.py
+-rw-r--r--  2.0 unx     1443 b- defN 20-Sep-30 13:07 ipaclient/plugins/internal.py
+-rw-r--r--  2.0 unx     1057 b- defN 20-Sep-30 13:07 ipaclient/plugins/location.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-Jan-19 08:00 ipaclient/plugins/migration.py
+-rw-r--r--  2.0 unx      886 b- defN 20-Sep-30 13:07 ipaclient/plugins/misc.py
+-rw-r--r--  2.0 unx     6395 b- defN 23-May-31 07:34 ipaclient/plugins/otptoken.py
+-rw-r--r--  2.0 unx     6413 b- defN 23-Jun-15 05:40 ipaclient/plugins/otptoken_yubikey.py
+-rw-r--r--  2.0 unx      441 b- defN 20-Sep-30 13:07 ipaclient/plugins/passwd.py
+-rw-r--r--  2.0 unx      774 b- defN 20-Sep-30 13:07 ipaclient/plugins/permission.py
+-rw-r--r--  2.0 unx     1651 b- defN 23-Jan-19 08:00 ipaclient/plugins/rpcclient.py
+-rw-r--r--  2.0 unx      626 b- defN 20-Sep-30 13:07 ipaclient/plugins/server.py
+-rw-r--r--  2.0 unx     1948 b- defN 20-Sep-30 13:07 ipaclient/plugins/service.py
+-rw-r--r--  2.0 unx      376 b- defN 23-Jun-07 16:59 ipaclient/plugins/stageuser.py
+-rw-r--r--  2.0 unx     2221 b- defN 23-Jun-15 05:40 ipaclient/plugins/sudorule.py
+-rw-r--r--  2.0 unx     1937 b- defN 20-Sep-30 13:07 ipaclient/plugins/topology.py
+-rw-r--r--  2.0 unx     1897 b- defN 20-Sep-30 13:07 ipaclient/plugins/trust.py
+-rw-r--r--  2.0 unx     2966 b- defN 23-Jun-15 05:34 ipaclient/plugins/user.py
+-rw-r--r--  2.0 unx    39982 b- defN 23-Jun-15 05:40 ipaclient/plugins/vault.py
+-rw-r--r--  2.0 unx     3963 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/__init__.py
+-rw-r--r--  2.0 unx     2462 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/compat.py
+-rw-r--r--  2.0 unx    18841 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/schema.py
+-rw-r--r--  2.0 unx      265 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/__init__.py
+-rw-r--r--  2.0 unx    25449 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/aci.py
+-rw-r--r--  2.0 unx    24427 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_114/automember.py
+-rw-r--r--  2.0 unx    35202 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/automount.py
+-rw-r--r--  2.0 unx     1806 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/batch.py
+-rw-r--r--  2.0 unx     9773 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_114/cert.py
+-rw-r--r--  2.0 unx    13684 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/config.py
+-rw-r--r--  2.0 unx    10698 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/delegation.py
+-rw-r--r--  2.0 unx   167818 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/dns.py
+-rw-r--r--  2.0 unx    26481 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_114/group.py
+-rw-r--r--  2.0 unx    35745 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/hbacrule.py
+-rw-r--r--  2.0 unx    11491 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/hbacsvc.py
+-rw-r--r--  2.0 unx    14599 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/hbacsvcgroup.py
+-rw-r--r--  2.0 unx     9123 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_114/hbactest.py
+-rw-r--r--  2.0 unx    45438 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/host.py
+-rw-r--r--  2.0 unx    20339 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/hostgroup.py
+-rw-r--r--  2.0 unx    19509 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_114/idrange.py
+-rw-r--r--  2.0 unx    39044 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/idviews.py
+-rw-r--r--  2.0 unx     2019 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/internal.py
+-rw-r--r--  2.0 unx     1537 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/join.py
+-rw-r--r--  2.0 unx     7559 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/krbtpolicy.py
+-rw-r--r--  2.0 unx    10437 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/migration.py
+-rw-r--r--  2.0 unx     2753 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/misc.py
+-rw-r--r--  2.0 unx    24339 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/netgroup.py
+-rw-r--r--  2.0 unx     6184 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/otpconfig.py
+-rw-r--r--  2.0 unx    25980 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_114/otptoken.py
+-rw-r--r--  2.0 unx      690 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/otptoken_yubikey.py
+-rw-r--r--  2.0 unx     2431 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/passwd.py
+-rw-r--r--  2.0 unx    31931 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/permission.py
+-rw-r--r--  2.0 unx     1675 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/ping.py
+-rw-r--r--  2.0 unx     1198 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/pkinit.py
+-rw-r--r--  2.0 unx    17885 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/privilege.py
+-rw-r--r--  2.0 unx    27438 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/pwpolicy.py
+-rw-r--r--  2.0 unx    15257 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/radiusproxy.py
+-rw-r--r--  2.0 unx     5425 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/realmdomains.py
+-rw-r--r--  2.0 unx    20693 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/role.py
+-rw-r--r--  2.0 unx     9336 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/selfservice.py
+-rw-r--r--  2.0 unx    25184 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/selinuxusermap.py
+-rw-r--r--  2.0 unx    32359 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/service.py
+-rw-r--r--  2.0 unx    25143 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/session.py
+-rw-r--r--  2.0 unx    10873 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/sudocmd.py
+-rw-r--r--  2.0 unx    14955 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/sudocmdgroup.py
+-rw-r--r--  2.0 unx    50226 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_114/sudorule.py
+-rw-r--r--  2.0 unx    35406 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_114/trust.py
+-rw-r--r--  2.0 unx    46927 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_114/user.py
+-rw-r--r--  2.0 unx      265 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/__init__.py
+-rw-r--r--  2.0 unx    25449 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/aci.py
+-rw-r--r--  2.0 unx    24427 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_156/automember.py
+-rw-r--r--  2.0 unx    35304 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/automount.py
+-rw-r--r--  2.0 unx     1806 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/batch.py
+-rw-r--r--  2.0 unx    31324 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/caacl.py
+-rw-r--r--  2.0 unx     9940 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_156/cert.py
+-rw-r--r--  2.0 unx    12586 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_156/certprofile.py
+-rw-r--r--  2.0 unx    13698 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/config.py
+-rw-r--r--  2.0 unx    10698 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/delegation.py
+-rw-r--r--  2.0 unx   161194 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/dns.py
+-rw-r--r--  2.0 unx     1199 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/domainlevel.py
+-rw-r--r--  2.0 unx    26515 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_156/group.py
+-rw-r--r--  2.0 unx    35779 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/hbacrule.py
+-rw-r--r--  2.0 unx    11525 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/hbacsvc.py
+-rw-r--r--  2.0 unx    14633 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/hbacsvcgroup.py
+-rw-r--r--  2.0 unx     9123 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_156/hbactest.py
+-rw-r--r--  2.0 unx    48912 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/host.py
+-rw-r--r--  2.0 unx    20373 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/hostgroup.py
+-rw-r--r--  2.0 unx    20053 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_156/idrange.py
+-rw-r--r--  2.0 unx    42287 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/idviews.py
+-rw-r--r--  2.0 unx     2019 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/internal.py
+-rw-r--r--  2.0 unx     1537 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/join.py
+-rw-r--r--  2.0 unx     7559 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/krbtpolicy.py
+-rw-r--r--  2.0 unx    11089 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/migration.py
+-rw-r--r--  2.0 unx     2753 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/misc.py
+-rw-r--r--  2.0 unx    24373 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/netgroup.py
+-rw-r--r--  2.0 unx     6184 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/otpconfig.py
+-rw-r--r--  2.0 unx    26015 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_156/otptoken.py
+-rw-r--r--  2.0 unx      690 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/otptoken_yubikey.py
+-rw-r--r--  2.0 unx     2431 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/passwd.py
+-rw-r--r--  2.0 unx    34289 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/permission.py
+-rw-r--r--  2.0 unx     1675 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/ping.py
+-rw-r--r--  2.0 unx     1198 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/pkinit.py
+-rw-r--r--  2.0 unx    17919 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/privilege.py
+-rw-r--r--  2.0 unx    27506 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/pwpolicy.py
+-rw-r--r--  2.0 unx    15291 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/radiusproxy.py
+-rw-r--r--  2.0 unx     5425 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/realmdomains.py
+-rw-r--r--  2.0 unx    20727 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/role.py
+-rw-r--r--  2.0 unx     9336 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/selfservice.py
+-rw-r--r--  2.0 unx    25218 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/selinuxusermap.py
+-rw-r--r--  2.0 unx     6296 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/server.py
+-rw-r--r--  2.0 unx    35920 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/service.py
+-rw-r--r--  2.0 unx    25495 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/servicedelegation.py
+-rw-r--r--  2.0 unx      678 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/session.py
+-rw-r--r--  2.0 unx    43617 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/stageuser.py
+-rw-r--r--  2.0 unx    10907 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/sudocmd.py
+-rw-r--r--  2.0 unx    14989 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/sudocmdgroup.py
+-rw-r--r--  2.0 unx    50260 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_156/sudorule.py
+-rw-r--r--  2.0 unx    32297 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/topology.py
+-rw-r--r--  2.0 unx    35970 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_156/trust.py
+-rw-r--r--  2.0 unx    55185 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/user.py
+-rw-r--r--  2.0 unx    45219 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_156/vault.py
+-rw-r--r--  2.0 unx      265 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/__init__.py
+-rw-r--r--  2.0 unx    25449 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/aci.py
+-rw-r--r--  2.0 unx    24426 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/automember.py
+-rw-r--r--  2.0 unx    35304 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/automount.py
+-rw-r--r--  2.0 unx     1806 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/batch.py
+-rw-r--r--  2.0 unx    31324 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/caacl.py
+-rw-r--r--  2.0 unx     9940 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_164/cert.py
+-rw-r--r--  2.0 unx    12586 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_164/certprofile.py
+-rw-r--r--  2.0 unx    13738 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/config.py
+-rw-r--r--  2.0 unx    10698 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/delegation.py
+-rw-r--r--  2.0 unx   161863 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/dns.py
+-rw-r--r--  2.0 unx     1161 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/domainlevel.py
+-rw-r--r--  2.0 unx    26514 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/group.py
+-rw-r--r--  2.0 unx    35779 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/hbacrule.py
+-rw-r--r--  2.0 unx    11525 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/hbacsvc.py
+-rw-r--r--  2.0 unx    14633 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/hbacsvcgroup.py
+-rw-r--r--  2.0 unx     9122 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/hbactest.py
+-rw-r--r--  2.0 unx    48912 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/host.py
+-rw-r--r--  2.0 unx    20373 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/hostgroup.py
+-rw-r--r--  2.0 unx    20053 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_164/idrange.py
+-rw-r--r--  2.0 unx    42287 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/idviews.py
+-rw-r--r--  2.0 unx     2019 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/internal.py
+-rw-r--r--  2.0 unx     1490 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/join.py
+-rw-r--r--  2.0 unx     7559 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/krbtpolicy.py
+-rw-r--r--  2.0 unx    11089 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/migration.py
+-rw-r--r--  2.0 unx     2753 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/misc.py
+-rw-r--r--  2.0 unx    24373 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/netgroup.py
+-rw-r--r--  2.0 unx     6184 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/otpconfig.py
+-rw-r--r--  2.0 unx    26015 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_164/otptoken.py
+-rw-r--r--  2.0 unx      690 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/otptoken_yubikey.py
+-rw-r--r--  2.0 unx     2428 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/passwd.py
+-rw-r--r--  2.0 unx    34289 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/permission.py
+-rw-r--r--  2.0 unx     1675 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/ping.py
+-rw-r--r--  2.0 unx     1198 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/pkinit.py
+-rw-r--r--  2.0 unx    17919 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/privilege.py
+-rw-r--r--  2.0 unx    27506 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/pwpolicy.py
+-rw-r--r--  2.0 unx    15291 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/radiusproxy.py
+-rw-r--r--  2.0 unx     5425 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/realmdomains.py
+-rw-r--r--  2.0 unx    20727 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/role.py
+-rw-r--r--  2.0 unx     9336 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/selfservice.py
+-rw-r--r--  2.0 unx    25218 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/selinuxusermap.py
+-rw-r--r--  2.0 unx     8308 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/server.py
+-rw-r--r--  2.0 unx    35920 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/service.py
+-rw-r--r--  2.0 unx    25495 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/servicedelegation.py
+-rw-r--r--  2.0 unx      678 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/session.py
+-rw-r--r--  2.0 unx    46972 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/stageuser.py
+-rw-r--r--  2.0 unx    10907 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/sudocmd.py
+-rw-r--r--  2.0 unx    14989 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/sudocmdgroup.py
+-rw-r--r--  2.0 unx    50260 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_164/sudorule.py
+-rw-r--r--  2.0 unx    33854 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/topology.py
+-rw-r--r--  2.0 unx    35969 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/trust.py
+-rw-r--r--  2.0 unx    58614 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/user.py
+-rw-r--r--  2.0 unx    45219 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_164/vault.py
+-rw-r--r--  2.0 unx      264 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/__init__.py
+-rw-r--r--  2.0 unx    25387 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/aci.py
+-rw-r--r--  2.0 unx    22254 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/automember.py
+-rw-r--r--  2.0 unx    34860 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/automount.py
+-rw-r--r--  2.0 unx     1778 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/batch.py
+-rw-r--r--  2.0 unx     5126 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/cert.py
+-rw-r--r--  2.0 unx    13121 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/config.py
+-rw-r--r--  2.0 unx    10719 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/delegation.py
+-rw-r--r--  2.0 unx   162895 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/dns.py
+-rw-r--r--  2.0 unx    10381 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/entitle.py
+-rw-r--r--  2.0 unx    24815 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/group.py
+-rw-r--r--  2.0 unx    33334 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/hbacrule.py
+-rw-r--r--  2.0 unx    10742 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/hbacsvc.py
+-rw-r--r--  2.0 unx    13533 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/hbacsvcgroup.py
+-rw-r--r--  2.0 unx     6574 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/hbactest.py
+-rw-r--r--  2.0 unx    30139 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/host.py
+-rw-r--r--  2.0 unx    19153 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/hostgroup.py
+-rw-r--r--  2.0 unx    18929 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_49/idrange.py
+-rw-r--r--  2.0 unx     1994 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/internal.py
+-rw-r--r--  2.0 unx     1537 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/join.py
+-rw-r--r--  2.0 unx     7610 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/krbtpolicy.py
+-rw-r--r--  2.0 unx    10395 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/migration.py
+-rw-r--r--  2.0 unx     2753 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/misc.py
+-rw-r--r--  2.0 unx    23320 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/netgroup.py
+-rw-r--r--  2.0 unx     2263 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/passwd.py
+-rw-r--r--  2.0 unx    21798 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/permission.py
+-rw-r--r--  2.0 unx     1648 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/ping.py
+-rw-r--r--  2.0 unx     1170 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/pkinit.py
+-rw-r--r--  2.0 unx    16284 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/privilege.py
+-rw-r--r--  2.0 unx    27724 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/pwpolicy.py
+-rw-r--r--  2.0 unx    18589 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/role.py
+-rw-r--r--  2.0 unx     9297 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/selfservice.py
+-rw-r--r--  2.0 unx    23713 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/selinuxusermap.py
+-rw-r--r--  2.0 unx    18039 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/service.py
+-rw-r--r--  2.0 unx    25115 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/session.py
+-rw-r--r--  2.0 unx    10124 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/sudocmd.py
+-rw-r--r--  2.0 unx    13741 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/sudocmdgroup.py
+-rw-r--r--  2.0 unx    44061 b- defN 23-Apr-18 05:46 ipaclient/remote_plugins/2_49/sudorule.py
+-rw-r--r--  2.0 unx    20233 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/trust.py
+-rw-r--r--  2.0 unx    39108 b- defN 20-Sep-30 13:07 ipaclient/remote_plugins/2_49/user.py
+-rw-rw-r--  2.0 unx    35147 b- defN 23-Jun-15 05:41 ipaclient-4.9.12.dist-info/COPYING
+-rw-r--r--  2.0 unx     1607 b- defN 23-Jun-15 05:41 ipaclient-4.9.12.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-15 05:41 ipaclient-4.9.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-15 05:41 ipaclient-4.9.12.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-15 05:41 ipaclient-4.9.12.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    22581 b- defN 23-Jun-15 05:41 ipaclient-4.9.12.dist-info/RECORD
+234 files, 4319584 bytes uncompressed, 554392 bytes compressed:  87.2%
```

## zipnote {}

```diff
@@ -1,82 +1,43 @@
 Filename: ipaclient/__init__.py
 Comment: 
 
 Filename: ipaclient/__main__.py
 Comment: 
 
-Filename: ipaclient/csrgen.py
-Comment: 
-
-Filename: ipaclient/csrgen_ffi.py
-Comment: 
-
 Filename: ipaclient/discovery.py
 Comment: 
 
 Filename: ipaclient/frontend.py
 Comment: 
 
-Filename: ipaclient/csrgen/profiles/caIPAserviceCert.json
-Comment: 
-
-Filename: ipaclient/csrgen/profiles/userCert.json
-Comment: 
-
-Filename: ipaclient/csrgen/rules/dataDNS.json
-Comment: 
-
-Filename: ipaclient/csrgen/rules/dataEmail.json
-Comment: 
-
-Filename: ipaclient/csrgen/rules/dataHostCN.json
-Comment: 
-
-Filename: ipaclient/csrgen/rules/dataSubjectBase.json
-Comment: 
-
-Filename: ipaclient/csrgen/rules/dataUsernameCN.json
-Comment: 
-
-Filename: ipaclient/csrgen/rules/syntaxSAN.json
-Comment: 
-
-Filename: ipaclient/csrgen/rules/syntaxSubject.json
-Comment: 
-
-Filename: ipaclient/csrgen/templates/openssl_base.tmpl
-Comment: 
-
-Filename: ipaclient/csrgen/templates/openssl_macros.tmpl
-Comment: 
-
 Filename: ipaclient/plugins/__init__.py
 Comment: 
 
 Filename: ipaclient/plugins/automember.py
 Comment: 
 
 Filename: ipaclient/plugins/automount.py
 Comment: 
 
+Filename: ipaclient/plugins/baseuser.py
+Comment: 
+
 Filename: ipaclient/plugins/ca.py
 Comment: 
 
 Filename: ipaclient/plugins/cert.py
 Comment: 
 
 Filename: ipaclient/plugins/certmap.py
 Comment: 
 
 Filename: ipaclient/plugins/certprofile.py
 Comment: 
 
-Filename: ipaclient/plugins/csrgen.py
-Comment: 
-
 Filename: ipaclient/plugins/dns.py
 Comment: 
 
 Filename: ipaclient/plugins/hbacrule.py
 Comment: 
 
 Filename: ipaclient/plugins/hbactest.py
@@ -117,14 +78,17 @@
 
 Filename: ipaclient/plugins/server.py
 Comment: 
 
 Filename: ipaclient/plugins/service.py
 Comment: 
 
+Filename: ipaclient/plugins/stageuser.py
+Comment: 
+
 Filename: ipaclient/plugins/sudorule.py
 Comment: 
 
 Filename: ipaclient/plugins/topology.py
 Comment: 
 
 Filename: ipaclient/plugins/trust.py
@@ -714,26 +678,26 @@
 
 Filename: ipaclient/remote_plugins/2_49/trust.py
 Comment: 
 
 Filename: ipaclient/remote_plugins/2_49/user.py
 Comment: 
 
-Filename: ipaclient-4.8.9.dist-info/COPYING
+Filename: ipaclient-4.9.12.dist-info/COPYING
 Comment: 
 
-Filename: ipaclient-4.8.9.dist-info/METADATA
+Filename: ipaclient-4.9.12.dist-info/METADATA
 Comment: 
 
-Filename: ipaclient-4.8.9.dist-info/WHEEL
+Filename: ipaclient-4.9.12.dist-info/WHEEL
 Comment: 
 
-Filename: ipaclient-4.8.9.dist-info/entry_points.txt
+Filename: ipaclient-4.9.12.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipaclient-4.8.9.dist-info/top_level.txt
+Filename: ipaclient-4.9.12.dist-info/top_level.txt
 Comment: 
 
-Filename: ipaclient-4.8.9.dist-info/RECORD
+Filename: ipaclient-4.9.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipaclient/discovery.py

```diff
@@ -16,23 +16,23 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 from __future__ import absolute_import
 
 import logging
-import socket
 
 import six
 
-from dns import resolver, rdatatype
+from dns import rdatatype
 from dns.exception import DNSException
 from ipalib import errors
+from ipalib.constants import FQDN
 from ipalib.util import validate_domain_name
-from ipapython.dnsutil import query_srv
+from ipapython.dnsutil import query_srv, resolve
 
 from ipaplatform.paths import paths
 from ipapython.ipautil import valid_ip, realm_to_suffix
 from ipapython.dn import DN
 
 try:
     import ldap  # pylint: disable=unused-import
@@ -218,15 +218,15 @@
         self.server = None
         autodiscovered = False
 
         if not servers:
             if not domain:  # domain not provided do full DNS discovery
                 # get the local host name
                 if not hostname:
-                    hostname = socket.getfqdn()
+                    hostname = FQDN
                     logger.debug('Hostname: %s', hostname)
                 if not hostname:
                     return BAD_HOST_CONFIG
 
                 if valid_ip(hostname):
                     return NOT_FQDN
 
@@ -558,15 +558,15 @@
             domain = self.domain
         # now, check for a Kerberos realm the local host or domain is in
         qname = "_kerberos." + domain
 
         logger.debug("Search DNS for TXT record of %s", qname)
 
         try:
-            answers = resolver.query(qname, rdatatype.TXT)
+            answers = resolve(qname, rdatatype.TXT)
         except DNSException as e:
             logger.debug("DNS record not found: %s", e.__class__.__name__)
             answers = []
 
         realm = None
         for answer in answers:
             logger.debug("DNS record found: %s", answer)
```

## ipaclient/frontend.py

```diff
@@ -122,33 +122,33 @@
         self.next = next_class(api)
 
     @classmethod
     def __get_next(cls):
         return api.get_plugin_next(cls)
 
     @classmethod
-    def __doc_getter(cls):
+    def __doc_getter(cls):  # pylint: disable=unused-private-member, #4756
         return cls.__get_next().doc
 
     doc = classproperty(__doc_getter)
 
     @classmethod
-    def __summary_getter(cls):
+    def __summary_getter(cls):  # pylint: disable=unused-private-member, #4756
         return cls.__get_next().summary
 
     summary = classproperty(__summary_getter)
 
     @classmethod
-    def __NO_CLI_getter(cls):
+    def __NO_CLI_getter(cls):  # pylint: disable=unused-private-member, #4756
         return cls.__get_next().NO_CLI
 
     NO_CLI = classproperty(__NO_CLI_getter)
 
     @classmethod
-    def __topic_getter(cls):
+    def __topic_getter(cls):  # pylint: disable=unused-private-member, #4756
         return cls.__get_next().topic
 
     topic = classproperty(__topic_getter)
 
     @property
     def forwarded_name(self):
         return self.next.forwarded_name
```

## ipaclient/plugins/automember.py

```diff
@@ -30,7 +30,15 @@
     has_output_params = (
         Str(
             'failed',
             label=_('Failed to add'),
             flags=['suppress_empty'],
         ),
     )
+
+
+@register(override=True, no_fail=True)
+class automember_rebuild(MethodOverride):
+    def interactive_prompt_callback(self, kw):
+        msg = _('IMPORTANT: In case of a high number of users, hosts or '
+                'groups, the operation may require high CPU usage.')
+        self.Backend.textui.print_plain(msg)
```

## ipaclient/plugins/automount.py

```diff
@@ -50,15 +50,15 @@
     name = 'automountlocation_show'
     NO_CLI = True
 
 
 @register(override=True, no_fail=True)
 class automountlocation_tofiles(MethodOverride):
     @classmethod
-    def __NO_CLI_getter(cls):
+    def __NO_CLI_getter(cls):  # pylint: disable=unused-private-member, #4756
         return (api.Command.get_plugin('automountlocation_show') is
                 _fake_automountlocation_show)
 
     NO_CLI = classproperty(__NO_CLI_getter)
 
     @property
     def api_version(self):
@@ -100,21 +100,23 @@
         textui.print_plain('')
         textui.print_plain(_('maps not connected to /etc/auto.master:'))
         for m in orphanmaps:
             textui.print_plain('---------------------------')
             textui.print_plain('/etc/%s:' % m['automountmapname'])
             for k in orphankeys:
                 if len(k) == 0: continue
-                dn = DN(k[0]['dn'])
-                if dn['automountmapname'] == m['automountmapname'][0]:
-                    textui.print_plain(
-                        '%s\t%s' % (
-                            k[0]['automountkey'][0], k[0]['automountinformation'][0]
+                for key in k:
+                    dn = DN(key['dn'])
+                    if dn['automountmapname'] == m['automountmapname'][0]:
+                        textui.print_plain(
+                            '%s\t%s' % (
+                                key['automountkey'][0],
+                                key['automountinformation'][0]
+                            )
                         )
-                    )
 
 
 @register()
 class automountlocation_import(Command):
     __doc__ = _('Import automount files for a specific location.')
 
     takes_args = (
@@ -212,24 +214,24 @@
                         raise errors.DuplicateEntry(
                             message=_('map %(map)s already exists') % dict(
                                 map=am[1]))
 
         # Now iterate over the map files and add the keys. To handle
         # continuation lines I'll make a pass through it to skip comments
         # etc and also to combine lines.
-        for m in maps:
-            map = self.__read_mapfile(maps[m])
+        for m, filename in maps.items():
+            map = self.__read_mapfile(filename)
             lines = []
             cont = ''
             for x in map:
                 if x.startswith('#'):
                     continue
                 x = x.rstrip()
                 if x.startswith('+'):
-                    result['skipped'].append([m, maps[m]])
+                    result['skipped'].append([m, filename])
                     continue
                 if len(x) == 0:
                     continue
                 if x.endswith("\\"):
                     cont = cont + x[:-1] + ' '
                 else:
                     lines.append(cont + x)
```

## ipaclient/plugins/cert.py

```diff
@@ -17,27 +17,22 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import base64
 
-import six
-
 from ipaclient.frontend import MethodOverride
 from ipalib import errors
 from ipalib import x509
 from ipalib import util
 from ipalib.parameters import BinaryFile, File, Flag, Str
 from ipalib.plugable import Registry
 from ipalib.text import _
 
-if six.PY3:
-    unicode = str
-
 register = Registry()
 
 
 class CertRetrieveOverride(MethodOverride):
     takes_options = (
         Str(
             'certificate_out?',
@@ -69,95 +64,20 @@
             x509.write_certificate_list(certs, certificate_out)
 
         return result
 
 
 @register(override=True, no_fail=True)
 class cert_request(CertRetrieveOverride):
-    takes_options = CertRetrieveOverride.takes_options + (
-        Str(
-            'database?',
-            label=_('Path to NSS database'),
-            doc=_('Path to NSS database to use for private key'),
-        ),
-        Str(
-            'private_key?',
-            label=_('Path to private key file'),
-            doc=_('Path to PEM file containing a private key'),
-        ),
-        Str(
-            'password_file?',
-            label=_(
-                'File containing a password for the private key or database'),
-        ),
-        Str(
-            'csr_profile_id?',
-            label=_('Name of CSR generation profile (if not the same as'
-                    ' profile_id)'),
-        ),
-    )
-
     def get_args(self):
         for arg in super(cert_request, self).get_args():
             if arg.name == 'csr':
                 arg = arg.clone_retype(arg.name, File, required=False)
             yield arg
 
-    def forward(self, csr=None, **options):
-        database = options.pop('database', None)
-        private_key = options.pop('private_key', None)
-        csr_profile_id = options.pop('csr_profile_id', None)
-        password_file = options.pop('password_file', None)
-
-        if csr is None:
-            # Deferred import, ipaclient.csrgen is expensive to load.
-            # see https://pagure.io/freeipa/issue/7484
-            from ipaclient import csrgen
-
-            if database:
-                adaptor = csrgen.NSSAdaptor(database, password_file)
-            elif private_key:
-                adaptor = csrgen.OpenSSLAdaptor(
-                    key_filename=private_key, password_filename=password_file)
-            else:
-                raise errors.InvocationError(
-                    message=u"One of 'database' or 'private_key' is required")
-
-            pubkey_info = adaptor.get_subject_public_key_info()
-            pubkey_info_b64 = base64.b64encode(pubkey_info)
-
-            # If csr_profile_id is passed, that takes precedence.
-            # Otherwise, use profile_id. If neither are passed, the default
-            # in cert_get_requestdata will be used.
-            profile_id = csr_profile_id
-            if profile_id is None:
-                profile_id = options.get('profile_id')
-
-            response = self.api.Command.cert_get_requestdata(
-                profile_id=profile_id,
-                principal=options.get('principal'),
-                public_key_info=pubkey_info_b64)
-
-            req_info_b64 = response['result']['request_info']
-            req_info = base64.b64decode(req_info_b64)
-
-            csr = adaptor.sign_csr(req_info)
-
-            if not csr:
-                raise errors.CertificateOperationError(
-                    error=(_('Generated CSR was empty')))
-
-        else:
-            if database is not None or private_key is not None:
-                raise errors.MutuallyExclusiveError(reason=_(
-                    "Options 'database' and 'private_key' are not compatible"
-                    " with 'csr'"))
-
-        return super(cert_request, self).forward(csr, **options)
-
 
 @register(override=True, no_fail=True)
 class cert_show(CertRetrieveOverride):
     def get_options(self):
         for option in super(cert_show, self).get_options():
             if option.name == 'out':
                 # skip server-defined --out
```

## ipaclient/plugins/otptoken.py

```diff
@@ -18,14 +18,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import print_function
 import sys
 
 from ipaclient.frontend import MethodOverride
 from ipalib import api, Str, Password, _
+from ipalib import errors
 from ipalib.messages import add_message, ResultFormattingError
 from ipalib.plugable import Registry
 from ipalib.frontend import Local
 from ipalib.util import create_https_connection
 from ipapython.version import API_VERSION
 
 import locale
@@ -125,15 +126,14 @@
 
     def __inner(self, host, **kwargs):
         tmp = self.__kwargs.copy()
         tmp.update(kwargs)
         return create_https_connection(host, **tmp)
 
     def https_open(self, req):
-        # pylint: disable=no-member
         return self.do_open(self.__inner, req)
 
 @register()
 class otptoken_sync(Local):
     __doc__ = _('Synchronize an OTP token.')
 
     header = 'X-IPA-TokenSync-Result'
@@ -152,39 +152,38 @@
     def forward(self, *args, **kwargs):
         status = {'result': {self.header: 'unknown'}}
 
         # Get the sync URI.
         segments = list(urllib.parse.urlparse(self.api.env.xmlrpc_uri))
         assert segments[0] == 'https' # Ensure encryption.
         segments[2] = segments[2].replace('/xml', '/session/sync_token')
-        # urlunparse *can* take one argument
-        # pylint: disable=too-many-function-args
         sync_uri = urllib.parse.urlunparse(segments)
 
         # Prepare the query.
         options = {x.name for x in self.takes_options}
         query = {k: v for k, v in kwargs.items() if k in options}
         if args and args[0] is not None:
             # sync_token converts token name to token DN
             query['token'] = args[0]
         query = urllib.parse.urlencode(query)
         query = query.encode('utf-8')
 
         # Sync the token.
-        # pylint: disable=E1101
         handler = HTTPSHandler(
             cafile=api.env.tls_ca_cert,
             tls_version_min=api.env.tls_version_min,
             tls_version_max=api.env.tls_version_max)
         rsp = urllib.request.build_opener(handler).open(sync_uri, query)
         if rsp.getcode() == 200:
             status['result'][self.header] = rsp.info().get(self.header, 'unknown')
         rsp.close()
 
+        if status['result'][self.header] != "ok":
+            msg = {'error': 'Error contacting server!',
+                   'invalid-credentials': 'Invalid Credentials!',
+                   }.get(status['result'][self.header], 'Unknown Error!')
+            raise errors.ExecutionError(
+                message=_("Unable to synchronize token: %s") % msg)
         return status
 
     def output_for_cli(self, textui, result, *keys, **options):
-        textui.print_plain({
-            'ok': 'Token synchronized.',
-            'error': 'Error contacting server!',
-            'invalid-credentials': 'Invalid Credentials!',
-        }.get(result['result'][self.header], 'Unknown Error!'))
+        textui.print_plain('Token synchronized.')
```

## ipaclient/plugins/otptoken_yubikey.py

```diff
@@ -77,15 +77,15 @@
             label=_('YubiKey slot'),
             values=(1, 2),
         ),
     )
     has_output_params = takes_options
 
     @classmethod
-    def __NO_CLI_getter(cls):
+    def __NO_CLI_getter(cls):  # pylint: disable=unused-private-member, #4756
         return api.Command.get_plugin('otptoken_add') is _fake_otptoken_add
 
     NO_CLI = classproperty(__NO_CLI_getter)
 
     @property
     def api_version(self):
         return self.api.Command.otptoken_add.api_version
```

## ipaclient/plugins/vault.py

```diff
@@ -21,29 +21,30 @@
 
 import base64
 import errno
 import io
 import json
 import logging
 import os
+import ssl
 import tempfile
 
 from cryptography.fernet import Fernet, InvalidToken
 from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes, serialization
+from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.padding import PKCS7
 from cryptography.hazmat.primitives.serialization import (
     load_pem_public_key, load_pem_private_key)
 
 from ipaclient.frontend import MethodOverride
 from ipalib import x509
-from ipalib.constants import USER_CACHE_PATH
+from ipalib import constants
 from ipalib.frontend import Local, Method, Object
 from ipalib.util import classproperty
 from ipalib import api, errors
 from ipalib import Bytes, Flag, Str
 from ipalib.plugable import Registry
 from ipalib import _
 from ipapython import ipautil
@@ -195,15 +196,15 @@
             'public_key_file?',
             cli_name='public_key_file',
             doc=_('File containing the vault public key'),
         ),
     )
 
     @classmethod
-    def __NO_CLI_getter(cls):
+    def __NO_CLI_getter(cls):  # pylint: disable=unused-private-member, #4756
         return (api.Command.get_plugin('vault_add_internal') is
                 _fake_vault_add_internal)
 
     NO_CLI = classproperty(__NO_CLI_getter)
 
     @property
     def api_version(self):
@@ -406,15 +407,15 @@
             'public_key_file?',
             cli_name='public_key_file',
             doc=_('File containing the new vault public key'),
         ),
     )
 
     @classmethod
-    def __NO_CLI_getter(cls):
+    def __NO_CLI_getter(cls):  # pylint: disable=unused-private-member, #4756
         return (api.Command.get_plugin('vault_mod_internal') is
                 _fake_vault_mod_internal)
 
     NO_CLI = classproperty(__NO_CLI_getter)
 
     @property
     def api_version(self):
@@ -542,73 +543,81 @@
             opts['override_password'] = True
 
             self.api.Command.vault_archive(*args, **opts)
 
         return response
 
 
-class _TransportCertCache:
+class _KraConfigCache:
+    """The KRA config cache stores vaultconfig-show result.
+    """
     def __init__(self):
         self._dirname = os.path.join(
-                USER_CACHE_PATH, 'ipa', 'kra-transport-certs'
+            constants.USER_CACHE_PATH, 'ipa', 'kra-config'
         )
 
     def _get_filename(self, domain):
-        basename = DNSName(domain).ToASCII() + '.pem'
+        basename = DNSName(domain).ToASCII() + '.json'
         return os.path.join(self._dirname, basename)
 
-    def load_cert(self, domain):
-        """Load cert from cache
+    def load(self, domain):
+        """Load config from cache
 
         :param domain: IPA domain
-        :return: cryptography.x509.Certificate or None
+        :return: dict or None
         """
         filename = self._get_filename(domain)
         try:
             try:
-                return x509.load_certificate_from_file(filename)
-            except EnvironmentError as e:
+                with open(filename) as f:
+                    return json.load(f)
+            except OSError as e:
                 if e.errno != errno.ENOENT:
                     raise
         except Exception:
             logger.warning("Failed to load %s", filename, exc_info=True)
+        return None
 
-    def store_cert(self, domain, transport_cert):
-        """Store a new cert or override existing cert
+    def store(self, domain, response):
+        """Store config in cache
 
         :param domain: IPA domain
-        :param transport_cert: cryptography.x509.Certificate
-        :return: True if cert was stored successfully
+        :param config: ipa vaultconfig-show response
+        :return: True if config was stored successfully
         """
+        config = response['result'].copy()
+        # store certificate as PEM-encoded ASCII
+        config['transport_cert'] = ssl.DER_cert_to_PEM_cert(
+            config['transport_cert']
+        )
         filename = self._get_filename(domain)
-        pem = transport_cert.public_bytes(serialization.Encoding.PEM)
         try:
             try:
                 os.makedirs(self._dirname)
             except EnvironmentError as e:
                 if e.errno != errno.EEXIST:
                     raise
             with tempfile.NamedTemporaryFile(dir=self._dirname, delete=False,
-                                             mode='wb') as f:
+                                             mode='w') as f:
                 try:
-                    f.write(pem)
+                    json.dump(config, f)
                     ipautil.flush_sync(f)
                     f.close()
                     os.rename(f.name, filename)
                 except Exception:
                     os.unlink(f.name)
                     raise
         except Exception:
             logger.warning("Failed to save %s", filename, exc_info=True)
             return False
         else:
             return True
 
-    def remove_cert(self, domain):
-        """Remove a cert from cache, ignores errors
+    def remove(self, domain):
+        """Remove a config from cache, ignores errors
 
         :param domain: IPA domain
         :return: True if cert was found and removed
         """
         filename = self._get_filename(domain)
         try:
             os.unlink(filename)
@@ -616,49 +625,88 @@
             if e.errno != errno.ENOENT:
                 logger.warning("Failed to remove %s", filename, exc_info=True)
             return False
         else:
             return True
 
 
-_transport_cert_cache = _TransportCertCache()
+_kra_config_cache = _KraConfigCache()
 
 
 @register(override=True, no_fail=True)
 class vaultconfig_show(MethodOverride):
     def forward(self, *args, **options):
 
         file = options.get('transport_out')
 
         # don't send these parameters to server
         if 'transport_out' in options:
             del options['transport_out']
 
         response = super(vaultconfig_show, self).forward(*args, **options)
 
-        # cache transport certificate
-        transport_cert = x509.load_der_x509_certificate(
-                response['result']['transport_cert'])
-
-        _transport_cert_cache.store_cert(
-            self.api.env.domain, transport_cert
-        )
+        # cache config
+        _kra_config_cache.store(self.api.env.domain, response)
 
         if file:
             with open(file, 'wb') as f:
                 f.write(response['result']['transport_cert'])
 
         return response
 
 
 class ModVaultData(Local):
-    def _generate_session_key(self):
-        key_length = max(algorithms.TripleDES.key_sizes)
-        algo = algorithms.TripleDES(os.urandom(key_length // 8))
-        return algo
+    def _generate_session_key(self, name):
+        if name not in constants.VAULT_WRAPPING_SUPPORTED_ALGOS:
+            msg = _("{algo} is not a supported vault wrapping algorithm")
+            raise errors.ValidationError(msg.format(algo=repr(name)))
+        if name == constants.VAULT_WRAPPING_AES128_CBC:
+            return algorithms.AES(os.urandom(128 // 8))
+        elif name == constants.VAULT_WRAPPING_3DES:
+            return algorithms.TripleDES(os.urandom(196 // 8))
+        else:
+            # unreachable
+            raise ValueError(name)
+
+    def _get_vaultconfig(self, force_refresh=False):
+        config = None
+        if not force_refresh:
+            config = _kra_config_cache.load(self.api.env.domain)
+        if config is None:
+            # vaultconfig_show also caches data
+            response = self.api.Command.vaultconfig_show()
+            config = response['result']
+            transport_cert = x509.load_der_x509_certificate(
+                config['transport_cert']
+            )
+        else:
+            # cached JSON uses PEM-encoded ASCII string
+            transport_cert = x509.load_pem_x509_certificate(
+                config['transport_cert'].encode('ascii')
+            )
+
+        default_algo = config.get('wrapping_default_algorithm')
+        if default_algo is None:
+            # old server
+            wrapping_algo = constants.VAULT_WRAPPING_3DES
+        elif default_algo in constants.VAULT_WRAPPING_SUPPORTED_ALGOS:
+            # try to use server default
+            wrapping_algo = default_algo
+        else:
+            # prefer server's sorting order
+            for algo in config['wrapping_supported_algorithms']:
+                if algo in constants.VAULT_WRAPPING_SUPPORTED_ALGOS:
+                    wrapping_algo = algo
+                    break
+            else:
+                raise errors.ValidationError(
+                    "No overlapping wrapping algorithm between server and "
+                    "client."
+                )
+        return transport_cert, wrapping_algo
 
     def _do_internal(self, algo, transport_cert, raise_unexpected,
                      *args, **options):
         public_key = transport_cert.public_key()
 
         # wrap session key with transport certificate
         wrapped_session_key = public_key.encrypt(
@@ -670,36 +718,31 @@
         name = self.name + '_internal'
         try:
             # ipalib.errors.NotFound exception can be propagated
             return self.api.Command[name](*args, **options)
         except (errors.InternalError,
                 errors.ExecutionError,
                 errors.GenericError):
-            _transport_cert_cache.remove_cert(self.api.env.domain)
+            _kra_config_cache.remove(self.api.env.domain)
             if raise_unexpected:
                 raise
+        return None
 
-    def internal(self, algo, *args, **options):
+    def internal(self, algo, transport_cert, *args, **options):
         """
         Calls the internal counterpart of the command.
         """
-        domain = self.api.env.domain
-
         # try call with cached transport certificate
-        transport_cert = _transport_cert_cache.load_cert(domain)
-        if transport_cert is not None:
-            result = self._do_internal(algo, transport_cert, False,
+        result = self._do_internal(algo, transport_cert, False,
                                        *args, **options)
-            if result is not None:
-                return result
+        if result is not None:
+            return result
 
         # retrieve transport certificate (cached by vaultconfig_show)
-        response = self.api.Command.vaultconfig_show()
-        transport_cert = x509.load_der_x509_certificate(
-            response['result']['transport_cert'])
+        transport_cert = self._get_vaultconfig(force_refresh=True)[0]
         # call with the retrieved transport certificate
         return self._do_internal(algo, transport_cert, True,
                                  *args, **options)
 
 
 @register(no_fail=True)
 class _fake_vault_archive_internal(Method):
@@ -733,15 +776,15 @@
         Flag(
             'override_password?',
             doc=_('Override existing password'),
         ),
     )
 
     @classmethod
-    def __NO_CLI_getter(cls):
+    def __NO_CLI_getter(cls):  # pylint: disable=unused-private-member, #4756
         return (api.Command.get_plugin('vault_archive_internal') is
                 _fake_vault_archive_internal)
 
     NO_CLI = classproperty(__NO_CLI_getter)
 
     @property
     def api_version(self):
@@ -754,15 +797,16 @@
             yield arg
 
     def get_options(self):
         for option in self.api.Command.vault_archive_internal.options():
             if option.name not in ('nonce',
                                    'session_key',
                                    'vault_data',
-                                   'version'):
+                                   'version',
+                                   'wrapping_algo'):
                 yield option
         for option in super(vault_archive, self).get_options():
             yield option
 
     def get_output_params(self):
         for param in self.api.Command.vault_archive_internal.output_params():
             yield param
@@ -771,15 +815,15 @@
 
     def _iter_output(self):
         return self.api.Command.vault_archive_internal.output()
 
     def _wrap_data(self, algo, json_vault_data):
         """Encrypt data with wrapped session key and transport cert
 
-        :param bytes algo: wrapping algorithm instance
+        :param algo: wrapping algorithm instance
         :param bytes json_vault_data: dumped vault data
         :return:
         """
         nonce = os.urandom(algo.block_size // 8)
 
         # wrap vault_data with session key
         padder = PKCS7(algo.block_size).padder()
@@ -923,23 +967,32 @@
         }
         if encrypted_key:
             vault_data[u'encrypted_key'] = base64.b64encode(encrypted_key)\
                 .decode('utf-8')
 
         json_vault_data = json.dumps(vault_data).encode('utf-8')
 
+        # get config
+        transport_cert, wrapping_algo = self._get_vaultconfig()
+        # let options override wrapping algo
+        # For backwards compatibility do not send old legacy wrapping algo
+        # to server. Only send the option when non-3DES is used.
+        wrapping_algo = options.pop('wrapping_algo', wrapping_algo)
+        if wrapping_algo != constants.VAULT_WRAPPING_3DES:
+            options['wrapping_algo'] = wrapping_algo
+
         # generate session key
-        algo = self._generate_session_key()
+        algo = self._generate_session_key(wrapping_algo)
         # wrap vault data
         nonce, wrapped_vault_data = self._wrap_data(algo, json_vault_data)
         options.update(
             nonce=nonce,
             vault_data=wrapped_vault_data
         )
-        return self.internal(algo, *args, **options)
+        return self.internal(algo, transport_cert, *args, **options)
 
 
 @register(no_fail=True)
 class _fake_vault_retrieve_internal(Method):
     name = 'vault_retrieve_internal'
     NO_CLI = True
 
@@ -979,15 +1032,15 @@
         Bytes(
             'data',
             label=_('Data'),
         ),
     )
 
     @classmethod
-    def __NO_CLI_getter(cls):
+    def __NO_CLI_getter(cls):  # pylint: disable=unused-private-member, #4756
         return (api.Command.get_plugin('vault_retrieve_internal') is
                 _fake_vault_retrieve_internal)
 
     NO_CLI = classproperty(__NO_CLI_getter)
 
     @property
     def api_version(self):
@@ -997,15 +1050,15 @@
         for arg in self.api.Command.vault_retrieve_internal.args():
             yield arg
         for arg in super(vault_retrieve, self).get_args():
             yield arg
 
     def get_options(self):
         for option in self.api.Command.vault_retrieve_internal.options():
-            if option.name not in ('session_key', 'version'):
+            if option.name not in ('session_key', 'version', 'wrapping_algo'):
                 yield option
         for option in super(vault_retrieve, self).get_options():
             yield option
 
     def get_output_params(self):
         for param in self.api.Command.vault_retrieve_internal.output_params():
             yield param
@@ -1055,18 +1108,27 @@
         if not backend.isconnected():
             backend.connect()
 
         # retrieve vault info
         vault = self.api.Command.vault_show(*args, **options)['result']
         vault_type = vault['ipavaulttype'][0]
 
+        # get config
+        transport_cert, wrapping_algo = self._get_vaultconfig()
+        # let options override wrapping algo
+        # For backwards compatibility do not send old legacy wrapping algo
+        # to server. Only send the option when non-3DES is used.
+        wrapping_algo = options.pop('wrapping_algo', wrapping_algo)
+        if wrapping_algo != constants.VAULT_WRAPPING_3DES:
+            options['wrapping_algo'] = wrapping_algo
+
         # generate session key
-        algo = self._generate_session_key()
+        algo = self._generate_session_key(wrapping_algo)
         # send retrieval request to server
-        response = self.internal(algo, *args, **options)
+        response = self.internal(algo, transport_cert, *args, **options)
         # unwrap data with session key
         vault_data = self._unwrap_response(
             algo,
             response['result']['nonce'],
             response['result']['vault_data']
         )
         del algo
```

## ipaclient/remote_plugins/__init__.py

```diff
@@ -1,50 +1,43 @@
 #
 # Copyright (C) 2016  FreeIPA Contributors see COPYING for license
 #
 
+from collections.abc import MutableMapping
 import errno
 import json
 import locale
 import logging
 import os
 import time
 
-import six
-
 from . import compat
 from . import schema
 from ipaclient.plugins.rpcclient import rpcclient
 from ipalib.constants import USER_CACHE_PATH
 from ipapython.dnsutil import DNSName
 
-# pylint: disable=no-name-in-module, import-error
-if six.PY3:
-    from collections.abc import MutableMapping
-else:
-    from collections import MutableMapping
-# pylint: enable=no-name-in-module, import-error
-
 logger = logging.getLogger(__name__)
 
 
 class ServerInfo(MutableMapping):
     _DIR = os.path.join(USER_CACHE_PATH, 'ipa', 'servers')
 
     def __init__(self, api):
         hostname = DNSName(api.env.server).ToASCII()
         self._path = os.path.join(self._DIR, hostname)
         self._force_check = api.env.force_schema_check
+        self._now = time.time()
         self._dict = {}
 
         # copy-paste from ipalib/rpc.py
         try:
             self._language = locale.setlocale(
                 locale.LC_MESSAGES, ''
-            ).split('.')[0].lower()
+            ).split('.', maxsplit=1)[0].lower()
         except locale.Error:
             self._language = 'en_us'
 
         self._read()
 
     def _read(self):
         try:
@@ -83,48 +76,49 @@
 
     def __iter__(self):
         return iter(self._dict)
 
     def __len__(self):
         return len(self._dict)
 
-    def update_validity(self, ttl=None):
-        if ttl is None:
-            ttl = 3600
-        self['expiration'] = time.time() + ttl
-        self['language'] = self._language
-        self._write()
+    def update_validity(self, ttl):
+        if not self.is_valid():
+            self['expiration'] = self._now + ttl
+            self['language'] = self._language
+            self._write()
 
     def is_valid(self):
         if self._force_check:
             return False
 
         try:
             expiration = self._dict['expiration']
             language = self._dict['language']
         except KeyError:
             # if any of these is missing consider the entry expired
             return False
 
-        if expiration < time.time():
-            # validity passed
+        if expiration < self._now:
             return False
 
         if language != self._language:
             # language changed since last check
             return False
 
         return True
 
 
 def get_package(api):
     if api.env.in_tree:
+        # server packages are not published on pypi.org
+        # pylint: disable=useless-suppression
         # pylint: disable=import-error,ipa-forbidden-import
         from ipaserver import plugins
         # pylint: enable=import-error,ipa-forbidden-import
+        # pylint: enable=useless-suppression
     else:
         try:
             plugins = api._remote_plugins
         except AttributeError:
             server_info = ServerInfo(api)
 
             client = rpcclient(api)
```

## ipaclient/remote_plugins/compat.py

```diff
@@ -54,15 +54,18 @@
             except KeyError:
                 match = None
             if match is not None:
                 server_version = match.group(1)
             else:
                 server_version = '2.0'
         server_info['version'] = server_version
-        server_info.update_validity()
+
+        # in compat mode we don't get the schema TTL from the server
+        # so use the client context value.
+        server_info.update_validity(client.api.env.schema_ttl)
 
     server_version = APIVersion(server_version)
 
     package_names = {}
     base_name = __name__.rpartition('.')[0]
     base_dir = os.path.dirname(__file__)
     for name in os.listdir(base_dir):
```

## ipaclient/remote_plugins/schema.py

```diff
@@ -1,11 +1,12 @@
 #
 # Copyright (C) 2016  FreeIPA Contributors see COPYING for license
 #
 
+from collections.abc import Mapping, Sequence
 import errno
 import json
 import logging
 import os
 import sys
 import tempfile
 import types
@@ -23,21 +24,14 @@
 from ipalib.output import Output
 from ipalib.parameters import DefaultFrom, Flag, Password, Str
 from ipapython import ipautil
 from ipapython.ipautil import fsdecode
 from ipapython.dn import DN
 from ipapython.dnsutil import DNSName
 
-# pylint: disable=no-name-in-module, import-error
-if six.PY3:
-    from collections.abc import Mapping, Sequence
-else:
-    from collections import Mapping, Sequence
-# pylint: enable=no-name-in-module, import-error
-
 logger = logging.getLogger(__name__)
 
 FORMAT = '1'
 
 if six.PY3:
     unicode = str
 
@@ -371,24 +365,23 @@
     >>> m['topics'][u'ping'][u'doc']
     u'Ping the remote IPA server to ...'
 
     """
     namespaces = {'classes', 'commands', 'topics'}
     _DIR = os.path.join(USER_CACHE_PATH, 'ipa', 'schema', FORMAT)
 
-    def __init__(self, client, fingerprint=None):
+    def __init__(self, client, fingerprint=None, ttl=0):
         self._dict = {}
         self._namespaces = {}
         self._help = None
 
         for ns in self.namespaces:
             self._dict[ns] = {}
             self._namespaces[ns] = _SchemaNameSpace(self, ns)
 
-        ttl = None
         read_failed = False
 
         if fingerprint is not None:
             try:
                 self._read_schema(fingerprint)
             except Exception as e:
                 # Failed to read the schema from cache. There may be a lot of
@@ -529,15 +522,15 @@
 
     def iter_namespace(self, namespace):
         return iter(self._dict[namespace])
 
     def get_help(self, namespace, member):
         if isinstance(self._help, bytes):
             self._help = json.loads(
-                self._help.decode('utf-8')  # pylint: disable=no-member
+                self._help.decode('utf-8')
             )
 
         return self._help[namespace][member]
 
 
 def get_package(server_info, client):
     NO_FINGERPRINT = object()
@@ -550,18 +543,18 @@
         try:
             try:
                 if fingerprint is NO_FINGERPRINT:
                     schema = Schema(client)
                 else:
                     schema = Schema(client, fingerprint)
             except SchemaUpToDate as e:
-                schema = Schema(client, e.fingerprint)
+                schema = Schema(client, e.fingerprint, e.ttl)
         except NotAvailable:
             fingerprint = None
-            ttl = None
+            ttl = 3600  # set a ttl so we don't hammer the remote server
         except SchemaUpToDate as e:
             fingerprint = e.fingerprint
             ttl = e.ttl
         else:
             fingerprint = schema.fingerprint
             ttl = schema.ttl
 
@@ -588,15 +581,15 @@
     module_name = '.'.join((package_name, 'plugins'))
     module = types.ModuleType(module_name)
     module.__file__ = os.path.join(package_dir, 'plugins.py')
     module.register = plugable.Registry()
     for plugin_cls in (_SchemaCommandPlugin, _SchemaObjectPlugin):
         for full_name in schema[plugin_cls.schema_key]:
             plugin = plugin_cls(schema, str(full_name))
-            plugin = module.register()(plugin)  # pylint: disable=no-member
+            plugin = module.register()(plugin)
     sys.modules[module_name] = module
 
     for full_name, topic in six.iteritems(schema['topics']):
         name = str(topic['name'])
         module_name = '.'.join((package_name, name))
         try:
             module = sys.modules[module_name]
```

## ipaclient/remote_plugins/2_114/idrange.py

```diff
@@ -116,15 +116,15 @@
 range it should be done with great care. Because UIDs are stored in the file
 system and are used for access control it might be possible that users are
 allowed to access files of other users if an ID range got deleted and reused
 for a different domain.
 
 (*) The RID is typically the last integer of a user or group SID which follows
 the domain SID. E.g. if the domain SID is S-1-5-21-123-456-789 and a user from
-this domain has the SID S-1-5-21-123-456-789-1010 then 1010 id the RID of the
+this domain has the SID S-1-5-21-123-456-789-1010 then 1010 is the RID of the
 user. RIDs are unique in a domain, 32bit values and are used for users and
 groups.
 
 WARNING:
 
 DNA plugin in 389-ds will allocate IDs based on the ranges configured for the
 local domain. Currently the DNA plugin *cannot* be reconfigured itself based
```

## ipaclient/remote_plugins/2_114/otptoken.py

```diff
@@ -128,15 +128,15 @@
             label=_(u'Digits'),
             doc=_(u'Number of digits each token code will have'),
         ),
         parameters.Int(
             'ipatokentotpclockoffset',
             required=False,
             label=_(u'Clock offset'),
-            doc=_(u'TOTP token / FreeIPA server time difference'),
+            doc=_(u'TOTP token / IPA server time difference'),
         ),
         parameters.Int(
             'ipatokentotptimestep',
             required=False,
             label=_(u'Clock interval'),
             doc=_(u'Length of TOTP token code validity'),
         ),
@@ -259,15 +259,15 @@
             autofill=True,
         ),
         parameters.Int(
             'ipatokentotpclockoffset',
             required=False,
             cli_name='offset',
             label=_(u'Clock offset'),
-            doc=_(u'TOTP token / FreeIPA server time difference'),
+            doc=_(u'TOTP token / IPA server time difference'),
             default=0,
             autofill=True,
         ),
         parameters.Int(
             'ipatokentotptimestep',
             required=False,
             cli_name='interval',
@@ -549,15 +549,15 @@
             default=6,
         ),
         parameters.Int(
             'ipatokentotpclockoffset',
             required=False,
             cli_name='offset',
             label=_(u'Clock offset'),
-            doc=_(u'TOTP token / FreeIPA server time difference'),
+            doc=_(u'TOTP token / IPA server time difference'),
             default=0,
         ),
         parameters.Int(
             'ipatokentotptimestep',
             required=False,
             cli_name='interval',
             label=_(u'Clock interval'),
```

## ipaclient/remote_plugins/2_114/sudorule.py

```diff
@@ -20,32 +20,34 @@
 Sudo Rules
 
 Sudo (su "do") allows a system administrator to delegate authority to
 give certain users (or groups of users) the ability to run some (or all)
 commands as root or another user while providing an audit trail of the
 commands and their arguments.
 
-FreeIPA provides a means to configure the various aspects of Sudo:
+IPA provides a means to configure the various aspects of Sudo:
    Users: The user(s)/group(s) allowed to invoke Sudo.
    Hosts: The host(s)/hostgroup(s) which the user is allowed to to invoke Sudo.
    Allow Command: The specific command(s) permitted to be run via Sudo.
    Deny Command: The specific command(s) prohibited to be run via Sudo.
    RunAsUser: The user(s) or group(s) of users whose rights Sudo will be invoked with.
    RunAsGroup: The group(s) whose gid rights Sudo will be invoked with.
    Options: The various Sudoers Options that can modify Sudo's behavior.
 
 An order can be added to a sudorule to control the order in which they
 are evaluated (if the client supports it). This order is an integer and
 must be unique.
 
-FreeIPA provides a designated binddn to use with Sudo located at:
+IPA provides a designated binddn to use with Sudo located at:
 uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
 
 To enable the binddn run the following command to set the password:
-LDAPTLS_CACERT=/etc/ipa/ca.crt /usr/bin/ldappasswd -S -W -h ipa.example.com -ZZ -D "cn=Directory Manager" uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
+LDAPTLS_CACERT=/etc/ipa/ca.crt /usr/bin/ldappasswd -S -W \\
+    -H ldap://ipa.example.com -ZZ -D "cn=Directory Manager" \\
+    uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
 
 EXAMPLES:
 
  Create a new rule:
    ipa sudorule-add readfiles
 
  Add sudo command object and add it as allowed command in the rule:
```

## ipaclient/remote_plugins/2_156/certprofile.py

```diff
@@ -51,15 +51,15 @@
     ipa certprofile-find --store=false
 
 PROFILE CONFIGURATION FORMAT:
 
 The profile configuration format is the raw property-list format
 used by Dogtag Certificate System.  The XML format is not supported.
 
-The following restrictions apply to profiles managed by FreeIPA:
+The following restrictions apply to profiles managed by IPA:
 
 - When importing a profile the "profileId" field, if present, must
   match the ID given on the command line.
 
 - The "classId" field must be set to "caEnrollImpl"
 
 - The "auth.instance_id" field must be set to "raCertAuth"
```

## ipaclient/remote_plugins/2_156/idrange.py

```diff
@@ -116,15 +116,15 @@
 range it should be done with great care. Because UIDs are stored in the file
 system and are used for access control it might be possible that users are
 allowed to access files of other users if an ID range got deleted and reused
 for a different domain.
 
 (*) The RID is typically the last integer of a user or group SID which follows
 the domain SID. E.g. if the domain SID is S-1-5-21-123-456-789 and a user from
-this domain has the SID S-1-5-21-123-456-789-1010 then 1010 id the RID of the
+this domain has the SID S-1-5-21-123-456-789-1010 then 1010 is the RID of the
 user. RIDs are unique in a domain, 32bit values and are used for users and
 groups.
 
 =======
 WARNING:
 
 DNA plugin in 389-ds will allocate IDs based on the ranges configured for the
```

## ipaclient/remote_plugins/2_156/otptoken.py

```diff
@@ -128,15 +128,15 @@
             label=_(u'Digits'),
             doc=_(u'Number of digits each token code will have'),
         ),
         parameters.Int(
             'ipatokentotpclockoffset',
             required=False,
             label=_(u'Clock offset'),
-            doc=_(u'TOTP token / FreeIPA server time difference'),
+            doc=_(u'TOTP token / IPA server time difference'),
         ),
         parameters.Int(
             'ipatokentotptimestep',
             required=False,
             label=_(u'Clock interval'),
             doc=_(u'Length of TOTP token code validity'),
         ),
@@ -259,15 +259,15 @@
             autofill=True,
         ),
         parameters.Int(
             'ipatokentotpclockoffset',
             required=False,
             cli_name='offset',
             label=_(u'Clock offset'),
-            doc=_(u'TOTP token / FreeIPA server time difference'),
+            doc=_(u'TOTP token / IPA server time difference'),
             default=0,
             autofill=True,
         ),
         parameters.Int(
             'ipatokentotptimestep',
             required=False,
             cli_name='interval',
@@ -549,15 +549,15 @@
             default=6,
         ),
         parameters.Int(
             'ipatokentotpclockoffset',
             required=False,
             cli_name='offset',
             label=_(u'Clock offset'),
-            doc=_(u'TOTP token / FreeIPA server time difference'),
+            doc=_(u'TOTP token / IPA server time difference'),
             default=0,
         ),
         parameters.Int(
             'ipatokentotptimestep',
             required=False,
             cli_name='interval',
             label=_(u'Clock interval'),
```

## ipaclient/remote_plugins/2_156/sudorule.py

```diff
@@ -20,32 +20,34 @@
 Sudo Rules
 
 Sudo (su "do") allows a system administrator to delegate authority to
 give certain users (or groups of users) the ability to run some (or all)
 commands as root or another user while providing an audit trail of the
 commands and their arguments.
 
-FreeIPA provides a means to configure the various aspects of Sudo:
+IPA provides a means to configure the various aspects of Sudo:
    Users: The user(s)/group(s) allowed to invoke Sudo.
    Hosts: The host(s)/hostgroup(s) which the user is allowed to to invoke Sudo.
    Allow Command: The specific command(s) permitted to be run via Sudo.
    Deny Command: The specific command(s) prohibited to be run via Sudo.
    RunAsUser: The user(s) or group(s) of users whose rights Sudo will be invoked with.
    RunAsGroup: The group(s) whose gid rights Sudo will be invoked with.
    Options: The various Sudoers Options that can modify Sudo's behavior.
 
 An order can be added to a sudorule to control the order in which they
 are evaluated (if the client supports it). This order is an integer and
 must be unique.
 
-FreeIPA provides a designated binddn to use with Sudo located at:
+IPA provides a designated binddn to use with Sudo located at:
 uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
 
 To enable the binddn run the following command to set the password:
-LDAPTLS_CACERT=/etc/ipa/ca.crt /usr/bin/ldappasswd -S -W -h ipa.example.com -ZZ -D "cn=Directory Manager" uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
+LDAPTLS_CACERT=/etc/ipa/ca.crt /usr/bin/ldappasswd -S -W \\
+    -H ldap://ipa.example.com -ZZ -D "cn=Directory Manager" \\
+    uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
 
 EXAMPLES:
 
  Create a new rule:
    ipa sudorule-add readfiles
 
  Add sudo command object and add it as allowed command in the rule:
```

## ipaclient/remote_plugins/2_164/certprofile.py

```diff
@@ -51,15 +51,15 @@
     ipa certprofile-find --store=false
 
 PROFILE CONFIGURATION FORMAT:
 
 The profile configuration format is the raw property-list format
 used by Dogtag Certificate System.  The XML format is not supported.
 
-The following restrictions apply to profiles managed by FreeIPA:
+The following restrictions apply to profiles managed by IPA:
 
 - When importing a profile the "profileId" field, if present, must
   match the ID given on the command line.
 
 - The "classId" field must be set to "caEnrollImpl"
 
 - The "auth.instance_id" field must be set to "raCertAuth"
```

## ipaclient/remote_plugins/2_164/idrange.py

```diff
@@ -116,15 +116,15 @@
 range it should be done with great care. Because UIDs are stored in the file
 system and are used for access control it might be possible that users are
 allowed to access files of other users if an ID range got deleted and reused
 for a different domain.
 
 (*) The RID is typically the last integer of a user or group SID which follows
 the domain SID. E.g. if the domain SID is S-1-5-21-123-456-789 and a user from
-this domain has the SID S-1-5-21-123-456-789-1010 then 1010 id the RID of the
+this domain has the SID S-1-5-21-123-456-789-1010 then 1010 is the RID of the
 user. RIDs are unique in a domain, 32bit values and are used for users and
 groups.
 
 =======
 WARNING:
 
 DNA plugin in 389-ds will allocate IDs based on the ranges configured for the
```

## ipaclient/remote_plugins/2_164/otptoken.py

```diff
@@ -128,15 +128,15 @@
             label=_(u'Digits'),
             doc=_(u'Number of digits each token code will have'),
         ),
         parameters.Int(
             'ipatokentotpclockoffset',
             required=False,
             label=_(u'Clock offset'),
-            doc=_(u'TOTP token / FreeIPA server time difference'),
+            doc=_(u'TOTP token / IPA server time difference'),
         ),
         parameters.Int(
             'ipatokentotptimestep',
             required=False,
             label=_(u'Clock interval'),
             doc=_(u'Length of TOTP token code validity'),
         ),
@@ -259,15 +259,15 @@
             autofill=True,
         ),
         parameters.Int(
             'ipatokentotpclockoffset',
             required=False,
             cli_name='offset',
             label=_(u'Clock offset'),
-            doc=_(u'TOTP token / FreeIPA server time difference'),
+            doc=_(u'TOTP token / IPA server time difference'),
             default=0,
             autofill=True,
         ),
         parameters.Int(
             'ipatokentotptimestep',
             required=False,
             cli_name='interval',
@@ -549,15 +549,15 @@
             default=6,
         ),
         parameters.Int(
             'ipatokentotpclockoffset',
             required=False,
             cli_name='offset',
             label=_(u'Clock offset'),
-            doc=_(u'TOTP token / FreeIPA server time difference'),
+            doc=_(u'TOTP token / IPA server time difference'),
             default=0,
         ),
         parameters.Int(
             'ipatokentotptimestep',
             required=False,
             cli_name='interval',
             label=_(u'Clock interval'),
```

## ipaclient/remote_plugins/2_164/sudorule.py

```diff
@@ -20,32 +20,34 @@
 Sudo Rules
 
 Sudo (su "do") allows a system administrator to delegate authority to
 give certain users (or groups of users) the ability to run some (or all)
 commands as root or another user while providing an audit trail of the
 commands and their arguments.
 
-FreeIPA provides a means to configure the various aspects of Sudo:
+IPA provides a means to configure the various aspects of Sudo:
    Users: The user(s)/group(s) allowed to invoke Sudo.
    Hosts: The host(s)/hostgroup(s) which the user is allowed to to invoke Sudo.
    Allow Command: The specific command(s) permitted to be run via Sudo.
    Deny Command: The specific command(s) prohibited to be run via Sudo.
    RunAsUser: The user(s) or group(s) of users whose rights Sudo will be invoked with.
    RunAsGroup: The group(s) whose gid rights Sudo will be invoked with.
    Options: The various Sudoers Options that can modify Sudo's behavior.
 
 An order can be added to a sudorule to control the order in which they
 are evaluated (if the client supports it). This order is an integer and
 must be unique.
 
-FreeIPA provides a designated binddn to use with Sudo located at:
+IPA provides a designated binddn to use with Sudo located at:
 uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
 
 To enable the binddn run the following command to set the password:
-LDAPTLS_CACERT=/etc/ipa/ca.crt /usr/bin/ldappasswd -S -W -h ipa.example.com -ZZ -D "cn=Directory Manager" uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
+LDAPTLS_CACERT=/etc/ipa/ca.crt /usr/bin/ldappasswd -S -W \\
+    -H ldap://ipa.example.com -ZZ -D "cn=Directory Manager" \\
+    uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
 
 EXAMPLES:
 
  Create a new rule:
    ipa sudorule-add readfiles
 
  Add sudo command object and add it as allowed command in the rule:
```

## ipaclient/remote_plugins/2_49/idrange.py

```diff
@@ -116,15 +116,15 @@
 range it should be done with great care. Because UIDs are stored in the file
 system and are used for access control it might be possible that users are
 allowed to access files of other users if an ID range got deleted and reused
 for a different domain.
 
 (*) The RID is typically the last integer of a user or group SID which follows
 the domain SID. E.g. if the domain SID is S-1-5-21-123-456-789 and a user from
-this domain has the SID S-1-5-21-123-456-789-1010 then 1010 id the RID of the
+this domain has the SID S-1-5-21-123-456-789-1010 then 1010 is the RID of the
 user. RIDs are unique in a domain, 32bit values and are used for users and
 groups.
 
 WARNING:
 
 DNA plugin in 389-ds will allocate IDs based on the ranges configured for the
 local domain. Currently the DNA plugin *cannot* be reconfigured itself based
```

## ipaclient/remote_plugins/2_49/sudorule.py

```diff
@@ -20,34 +20,36 @@
 Sudo Rules
 
 Sudo (su "do") allows a system administrator to delegate authority to
 give certain users (or groups of users) the ability to run some (or all)
 commands as root or another user while providing an audit trail of the
 commands and their arguments.
 
-FreeIPA provides a means to configure the various aspects of Sudo:
+IPA provides a means to configure the various aspects of Sudo:
    Users: The user(s)/group(s) allowed to invoke Sudo.
    Hosts: The host(s)/hostgroup(s) which the user is allowed to to invoke Sudo.
    Allow Command: The specific command(s) permitted to be run via Sudo.
    Deny Command: The specific command(s) prohibited to be run via Sudo.
    RunAsUser: The user(s) or group(s) of users whose rights Sudo will be invoked with.
    RunAsGroup: The group(s) whose gid rights Sudo will be invoked with.
    Options: The various Sudoers Options that can modify Sudo's behavior.
 
 An order can be added to a sudorule to control the order in which they
 are evaluated (if the client supports it). This order is an integer and
 must be unique.
 
-FreeIPA provides a designated binddn to use with Sudo located at:
+IPA provides a designated binddn to use with Sudo located at:
 uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
 
 To enable the binddn run the following command to set the password:
-LDAPTLS_CACERT=/etc/ipa/ca.crt /usr/bin/ldappasswd -S -W -h ipa.example.com -ZZ -D "cn=Directory Manager" uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
+LDAPTLS_CACERT=/etc/ipa/ca.crt /usr/bin/ldappasswd -S -W \\
+    -H ldap://ipa.example.com -ZZ -D "cn=Directory Manager" \\
+    uid=sudo,cn=sysaccounts,cn=etc,dc=example,dc=com
 
-For more information, see the FreeIPA Documentation to Sudo.
+For more information, see the IPA Documentation to Sudo.
 """)
 
 register = Registry()
 
 
 @register()
 class sudorule(Object):
```

## Comparing `ipaclient-4.8.9.dist-info/COPYING` & `ipaclient-4.9.12.dist-info/COPYING`

 * *Files identical despite different names*

## Comparing `ipaclient-4.8.9.dist-info/METADATA` & `ipaclient-4.9.12.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ipaclient
-Version: 4.8.9
+Version: 4.9.12
 Summary: FreeIPA client library
 Home-page: https://www.freeipa.org/
+Download-URL: https://www.freeipa.org/page/Downloads
 Author: FreeIPA Developers
 Author-email: freeipa-devel@lists.fedorahosted.org
 Maintainer: FreeIPA Developers
 Maintainer-email: freeipa-devel@redhat.com
 License: GPLv3
-Download-URL: https://www.freeipa.org/page/Downloads
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -21,26 +21,22 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
 Requires-Python: >=3.6.0
+License-File: ../COPYING
 Requires-Dist: cryptography (>=1.6)
-Requires-Dist: ipalib (==4.8.9)
-Requires-Dist: ipapython (==4.8.9)
+Requires-Dist: ipalib (==4.9.12)
+Requires-Dist: ipapython (==4.9.12)
 Requires-Dist: qrcode (>=5.0)
 Requires-Dist: six
-Provides-Extra: csrgen
-Requires-Dist: cffi ; extra == 'csrgen'
-Requires-Dist: jinja2 ; extra == 'csrgen'
 Provides-Extra: install
 Requires-Dist: ipaplatform ; extra == 'install'
 Provides-Extra: ldap
 Requires-Dist: python-ldap ; extra == 'ldap'
 Provides-Extra: otptoken_yubikey
 Requires-Dist: python-yubico ; extra == 'otptoken_yubikey'
 Requires-Dist: pyusb ; extra == 'otptoken_yubikey'
 
 FreeIPA client library
-
-
```

## Comparing `ipaclient-4.8.9.dist-info/RECORD` & `ipaclient-4.9.12.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,44 @@
 ipaclient/__init__.py,sha256=au43u6t_OlioBLu6wUGhA9XsZmdO9GNHfDEotTm_pWE,766
 ipaclient/__main__.py,sha256=hZTfJ4NHa34AV3DGEnZEWU_YKZqW7PJ6np7gzigcdpk,276
-ipaclient/csrgen.py,sha256=xOF02PQwfFIKQflYpyOIq1dkcKbJ-JPMcGPrZxe0Bvg,17008
-ipaclient/csrgen_ffi.py,sha256=DUqbASuSigqmWQxQrTUDfeFb-VJD7oCpb5tDwJkGGVs,11568
-ipaclient/discovery.py,sha256=cGOLhqS4wfF4yX6NMMfnrKi-vLIiJ9408a2d0DLGUhI,23867
-ipaclient/frontend.py,sha256=6GSRxYVE6XH4wQLcK3T_4GJJmC1iZmdhChNV143NB2o,5431
-ipaclient/csrgen/profiles/caIPAserviceCert.json,sha256=vWZgfZmUWXQY80-aseFCEC06cnnwSyTXkD99NQcKNT0,229
-ipaclient/csrgen/profiles/userCert.json,sha256=Z2CMS0V31XMa7rFWlw0p8djhvJpFaESKnqvvn7oP7eg,235
-ipaclient/csrgen/rules/dataDNS.json,sha256=EbjBZYLlMgOL-i5g8pragJWHp835fBSJ3MWbdeeJw0g,215
-ipaclient/csrgen/rules/dataEmail.json,sha256=7qqt41cXtH_02RAgcxnuo7aLdDG5iyFZU0_d_H-4ptQ,121
-ipaclient/csrgen/rules/dataHostCN.json,sha256=NFcohf4ecO4d2I5coKo3BoYprusAM74nmWsPDtOkK1A,212
-ipaclient/csrgen/rules/dataSubjectBase.json,sha256=ji_ck7TQJ9H9npIoR_p7ZDA-JrXs4pb2w2DpdailD_A,153
-ipaclient/csrgen/rules/dataUsernameCN.json,sha256=Jb33ksnGV-NkBoSPab2IEqCUWYCk__0Ghqx31zuHIso,114
-ipaclient/csrgen/rules/syntaxSAN.json,sha256=44s2yH5H46u1NG0RHvB-kxZpagShL8wyOeLbZ_hnmGY,166
-ipaclient/csrgen/rules/syntaxSubject.json,sha256=3sO4TXpsg2DORaRCKtgMLt_kJ9BzkV_R0qNRxEJXrAw,213
-ipaclient/csrgen/templates/openssl_base.tmpl,sha256=X0TZQDTGpkv1BRgOWRsue52QcKMvSMu1VO_qVVWGJTs,428
-ipaclient/csrgen/templates/openssl_macros.tmpl,sha256=ocLyWhS7_Vwc5YJ8rY7iEfBAL6pGEKmmW-6pkRLYCJQ,890
+ipaclient/discovery.py,sha256=uVykCEV1FOfQZ8AKZPUwUX_qRzN-_fxf6CZAj3XdJGo,23867
+ipaclient/frontend.py,sha256=rTTFGhd_VpArF_vOVmoJ4yhipxOX-zJxdqjbYCnSSso,5623
 ipaclient/plugins/__init__.py,sha256=9kx4o36g9UT9rqeB86S2Vl7Fin1UJZq5Iuhc1IwiA_M,123
-ipaclient/plugins/automember.py,sha256=gz5yhzWhukkkjsdTvbwIsyMUyFnsvo9YGnwDLc1XBrI,1178
-ipaclient/plugins/automount.py,sha256=Ihi2j54l2kdijcOA89xKIF7P0sRoCn9NATWbb7p1iO4,10638
+ipaclient/plugins/automember.py,sha256=irwY16jscqAyLbBvR2PpLa5cMwO8JPZPAcxDCqgSGqU,1496
+ipaclient/plugins/automount.py,sha256=QqiqYeYzkszvu2SzeQlDyLqcO7VBeZ88eVo5GTlIvRk,10793
+ipaclient/plugins/baseuser.py,sha256=9j3b7uYRq-5nipyY56OdrEL0nuTGGz7VtrdwOJCmEyU,4095
 ipaclient/plugins/ca.py,sha256=CU2ThrZwTNGA0OV4Qw0e6xUtckn42YUc8SYFDAzMn4c,2087
-ipaclient/plugins/cert.py,sha256=EiHxqd5Bs5DMyTvEnzFg-h0Ab19HsI25-ElX4S72a2k,7401
+ipaclient/plugins/cert.py,sha256=HN9TAFlOZ8srbpiK4OkbI7J3AyPYZD0EdpYaz9Ny-Qw,4516
 ipaclient/plugins/certmap.py,sha256=Q7xtArY5YRdC8hesQGaitFzI7CFGXHDBjaW1POmHmEY,1596
 ipaclient/plugins/certprofile.py,sha256=_jxEzQj_9H8NK6uAtbrS66bOTqcKwSyd3fZer5h2bVw,1499
-ipaclient/plugins/csrgen.py,sha256=59OdAg3iICz3Uj2ttDPj0x66wZ3AhzKqlUDostt3qaA,3627
 ipaclient/plugins/dns.py,sha256=rSw2wCH6me0PouNWwiDmhtaYCyYqRQ-Z8QDwEcJxQaM,18526
 ipaclient/plugins/hbacrule.py,sha256=0E6S7RQrIwLS32mjOncPVN3u0__lQMgZt_Amq9BC-VU,1509
 ipaclient/plugins/hbactest.py,sha256=uAQj1MUqUFOJlgv9ikFtn5DqBwbil_QF0_1eGernRIs,2175
 ipaclient/plugins/host.py,sha256=hL3VbKGu9CMw7bupTe9Ynmfa2kdEtQPI9ULE11qPPfY,1876
 ipaclient/plugins/idrange.py,sha256=kMgaLHnPltTb0RgOrj0l_j7HzoT2TmAqv8eFzfk2ed8,3404
 ipaclient/plugins/internal.py,sha256=e4hwyfjlHj-r9OSs8gOjCyzX8RyOoJjKZnWM0DnUo_8,1443
 ipaclient/plugins/location.py,sha256=FR5pmZMTIo3bcAiRgIGli6l-Duw_1Q5rYlvbjSb5rac,1057
 ipaclient/plugins/migration.py,sha256=jbP7Ssmp3fkzqlMK_8BfKzUO8gT2IumJXswnoiT__N4,3040
 ipaclient/plugins/misc.py,sha256=PXhxeJqpogh9az8b74KKXs5Li57D1j9dTt9pgyx28TA,886
-ipaclient/plugins/otptoken.py,sha256=xBJ48KIonqlHmnXf_bOZ1huOmhIDljXbYNnxs4ny_fg,6368
-ipaclient/plugins/otptoken_yubikey.py,sha256=jx4KYB8yljL7U8yLMQGkS_i_juUjxuz8SHbjahH8jL0,6365
+ipaclient/plugins/otptoken.py,sha256=OfbCWfkNAsVbSckmC1bYly7VmMha2Iuzaz4d8zTnULg,6395
+ipaclient/plugins/otptoken_yubikey.py,sha256=Z0CJ4laLd22a7o1I0op_YtM5ApRyy7x3-f_CWci0NwY,6413
 ipaclient/plugins/passwd.py,sha256=H4RO8TgzWxsiNPlJVZCblkqM-OwzbrqGttN94U2F780,441
 ipaclient/plugins/permission.py,sha256=il4i9QjBoFTPkhljhYgeRVHGcgvDlCWgUOfMdfTMILw,774
 ipaclient/plugins/rpcclient.py,sha256=yBK0Vwz4nTX67O8X6K1Slji-wJ77oc7wy8wL7frV_Kg,1651
 ipaclient/plugins/server.py,sha256=8hE6LIVZAVAbdiNStNf5YEu-WjMj6GYx0lIeqeVJZyQ,626
 ipaclient/plugins/service.py,sha256=zTk5YTiGr37rL_bfc110__VwTAteE3of--enuGEOAQ0,1948
+ipaclient/plugins/stageuser.py,sha256=IJebJoRWK-Fb_wgWOjdW-_Zx_2iLzH_JybMImmZ7ihI,376
 ipaclient/plugins/sudorule.py,sha256=49rVWYdfzDlJGbuQvHBTdJJzZ8A3XR9L60WvFZnJgIY,2221
 ipaclient/plugins/topology.py,sha256=KknzfhBOgYPtT6RxkKMF0ARrQ-EERMTv0tcldI2qIuI,1937
 ipaclient/plugins/trust.py,sha256=pagpsi-oIs9oZG2NhWcI_jilPpbUbFhVDl2O0N6VamY,1897
 ipaclient/plugins/user.py,sha256=fgyN96U2Y7akOItU8bbINkii5VShRL19y2dZMNzzqec,2966
-ipaclient/plugins/vault.py,sha256=1opGUFI4nCeHYVEaMICmesEg9qnYQkwptxcnbK3o53c,37158
-ipaclient/remote_plugins/__init__.py,sha256=y58-HtnRx0xAfdXv2lsQG5b9aoXCncU_tnsdEtU559g,3991
-ipaclient/remote_plugins/compat.py,sha256=qBXkqPZU-FEm9whljBuFjPFi8EXQvsvnvXJKQ5HoIzE,2324
-ipaclient/remote_plugins/schema.py,sha256=J8WG6bBtfUT8x8kJWAXcKpGxIA4VreHXFge2Kx7DOUc,19022
+ipaclient/plugins/vault.py,sha256=GSxw-SveT0kPNN_gcmnzOpHH45oToYnfc-Ec_XHkOxM,39982
+ipaclient/remote_plugins/__init__.py,sha256=jW1gdF8Ar01KfWaqGFE5Fsbjdpetksq0fMzePDVWc10,3963
+ipaclient/remote_plugins/compat.py,sha256=IZC-HJ-Pb_GVPPPs8BS6NcVztHNmggpETdhAo6jMKw0,2462
+ipaclient/remote_plugins/schema.py,sha256=1utOewv3v9gndBXnGg9vMSvZ5-LNTA_cP0CQhIk9bS4,18841
 ipaclient/remote_plugins/2_114/__init__.py,sha256=wcazj928RrNnDaqwu1CMH294e3R4fVg6M-cpyok6nKo,265
 ipaclient/remote_plugins/2_114/aci.py,sha256=2BrUjd6V9A73gq53le2VMOQHTe6iFwtieBxWqAcLrZA,25449
 ipaclient/remote_plugins/2_114/automember.py,sha256=FvsOifByHokDEHWrFOmk2_NJEeXzjjmpN7K7R6v1BKo,24427
 ipaclient/remote_plugins/2_114/automount.py,sha256=EiXF_1LVZsKFk3mjpcYzHsbxTCfbhlvS8jcdV_rWEKY,35202
 ipaclient/remote_plugins/2_114/batch.py,sha256=9hIvEUXtbVYHR2ynTIIcmjGdsscg8gUerX8cm7TTpIU,1806
 ipaclient/remote_plugins/2_114/cert.py,sha256=HcwCbS5xPCXiRM6Mg2z4EmF5_Z2H6pnpNwOOY5L3RJ0,9773
 ipaclient/remote_plugins/2_114/config.py,sha256=RnQYYTyFYHQW-vCWisJoF-1H67Njh0yd6YaI-s1mYAY,13684
@@ -59,24 +47,24 @@
 ipaclient/remote_plugins/2_114/group.py,sha256=J5RtSWR5oPqlA5qkLp3NByyuJY125ZptXnfsCvFYF5A,26481
 ipaclient/remote_plugins/2_114/hbacrule.py,sha256=vxHU4gB6ji4ictpZN8XOQPivSjcrXC30l-vFgq1jSVE,35745
 ipaclient/remote_plugins/2_114/hbacsvc.py,sha256=yA6uDjfiWL94D1oKRIzzZaUOBNIT2u543-KC4YwWrBE,11491
 ipaclient/remote_plugins/2_114/hbacsvcgroup.py,sha256=CF4Y3dVH5tRZ9a8NEc1qM_4d61SlPc8gCwYyDWBSigQ,14599
 ipaclient/remote_plugins/2_114/hbactest.py,sha256=JlRzffaeKar_y3lulq5R681fuJ0mU4dGA7dxKpW0x1Q,9123
 ipaclient/remote_plugins/2_114/host.py,sha256=sObFhWXCUVopbX62RZQZmjW9PSvzkLrivWP9WzZu4nE,45438
 ipaclient/remote_plugins/2_114/hostgroup.py,sha256=mzYBUb_Vq-eRZFbPfDmzQVeJskkk-KDXXVu4PqDkmvQ,20339
-ipaclient/remote_plugins/2_114/idrange.py,sha256=4gJ_DfdSgq5yzjxg6idL5QwWuRbwl9786MRGq1rk2Xk,19509
+ipaclient/remote_plugins/2_114/idrange.py,sha256=1yB4bTOaA3hWml4vMveCAaag8oVwHWu3__82kqqTuK4,19509
 ipaclient/remote_plugins/2_114/idviews.py,sha256=f8qhNSbvS-jcC3HIKW7WgR_wfybImPbRI0YyyKu2OrQ,39044
 ipaclient/remote_plugins/2_114/internal.py,sha256=Pav7pfHuSHyVW3T2Z9dtyfgPcVqUtLZ0pxxMr17IVr0,2019
 ipaclient/remote_plugins/2_114/join.py,sha256=1xuKidvyu-0JmH0rCW11w2Sm3-KD21gzrSenEMRAZOE,1537
 ipaclient/remote_plugins/2_114/krbtpolicy.py,sha256=Kej6uy5gsUE7I0yYYbhvnfj6-LajENtitVDNy4IGRl0,7559
 ipaclient/remote_plugins/2_114/migration.py,sha256=5YpFFQroHLEx6PkGQLdU2vBkc-S3uO96o3Bq9l3GcIY,10437
 ipaclient/remote_plugins/2_114/misc.py,sha256=ww6uMauAvVYutlNHSSqkoBVpdW1kT5rHeXekLJMEGZk,2753
 ipaclient/remote_plugins/2_114/netgroup.py,sha256=Hh_WdQtSQaU_JLYM0msXW3c6T9qPzgidwZ-Ge2_tfTI,24339
 ipaclient/remote_plugins/2_114/otpconfig.py,sha256=sOorsTPvhq2qeo1wlNcaVbyWLYjXBUY82Dui7apDkSg,6184
-ipaclient/remote_plugins/2_114/otptoken.py,sha256=9A41RH8MChwI_xFj5eD69KBOgCRhIQIDxG2m4coHtdc,25992
+ipaclient/remote_plugins/2_114/otptoken.py,sha256=CHxukbWtey1A7VSw4gDmNwiEbF_Jt1hFptEQeCDq5k4,25980
 ipaclient/remote_plugins/2_114/otptoken_yubikey.py,sha256=Rlk4ZpowXusMdYcPlIb_slO4dhZvJkFU3jYsMezNgEE,690
 ipaclient/remote_plugins/2_114/passwd.py,sha256=UYpt_i1dh7xMXjTyBkEjHSFweJg1hUlhMke8ZZRcPo8,2431
 ipaclient/remote_plugins/2_114/permission.py,sha256=g-41qjiv-RPNnBL11RuGx-v1NGA1AnY5eYjFM1v5WJU,31931
 ipaclient/remote_plugins/2_114/ping.py,sha256=QU6VwHCQUQrkFqCqqXyZnRgtxySWdqZlvhHVlOdJ4mA,1675
 ipaclient/remote_plugins/2_114/pkinit.py,sha256=VbluXcEICjl15p3l27J802BcIEsYXKiAYNxAi__LDXk,1198
 ipaclient/remote_plugins/2_114/privilege.py,sha256=1uP-XdITAkam7ZMQ-8SCVxiEu9_eHv7fW0DiC04gbmo,17885
 ipaclient/remote_plugins/2_114/pwpolicy.py,sha256=ZjrKaO9YvkNQo-gMvPbZz0Fhpfc9c1Ov16nYzUYWfe0,27438
@@ -85,46 +73,46 @@
 ipaclient/remote_plugins/2_114/role.py,sha256=SfgAws6v8fw5b7bGdwaXC3zYmWCDk45mE4Osc4UwgwI,20693
 ipaclient/remote_plugins/2_114/selfservice.py,sha256=sLoYwRGuJs_GFXPRVZuJEZda1tYRlMYCInp5jOSIRFU,9336
 ipaclient/remote_plugins/2_114/selinuxusermap.py,sha256=dB-zRnCZ_MqiivckQ8g9rmPDImQnrtLEFYQVWWlAwUo,25184
 ipaclient/remote_plugins/2_114/service.py,sha256=IdTTJXxLdWitG98BKEEuZeh-t8w9ynH6Kj6FKsyI39c,32359
 ipaclient/remote_plugins/2_114/session.py,sha256=C3UY7aNlPKj3I0oFMpPwQqHV-v8kvAQgLYJPI7okF-Q,25143
 ipaclient/remote_plugins/2_114/sudocmd.py,sha256=7-vvmoL6fw35uIL6B1hOdD3KvcInD_122RBNqPSDiOU,10873
 ipaclient/remote_plugins/2_114/sudocmdgroup.py,sha256=AgQDZsc04F3n97HCeFjLvol92aEfYToQ2XwSie0ORmk,14955
-ipaclient/remote_plugins/2_114/sudorule.py,sha256=dqj0SnfJmiSutandsRUEbI4MoRLsZ54zqI4Z1ZuPBdE,50213
+ipaclient/remote_plugins/2_114/sudorule.py,sha256=QK0zozgiVOB1ogxMxGrc-SJg4JHhArtW_3Oi3EMv4WU,50226
 ipaclient/remote_plugins/2_114/trust.py,sha256=njfYrOMy3SnChJd7BgZqrBr3VuFrekAPZcKNE40SafA,35406
 ipaclient/remote_plugins/2_114/user.py,sha256=jpFpq1KxuUZDEsU8oQUoA-yrZisrxwCezMNQDMSqYY0,46927
 ipaclient/remote_plugins/2_156/__init__.py,sha256=a_4akEC6LJDnx3LYF9fP1kjkjgu9ujW_OQoEQ6C8_x8,265
 ipaclient/remote_plugins/2_156/aci.py,sha256=2BrUjd6V9A73gq53le2VMOQHTe6iFwtieBxWqAcLrZA,25449
 ipaclient/remote_plugins/2_156/automember.py,sha256=FvsOifByHokDEHWrFOmk2_NJEeXzjjmpN7K7R6v1BKo,24427
 ipaclient/remote_plugins/2_156/automount.py,sha256=U8jEPB7KvNUzavutqoIhbHa-YpimtlaZYXyO0qC9Zr8,35304
 ipaclient/remote_plugins/2_156/batch.py,sha256=9hIvEUXtbVYHR2ynTIIcmjGdsscg8gUerX8cm7TTpIU,1806
 ipaclient/remote_plugins/2_156/caacl.py,sha256=_zT0u6kbrqlxyENfku_vyY1eJVgn-fc7rwa_i94K0yo,31324
 ipaclient/remote_plugins/2_156/cert.py,sha256=2wOqYduwGkCGgCnbsvm63rsS9b_M-GhOw-SGEHXy4cM,9940
-ipaclient/remote_plugins/2_156/certprofile.py,sha256=KzGpDxG6rLpomED8JinOyoivoSwDliRGG1OQT9YMGZ0,12590
+ipaclient/remote_plugins/2_156/certprofile.py,sha256=9aFdkjMroDo-REubQ2xOnmBBLAXe9O15v6a4_5aGdpw,12586
 ipaclient/remote_plugins/2_156/config.py,sha256=E27WIvtnJlU6VKOn7WMsHbns2M1vjxd-NT7KtrcB7Ng,13698
 ipaclient/remote_plugins/2_156/delegation.py,sha256=yzNKTvfkD0NO_8eHWhpLkFRJIRE6J1NkHfb_r5QrSNE,10698
 ipaclient/remote_plugins/2_156/dns.py,sha256=G0kBEMEF9KgWln32--fC-n2hnRp_-P4pJ6iTqqZ-ibU,161194
 ipaclient/remote_plugins/2_156/domainlevel.py,sha256=gx2UaJ695nGuvD2uT9Ya3aiS-a-_dthgWt-6Ne35DBQ,1199
 ipaclient/remote_plugins/2_156/group.py,sha256=jEUZfzlo_lVNWfL4saVuDwL8__o4r2VpP7ItitcDmOI,26515
 ipaclient/remote_plugins/2_156/hbacrule.py,sha256=C86OFQtwSHqoEQInRw-MYQI0X9tU4yhSYu3PLsuM-js,35779
 ipaclient/remote_plugins/2_156/hbacsvc.py,sha256=88pKqHrXjDh8uuyqOP3ZktCLq8-NnvDk3HaIyQwSXFw,11525
 ipaclient/remote_plugins/2_156/hbacsvcgroup.py,sha256=xw00dB-y39l0YnptfTO-A7mZcAqVN8CrXiaVhPklufY,14633
 ipaclient/remote_plugins/2_156/hbactest.py,sha256=JlRzffaeKar_y3lulq5R681fuJ0mU4dGA7dxKpW0x1Q,9123
 ipaclient/remote_plugins/2_156/host.py,sha256=pZFjA0WHxv-laXj2l2tHq5punBLYb3icYYPVfIBzpMs,48912
 ipaclient/remote_plugins/2_156/hostgroup.py,sha256=Qr5M8Bbvm0t_HMISVpXF_nvthRFUR1ETIGi44xjSXT8,20373
-ipaclient/remote_plugins/2_156/idrange.py,sha256=T9tGjMMc0B2NYf96_kChZglGhO1OccqoToKaGM65ubU,20053
+ipaclient/remote_plugins/2_156/idrange.py,sha256=1x5YAexoN0qVG3yWRUzPPS0jiZGH9RkgsJ6zqH6AXP0,20053
 ipaclient/remote_plugins/2_156/idviews.py,sha256=ML_jlSYXiI34CtAKIbGSebUoLnwmyX0vpiUSnqj8kgI,42287
 ipaclient/remote_plugins/2_156/internal.py,sha256=Pav7pfHuSHyVW3T2Z9dtyfgPcVqUtLZ0pxxMr17IVr0,2019
 ipaclient/remote_plugins/2_156/join.py,sha256=1xuKidvyu-0JmH0rCW11w2Sm3-KD21gzrSenEMRAZOE,1537
 ipaclient/remote_plugins/2_156/krbtpolicy.py,sha256=Kej6uy5gsUE7I0yYYbhvnfj6-LajENtitVDNy4IGRl0,7559
 ipaclient/remote_plugins/2_156/migration.py,sha256=Y02IG6RITggfBI6M-GUfGqo5IV3kA7GBq9jPkeopcro,11089
 ipaclient/remote_plugins/2_156/misc.py,sha256=ww6uMauAvVYutlNHSSqkoBVpdW1kT5rHeXekLJMEGZk,2753
 ipaclient/remote_plugins/2_156/netgroup.py,sha256=y634jT1YOSt0_Svqsvkxg2Bc16WFWI5d2s9cz_vc18c,24373
 ipaclient/remote_plugins/2_156/otpconfig.py,sha256=sOorsTPvhq2qeo1wlNcaVbyWLYjXBUY82Dui7apDkSg,6184
-ipaclient/remote_plugins/2_156/otptoken.py,sha256=HSPYYJtnrla3Ing2Edv4V-_8XRQbSFs1M1aoLGBW5sY,26027
+ipaclient/remote_plugins/2_156/otptoken.py,sha256=ByNYdtnQO3O4YO5iSSP6u3vrKWUOXvZe6e3RdG_sLyw,26015
 ipaclient/remote_plugins/2_156/otptoken_yubikey.py,sha256=Rlk4ZpowXusMdYcPlIb_slO4dhZvJkFU3jYsMezNgEE,690
 ipaclient/remote_plugins/2_156/passwd.py,sha256=UYpt_i1dh7xMXjTyBkEjHSFweJg1hUlhMke8ZZRcPo8,2431
 ipaclient/remote_plugins/2_156/permission.py,sha256=ayENBpx_qRu1c_WfSs_ZcL8UEWXcr0r5-oisQREI748,34289
 ipaclient/remote_plugins/2_156/ping.py,sha256=QU6VwHCQUQrkFqCqqXyZnRgtxySWdqZlvhHVlOdJ4mA,1675
 ipaclient/remote_plugins/2_156/pkinit.py,sha256=VbluXcEICjl15p3l27J802BcIEsYXKiAYNxAi__LDXk,1198
 ipaclient/remote_plugins/2_156/privilege.py,sha256=TLxb6UifddQ0XofyJU8hPCWSlSlAU1sv_Krc1F94vR0,17919
 ipaclient/remote_plugins/2_156/pwpolicy.py,sha256=shkmQBFbec-ADLU0MUehXltYD1_Q55Tq_iOZ5NhrzB0,27506
@@ -136,48 +124,48 @@
 ipaclient/remote_plugins/2_156/server.py,sha256=zt3ZTlce4mDtDgGkPWx1YfkDLSjHlph33eXcs6tvO60,6296
 ipaclient/remote_plugins/2_156/service.py,sha256=qCHiazmIMZ70BO6mFWpvDeJ79fORydAKrkixHggNXdg,35920
 ipaclient/remote_plugins/2_156/servicedelegation.py,sha256=zKUP972ZB_aEuHGyDrIVgQaAeJWwkwMYlT2Tem1FyOc,25495
 ipaclient/remote_plugins/2_156/session.py,sha256=1XLaG9O7rcJfwYaU-usj6wGKG4hWJT8fONv-OXdsK7E,678
 ipaclient/remote_plugins/2_156/stageuser.py,sha256=_BdgHbv-QvU5Fqv29FekuqP2v-qp6G_KbFlpMQubSek,43617
 ipaclient/remote_plugins/2_156/sudocmd.py,sha256=c6dw9JgVhUvFPuy2YFigNTh4AjrQFbCngjdvTnlQFJE,10907
 ipaclient/remote_plugins/2_156/sudocmdgroup.py,sha256=BUpBtgDGPW1LT9RTz2mTaIUauIVSzudLNqaBIb2rO-0,14989
-ipaclient/remote_plugins/2_156/sudorule.py,sha256=GZOsXikNwfubxNg4ggfGEARHUxLnSU0fUQdHd18Fd3U,50247
+ipaclient/remote_plugins/2_156/sudorule.py,sha256=eAKPm125EiRy_RXJUuV9OslN68bndqTW9FIzA4z76cA,50260
 ipaclient/remote_plugins/2_156/topology.py,sha256=VONAff9BrbjlLZJqAvnh5zrMXt8XQZRL3rhelVckoAM,32297
 ipaclient/remote_plugins/2_156/trust.py,sha256=7KdU0TU5hRSMvrJ-XANYnKAnqUsBBGp23V9tByD4NLc,35970
 ipaclient/remote_plugins/2_156/user.py,sha256=NQHJMVpSc7eZCvUPs-H-pGo3sdLEJfh-jYeYauvLAyU,55185
 ipaclient/remote_plugins/2_156/vault.py,sha256=OyfsS96HeJ0c4EfHnpempXGJmEySYdQILOTZ7I9OrKs,45219
 ipaclient/remote_plugins/2_164/__init__.py,sha256=NhtehSyWY0Z5F0_yBo6Fy86WccMybxNBF6grD8p4kRg,265
 ipaclient/remote_plugins/2_164/aci.py,sha256=2BrUjd6V9A73gq53le2VMOQHTe6iFwtieBxWqAcLrZA,25449
 ipaclient/remote_plugins/2_164/automember.py,sha256=GCwir00SfOGV8aqDOfFWK90xxnCJhT4L1jUM0-tPpLs,24426
 ipaclient/remote_plugins/2_164/automount.py,sha256=U8jEPB7KvNUzavutqoIhbHa-YpimtlaZYXyO0qC9Zr8,35304
 ipaclient/remote_plugins/2_164/batch.py,sha256=9hIvEUXtbVYHR2ynTIIcmjGdsscg8gUerX8cm7TTpIU,1806
 ipaclient/remote_plugins/2_164/caacl.py,sha256=_zT0u6kbrqlxyENfku_vyY1eJVgn-fc7rwa_i94K0yo,31324
 ipaclient/remote_plugins/2_164/cert.py,sha256=2wOqYduwGkCGgCnbsvm63rsS9b_M-GhOw-SGEHXy4cM,9940
-ipaclient/remote_plugins/2_164/certprofile.py,sha256=KzGpDxG6rLpomED8JinOyoivoSwDliRGG1OQT9YMGZ0,12590
+ipaclient/remote_plugins/2_164/certprofile.py,sha256=9aFdkjMroDo-REubQ2xOnmBBLAXe9O15v6a4_5aGdpw,12586
 ipaclient/remote_plugins/2_164/config.py,sha256=ZwFySXlHPTXsUnlV2nx6QXYEQdoGJxep7Np3KHY-JEg,13738
 ipaclient/remote_plugins/2_164/delegation.py,sha256=yzNKTvfkD0NO_8eHWhpLkFRJIRE6J1NkHfb_r5QrSNE,10698
 ipaclient/remote_plugins/2_164/dns.py,sha256=gJcCaEeUC_ycizMW-MKNgl-k2-jrTuClVftcgo1CEFQ,161863
 ipaclient/remote_plugins/2_164/domainlevel.py,sha256=ohcLOAIcTmkAqQN1JpUEe5-fiQybZxgK0rM8QJU2I-g,1161
 ipaclient/remote_plugins/2_164/group.py,sha256=TQ0bkuoCSkEDNfEvJvVL9Z2QVycQEmkacxarO_h3V5g,26514
 ipaclient/remote_plugins/2_164/hbacrule.py,sha256=C86OFQtwSHqoEQInRw-MYQI0X9tU4yhSYu3PLsuM-js,35779
 ipaclient/remote_plugins/2_164/hbacsvc.py,sha256=88pKqHrXjDh8uuyqOP3ZktCLq8-NnvDk3HaIyQwSXFw,11525
 ipaclient/remote_plugins/2_164/hbacsvcgroup.py,sha256=xw00dB-y39l0YnptfTO-A7mZcAqVN8CrXiaVhPklufY,14633
 ipaclient/remote_plugins/2_164/hbactest.py,sha256=924-cov4-_WKupa_noX0rc4Od1LSbdr5I41jnrHfsjY,9122
 ipaclient/remote_plugins/2_164/host.py,sha256=pZFjA0WHxv-laXj2l2tHq5punBLYb3icYYPVfIBzpMs,48912
 ipaclient/remote_plugins/2_164/hostgroup.py,sha256=Qr5M8Bbvm0t_HMISVpXF_nvthRFUR1ETIGi44xjSXT8,20373
-ipaclient/remote_plugins/2_164/idrange.py,sha256=T9tGjMMc0B2NYf96_kChZglGhO1OccqoToKaGM65ubU,20053
+ipaclient/remote_plugins/2_164/idrange.py,sha256=1x5YAexoN0qVG3yWRUzPPS0jiZGH9RkgsJ6zqH6AXP0,20053
 ipaclient/remote_plugins/2_164/idviews.py,sha256=ML_jlSYXiI34CtAKIbGSebUoLnwmyX0vpiUSnqj8kgI,42287
 ipaclient/remote_plugins/2_164/internal.py,sha256=Pav7pfHuSHyVW3T2Z9dtyfgPcVqUtLZ0pxxMr17IVr0,2019
 ipaclient/remote_plugins/2_164/join.py,sha256=y90IQparbpYtdGsihZZVvq2fI-l1tjlnXKwort5RVlU,1490
 ipaclient/remote_plugins/2_164/krbtpolicy.py,sha256=Kej6uy5gsUE7I0yYYbhvnfj6-LajENtitVDNy4IGRl0,7559
 ipaclient/remote_plugins/2_164/migration.py,sha256=Y02IG6RITggfBI6M-GUfGqo5IV3kA7GBq9jPkeopcro,11089
 ipaclient/remote_plugins/2_164/misc.py,sha256=ww6uMauAvVYutlNHSSqkoBVpdW1kT5rHeXekLJMEGZk,2753
 ipaclient/remote_plugins/2_164/netgroup.py,sha256=y634jT1YOSt0_Svqsvkxg2Bc16WFWI5d2s9cz_vc18c,24373
 ipaclient/remote_plugins/2_164/otpconfig.py,sha256=sOorsTPvhq2qeo1wlNcaVbyWLYjXBUY82Dui7apDkSg,6184
-ipaclient/remote_plugins/2_164/otptoken.py,sha256=HSPYYJtnrla3Ing2Edv4V-_8XRQbSFs1M1aoLGBW5sY,26027
+ipaclient/remote_plugins/2_164/otptoken.py,sha256=ByNYdtnQO3O4YO5iSSP6u3vrKWUOXvZe6e3RdG_sLyw,26015
 ipaclient/remote_plugins/2_164/otptoken_yubikey.py,sha256=Rlk4ZpowXusMdYcPlIb_slO4dhZvJkFU3jYsMezNgEE,690
 ipaclient/remote_plugins/2_164/passwd.py,sha256=AGQdxirIgju6LdATI_NbHR273BWazZHPYR1zNk1Kd8s,2428
 ipaclient/remote_plugins/2_164/permission.py,sha256=ayENBpx_qRu1c_WfSs_ZcL8UEWXcr0r5-oisQREI748,34289
 ipaclient/remote_plugins/2_164/ping.py,sha256=QU6VwHCQUQrkFqCqqXyZnRgtxySWdqZlvhHVlOdJ4mA,1675
 ipaclient/remote_plugins/2_164/pkinit.py,sha256=VbluXcEICjl15p3l27J802BcIEsYXKiAYNxAi__LDXk,1198
 ipaclient/remote_plugins/2_164/privilege.py,sha256=TLxb6UifddQ0XofyJU8hPCWSlSlAU1sv_Krc1F94vR0,17919
 ipaclient/remote_plugins/2_164/pwpolicy.py,sha256=shkmQBFbec-ADLU0MUehXltYD1_Q55Tq_iOZ5NhrzB0,27506
@@ -189,15 +177,15 @@
 ipaclient/remote_plugins/2_164/server.py,sha256=pRTjZH-Sc8GPagW0GXTJLA_fgiPxYCFKD9oCbHaXPrI,8308
 ipaclient/remote_plugins/2_164/service.py,sha256=qCHiazmIMZ70BO6mFWpvDeJ79fORydAKrkixHggNXdg,35920
 ipaclient/remote_plugins/2_164/servicedelegation.py,sha256=zKUP972ZB_aEuHGyDrIVgQaAeJWwkwMYlT2Tem1FyOc,25495
 ipaclient/remote_plugins/2_164/session.py,sha256=1XLaG9O7rcJfwYaU-usj6wGKG4hWJT8fONv-OXdsK7E,678
 ipaclient/remote_plugins/2_164/stageuser.py,sha256=CufdI6vxyGsSjy4dr4zFkChFycudvOkzNNrH8q1Av_Y,46972
 ipaclient/remote_plugins/2_164/sudocmd.py,sha256=c6dw9JgVhUvFPuy2YFigNTh4AjrQFbCngjdvTnlQFJE,10907
 ipaclient/remote_plugins/2_164/sudocmdgroup.py,sha256=BUpBtgDGPW1LT9RTz2mTaIUauIVSzudLNqaBIb2rO-0,14989
-ipaclient/remote_plugins/2_164/sudorule.py,sha256=GZOsXikNwfubxNg4ggfGEARHUxLnSU0fUQdHd18Fd3U,50247
+ipaclient/remote_plugins/2_164/sudorule.py,sha256=eAKPm125EiRy_RXJUuV9OslN68bndqTW9FIzA4z76cA,50260
 ipaclient/remote_plugins/2_164/topology.py,sha256=_go5RuzHR6J1EA6KoZVUkjtky_zaUlKqwx-i2MBepto,33854
 ipaclient/remote_plugins/2_164/trust.py,sha256=7dYZMS62HqLrLQT6f3YZ9taEBN6PqTasS9_i4luAAFg,35969
 ipaclient/remote_plugins/2_164/user.py,sha256=AEItqkaMO-ATDpx6-XehEdn32Gx2u6jCCLG0i8em7ns,58614
 ipaclient/remote_plugins/2_164/vault.py,sha256=OyfsS96HeJ0c4EfHnpempXGJmEySYdQILOTZ7I9OrKs,45219
 ipaclient/remote_plugins/2_49/__init__.py,sha256=D66q144hrWbLQBEXfkW6_ZDUyHoHy78cxLYtGDx9XXc,264
 ipaclient/remote_plugins/2_49/aci.py,sha256=axrtqm0Vp_UOwsNPKEtqTTqp-NcEFO0i4u29Mi1M7w0,25387
 ipaclient/remote_plugins/2_49/automember.py,sha256=d_Z_J0TPaFoBOaAOJDJgttjhiYBQBlxLjW9OxSd2DTM,22254
@@ -211,15 +199,15 @@
 ipaclient/remote_plugins/2_49/group.py,sha256=myAaP-TaqclzUNOiLCY6emI0b9qowuIeofBe3B1zm_w,24815
 ipaclient/remote_plugins/2_49/hbacrule.py,sha256=CpcmBVxQ0FCfFnR4LdWTT9gyR1DOZD-0ul9JSaJ3nOA,33334
 ipaclient/remote_plugins/2_49/hbacsvc.py,sha256=aqqqHU1cV-VvtP5ogA-CmhU69ib9WSt3grGtQYX8hko,10742
 ipaclient/remote_plugins/2_49/hbacsvcgroup.py,sha256=RbwdYw5lKwS2DIpgj6Yg0n-YpHWRXscrSi7Xkf2JmKM,13533
 ipaclient/remote_plugins/2_49/hbactest.py,sha256=xR1_Zj5cjTQIhtYizaLNHh9-YIM9QYDG1i76KnqRIYk,6574
 ipaclient/remote_plugins/2_49/host.py,sha256=71gr0aw84i8UrWoaNIqPsSSH-IvLsn4YPq21Uiayuug,30139
 ipaclient/remote_plugins/2_49/hostgroup.py,sha256=COuZ2ixUSD7SERr5Y2INHnr461xm03FnBiRNdGbZk3g,19153
-ipaclient/remote_plugins/2_49/idrange.py,sha256=PSyZD-F7qkjSlZb4L9h8ewHrEThAIH8n_1EBm0dcRfY,18929
+ipaclient/remote_plugins/2_49/idrange.py,sha256=ff6hSN6ewvIPGaHStPGKt2CHnszIMkNxx9c8q6h2OCI,18929
 ipaclient/remote_plugins/2_49/internal.py,sha256=UwMEwiGG2sSujYAB4qxh7bC_RxGc8ykb3qfauFndWgI,1994
 ipaclient/remote_plugins/2_49/join.py,sha256=1xuKidvyu-0JmH0rCW11w2Sm3-KD21gzrSenEMRAZOE,1537
 ipaclient/remote_plugins/2_49/krbtpolicy.py,sha256=0RPkeVMJ1z_vUHUbI-7n2IUwlGIZMLYodRrAbDRuAr8,7610
 ipaclient/remote_plugins/2_49/migration.py,sha256=nl-E4hw8JjjvQ4CkMmT9Su3aJZYAuZpI3eQpt0EOR8M,10395
 ipaclient/remote_plugins/2_49/misc.py,sha256=ww6uMauAvVYutlNHSSqkoBVpdW1kT5rHeXekLJMEGZk,2753
 ipaclient/remote_plugins/2_49/netgroup.py,sha256=56MzyrAGgnAkbALf6LQp8IaokipzWRbR682stLbZFPA,23320
 ipaclient/remote_plugins/2_49/passwd.py,sha256=Qqw7o_k8rDcbYp4fpK6iKrG2W57SWzLyOm7biAqY4lk,2263
@@ -231,16 +219,16 @@
 ipaclient/remote_plugins/2_49/role.py,sha256=8gTjKIE7IEv19Vq3qxarYvMunl6kDoz4H-IFUusrD08,18589
 ipaclient/remote_plugins/2_49/selfservice.py,sha256=kzPrWfaou27-GhqjYZrko7LFffyPUsv7gByQr9gKKy4,9297
 ipaclient/remote_plugins/2_49/selinuxusermap.py,sha256=vj--mFAbc6rEFIYontmUo9s2ys6-t_Dv0x8b7Ztkse4,23713
 ipaclient/remote_plugins/2_49/service.py,sha256=tiP6nmjSk3SnkSyWR-zVJ2IAL1OLL4y_UPVwX805-YU,18039
 ipaclient/remote_plugins/2_49/session.py,sha256=-XImG3BE_mTICnWVbZFIbSH04gpG7mIfPhayQKV5Bxo,25115
 ipaclient/remote_plugins/2_49/sudocmd.py,sha256=WaX2Jpf_4fpaVOP7T9ZauJnB6_GFWbF-fDTdpOjWtxM,10124
 ipaclient/remote_plugins/2_49/sudocmdgroup.py,sha256=t3sCyZ99SzK46gkxS78hC6bbSiym-w0eJftU364K-ew,13741
-ipaclient/remote_plugins/2_49/sudorule.py,sha256=RQ_oKZC2x58vCjTcHuAM3Ma376z2Pf1iHnl0QfLh5lU,44052
+ipaclient/remote_plugins/2_49/sudorule.py,sha256=uKICfFRQRRu4AyGbGYsAWMEFkIaggztpPsBgy-IFcqc,44061
 ipaclient/remote_plugins/2_49/trust.py,sha256=8bQoyD2ZtjJHVgGGsmJLD8ZxBz0U32cRgJa4rHPQpGo,20233
 ipaclient/remote_plugins/2_49/user.py,sha256=vVK_qOETHFRB7iLHJ1TS4b6NIu_6CaeL6oiKEbQZaUY,39108
-ipaclient-4.8.9.dist-info/COPYING,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
-ipaclient-4.8.9.dist-info/METADATA,sha256=RxmWTT2j5d_w1cq-SxvjJfCEQSWWFL0WIL7AJSrcwm8,1686
-ipaclient-4.8.9.dist-info/WHEEL,sha256=8zNYZbwQSXoB9IfXOjPfeNwvAsALAjffgk27FqvCWbo,110
-ipaclient-4.8.9.dist-info/entry_points.txt,sha256=McyzcqFKM1BRapoNRPIbM5zq37fdudKp99WTZUjtPQs,49
-ipaclient-4.8.9.dist-info/top_level.txt,sha256=sfyzA6xhyMqxuNCw5sOP_IzH7aAHH8op5jHTOK8rmNg,10
-ipaclient-4.8.9.dist-info/RECORD,,
+ipaclient-4.9.12.dist-info/COPYING,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
+ipaclient-4.9.12.dist-info/METADATA,sha256=xz5Tj2j_lZb2U87Vu5R9iKkDiPus4_LxbC0Zps422to,1607
+ipaclient-4.9.12.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+ipaclient-4.9.12.dist-info/entry_points.txt,sha256=XzS2l_vN8KEg3N8wcpWs5wpig3cDFPzGoti48aJUuLc,48
+ipaclient-4.9.12.dist-info/top_level.txt,sha256=sfyzA6xhyMqxuNCw5sOP_IzH7aAHH8op5jHTOK8rmNg,10
+ipaclient-4.9.12.dist-info/RECORD,,
```

