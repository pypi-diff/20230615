# Comparing `tmp/finance_enums-0.2.1.tar.gz` & `tmp/finance_enums-0.2.2.tar.gz`

## Comparing `finance_enums-0.2.1.tar` & `finance_enums-0.2.2.tar`

### file list

```diff
@@ -1,326 +1,326 @@
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 finance_enums-0.2.1/local_dependencies/finance_enums/Cargo.toml
--rw-r--r--   0     1001      123     1587 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/Makefile
--rw-r--r--   0     1001      123        1 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/common/mod.rs
--rw-r--r--   0     1001      123   157747 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/country/iso3166.rs
--rw-r--r--   0     1001      123       34 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/country/mod.rs
--rw-r--r--   0     1001      123    10861 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/currency/iso4217.rs
--rw-r--r--   0     1001      123       33 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/currency/mod.rs
--rw-r--r--   0     1001      123     3769 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/exchange/iso10383.rs
--rw-r--r--   0     1001      123       87 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/exchange/mod.rs
--rw-r--r--   0     1001      123       44 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/instrument/iso10962.rs
--rw-r--r--   0     1001      123      457 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/instrument/mod.rs
--rw-r--r--   0     1001      123      351 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/lib.rs
--rw-r--r--   0     1001      123    22775 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/sector/industry.rs
--rw-r--r--   0     1001      123    10828 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/sector/industry_group.rs
--rw-r--r--   0     1001      123      314 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/sector/mod.rs
--rw-r--r--   0     1001      123     5173 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/sector/sector.rs
--rw-r--r--   0     1001      123    24083 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/sector/subindustry.rs
--rw-r--r--   0     1001      123      239 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/security/bond.rs
--rw-r--r--   0     1001      123     1229 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/security/commodity.rs
--rw-r--r--   0     1001      123        1 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/security/currency.rs
--rw-r--r--   0     1001      123      306 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/security/equity.rs
--rw-r--r--   0     1001      123      623 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/security/fund.rs
--rw-r--r--   0     1001      123      415 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/security/future.rs
--rw-r--r--   0     1001      123      290 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/security/mod.rs
--rw-r--r--   0     1001      123      422 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/security/option.rs
--rw-r--r--   0     1001      123      349 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/security/security.rs
--rw-r--r--   0     1001      123      796 2023-06-13 21:08:39.000000 finance_enums-0.2.1/local_dependencies/finance_enums/src/trading/mod.rs
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 finance_enums-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123      414 2023-06-13 21:08:39.000000 finance_enums-0.2.1/.bumpversion.cfg
--rw-r--r--   0     1001      123      147 2023-06-13 21:08:39.000000 finance_enums-0.2.1/.gitattributes
--rw-r--r--   0     1001      123     3352 2023-06-13 21:08:39.000000 finance_enums-0.2.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123      834 2023-06-13 21:08:39.000000 finance_enums-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      123      595 2023-06-13 21:08:39.000000 finance_enums-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      123      206 2023-06-13 21:08:39.000000 finance_enums-0.2.1/.github/dependabot.yml
--rw-r--r--   0     1001      123     1608 2023-06-13 21:08:39.000000 finance_enums-0.2.1/.github/workflows/build.yml
--rw-r--r--   0     1001      123     4126 2023-06-13 21:08:39.000000 finance_enums-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0     1001      123     2275 2023-06-13 21:08:39.000000 finance_enums-0.2.1/.gitignore
--rw-r--r--   0     1001      123    11351 2023-06-13 21:08:39.000000 finance_enums-0.2.1/LICENSE
--rw-r--r--   0     1001      123     1990 2023-06-13 21:08:39.000000 finance_enums-0.2.1/Makefile
--rw-r--r--   0     1001      123     1246 2023-06-13 21:08:39.000000 finance_enums-0.2.1/README.md
--rw-r--r--   0     1001      123       52 2023-06-13 21:08:39.000000 finance_enums-0.2.1/finance_enums/__init__.py
--rw-r--r--   0     1001      123       52 2023-06-13 21:08:39.000000 finance_enums-0.2.1/finance_enums/tests/test_all.py
--rw-r--r--   0     1001      123      195 2023-06-13 21:08:39.000000 finance_enums-0.2.1/finance_enums/tests/test_country.py
--rw-r--r--   0     1001      123      239 2023-06-13 21:08:39.000000 finance_enums-0.2.1/finance_enums/tests/test_currency.py
--rw-r--r--   0     1001      123      137 2023-06-13 21:08:39.000000 finance_enums-0.2.1/finance_enums/tests/test_exchange.py
--rw-r--r--   0     1001      123        0 2023-06-13 21:08:39.000000 finance_enums-0.2.1/finance_enums/tests/test_instrument.py
--rw-r--r--   0     1001      123      428 2023-06-13 21:08:39.000000 finance_enums-0.2.1/finance_enums/tests/test_sector.py
--rw-r--r--   0     1001      123     1024 2023-06-13 21:08:39.000000 finance_enums-0.2.1/finance_enums/tests/test_security.py
--rw-r--r--   0     1001      123      413 2023-06-13 21:08:39.000000 finance_enums-0.2.1/finance_enums/tests/test_trading.py
--rw-r--r--   0     1001      123      309 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AD.png
--rw-r--r--   0     1001      123      122 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AE.png
--rw-r--r--   0     1001      123      586 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AF.png
--rw-r--r--   0     1001      123      443 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AG.png
--rw-r--r--   0     1001      123      410 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AI.png
--rw-r--r--   0     1001      123      315 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AL.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AM.png
--rw-r--r--   0     1001      123      285 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AO.png
--rw-r--r--   0     1001      123      300 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AQ.png
--rw-r--r--   0     1001      123      150 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AR.png
--rw-r--r--   0     1001      123      469 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AS.png
--rw-r--r--   0     1001      123       93 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AT.png
--rw-r--r--   0     1001      123      405 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AU.png
--rw-r--r--   0     1001      123      176 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AW.png
--rw-r--r--   0     1001      123      155 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AX.png
--rw-r--r--   0     1001      123      165 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/AZ.png
--rw-r--r--   0     1001      123      321 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BA.png
--rw-r--r--   0     1001      123      235 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BB.png
--rw-r--r--   0     1001      123      246 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BD.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BE.png
--rw-r--r--   0     1001      123      173 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BF.png
--rw-r--r--   0     1001      123      116 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BG.png
--rw-r--r--   0     1001      123      189 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BH.png
--rw-r--r--   0     1001      123      394 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BI.png
--rw-r--r--   0     1001      123      122 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BJ.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BL.png
--rw-r--r--   0     1001      123      461 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BM.png
--rw-r--r--   0     1001      123      547 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BN.png
--rw-r--r--   0     1001      123      217 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BO.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BQ.png
--rw-r--r--   0     1001      123      438 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BR.png
--rw-r--r--   0     1001      123      181 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BS.png
--rw-r--r--   0     1001      123      570 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BT.png
--rw-r--r--   0     1001      123      153 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BV.png
--rw-r--r--   0     1001      123      111 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BW.png
--rw-r--r--   0     1001      123      206 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BY.png
--rw-r--r--   0     1001      123      378 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/BZ.png
--rw-r--r--   0     1001      123      259 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CA.png
--rw-r--r--   0     1001      123      365 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CC.png
--rw-r--r--   0     1001      123      350 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CD.png
--rw-r--r--   0     1001      123      246 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CF.png
--rw-r--r--   0     1001      123      330 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CG.png
--rw-r--r--   0     1001      123      113 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CH.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CI.png
--rw-r--r--   0     1001      123      487 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CK.png
--rw-r--r--   0     1001      123      186 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CL.png
--rw-r--r--   0     1001      123      158 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CM.png
--rw-r--r--   0     1001      123      214 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CN.png
--rw-r--r--   0     1001      123      116 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CO.png
--rw-r--r--   0     1001      123      123 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CR.png
--rw-r--r--   0     1001      123      240 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CU.png
--rw-r--r--   0     1001      123      267 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CV.png
--rw-r--r--   0     1001      123      189 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CW.png
--rw-r--r--   0     1001      123      508 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CX.png
--rw-r--r--   0     1001      123      318 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CY.png
--rw-r--r--   0     1001      123      273 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/CZ.png
--rw-r--r--   0     1001      123      116 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/DE.png
--rw-r--r--   0     1001      123      358 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/DJ.png
--rw-r--r--   0     1001      123      124 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/DK.png
--rw-r--r--   0     1001      123      269 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/DM.png
--rw-r--r--   0     1001      123      158 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/DO.png
--rw-r--r--   0     1001      123      276 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/DZ.png
--rw-r--r--   0     1001      123      325 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/EC.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/EE.png
--rw-r--r--   0     1001      123      175 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/EG.png
--rw-r--r--   0     1001      123      271 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/EH.png
--rw-r--r--   0     1001      123      465 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/ER.png
--rw-r--r--   0     1001      123      273 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/ES.png
--rw-r--r--   0     1001      123      324 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/ET.png
--rw-r--r--   0     1001      123      130 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/FI.png
--rw-r--r--   0     1001      123      456 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/FJ.png
--rw-r--r--   0     1001      123      475 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/FK.png
--rw-r--r--   0     1001      123      183 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/FM.png
--rw-r--r--   0     1001      123      150 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/FO.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/FR.png
--rw-r--r--   0     1001      123       98 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GA.png
--rw-r--r--   0     1001      123      490 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GB.png
--rw-r--r--   0     1001      123      417 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GD.png
--rw-r--r--   0     1001      123      155 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GE.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GF.png
--rw-r--r--   0     1001      123      184 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GG.png
--rw-r--r--   0     1001      123      180 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GH.png
--rw-r--r--   0     1001      123      288 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GI.png
--rw-r--r--   0     1001      123      302 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GL.png
--rw-r--r--   0     1001      123      110 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GM.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GN.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GP.png
--rw-r--r--   0     1001      123      305 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GQ.png
--rw-r--r--   0     1001      123      180 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GR.png
--rw-r--r--   0     1001      123      517 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GS.png
--rw-r--r--   0     1001      123      210 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GT.png
--rw-r--r--   0     1001      123      237 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GU.png
--rw-r--r--   0     1001      123      168 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GW.png
--rw-r--r--   0     1001      123      375 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/GY.png
--rw-r--r--   0     1001      123      321 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/HK.png
--rw-r--r--   0     1001      123      405 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/HM.png
--rw-r--r--   0     1001      123      137 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/HN.png
--rw-r--r--   0     1001      123      262 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/HR.png
--rw-r--r--   0     1001      123      171 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/HT.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/HU.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/ID.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/IE.png
--rw-r--r--   0     1001      123      170 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/IL.png
--rw-r--r--   0     1001      123      250 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/IM.png
--rw-r--r--   0     1001      123      182 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/IN.png
--rw-r--r--   0     1001      123      952 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/IO.png
--rw-r--r--   0     1001      123      203 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/IQ.png
--rw-r--r--   0     1001      123      356 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/IR.png
--rw-r--r--   0     1001      123      153 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/IS.png
--rw-r--r--   0     1001      123      122 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/IT.png
--rw-r--r--   0     1001      123      453 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/JE.png
--rw-r--r--   0     1001      123      322 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/JM.png
--rw-r--r--   0     1001      123      250 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/JO.png
--rw-r--r--   0     1001      123      240 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/JP.png
--rw-r--r--   0     1001      123      294 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KE.png
--rw-r--r--   0     1001      123      327 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KG.png
--rw-r--r--   0     1001      123      271 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KH.png
--rw-r--r--   0     1001      123      604 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KI.png
--rw-r--r--   0     1001      123      413 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KM.png
--rw-r--r--   0     1001      123      618 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KN.png
--rw-r--r--   0     1001      123      233 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KP.png
--rw-r--r--   0     1001      123      447 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KR.png
--rw-r--r--   0     1001      123      195 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KW.png
--rw-r--r--   0     1001      123      456 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KY.png
--rw-r--r--   0     1001      123      331 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/KZ.png
--rw-r--r--   0     1001      123      173 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LA.png
--rw-r--r--   0     1001      123      308 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LB.png
--rw-r--r--   0     1001      123      261 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LC.png
--rw-r--r--   0     1001      123      199 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LI.png
--rw-r--r--   0     1001      123      492 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LK.png
--rw-r--r--   0     1001      123      205 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LR.png
--rw-r--r--   0     1001      123      209 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LS.png
--rw-r--r--   0     1001      123      116 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LT.png
--rw-r--r--   0     1001      123      116 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LU.png
--rw-r--r--   0     1001      123      103 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LV.png
--rw-r--r--   0     1001      123      149 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/LY.png
--rw-r--r--   0     1001      123      190 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MA.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MC.png
--rw-r--r--   0     1001      123      249 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MD.png
--rw-r--r--   0     1001      123      335 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/ME.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MF.png
--rw-r--r--   0     1001      123      122 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MG.png
--rw-r--r--   0     1001      123      520 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MH.png
--rw-r--r--   0     1001      123      418 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MK.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/ML.png
--rw-r--r--   0     1001      123      280 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MM.png
--rw-r--r--   0     1001      123      243 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MN.png
--rw-r--r--   0     1001      123      311 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MO.png
--rw-r--r--   0     1001      123      450 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MP.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MQ.png
--rw-r--r--   0     1001      123      266 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MR.png
--rw-r--r--   0     1001      123      454 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MS.png
--rw-r--r--   0     1001      123      174 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MT.png
--rw-r--r--   0     1001      123      132 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MU.png
--rw-r--r--   0     1001      123      187 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MV.png
--rw-r--r--   0     1001      123      231 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MW.png
--rw-r--r--   0     1001      123      247 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MX.png
--rw-r--r--   0     1001      123      304 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MY.png
--rw-r--r--   0     1001      123      395 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/MZ.png
--rw-r--r--   0     1001      123      602 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NA.png
--rw-r--r--   0     1001      123      393 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NC.png
--rw-r--r--   0     1001      123      152 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NE.png
--rw-r--r--   0     1001      123      284 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NF.png
--rw-r--r--   0     1001      123       96 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NG.png
--rw-r--r--   0     1001      123      193 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NI.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NL.png
--rw-r--r--   0     1001      123      153 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NO.png
--rw-r--r--   0     1001      123      646 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NP.png
--rw-r--r--   0     1001      123      151 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NR.png
--rw-r--r--   0     1001      123      336 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NU.png
--rw-r--r--   0     1001      123      376 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/NZ.png
--rw-r--r--   0     1001      123      179 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/OM.png
--rw-r--r--   0     1001      123      294 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PA.png
--rw-r--r--   0     1001      123       96 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PE.png
--rw-r--r--   0     1001      123      294 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PF.png
--rw-r--r--   0     1001      123      377 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PG.png
--rw-r--r--   0     1001      123      319 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PH.png
--rw-r--r--   0     1001      123      295 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PK.png
--rw-r--r--   0     1001      123       92 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PL.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PM.png
--rw-r--r--   0     1001      123      556 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PN.png
--rw-r--r--   0     1001      123      296 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PR.png
--rw-r--r--   0     1001      123      293 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PS.png
--rw-r--r--   0     1001      123      354 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PT.png
--rw-r--r--   0     1001      123      239 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PW.png
--rw-r--r--   0     1001      123      190 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/PY.png
--rw-r--r--   0     1001      123      104 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/QA.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/RE.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/RO.png
--rw-r--r--   0     1001      123      398 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/RS.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/RU.png
--rw-r--r--   0     1001      123      212 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/RW.png
--rw-r--r--   0     1001      123      334 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SA.png
--rw-r--r--   0     1001      123      477 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SB.png
--rw-r--r--   0     1001      123      517 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SC.png
--rw-r--r--   0     1001      123      222 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SD.png
--rw-r--r--   0     1001      123      130 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SE.png
--rw-r--r--   0     1001      123      249 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SG.png
--rw-r--r--   0     1001      123      490 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SH.png
--rw-r--r--   0     1001      123      173 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SI.png
--rw-r--r--   0     1001      123      153 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SJ.png
--rw-r--r--   0     1001      123      326 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SK.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SL.png
--rw-r--r--   0     1001      123      362 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SM.png
--rw-r--r--   0     1001      123      158 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SN.png
--rw-r--r--   0     1001      123      198 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SO.png
--rw-r--r--   0     1001      123      215 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SR.png
--rw-r--r--   0     1001      123      264 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SS.png
--rw-r--r--   0     1001      123      254 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/ST.png
--rw-r--r--   0     1001      123      195 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SV.png
--rw-r--r--   0     1001      123      419 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SX.png
--rw-r--r--   0     1001      123      182 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SY.png
--rw-r--r--   0     1001      123      436 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/SZ.png
--rw-r--r--   0     1001      123      414 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TC.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TD.png
--rw-r--r--   0     1001      123      328 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TF.png
--rw-r--r--   0     1001      123      248 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TG.png
--rw-r--r--   0     1001      123      114 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TH.png
--rw-r--r--   0     1001      123      196 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TJ.png
--rw-r--r--   0     1001      123      384 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TK.png
--rw-r--r--   0     1001      123      280 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TL.png
--rw-r--r--   0     1001      123      486 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TM.png
--rw-r--r--   0     1001      123      285 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TN.png
--rw-r--r--   0     1001      123      142 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TO.png
--rw-r--r--   0     1001      123      263 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TR.png
--rw-r--r--   0     1001      123      466 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TT.png
--rw-r--r--   0     1001      123      482 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TV.png
--rw-r--r--   0     1001      123      235 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TW.png
--rw-r--r--   0     1001      123      511 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/TZ.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/UA.png
--rw-r--r--   0     1001      123      231 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/UG.png
--rw-r--r--   0     1001      123      333 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/UM.png
--rw-r--r--   0     1001      123      333 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/US.png
--rw-r--r--   0     1001      123      294 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/UY.png
--rw-r--r--   0     1001      123      213 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/UZ.png
--rw-r--r--   0     1001      123      282 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/VA.png
--rw-r--r--   0     1001      123      239 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/VC.png
--rw-r--r--   0     1001      123      197 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/VE.png
--rw-r--r--   0     1001      123      471 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/VG.png
--rw-r--r--   0     1001      123      795 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/VI.png
--rw-r--r--   0     1001      123      205 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/VN.png
--rw-r--r--   0     1001      123      427 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/VU.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/WF.png
--rw-r--r--   0     1001      123      182 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/WS.png
--rw-r--r--   0     1001      123      100 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/YE.png
--rw-r--r--   0     1001      123      108 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/YT.png
--rw-r--r--   0     1001      123      406 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/ZA.png
--rw-r--r--   0     1001      123      225 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/ZM.png
--rw-r--r--   0     1001      123      295 2023-06-13 21:08:39.000000 finance_enums-0.2.1/flags/ZW.png
--rw-r--r--   0     1001      123    79321 2023-06-13 21:08:39.000000 finance_enums-0.2.1/helpers/GICS Map 2023.xlsx
--rw-r--r--   0     1001      123   509696 2023-06-13 21:08:39.000000 finance_enums-0.2.1/helpers/ISO10383_MIC.csv
--rw-r--r--   0     1001      123      402 2023-06-13 21:08:39.000000 finance_enums-0.2.1/helpers/flags_to_strings.py
--rw-r--r--   0     1001      123   149841 2023-06-13 21:08:39.000000 finance_enums-0.2.1/helpers/iso10383_generated.rs
--rw-r--r--   0     1001      123     4962 2023-06-13 21:08:39.000000 finance_enums-0.2.1/helpers/process_mics.py
--rw-r--r--   0     1001      123      577 2023-06-13 21:08:39.000000 finance_enums-0.2.1/helpers/scrape_flags.py
--rw-r--r--   0     1001      123     1526 2023-06-13 21:08:39.000000 finance_enums-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123    58696 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/country/mod.rs
--rw-r--r--   0     1001      123    27210 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/currency/mod.rs
--rw-r--r--   0     1001      123     4106 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/exchange/mod.rs
--rw-r--r--   0     1001      123        0 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/instrument/mod.rs
--rw-r--r--   0     1001      123     1302 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123    14542 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/sector/industry.rs
--rw-r--r--   0     1001      123     6641 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/sector/industry_group.rs
--rw-r--r--   0     1001      123      190 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/sector/mod.rs
--rw-r--r--   0     1001      123     3011 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/sector/sector.rs
--rw-r--r--   0     1001      123    32067 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/sector/subindustry.rs
--rw-r--r--   0     1001      123     1581 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/security/bond.rs
--rw-r--r--   0     1001      123     1681 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/security/commodity.rs
--rw-r--r--   0     1001      123        0 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/security/currency.rs
--rw-r--r--   0     1001      123     2018 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/security/equity.rs
--rw-r--r--   0     1001      123     4717 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/security/fund.rs
--rw-r--r--   0     1001      123      259 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/security/mod.rs
--rw-r--r--   0     1001      123     3113 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/security/option.rs
--rw-r--r--   0     1001      123     3115 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/security/security.rs
--rw-r--r--   0     1001      123     5933 2023-06-13 21:08:39.000000 finance_enums-0.2.1/src/trading/mod.rs
--rw-r--r--   0     1001      123    17385 2023-06-13 21:09:16.000000 finance_enums-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     2720 1970-01-01 00:00:00.000000 finance_enums-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 finance_enums-0.2.2/local_dependencies/finance_enums/Cargo.toml
+-rw-r--r--   0     1001      123     1587 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/Makefile
+-rw-r--r--   0     1001      123        1 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/common/mod.rs
+-rw-r--r--   0     1001      123   157760 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/country/iso3166.rs
+-rw-r--r--   0     1001      123       34 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/country/mod.rs
+-rw-r--r--   0     1001      123    11111 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/currency/iso4217.rs
+-rw-r--r--   0     1001      123       33 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/currency/mod.rs
+-rw-r--r--   0     1001      123     3782 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/exchange/iso10383.rs
+-rw-r--r--   0     1001      123       87 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/exchange/mod.rs
+-rw-r--r--   0     1001      123       44 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/instrument/iso10962.rs
+-rw-r--r--   0     1001      123      470 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/instrument/mod.rs
+-rw-r--r--   0     1001      123      351 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/lib.rs
+-rw-r--r--   0     1001      123    22788 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/industry.rs
+-rw-r--r--   0     1001      123    10841 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/industry_group.rs
+-rw-r--r--   0     1001      123      314 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/mod.rs
+-rw-r--r--   0     1001      123     5186 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/sector.rs
+-rw-r--r--   0     1001      123    24096 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/subindustry.rs
+-rw-r--r--   0     1001      123      252 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/bond.rs
+-rw-r--r--   0     1001      123     1287 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/commodity.rs
+-rw-r--r--   0     1001      123        1 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/currency.rs
+-rw-r--r--   0     1001      123      319 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/equity.rs
+-rw-r--r--   0     1001      123      662 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/fund.rs
+-rw-r--r--   0     1001      123      441 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/future.rs
+-rw-r--r--   0     1001      123      290 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/mod.rs
+-rw-r--r--   0     1001      123      448 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/option.rs
+-rw-r--r--   0     1001      123      362 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/security.rs
+-rw-r--r--   0     1001      123      848 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/trading/mod.rs
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 finance_enums-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123      414 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.bumpversion.cfg
+-rw-r--r--   0     1001      123      147 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.gitattributes
+-rw-r--r--   0     1001      123     3352 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123      834 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      595 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123      206 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/dependabot.yml
+-rw-r--r--   0     1001      123     1608 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/workflows/build.yml
+-rw-r--r--   0     1001      123     4126 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123     2284 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.gitignore
+-rw-r--r--   0     1001      123    11351 2023-06-15 20:52:19.000000 finance_enums-0.2.2/LICENSE
+-rw-r--r--   0     1001      123     1990 2023-06-15 20:52:19.000000 finance_enums-0.2.2/Makefile
+-rw-r--r--   0     1001      123     1246 2023-06-15 20:52:19.000000 finance_enums-0.2.2/README.md
+-rw-r--r--   0     1001      123       52 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/__init__.py
+-rw-r--r--   0     1001      123       52 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_all.py
+-rw-r--r--   0     1001      123      195 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_country.py
+-rw-r--r--   0     1001      123      429 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_currency.py
+-rw-r--r--   0     1001      123      137 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_exchange.py
+-rw-r--r--   0     1001      123        0 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_instrument.py
+-rw-r--r--   0     1001      123      428 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_sector.py
+-rw-r--r--   0     1001      123     1024 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_security.py
+-rw-r--r--   0     1001      123      413 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_trading.py
+-rw-r--r--   0     1001      123      309 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AD.png
+-rw-r--r--   0     1001      123      122 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AE.png
+-rw-r--r--   0     1001      123      586 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AF.png
+-rw-r--r--   0     1001      123      443 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AG.png
+-rw-r--r--   0     1001      123      410 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AI.png
+-rw-r--r--   0     1001      123      315 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AL.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AM.png
+-rw-r--r--   0     1001      123      285 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AO.png
+-rw-r--r--   0     1001      123      300 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AQ.png
+-rw-r--r--   0     1001      123      150 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AR.png
+-rw-r--r--   0     1001      123      469 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AS.png
+-rw-r--r--   0     1001      123       93 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AT.png
+-rw-r--r--   0     1001      123      405 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AU.png
+-rw-r--r--   0     1001      123      176 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AW.png
+-rw-r--r--   0     1001      123      155 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AX.png
+-rw-r--r--   0     1001      123      165 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AZ.png
+-rw-r--r--   0     1001      123      321 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BA.png
+-rw-r--r--   0     1001      123      235 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BB.png
+-rw-r--r--   0     1001      123      246 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BD.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BE.png
+-rw-r--r--   0     1001      123      173 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BF.png
+-rw-r--r--   0     1001      123      116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BG.png
+-rw-r--r--   0     1001      123      189 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BH.png
+-rw-r--r--   0     1001      123      394 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BI.png
+-rw-r--r--   0     1001      123      122 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BJ.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BL.png
+-rw-r--r--   0     1001      123      461 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BM.png
+-rw-r--r--   0     1001      123      547 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BN.png
+-rw-r--r--   0     1001      123      217 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BO.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BQ.png
+-rw-r--r--   0     1001      123      438 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BR.png
+-rw-r--r--   0     1001      123      181 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BS.png
+-rw-r--r--   0     1001      123      570 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BT.png
+-rw-r--r--   0     1001      123      153 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BV.png
+-rw-r--r--   0     1001      123      111 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BW.png
+-rw-r--r--   0     1001      123      206 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BY.png
+-rw-r--r--   0     1001      123      378 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BZ.png
+-rw-r--r--   0     1001      123      259 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CA.png
+-rw-r--r--   0     1001      123      365 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CC.png
+-rw-r--r--   0     1001      123      350 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CD.png
+-rw-r--r--   0     1001      123      246 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CF.png
+-rw-r--r--   0     1001      123      330 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CG.png
+-rw-r--r--   0     1001      123      113 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CH.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CI.png
+-rw-r--r--   0     1001      123      487 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CK.png
+-rw-r--r--   0     1001      123      186 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CL.png
+-rw-r--r--   0     1001      123      158 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CM.png
+-rw-r--r--   0     1001      123      214 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CN.png
+-rw-r--r--   0     1001      123      116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CO.png
+-rw-r--r--   0     1001      123      123 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CR.png
+-rw-r--r--   0     1001      123      240 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CU.png
+-rw-r--r--   0     1001      123      267 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CV.png
+-rw-r--r--   0     1001      123      189 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CW.png
+-rw-r--r--   0     1001      123      508 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CX.png
+-rw-r--r--   0     1001      123      318 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CY.png
+-rw-r--r--   0     1001      123      273 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CZ.png
+-rw-r--r--   0     1001      123      116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DE.png
+-rw-r--r--   0     1001      123      358 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DJ.png
+-rw-r--r--   0     1001      123      124 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DK.png
+-rw-r--r--   0     1001      123      269 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DM.png
+-rw-r--r--   0     1001      123      158 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DO.png
+-rw-r--r--   0     1001      123      276 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DZ.png
+-rw-r--r--   0     1001      123      325 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/EC.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/EE.png
+-rw-r--r--   0     1001      123      175 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/EG.png
+-rw-r--r--   0     1001      123      271 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/EH.png
+-rw-r--r--   0     1001      123      465 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ER.png
+-rw-r--r--   0     1001      123      273 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ES.png
+-rw-r--r--   0     1001      123      324 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ET.png
+-rw-r--r--   0     1001      123      130 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FI.png
+-rw-r--r--   0     1001      123      456 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FJ.png
+-rw-r--r--   0     1001      123      475 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FK.png
+-rw-r--r--   0     1001      123      183 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FM.png
+-rw-r--r--   0     1001      123      150 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FO.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FR.png
+-rw-r--r--   0     1001      123       98 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GA.png
+-rw-r--r--   0     1001      123      490 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GB.png
+-rw-r--r--   0     1001      123      417 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GD.png
+-rw-r--r--   0     1001      123      155 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GE.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GF.png
+-rw-r--r--   0     1001      123      184 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GG.png
+-rw-r--r--   0     1001      123      180 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GH.png
+-rw-r--r--   0     1001      123      288 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GI.png
+-rw-r--r--   0     1001      123      302 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GL.png
+-rw-r--r--   0     1001      123      110 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GM.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GN.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GP.png
+-rw-r--r--   0     1001      123      305 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GQ.png
+-rw-r--r--   0     1001      123      180 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GR.png
+-rw-r--r--   0     1001      123      517 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GS.png
+-rw-r--r--   0     1001      123      210 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GT.png
+-rw-r--r--   0     1001      123      237 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GU.png
+-rw-r--r--   0     1001      123      168 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GW.png
+-rw-r--r--   0     1001      123      375 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GY.png
+-rw-r--r--   0     1001      123      321 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HK.png
+-rw-r--r--   0     1001      123      405 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HM.png
+-rw-r--r--   0     1001      123      137 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HN.png
+-rw-r--r--   0     1001      123      262 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HR.png
+-rw-r--r--   0     1001      123      171 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HT.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HU.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ID.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IE.png
+-rw-r--r--   0     1001      123      170 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IL.png
+-rw-r--r--   0     1001      123      250 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IM.png
+-rw-r--r--   0     1001      123      182 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IN.png
+-rw-r--r--   0     1001      123      952 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IO.png
+-rw-r--r--   0     1001      123      203 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IQ.png
+-rw-r--r--   0     1001      123      356 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IR.png
+-rw-r--r--   0     1001      123      153 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IS.png
+-rw-r--r--   0     1001      123      122 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IT.png
+-rw-r--r--   0     1001      123      453 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/JE.png
+-rw-r--r--   0     1001      123      322 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/JM.png
+-rw-r--r--   0     1001      123      250 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/JO.png
+-rw-r--r--   0     1001      123      240 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/JP.png
+-rw-r--r--   0     1001      123      294 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KE.png
+-rw-r--r--   0     1001      123      327 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KG.png
+-rw-r--r--   0     1001      123      271 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KH.png
+-rw-r--r--   0     1001      123      604 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KI.png
+-rw-r--r--   0     1001      123      413 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KM.png
+-rw-r--r--   0     1001      123      618 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KN.png
+-rw-r--r--   0     1001      123      233 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KP.png
+-rw-r--r--   0     1001      123      447 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KR.png
+-rw-r--r--   0     1001      123      195 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KW.png
+-rw-r--r--   0     1001      123      456 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KY.png
+-rw-r--r--   0     1001      123      331 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KZ.png
+-rw-r--r--   0     1001      123      173 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LA.png
+-rw-r--r--   0     1001      123      308 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LB.png
+-rw-r--r--   0     1001      123      261 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LC.png
+-rw-r--r--   0     1001      123      199 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LI.png
+-rw-r--r--   0     1001      123      492 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LK.png
+-rw-r--r--   0     1001      123      205 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LR.png
+-rw-r--r--   0     1001      123      209 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LS.png
+-rw-r--r--   0     1001      123      116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LT.png
+-rw-r--r--   0     1001      123      116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LU.png
+-rw-r--r--   0     1001      123      103 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LV.png
+-rw-r--r--   0     1001      123      149 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LY.png
+-rw-r--r--   0     1001      123      190 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MA.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MC.png
+-rw-r--r--   0     1001      123      249 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MD.png
+-rw-r--r--   0     1001      123      335 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ME.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MF.png
+-rw-r--r--   0     1001      123      122 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MG.png
+-rw-r--r--   0     1001      123      520 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MH.png
+-rw-r--r--   0     1001      123      418 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MK.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ML.png
+-rw-r--r--   0     1001      123      280 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MM.png
+-rw-r--r--   0     1001      123      243 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MN.png
+-rw-r--r--   0     1001      123      311 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MO.png
+-rw-r--r--   0     1001      123      450 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MP.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MQ.png
+-rw-r--r--   0     1001      123      266 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MR.png
+-rw-r--r--   0     1001      123      454 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MS.png
+-rw-r--r--   0     1001      123      174 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MT.png
+-rw-r--r--   0     1001      123      132 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MU.png
+-rw-r--r--   0     1001      123      187 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MV.png
+-rw-r--r--   0     1001      123      231 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MW.png
+-rw-r--r--   0     1001      123      247 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MX.png
+-rw-r--r--   0     1001      123      304 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MY.png
+-rw-r--r--   0     1001      123      395 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MZ.png
+-rw-r--r--   0     1001      123      602 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NA.png
+-rw-r--r--   0     1001      123      393 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NC.png
+-rw-r--r--   0     1001      123      152 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NE.png
+-rw-r--r--   0     1001      123      284 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NF.png
+-rw-r--r--   0     1001      123       96 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NG.png
+-rw-r--r--   0     1001      123      193 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NI.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NL.png
+-rw-r--r--   0     1001      123      153 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NO.png
+-rw-r--r--   0     1001      123      646 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NP.png
+-rw-r--r--   0     1001      123      151 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NR.png
+-rw-r--r--   0     1001      123      336 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NU.png
+-rw-r--r--   0     1001      123      376 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NZ.png
+-rw-r--r--   0     1001      123      179 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/OM.png
+-rw-r--r--   0     1001      123      294 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PA.png
+-rw-r--r--   0     1001      123       96 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PE.png
+-rw-r--r--   0     1001      123      294 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PF.png
+-rw-r--r--   0     1001      123      377 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PG.png
+-rw-r--r--   0     1001      123      319 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PH.png
+-rw-r--r--   0     1001      123      295 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PK.png
+-rw-r--r--   0     1001      123       92 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PL.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PM.png
+-rw-r--r--   0     1001      123      556 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PN.png
+-rw-r--r--   0     1001      123      296 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PR.png
+-rw-r--r--   0     1001      123      293 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PS.png
+-rw-r--r--   0     1001      123      354 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PT.png
+-rw-r--r--   0     1001      123      239 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PW.png
+-rw-r--r--   0     1001      123      190 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PY.png
+-rw-r--r--   0     1001      123      104 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/QA.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/RE.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/RO.png
+-rw-r--r--   0     1001      123      398 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/RS.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/RU.png
+-rw-r--r--   0     1001      123      212 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/RW.png
+-rw-r--r--   0     1001      123      334 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SA.png
+-rw-r--r--   0     1001      123      477 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SB.png
+-rw-r--r--   0     1001      123      517 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SC.png
+-rw-r--r--   0     1001      123      222 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SD.png
+-rw-r--r--   0     1001      123      130 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SE.png
+-rw-r--r--   0     1001      123      249 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SG.png
+-rw-r--r--   0     1001      123      490 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SH.png
+-rw-r--r--   0     1001      123      173 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SI.png
+-rw-r--r--   0     1001      123      153 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SJ.png
+-rw-r--r--   0     1001      123      326 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SK.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SL.png
+-rw-r--r--   0     1001      123      362 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SM.png
+-rw-r--r--   0     1001      123      158 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SN.png
+-rw-r--r--   0     1001      123      198 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SO.png
+-rw-r--r--   0     1001      123      215 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SR.png
+-rw-r--r--   0     1001      123      264 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SS.png
+-rw-r--r--   0     1001      123      254 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ST.png
+-rw-r--r--   0     1001      123      195 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SV.png
+-rw-r--r--   0     1001      123      419 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SX.png
+-rw-r--r--   0     1001      123      182 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SY.png
+-rw-r--r--   0     1001      123      436 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SZ.png
+-rw-r--r--   0     1001      123      414 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TC.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TD.png
+-rw-r--r--   0     1001      123      328 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TF.png
+-rw-r--r--   0     1001      123      248 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TG.png
+-rw-r--r--   0     1001      123      114 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TH.png
+-rw-r--r--   0     1001      123      196 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TJ.png
+-rw-r--r--   0     1001      123      384 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TK.png
+-rw-r--r--   0     1001      123      280 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TL.png
+-rw-r--r--   0     1001      123      486 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TM.png
+-rw-r--r--   0     1001      123      285 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TN.png
+-rw-r--r--   0     1001      123      142 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TO.png
+-rw-r--r--   0     1001      123      263 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TR.png
+-rw-r--r--   0     1001      123      466 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TT.png
+-rw-r--r--   0     1001      123      482 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TV.png
+-rw-r--r--   0     1001      123      235 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TW.png
+-rw-r--r--   0     1001      123      511 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TZ.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/UA.png
+-rw-r--r--   0     1001      123      231 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/UG.png
+-rw-r--r--   0     1001      123      333 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/UM.png
+-rw-r--r--   0     1001      123      333 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/US.png
+-rw-r--r--   0     1001      123      294 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/UY.png
+-rw-r--r--   0     1001      123      213 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/UZ.png
+-rw-r--r--   0     1001      123      282 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VA.png
+-rw-r--r--   0     1001      123      239 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VC.png
+-rw-r--r--   0     1001      123      197 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VE.png
+-rw-r--r--   0     1001      123      471 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VG.png
+-rw-r--r--   0     1001      123      795 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VI.png
+-rw-r--r--   0     1001      123      205 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VN.png
+-rw-r--r--   0     1001      123      427 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VU.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/WF.png
+-rw-r--r--   0     1001      123      182 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/WS.png
+-rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/YE.png
+-rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/YT.png
+-rw-r--r--   0     1001      123      406 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ZA.png
+-rw-r--r--   0     1001      123      225 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ZM.png
+-rw-r--r--   0     1001      123      295 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ZW.png
+-rw-r--r--   0     1001      123    79321 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/GICS Map 2023.xlsx
+-rw-r--r--   0     1001      123   509696 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/ISO10383_MIC.csv
+-rw-r--r--   0     1001      123      402 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/flags_to_strings.py
+-rw-r--r--   0     1001      123   149847 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/iso10383_generated.rs
+-rw-r--r--   0     1001      123     4968 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/process_mics.py
+-rw-r--r--   0     1001      123      577 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/scrape_flags.py
+-rw-r--r--   0     1001      123     1526 2023-06-15 20:52:19.000000 finance_enums-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      123    52004 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/country/mod.rs
+-rw-r--r--   0     1001      123    23116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/currency/mod.rs
+-rw-r--r--   0     1001      123     4020 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/exchange/mod.rs
+-rw-r--r--   0     1001      123        0 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/instrument/mod.rs
+-rw-r--r--   0     1001      123     1302 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123    12919 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/sector/industry.rs
+-rw-r--r--   0     1001      123     6439 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/sector/industry_group.rs
+-rw-r--r--   0     1001      123      190 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/sector/mod.rs
+-rw-r--r--   0     1001      123     3215 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/sector/sector.rs
+-rw-r--r--   0     1001      123    27863 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/sector/subindustry.rs
+-rw-r--r--   0     1001      123     2013 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/bond.rs
+-rw-r--r--   0     1001      123     2113 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/commodity.rs
+-rw-r--r--   0     1001      123        0 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/currency.rs
+-rw-r--r--   0     1001      123     2392 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/equity.rs
+-rw-r--r--   0     1001      123     5893 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/fund.rs
+-rw-r--r--   0     1001      123      259 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/mod.rs
+-rw-r--r--   0     1001      123     3948 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/option.rs
+-rw-r--r--   0     1001      123     3290 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/security.rs
+-rw-r--r--   0     1001      123     7342 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/trading/mod.rs
+-rw-r--r--   0     1001      123    17385 2023-06-15 20:52:54.000000 finance_enums-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     2720 1970-01-01 00:00:00.000000 finance_enums-0.2.2/PKG-INFO
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/Cargo.toml` & `finance_enums-0.2.2/local_dependencies/finance_enums/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "finance_enums"
-version = "0.2.1"
+version = "0.2.2"
 authors = ["timkpaine <t.paine154@gmail.com>"]
 edition = "2021"
 license = "Apache-2.0"
 readme = "../README.md"
 repository = "https://github.com/timkpaine/finance-enums"
 description = "Standard Financial Enumerations"
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/Makefile` & `finance_enums-0.2.2/local_dependencies/finance_enums/Makefile`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/src/country/iso3166.rs` & `finance_enums-0.2.2/local_dependencies/finance_enums/src/country/iso3166.rs`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,17 @@
     WF,
     EH,
     YE,
     ZM,
     ZW,
 }
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "UPPERCASE")]
 pub enum CountryCode3 {
     AFG,
     ALA,
     ALB,
     DZA,
     ASM,
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/src/currency/iso4217.rs` & `finance_enums-0.2.2/local_dependencies/finance_enums/src/currency/iso4217.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 // https://en.wikipedia.org/wiki/ISO_4217
 use crate::CountryCode;
 use serde::{Deserialize, Serialize};
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "UPPERCASE")]
 pub enum Currency {
     AED,
     AFN,
     ALL,
     AMD,
     ANG,
@@ -49,17 +51,19 @@
     DKK,
     DOP,
     DZD,
     EGP,
     ERN,
     ETB,
     EUR,
+    EUX, // NOTE: non ISO 4217
     FJD,
     FKP,
     GBP,
+    GBX, // NOTE: non ISO 4217
     GEL,
     GHS,
     GIP,
     GMD,
     GNF,
     GTQ,
     GYD,
@@ -150,14 +154,15 @@
     TRY,
     TTD,
     TWD,
     TZS,
     UAH,
     UGX,
     USD,
+    USX, // NOTE: non ISO 4217
     USN,
     UYI,
     UYU,
     UYW,
     UZS,
     VED,
     VES,
@@ -234,17 +239,19 @@
             Currency::DKK => "Danish krone",
             Currency::DOP => "Dominican peso",
             Currency::DZD => "Algerian dinar",
             Currency::EGP => "Egyptian pound",
             Currency::ERN => "Eritrean nakfa",
             Currency::ETB => "Ethiopian birr",
             Currency::EUR => "Euro",
+            Currency::EUX => "Euro (cents)",
             Currency::FJD => "Fiji dollar",
             Currency::FKP => "Falkland Islands pound",
             Currency::GBP => "Pound sterling",
+            Currency::GBX => "Penny sterling",
             Currency::GEL => "Georgian lari",
             Currency::GHS => "Ghanaian cedi",
             Currency::GIP => "Gibraltar pound",
             Currency::GMD => "Gambian dalasi",
             Currency::GNF => "Guinean franc",
             Currency::GTQ => "Guatemalan quetzal",
             Currency::GYD => "Guyanese dollar",
@@ -335,14 +342,15 @@
             Currency::TRY => "Turkish lira",
             Currency::TTD => "Trinidad and Tobago dollar",
             Currency::TWD => "New Taiwan dollar",
             Currency::TZS => "Tanzanian shilling",
             Currency::UAH => "Ukrainian hryvnia",
             Currency::UGX => "Ugandan shilling",
             Currency::USD => "United States dollar",
+            Currency::USX => "United States penny",
             Currency::USN => "United States dollar",
             Currency::UYI => "Uruguay Peso en Unidades Indexadas",
             Currency::UYU => "Uruguayan peso",
             Currency::UYW => "Unidad previsional",
             Currency::UZS => "Uzbekistan sum",
             Currency::VED => "Venezuelan digital bolívar",
             Currency::VES => "Venezuelan sovereign bolívar",
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/src/exchange/iso10383.rs` & `finance_enums-0.2.2/local_dependencies/finance_enums/src/exchange/iso10383.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 use crate::CountryCode;
 use serde::{Deserialize, Serialize};
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
 pub enum MIC {
     // NYSE
     XNYS,
     ARCX,
     XASE,
     XCIS,
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/src/sector/industry.rs` & `finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/industry.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 use super::{IndustryGroup, SubIndustry};
 use serde::{Deserialize, Serialize};
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
 pub enum Industry {
     // Energy
     EnergyEquipmentAndServices,
     OilGasAndConsumeableFules,
     // Materials,
     Chemicals,
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/src/sector/industry_group.rs` & `finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/industry_group.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 use super::{Industry, Sector};
 use serde::{Deserialize, Serialize};
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
 pub enum IndustryGroup {
     // Energy
     Energy,
     // Materials
     Materials,
     // Industrials
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/src/sector/sector.rs` & `finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/sector.rs`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 //                     #[strum(serialize=stringify!($field_name), serialize=stringify!(lower!($field_name)), serialize=stringify!(snake!($field_name)), serialize=stringify!(shouty!($field_name)))]
 //                     $field_name,
 //                 )*
 //             }
 //     }
 // }
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
 pub enum Sector {
     Energy,
     Materials,
     Industrials,
     ConsumerDiscretionary,
     ConsumerStaples,
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/src/sector/subindustry.rs` & `finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/subindustry.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 use super::Industry;
 use serde::{Deserialize, Serialize};
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
 pub enum SubIndustry {
     // Energy -> Energy Equipment and Services
     OilAndGasDrilling,
     OilAndGasEquipmentAndServices,
     // Energy -> Oil, Gas, and Consumeable Fuels
     IntegratedOilAndGas,
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/src/security/commodity.rs` & `finance_enums-0.2.2/local_dependencies/finance_enums/src/security/commodity.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 use serde::{Deserialize, Serialize};
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
 pub enum CommodityType {
     Energy,
     Metals,
     Agriculture,
 }
 
 // TODO
-// #[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+// #[derive(Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
 // #[strum(serialize_all = "PascalCase")]
 // pub enum CommoditySubType {
 //     EnergyType(Energy),
 //     MetalType(Metals),
 //     AgricultureType(Agriculture),
 // }
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
 pub enum Energy {
     Crude,
     WTICrude,
     BrentCrude,
     NaturalGas,
 }
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
 pub enum Metals {
     Gold,
     Silver,
     Copper,
     Platinum,
     Palladium,
 }
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
 pub enum Agriculture {
     Corn,
     Wheat,
     Oats,
     Soybean,
     Cocoa,
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/src/security/fund.rs` & `finance_enums-0.2.2/local_dependencies/finance_enums/src/trading/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 use serde::{Deserialize, Serialize};
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
-pub enum FundType {
-    ETF,
-    MutualFund,
-    REIT,
+pub enum OrderType {
+    Market,
+    Limit,
+    Stop,
 }
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
-pub enum FundSubType {
-    Index,
-    Sector,
-    Active,
-    Passive,
+pub enum Side {
+    Buy,
+    Sell,
 }
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
-pub enum MutualFundEndedness {
-    Open,
-    Close,
+pub enum TimeInForce {
+    Day,
+    GTC,
+}
+
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
+#[strum(serialize_all = "PascalCase")]
+pub enum OrderFlag {
+    None,
+    FillOrKill,
+    ImmediateOrCancel,
+    AllOrNone,
 }
```

### Comparing `finance_enums-0.2.1/local_dependencies/finance_enums/src/trading/mod.rs` & `finance_enums-0.2.2/local_dependencies/finance_enums/src/security/fund.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 use serde::{Deserialize, Serialize};
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
-pub enum OrderType {
-    Market,
-    Limit,
-    Stop,
+pub enum FundType {
+    ETF,
+    MutualFund,
+    REIT,
 }
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
-pub enum Side {
-    Buy,
-    Sell,
+pub enum FundSubType {
+    Index,
+    Sector,
+    Active,
+    Passive,
 }
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
 #[strum(serialize_all = "PascalCase")]
-pub enum TimeInForce {
-    Day,
-    GTC,
-}
-
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
-#[strum(serialize_all = "PascalCase")]
-pub enum OrderFlag {
-    None,
-    FillOrKill,
-    ImmediateOrCancel,
-    AllOrNone,
+pub enum MutualFundEndedness {
+    Open,
+    Close,
 }
```

### Comparing `finance_enums-0.2.1/Cargo.toml` & `finance_enums-0.2.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/.github/CODE_OF_CONDUCT.md` & `finance_enums-0.2.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `finance_enums-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `finance_enums-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/.github/workflows/build.yml` & `finance_enums-0.2.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/.github/workflows/publish.yml` & `finance_enums-0.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/.gitignore` & `finance_enums-0.2.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
+_skbuild
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
```

### Comparing `finance_enums-0.2.1/LICENSE` & `finance_enums-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/Makefile` & `finance_enums-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/README.md` & `finance_enums-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/finance_enums/tests/test_security.py` & `finance_enums-0.2.2/finance_enums/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/AF.png` & `finance_enums-0.2.2/flags/AF.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/BN.png` & `finance_enums-0.2.2/flags/BN.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/BT.png` & `finance_enums-0.2.2/flags/BT.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/GS.png` & `finance_enums-0.2.2/flags/GS.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/IO.png` & `finance_enums-0.2.2/flags/IO.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/KI.png` & `finance_enums-0.2.2/flags/KI.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/KN.png` & `finance_enums-0.2.2/flags/KN.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/MH.png` & `finance_enums-0.2.2/flags/MH.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/NA.png` & `finance_enums-0.2.2/flags/NA.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/NP.png` & `finance_enums-0.2.2/flags/NP.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/PN.png` & `finance_enums-0.2.2/flags/PN.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/SC.png` & `finance_enums-0.2.2/flags/SC.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/flags/VI.png` & `finance_enums-0.2.2/flags/VI.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/helpers/GICS Map 2023.xlsx` & `finance_enums-0.2.2/helpers/GICS Map 2023.xlsx`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/helpers/ISO10383_MIC.csv` & `finance_enums-0.2.2/helpers/ISO10383_MIC.csv`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/helpers/iso10383_generated.rs` & `finance_enums-0.2.2/helpers/iso10383_generated.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 use super::CountryCode;
 use serde::{Deserialize, Serialize};
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
 #[strum(serialize_all = "PascalCase")]
 pub enum MIC {
 	DRSP,
 	XCNQ,
 	ZODM,
 	NORX,
 	POSE,
```

### Comparing `finance_enums-0.2.1/helpers/process_mics.py` & `finance_enums-0.2.2/helpers/process_mics.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     mic_to_country[record["MIC"]] = record["ISO COUNTRY CODE (ISO 3166)"]
     mic_to_lei[record["MIC"]] = record["LEI"]
 
 to_writeout = """
 use super::CountryCode;
 use serde::{Deserialize, Serialize};
 
-#[derive(Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
+#[derive(Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize)]
 #[strum(serialize_all = "PascalCase")]
 pub enum MIC {
 """
 
 for key in mic_to_operating:
     to_writeout += f"\t{key},\n"
```

### Comparing `finance_enums-0.2.1/helpers/scrape_flags.py` & `finance_enums-0.2.2/helpers/scrape_flags.py`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/pyproject.toml` & `finance_enums-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["maturin>=1,<2"]
 build-backend = "maturin"
 
 [project]
 name = "finance-enums"
 authors = [{name = "Tim Paine", email = "t.paine154@gmail.com"}]
 description="Standard Financial Enumerations"
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `finance_enums-0.2.1/src/country/mod.rs` & `finance_enums-0.2.2/src/country/mod.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+#![allow(non_snake_case)]
+
 use pyo3::prelude::*;
+use pyo3::class::basic::CompareOp;
 use pyo3::types::PyType;
 use strum::IntoEnumIterator;
 use std::str::FromStr;
 
 use finance_enums::{CountryCode, CountryCode3};
 
 #[pyclass]
@@ -32,16 +35,23 @@
         Ok(format!("{}", self.name))
     }
 
     fn __repr__(&self) -> PyResult<String>   {
         Ok(format!("Country<{}>", self.code.to_string()))
     }
 
-    fn __eq__(&self, other: &Self) -> bool   {
-        self.code == other.code
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Lt => Ok(self.code.to_string() < other.code.to_string()),
+            CompareOp::Le => Ok(self.code.to_string() <= other.code.to_string()),
+            CompareOp::Eq => Ok(self.code == other.code),
+            CompareOp::Ne => Ok(self.code != other.code),
+            CompareOp::Gt => Ok(self.code.to_string() > other.code.to_string()),
+            CompareOp::Ge => Ok(self.code.to_string() >= other.code.to_string()),
+        }
     }
 
     #[getter]
     fn code(&self) -> PyResult<String> {
         Ok(self.code.to_string())
     }
     
@@ -69,2247 +79,1998 @@
     // is way too complicated in pyo3 rn
     #[staticmethod]
     fn members() -> Vec<Country> {
         CountryCode::iter().map(|item: CountryCode| Country{code: item, code3: item.codethree(), name: item.str()} ).collect()
     }
 
     #[classattr]
-    #[allow(non_snake_case)]
     fn AF() -> Country {
         Country {
             code: CountryCode::AF,
             code3: CountryCode::AF.codethree(),
             name: CountryCode::AF.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AX() -> Country {
         Country {
             code: CountryCode::AX,
             code3: CountryCode::AX.codethree(),
             name: CountryCode::AX.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AL() -> Country {
         Country {
             code: CountryCode::AL,
             code3: CountryCode::AL.codethree(),
             name: CountryCode::AL.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn DZ() -> Country {
         Country {
             code: CountryCode::DZ,
             code3: CountryCode::DZ.codethree(),
             name: CountryCode::DZ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AS() -> Country {
         Country {
             code: CountryCode::AS,
             code3: CountryCode::AS.codethree(),
             name: CountryCode::AS.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AD() -> Country {
         Country {
             code: CountryCode::AD,
             code3: CountryCode::AD.codethree(),
             name: CountryCode::AD.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AO() -> Country {
         Country {
             code: CountryCode::AO,
             code3: CountryCode::AO.codethree(),
             name: CountryCode::AO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AI() -> Country {
         Country {
             code: CountryCode::AI,
             code3: CountryCode::AI.codethree(),
             name: CountryCode::AI.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AQ() -> Country {
         Country {
             code: CountryCode::AQ,
             code3: CountryCode::AQ.codethree(),
             name: CountryCode::AQ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AG() -> Country {
         Country {
             code: CountryCode::AG,
             code3: CountryCode::AG.codethree(),
             name: CountryCode::AG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AR() -> Country {
         Country {
             code: CountryCode::AR,
             code3: CountryCode::AR.codethree(),
             name: CountryCode::AR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AM() -> Country {
         Country {
             code: CountryCode::AM,
             code3: CountryCode::AM.codethree(),
             name: CountryCode::AM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AW() -> Country {
         Country {
             code: CountryCode::AW,
             code3: CountryCode::AW.codethree(),
             name: CountryCode::AW.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AU() -> Country {
         Country {
             code: CountryCode::AU,
             code3: CountryCode::AU.codethree(),
             name: CountryCode::AU.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AT() -> Country {
         Country {
             code: CountryCode::AT,
             code3: CountryCode::AT.codethree(),
             name: CountryCode::AT.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AZ() -> Country {
         Country {
             code: CountryCode::AZ,
             code3: CountryCode::AZ.codethree(),
             name: CountryCode::AZ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BS() -> Country {
         Country {
             code: CountryCode::BS,
             code3: CountryCode::BS.codethree(),
             name: CountryCode::BS.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BH() -> Country {
         Country {
             code: CountryCode::BH,
             code3: CountryCode::BH.codethree(),
             name: CountryCode::BH.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BD() -> Country {
         Country {
             code: CountryCode::BD,
             code3: CountryCode::BD.codethree(),
             name: CountryCode::BD.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BB() -> Country {
         Country {
             code: CountryCode::BB,
             code3: CountryCode::BB.codethree(),
             name: CountryCode::BB.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BY() -> Country {
         Country {
             code: CountryCode::BY,
             code3: CountryCode::BY.codethree(),
             name: CountryCode::BY.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BE() -> Country {
         Country {
             code: CountryCode::BE,
             code3: CountryCode::BE.codethree(),
             name: CountryCode::BE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BZ() -> Country {
         Country {
             code: CountryCode::BZ,
             code3: CountryCode::BZ.codethree(),
             name: CountryCode::BZ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BJ() -> Country {
         Country {
             code: CountryCode::BJ,
             code3: CountryCode::BJ.codethree(),
             name: CountryCode::BJ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BM() -> Country {
         Country {
             code: CountryCode::BM,
             code3: CountryCode::BM.codethree(),
             name: CountryCode::BM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BT() -> Country {
         Country {
             code: CountryCode::BT,
             code3: CountryCode::BT.codethree(),
             name: CountryCode::BT.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BO() -> Country {
         Country {
             code: CountryCode::BO,
             code3: CountryCode::BO.codethree(),
             name: CountryCode::BO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BQ() -> Country {
         Country {
             code: CountryCode::BQ,
             code3: CountryCode::BQ.codethree(),
             name: CountryCode::BQ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BA() -> Country {
         Country {
             code: CountryCode::BA,
             code3: CountryCode::BA.codethree(),
             name: CountryCode::BA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BW() -> Country {
         Country {
             code: CountryCode::BW,
             code3: CountryCode::BW.codethree(),
             name: CountryCode::BW.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BV() -> Country {
         Country {
             code: CountryCode::BV,
             code3: CountryCode::BV.codethree(),
             name: CountryCode::BV.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BR() -> Country {
         Country {
             code: CountryCode::BR,
             code3: CountryCode::BR.codethree(),
             name: CountryCode::BR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn IO() -> Country {
         Country {
             code: CountryCode::IO,
             code3: CountryCode::IO.codethree(),
             name: CountryCode::IO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BN() -> Country {
         Country {
             code: CountryCode::BN,
             code3: CountryCode::BN.codethree(),
             name: CountryCode::BN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BG() -> Country {
         Country {
             code: CountryCode::BG,
             code3: CountryCode::BG.codethree(),
             name: CountryCode::BG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BF() -> Country {
         Country {
             code: CountryCode::BF,
             code3: CountryCode::BF.codethree(),
             name: CountryCode::BF.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BI() -> Country {
         Country {
             code: CountryCode::BI,
             code3: CountryCode::BI.codethree(),
             name: CountryCode::BI.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CV() -> Country {
         Country {
             code: CountryCode::CV,
             code3: CountryCode::CV.codethree(),
             name: CountryCode::CV.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KH() -> Country {
         Country {
             code: CountryCode::KH,
             code3: CountryCode::KH.codethree(),
             name: CountryCode::KH.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CM() -> Country {
         Country {
             code: CountryCode::CM,
             code3: CountryCode::CM.codethree(),
             name: CountryCode::CM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CA() -> Country {
         Country {
             code: CountryCode::CA,
             code3: CountryCode::CA.codethree(),
             name: CountryCode::CA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KY() -> Country {
         Country {
             code: CountryCode::KY,
             code3: CountryCode::KY.codethree(),
             name: CountryCode::KY.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CF() -> Country {
         Country {
             code: CountryCode::CF,
             code3: CountryCode::CF.codethree(),
             name: CountryCode::CF.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TD() -> Country {
         Country {
             code: CountryCode::TD,
             code3: CountryCode::TD.codethree(),
             name: CountryCode::TD.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CL() -> Country {
         Country {
             code: CountryCode::CL,
             code3: CountryCode::CL.codethree(),
             name: CountryCode::CL.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CN() -> Country {
         Country {
             code: CountryCode::CN,
             code3: CountryCode::CN.codethree(),
             name: CountryCode::CN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CX() -> Country {
         Country {
             code: CountryCode::CX,
             code3: CountryCode::CX.codethree(),
             name: CountryCode::CX.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CC() -> Country {
         Country {
             code: CountryCode::CC,
             code3: CountryCode::CC.codethree(),
             name: CountryCode::CC.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CO() -> Country {
         Country {
             code: CountryCode::CO,
             code3: CountryCode::CO.codethree(),
             name: CountryCode::CO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KM() -> Country {
         Country {
             code: CountryCode::KM,
             code3: CountryCode::KM.codethree(),
             name: CountryCode::KM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CG() -> Country {
         Country {
             code: CountryCode::CG,
             code3: CountryCode::CG.codethree(),
             name: CountryCode::CG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CD() -> Country {
         Country {
             code: CountryCode::CD,
             code3: CountryCode::CD.codethree(),
             name: CountryCode::CD.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CK() -> Country {
         Country {
             code: CountryCode::CK,
             code3: CountryCode::CK.codethree(),
             name: CountryCode::CK.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CR() -> Country {
         Country {
             code: CountryCode::CR,
             code3: CountryCode::CR.codethree(),
             name: CountryCode::CR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CI() -> Country {
         Country {
             code: CountryCode::CI,
             code3: CountryCode::CI.codethree(),
             name: CountryCode::CI.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn HR() -> Country {
         Country {
             code: CountryCode::HR,
             code3: CountryCode::HR.codethree(),
             name: CountryCode::HR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CU() -> Country {
         Country {
             code: CountryCode::CU,
             code3: CountryCode::CU.codethree(),
             name: CountryCode::CU.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CW() -> Country {
         Country {
             code: CountryCode::CW,
             code3: CountryCode::CW.codethree(),
             name: CountryCode::CW.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CY() -> Country {
         Country {
             code: CountryCode::CY,
             code3: CountryCode::CY.codethree(),
             name: CountryCode::CY.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CZ() -> Country {
         Country {
             code: CountryCode::CZ,
             code3: CountryCode::CZ.codethree(),
             name: CountryCode::CZ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn DK() -> Country {
         Country {
             code: CountryCode::DK,
             code3: CountryCode::DK.codethree(),
             name: CountryCode::DK.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn DJ() -> Country {
         Country {
             code: CountryCode::DJ,
             code3: CountryCode::DJ.codethree(),
             name: CountryCode::DJ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn DM() -> Country {
         Country {
             code: CountryCode::DM,
             code3: CountryCode::DM.codethree(),
             name: CountryCode::DM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn DO() -> Country {
         Country {
             code: CountryCode::DO,
             code3: CountryCode::DO.codethree(),
             name: CountryCode::DO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn EC() -> Country {
         Country {
             code: CountryCode::EC,
             code3: CountryCode::EC.codethree(),
             name: CountryCode::EC.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn EG() -> Country {
         Country {
             code: CountryCode::EG,
             code3: CountryCode::EG.codethree(),
             name: CountryCode::EG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SV() -> Country {
         Country {
             code: CountryCode::SV,
             code3: CountryCode::SV.codethree(),
             name: CountryCode::SV.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GQ() -> Country {
         Country {
             code: CountryCode::GQ,
             code3: CountryCode::GQ.codethree(),
             name: CountryCode::GQ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ER() -> Country {
         Country {
             code: CountryCode::ER,
             code3: CountryCode::ER.codethree(),
             name: CountryCode::ER.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn EE() -> Country {
         Country {
             code: CountryCode::EE,
             code3: CountryCode::EE.codethree(),
             name: CountryCode::EE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SZ() -> Country {
         Country {
             code: CountryCode::SZ,
             code3: CountryCode::SZ.codethree(),
             name: CountryCode::SZ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ET() -> Country {
         Country {
             code: CountryCode::ET,
             code3: CountryCode::ET.codethree(),
             name: CountryCode::ET.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn FK() -> Country {
         Country {
             code: CountryCode::FK,
             code3: CountryCode::FK.codethree(),
             name: CountryCode::FK.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn FO() -> Country {
         Country {
             code: CountryCode::FO,
             code3: CountryCode::FO.codethree(),
             name: CountryCode::FO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn FJ() -> Country {
         Country {
             code: CountryCode::FJ,
             code3: CountryCode::FJ.codethree(),
             name: CountryCode::FJ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn FI() -> Country {
         Country {
             code: CountryCode::FI,
             code3: CountryCode::FI.codethree(),
             name: CountryCode::FI.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn FR() -> Country {
         Country {
             code: CountryCode::FR,
             code3: CountryCode::FR.codethree(),
             name: CountryCode::FR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GF() -> Country {
         Country {
             code: CountryCode::GF,
             code3: CountryCode::GF.codethree(),
             name: CountryCode::GF.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PF() -> Country {
         Country {
             code: CountryCode::PF,
             code3: CountryCode::PF.codethree(),
             name: CountryCode::PF.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TF() -> Country {
         Country {
             code: CountryCode::TF,
             code3: CountryCode::TF.codethree(),
             name: CountryCode::TF.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GA() -> Country {
         Country {
             code: CountryCode::GA,
             code3: CountryCode::GA.codethree(),
             name: CountryCode::GA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GM() -> Country {
         Country {
             code: CountryCode::GM,
             code3: CountryCode::GM.codethree(),
             name: CountryCode::GM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GE() -> Country {
         Country {
             code: CountryCode::GE,
             code3: CountryCode::GE.codethree(),
             name: CountryCode::GE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn DE() -> Country {
         Country {
             code: CountryCode::DE,
             code3: CountryCode::DE.codethree(),
             name: CountryCode::DE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GH() -> Country {
         Country {
             code: CountryCode::GH,
             code3: CountryCode::GH.codethree(),
             name: CountryCode::GH.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GI() -> Country {
         Country {
             code: CountryCode::GI,
             code3: CountryCode::GI.codethree(),
             name: CountryCode::GI.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GR() -> Country {
         Country {
             code: CountryCode::GR,
             code3: CountryCode::GR.codethree(),
             name: CountryCode::GR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GL() -> Country {
         Country {
             code: CountryCode::GL,
             code3: CountryCode::GL.codethree(),
             name: CountryCode::GL.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GD() -> Country {
         Country {
             code: CountryCode::GD,
             code3: CountryCode::GD.codethree(),
             name: CountryCode::GD.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GP() -> Country {
         Country {
             code: CountryCode::GP,
             code3: CountryCode::GP.codethree(),
             name: CountryCode::GP.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GU() -> Country {
         Country {
             code: CountryCode::GU,
             code3: CountryCode::GU.codethree(),
             name: CountryCode::GU.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GT() -> Country {
         Country {
             code: CountryCode::GT,
             code3: CountryCode::GT.codethree(),
             name: CountryCode::GT.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GG() -> Country {
         Country {
             code: CountryCode::GG,
             code3: CountryCode::GG.codethree(),
             name: CountryCode::GG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GN() -> Country {
         Country {
             code: CountryCode::GN,
             code3: CountryCode::GN.codethree(),
             name: CountryCode::GN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GW() -> Country {
         Country {
             code: CountryCode::GW,
             code3: CountryCode::GW.codethree(),
             name: CountryCode::GW.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GY() -> Country {
         Country {
             code: CountryCode::GY,
             code3: CountryCode::GY.codethree(),
             name: CountryCode::GY.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn HT() -> Country {
         Country {
             code: CountryCode::HT,
             code3: CountryCode::HT.codethree(),
             name: CountryCode::HT.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn HM() -> Country {
         Country {
             code: CountryCode::HM,
             code3: CountryCode::HM.codethree(),
             name: CountryCode::HM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn VA() -> Country {
         Country {
             code: CountryCode::VA,
             code3: CountryCode::VA.codethree(),
             name: CountryCode::VA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn HN() -> Country {
         Country {
             code: CountryCode::HN,
             code3: CountryCode::HN.codethree(),
             name: CountryCode::HN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn HK() -> Country {
         Country {
             code: CountryCode::HK,
             code3: CountryCode::HK.codethree(),
             name: CountryCode::HK.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn HU() -> Country {
         Country {
             code: CountryCode::HU,
             code3: CountryCode::HU.codethree(),
             name: CountryCode::HU.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn IS() -> Country {
         Country {
             code: CountryCode::IS,
             code3: CountryCode::IS.codethree(),
             name: CountryCode::IS.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn IN() -> Country {
         Country {
             code: CountryCode::IN,
             code3: CountryCode::IN.codethree(),
             name: CountryCode::IN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ID() -> Country {
         Country {
             code: CountryCode::ID,
             code3: CountryCode::ID.codethree(),
             name: CountryCode::ID.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn IR() -> Country {
         Country {
             code: CountryCode::IR,
             code3: CountryCode::IR.codethree(),
             name: CountryCode::IR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn IQ() -> Country {
         Country {
             code: CountryCode::IQ,
             code3: CountryCode::IQ.codethree(),
             name: CountryCode::IQ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn IE() -> Country {
         Country {
             code: CountryCode::IE,
             code3: CountryCode::IE.codethree(),
             name: CountryCode::IE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn IM() -> Country {
         Country {
             code: CountryCode::IM,
             code3: CountryCode::IM.codethree(),
             name: CountryCode::IM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn IL() -> Country {
         Country {
             code: CountryCode::IL,
             code3: CountryCode::IL.codethree(),
             name: CountryCode::IL.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn IT() -> Country {
         Country {
             code: CountryCode::IT,
             code3: CountryCode::IT.codethree(),
             name: CountryCode::IT.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn JM() -> Country {
         Country {
             code: CountryCode::JM,
             code3: CountryCode::JM.codethree(),
             name: CountryCode::JM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn JP() -> Country {
         Country {
             code: CountryCode::JP,
             code3: CountryCode::JP.codethree(),
             name: CountryCode::JP.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn JE() -> Country {
         Country {
             code: CountryCode::JE,
             code3: CountryCode::JE.codethree(),
             name: CountryCode::JE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn JO() -> Country {
         Country {
             code: CountryCode::JO,
             code3: CountryCode::JO.codethree(),
             name: CountryCode::JO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KZ() -> Country {
         Country {
             code: CountryCode::KZ,
             code3: CountryCode::KZ.codethree(),
             name: CountryCode::KZ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KE() -> Country {
         Country {
             code: CountryCode::KE,
             code3: CountryCode::KE.codethree(),
             name: CountryCode::KE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KI() -> Country {
         Country {
             code: CountryCode::KI,
             code3: CountryCode::KI.codethree(),
             name: CountryCode::KI.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KP() -> Country {
         Country {
             code: CountryCode::KP,
             code3: CountryCode::KP.codethree(),
             name: CountryCode::KP.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KR() -> Country {
         Country {
             code: CountryCode::KR,
             code3: CountryCode::KR.codethree(),
             name: CountryCode::KR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KW() -> Country {
         Country {
             code: CountryCode::KW,
             code3: CountryCode::KW.codethree(),
             name: CountryCode::KW.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KG() -> Country {
         Country {
             code: CountryCode::KG,
             code3: CountryCode::KG.codethree(),
             name: CountryCode::KG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LA() -> Country {
         Country {
             code: CountryCode::LA,
             code3: CountryCode::LA.codethree(),
             name: CountryCode::LA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LV() -> Country {
         Country {
             code: CountryCode::LV,
             code3: CountryCode::LV.codethree(),
             name: CountryCode::LV.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LB() -> Country {
         Country {
             code: CountryCode::LB,
             code3: CountryCode::LB.codethree(),
             name: CountryCode::LB.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LS() -> Country {
         Country {
             code: CountryCode::LS,
             code3: CountryCode::LS.codethree(),
             name: CountryCode::LS.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LR() -> Country {
         Country {
             code: CountryCode::LR,
             code3: CountryCode::LR.codethree(),
             name: CountryCode::LR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LY() -> Country {
         Country {
             code: CountryCode::LY,
             code3: CountryCode::LY.codethree(),
             name: CountryCode::LY.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LI() -> Country {
         Country {
             code: CountryCode::LI,
             code3: CountryCode::LI.codethree(),
             name: CountryCode::LI.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LT() -> Country {
         Country {
             code: CountryCode::LT,
             code3: CountryCode::LT.codethree(),
             name: CountryCode::LT.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LU() -> Country {
         Country {
             code: CountryCode::LU,
             code3: CountryCode::LU.codethree(),
             name: CountryCode::LU.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MO() -> Country {
         Country {
             code: CountryCode::MO,
             code3: CountryCode::MO.codethree(),
             name: CountryCode::MO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MG() -> Country {
         Country {
             code: CountryCode::MG,
             code3: CountryCode::MG.codethree(),
             name: CountryCode::MG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MW() -> Country {
         Country {
             code: CountryCode::MW,
             code3: CountryCode::MW.codethree(),
             name: CountryCode::MW.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MY() -> Country {
         Country {
             code: CountryCode::MY,
             code3: CountryCode::MY.codethree(),
             name: CountryCode::MY.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MV() -> Country {
         Country {
             code: CountryCode::MV,
             code3: CountryCode::MV.codethree(),
             name: CountryCode::MV.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ML() -> Country {
         Country {
             code: CountryCode::ML,
             code3: CountryCode::ML.codethree(),
             name: CountryCode::ML.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MT() -> Country {
         Country {
             code: CountryCode::MT,
             code3: CountryCode::MT.codethree(),
             name: CountryCode::MT.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MH() -> Country {
         Country {
             code: CountryCode::MH,
             code3: CountryCode::MH.codethree(),
             name: CountryCode::MH.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MQ() -> Country {
         Country {
             code: CountryCode::MQ,
             code3: CountryCode::MQ.codethree(),
             name: CountryCode::MQ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MR() -> Country {
         Country {
             code: CountryCode::MR,
             code3: CountryCode::MR.codethree(),
             name: CountryCode::MR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MU() -> Country {
         Country {
             code: CountryCode::MU,
             code3: CountryCode::MU.codethree(),
             name: CountryCode::MU.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn YT() -> Country {
         Country {
             code: CountryCode::YT,
             code3: CountryCode::YT.codethree(),
             name: CountryCode::YT.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MX() -> Country {
         Country {
             code: CountryCode::MX,
             code3: CountryCode::MX.codethree(),
             name: CountryCode::MX.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn FM() -> Country {
         Country {
             code: CountryCode::FM,
             code3: CountryCode::FM.codethree(),
             name: CountryCode::FM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MD() -> Country {
         Country {
             code: CountryCode::MD,
             code3: CountryCode::MD.codethree(),
             name: CountryCode::MD.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MC() -> Country {
         Country {
             code: CountryCode::MC,
             code3: CountryCode::MC.codethree(),
             name: CountryCode::MC.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MN() -> Country {
         Country {
             code: CountryCode::MN,
             code3: CountryCode::MN.codethree(),
             name: CountryCode::MN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ME() -> Country {
         Country {
             code: CountryCode::ME,
             code3: CountryCode::ME.codethree(),
             name: CountryCode::ME.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MS() -> Country {
         Country {
             code: CountryCode::MS,
             code3: CountryCode::MS.codethree(),
             name: CountryCode::MS.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MA() -> Country {
         Country {
             code: CountryCode::MA,
             code3: CountryCode::MA.codethree(),
             name: CountryCode::MA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MZ() -> Country {
         Country {
             code: CountryCode::MZ,
             code3: CountryCode::MZ.codethree(),
             name: CountryCode::MZ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MM() -> Country {
         Country {
             code: CountryCode::MM,
             code3: CountryCode::MM.codethree(),
             name: CountryCode::MM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NA() -> Country {
         Country {
             code: CountryCode::NA,
             code3: CountryCode::NA.codethree(),
             name: CountryCode::NA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NR() -> Country {
         Country {
             code: CountryCode::NR,
             code3: CountryCode::NR.codethree(),
             name: CountryCode::NR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NP() -> Country {
         Country {
             code: CountryCode::NP,
             code3: CountryCode::NP.codethree(),
             name: CountryCode::NP.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NL() -> Country {
         Country {
             code: CountryCode::NL,
             code3: CountryCode::NL.codethree(),
             name: CountryCode::NL.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NC() -> Country {
         Country {
             code: CountryCode::NC,
             code3: CountryCode::NC.codethree(),
             name: CountryCode::NC.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NZ() -> Country {
         Country {
             code: CountryCode::NZ,
             code3: CountryCode::NZ.codethree(),
             name: CountryCode::NZ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NI() -> Country {
         Country {
             code: CountryCode::NI,
             code3: CountryCode::NI.codethree(),
             name: CountryCode::NI.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NE() -> Country {
         Country {
             code: CountryCode::NE,
             code3: CountryCode::NE.codethree(),
             name: CountryCode::NE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NG() -> Country {
         Country {
             code: CountryCode::NG,
             code3: CountryCode::NG.codethree(),
             name: CountryCode::NG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NU() -> Country {
         Country {
             code: CountryCode::NU,
             code3: CountryCode::NU.codethree(),
             name: CountryCode::NU.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NF() -> Country {
         Country {
             code: CountryCode::NF,
             code3: CountryCode::NF.codethree(),
             name: CountryCode::NF.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MK() -> Country {
         Country {
             code: CountryCode::MK,
             code3: CountryCode::MK.codethree(),
             name: CountryCode::MK.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MP() -> Country {
         Country {
             code: CountryCode::MP,
             code3: CountryCode::MP.codethree(),
             name: CountryCode::MP.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn NO() -> Country {
         Country {
             code: CountryCode::NO,
             code3: CountryCode::NO.codethree(),
             name: CountryCode::NO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn OM() -> Country {
         Country {
             code: CountryCode::OM,
             code3: CountryCode::OM.codethree(),
             name: CountryCode::OM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PK() -> Country {
         Country {
             code: CountryCode::PK,
             code3: CountryCode::PK.codethree(),
             name: CountryCode::PK.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PW() -> Country {
         Country {
             code: CountryCode::PW,
             code3: CountryCode::PW.codethree(),
             name: CountryCode::PW.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PS() -> Country {
         Country {
             code: CountryCode::PS,
             code3: CountryCode::PS.codethree(),
             name: CountryCode::PS.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PA() -> Country {
         Country {
             code: CountryCode::PA,
             code3: CountryCode::PA.codethree(),
             name: CountryCode::PA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PG() -> Country {
         Country {
             code: CountryCode::PG,
             code3: CountryCode::PG.codethree(),
             name: CountryCode::PG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PY() -> Country {
         Country {
             code: CountryCode::PY,
             code3: CountryCode::PY.codethree(),
             name: CountryCode::PY.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PE() -> Country {
         Country {
             code: CountryCode::PE,
             code3: CountryCode::PE.codethree(),
             name: CountryCode::PE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PH() -> Country {
         Country {
             code: CountryCode::PH,
             code3: CountryCode::PH.codethree(),
             name: CountryCode::PH.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PN() -> Country {
         Country {
             code: CountryCode::PN,
             code3: CountryCode::PN.codethree(),
             name: CountryCode::PN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PL() -> Country {
         Country {
             code: CountryCode::PL,
             code3: CountryCode::PL.codethree(),
             name: CountryCode::PL.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PT() -> Country {
         Country {
             code: CountryCode::PT,
             code3: CountryCode::PT.codethree(),
             name: CountryCode::PT.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PR() -> Country {
         Country {
             code: CountryCode::PR,
             code3: CountryCode::PR.codethree(),
             name: CountryCode::PR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn QA() -> Country {
         Country {
             code: CountryCode::QA,
             code3: CountryCode::QA.codethree(),
             name: CountryCode::QA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn RE() -> Country {
         Country {
             code: CountryCode::RE,
             code3: CountryCode::RE.codethree(),
             name: CountryCode::RE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn RO() -> Country {
         Country {
             code: CountryCode::RO,
             code3: CountryCode::RO.codethree(),
             name: CountryCode::RO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn RU() -> Country {
         Country {
             code: CountryCode::RU,
             code3: CountryCode::RU.codethree(),
             name: CountryCode::RU.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn RW() -> Country {
         Country {
             code: CountryCode::RW,
             code3: CountryCode::RW.codethree(),
             name: CountryCode::RW.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn BL() -> Country {
         Country {
             code: CountryCode::BL,
             code3: CountryCode::BL.codethree(),
             name: CountryCode::BL.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SH() -> Country {
         Country {
             code: CountryCode::SH,
             code3: CountryCode::SH.codethree(),
             name: CountryCode::SH.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn KN() -> Country {
         Country {
             code: CountryCode::KN,
             code3: CountryCode::KN.codethree(),
             name: CountryCode::KN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LC() -> Country {
         Country {
             code: CountryCode::LC,
             code3: CountryCode::LC.codethree(),
             name: CountryCode::LC.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MF() -> Country {
         Country {
             code: CountryCode::MF,
             code3: CountryCode::MF.codethree(),
             name: CountryCode::MF.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PM() -> Country {
         Country {
             code: CountryCode::PM,
             code3: CountryCode::PM.codethree(),
             name: CountryCode::PM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn VC() -> Country {
         Country {
             code: CountryCode::VC,
             code3: CountryCode::VC.codethree(),
             name: CountryCode::VC.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn WS() -> Country {
         Country {
             code: CountryCode::WS,
             code3: CountryCode::WS.codethree(),
             name: CountryCode::WS.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SM() -> Country {
         Country {
             code: CountryCode::SM,
             code3: CountryCode::SM.codethree(),
             name: CountryCode::SM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ST() -> Country {
         Country {
             code: CountryCode::ST,
             code3: CountryCode::ST.codethree(),
             name: CountryCode::ST.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SA() -> Country {
         Country {
             code: CountryCode::SA,
             code3: CountryCode::SA.codethree(),
             name: CountryCode::SA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SN() -> Country {
         Country {
             code: CountryCode::SN,
             code3: CountryCode::SN.codethree(),
             name: CountryCode::SN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn RS() -> Country {
         Country {
             code: CountryCode::RS,
             code3: CountryCode::RS.codethree(),
             name: CountryCode::RS.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SC() -> Country {
         Country {
             code: CountryCode::SC,
             code3: CountryCode::SC.codethree(),
             name: CountryCode::SC.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SL() -> Country {
         Country {
             code: CountryCode::SL,
             code3: CountryCode::SL.codethree(),
             name: CountryCode::SL.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SG() -> Country {
         Country {
             code: CountryCode::SG,
             code3: CountryCode::SG.codethree(),
             name: CountryCode::SG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SX() -> Country {
         Country {
             code: CountryCode::SX,
             code3: CountryCode::SX.codethree(),
             name: CountryCode::SX.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SK() -> Country {
         Country {
             code: CountryCode::SK,
             code3: CountryCode::SK.codethree(),
             name: CountryCode::SK.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SI() -> Country {
         Country {
             code: CountryCode::SI,
             code3: CountryCode::SI.codethree(),
             name: CountryCode::SI.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SB() -> Country {
         Country {
             code: CountryCode::SB,
             code3: CountryCode::SB.codethree(),
             name: CountryCode::SB.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SO() -> Country {
         Country {
             code: CountryCode::SO,
             code3: CountryCode::SO.codethree(),
             name: CountryCode::SO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ZA() -> Country {
         Country {
             code: CountryCode::ZA,
             code3: CountryCode::ZA.codethree(),
             name: CountryCode::ZA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GS() -> Country {
         Country {
             code: CountryCode::GS,
             code3: CountryCode::GS.codethree(),
             name: CountryCode::GS.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SS() -> Country {
         Country {
             code: CountryCode::SS,
             code3: CountryCode::SS.codethree(),
             name: CountryCode::SS.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ES() -> Country {
         Country {
             code: CountryCode::ES,
             code3: CountryCode::ES.codethree(),
             name: CountryCode::ES.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn LK() -> Country {
         Country {
             code: CountryCode::LK,
             code3: CountryCode::LK.codethree(),
             name: CountryCode::LK.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SD() -> Country {
         Country {
             code: CountryCode::SD,
             code3: CountryCode::SD.codethree(),
             name: CountryCode::SD.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SR() -> Country {
         Country {
             code: CountryCode::SR,
             code3: CountryCode::SR.codethree(),
             name: CountryCode::SR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SJ() -> Country {
         Country {
             code: CountryCode::SJ,
             code3: CountryCode::SJ.codethree(),
             name: CountryCode::SJ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SE() -> Country {
         Country {
             code: CountryCode::SE,
             code3: CountryCode::SE.codethree(),
             name: CountryCode::SE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn CH() -> Country {
         Country {
             code: CountryCode::CH,
             code3: CountryCode::CH.codethree(),
             name: CountryCode::CH.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SY() -> Country {
         Country {
             code: CountryCode::SY,
             code3: CountryCode::SY.codethree(),
             name: CountryCode::SY.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TW() -> Country {
         Country {
             code: CountryCode::TW,
             code3: CountryCode::TW.codethree(),
             name: CountryCode::TW.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TJ() -> Country {
         Country {
             code: CountryCode::TJ,
             code3: CountryCode::TJ.codethree(),
             name: CountryCode::TJ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TZ() -> Country {
         Country {
             code: CountryCode::TZ,
             code3: CountryCode::TZ.codethree(),
             name: CountryCode::TZ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TH() -> Country {
         Country {
             code: CountryCode::TH,
             code3: CountryCode::TH.codethree(),
             name: CountryCode::TH.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TL() -> Country {
         Country {
             code: CountryCode::TL,
             code3: CountryCode::TL.codethree(),
             name: CountryCode::TL.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TG() -> Country {
         Country {
             code: CountryCode::TG,
             code3: CountryCode::TG.codethree(),
             name: CountryCode::TG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TK() -> Country {
         Country {
             code: CountryCode::TK,
             code3: CountryCode::TK.codethree(),
             name: CountryCode::TK.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TO() -> Country {
         Country {
             code: CountryCode::TO,
             code3: CountryCode::TO.codethree(),
             name: CountryCode::TO.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TT() -> Country {
         Country {
             code: CountryCode::TT,
             code3: CountryCode::TT.codethree(),
             name: CountryCode::TT.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TN() -> Country {
         Country {
             code: CountryCode::TN,
             code3: CountryCode::TN.codethree(),
             name: CountryCode::TN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TR() -> Country {
         Country {
             code: CountryCode::TR,
             code3: CountryCode::TR.codethree(),
             name: CountryCode::TR.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TM() -> Country {
         Country {
             code: CountryCode::TM,
             code3: CountryCode::TM.codethree(),
             name: CountryCode::TM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TC() -> Country {
         Country {
             code: CountryCode::TC,
             code3: CountryCode::TC.codethree(),
             name: CountryCode::TC.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TV() -> Country {
         Country {
             code: CountryCode::TV,
             code3: CountryCode::TV.codethree(),
             name: CountryCode::TV.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn UG() -> Country {
         Country {
             code: CountryCode::UG,
             code3: CountryCode::UG.codethree(),
             name: CountryCode::UG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn UA() -> Country {
         Country {
             code: CountryCode::UA,
             code3: CountryCode::UA.codethree(),
             name: CountryCode::UA.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AE() -> Country {
         Country {
             code: CountryCode::AE,
             code3: CountryCode::AE.codethree(),
             name: CountryCode::AE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GB() -> Country {
         Country {
             code: CountryCode::GB,
             code3: CountryCode::GB.codethree(),
             name: CountryCode::GB.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn US() -> Country {
         Country {
             code: CountryCode::US,
             code3: CountryCode::US.codethree(),
             name: CountryCode::US.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn UM() -> Country {
         Country {
             code: CountryCode::UM,
             code3: CountryCode::UM.codethree(),
             name: CountryCode::UM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn UY() -> Country {
         Country {
             code: CountryCode::UY,
             code3: CountryCode::UY.codethree(),
             name: CountryCode::UY.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn UZ() -> Country {
         Country {
             code: CountryCode::UZ,
             code3: CountryCode::UZ.codethree(),
             name: CountryCode::UZ.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn VU() -> Country {
         Country {
             code: CountryCode::VU,
             code3: CountryCode::VU.codethree(),
             name: CountryCode::VU.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn VE() -> Country {
         Country {
             code: CountryCode::VE,
             code3: CountryCode::VE.codethree(),
             name: CountryCode::VE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn VN() -> Country {
         Country {
             code: CountryCode::VN,
             code3: CountryCode::VN.codethree(),
             name: CountryCode::VN.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn VG() -> Country {
         Country {
             code: CountryCode::VG,
             code3: CountryCode::VG.codethree(),
             name: CountryCode::VG.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn VI() -> Country {
         Country {
             code: CountryCode::VI,
             code3: CountryCode::VI.codethree(),
             name: CountryCode::VI.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn WF() -> Country {
         Country {
             code: CountryCode::WF,
             code3: CountryCode::WF.codethree(),
             name: CountryCode::WF.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn EH() -> Country {
         Country {
             code: CountryCode::EH,
             code3: CountryCode::EH.codethree(),
             name: CountryCode::EH.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn YE() -> Country {
         Country {
             code: CountryCode::YE,
             code3: CountryCode::YE.codethree(),
             name: CountryCode::YE.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ZM() -> Country {
         Country {
             code: CountryCode::ZM,
             code3: CountryCode::ZM.codethree(),
             name: CountryCode::ZM.str(),
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ZW() -> Country {
         Country {
             code: CountryCode::ZW,
             code3: CountryCode::ZW.codethree(),
             name: CountryCode::ZW.str(),
         }
     }
```

### Comparing `finance_enums-0.2.1/src/lib.rs` & `finance_enums-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.1/src/sector/industry_group.rs` & `finance_enums-0.2.2/src/sector/industry_group.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+#![allow(non_snake_case)]
+
 use pyo3::prelude::*;
+use pyo3::class::basic::CompareOp;
 use pyo3::types::PyType;
 use strum::IntoEnumIterator;
 use std::str::FromStr;
 
 use finance_enums::{IndustryGroup as BaseIndustryGroup};
 use super::{Sector, Industry};
 
@@ -27,17 +30,24 @@
         Ok(format!("{}", self.typ.to_string()))
     }
 
     fn __repr__(&self) -> PyResult<String>   {
         Ok(format!("IndustryGroup<{}>", self.typ.to_string()))
     }
 
-    fn __eq__(&self, other: &Self) -> bool   {
-        self.typ == other.typ
-    }
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Lt => Ok(self.typ.to_string() < other.typ.to_string()),
+            CompareOp::Le => Ok(self.typ.to_string() <= other.typ.to_string()),
+            CompareOp::Eq => Ok(self.typ == other.typ),
+            CompareOp::Ne => Ok(self.typ != other.typ),
+            CompareOp::Gt => Ok(self.typ.to_string() > other.typ.to_string()),
+            CompareOp::Ge => Ok(self.typ.to_string() >= other.typ.to_string()),
+        }
+    }    
 
     fn sector(&self) -> Sector {
         Sector {
             typ: self.typ.sector()
         }
     }
 
@@ -55,197 +65,172 @@
     #[staticmethod]
     fn members() -> Vec<IndustryGroup> {
         BaseIndustryGroup::iter().map(|item: BaseIndustryGroup| IndustryGroup{typ: item} ).collect()
     }
 
     // Energy
     #[classattr]
-    #[allow(non_snake_case)]
     fn Energy() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::Energy
         }
     }
 
     // Materials
     #[classattr]
-    #[allow(non_snake_case)]
     fn Materials() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::Materials
         }
     }
 
     // Industrials
     #[classattr]
-    #[allow(non_snake_case)]
     fn CapitalGoods() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::CapitalGoods
         }
     }
 
     #[classattr]
-    #[allow(non_snake_case)]
     fn CommercialAndProfessionalServices() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::CommercialAndProfessionalServices
         }
     }
 
     #[classattr]
-    #[allow(non_snake_case)]
     fn Transportation() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::Transportation
         }
     }
     
     // Consumer Discretionary
     #[classattr]
-    #[allow(non_snake_case)]
     fn AutomobilesAndComponents() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::AutomobilesAndComponents
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ConsumerDurablesAndApparel() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::ConsumerDurablesAndApparel
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ConsumerServices() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::ConsumerServices
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ConsumerDiscretionaryDistributionAndRetail() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::ConsumerDiscretionaryDistributionAndRetail
         }
     }
     // Consumer Staples
     #[classattr]
-    #[allow(non_snake_case)]
     fn ConsumerStaplesDistributionAndRetail() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::ConsumerStaplesDistributionAndRetail
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn FoodBeverageAndTobacco() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::FoodBeverageAndTobacco
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn HouseholdAndPersonalProducts() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::HouseholdAndPersonalProducts
         }
     }
     // Health Care
     #[classattr]
-    #[allow(non_snake_case)]
     fn HealthCareEquipmentAndServices() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::HealthCareEquipmentAndServices
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn PharmaceuticalsBiotechnologyAndLifeSciences() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::PharmaceuticalsBiotechnologyAndLifeSciences
         }
     }
     // Financials
     #[classattr]
-    #[allow(non_snake_case)]
     fn Banks() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::Banks
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn FinancialServices() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::FinancialServices
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn Insurance() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::Insurance
         }
     }
     // Information Technology
     #[classattr]
-    #[allow(non_snake_case)]
     fn SoftwareAndServices() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::SoftwareAndServices
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn TechnologyHardwareAndEquipment() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::TechnologyHardwareAndEquipment
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn SemiconductorsAndSemiconductorEquipment() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::SemiconductorsAndSemiconductorEquipment
         }
     }
     // Communication Services
     #[classattr]
-    #[allow(non_snake_case)]
     fn TelecommunicationServices() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::TelecommunicationServices
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn MediaAndEntertainment() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::MediaAndEntertainment
         }
     }
     // Utilities
     #[classattr]
-    #[allow(non_snake_case)]
     fn Utilities() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::Utilities
         }
     }
     // Real Estate
     #[classattr]
-    #[allow(non_snake_case)]
     fn EquityRealEstateInvestmentTrusts() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::EquityRealEstateInvestmentTrusts
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn RealEstateManagementAndDevelopment() -> IndustryGroup {
         IndustryGroup {
             typ: BaseIndustryGroup::RealEstateManagementAndDevelopment
         }
     }
 }
```

### Comparing `finance_enums-0.2.1/src/security/bond.rs` & `finance_enums-0.2.2/src/security/bond.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+#![allow(non_snake_case)]
+
 use pyo3::prelude::*;
+use pyo3::class::basic::CompareOp;
 use pyo3::types::PyType;
 use strum::IntoEnumIterator;
 use std::str::FromStr;
 
 use finance_enums::{BondType as BaseBondType};
 
 #[pyclass]
@@ -25,16 +28,23 @@
         Ok(format!("{}", self.typ.to_string()))
     }
     
     fn __repr__(&self) -> PyResult<String>   {
         Ok(format!("BondType<{}>", self.typ.to_string()))
     }
     
-    fn __eq__(&self, other: &Self) -> bool   {
-        self.typ == other.typ
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Lt => Ok(self.typ.to_string() < other.typ.to_string()),
+            CompareOp::Le => Ok(self.typ.to_string() <= other.typ.to_string()),
+            CompareOp::Eq => Ok(self.typ == other.typ),
+            CompareOp::Ne => Ok(self.typ != other.typ),
+            CompareOp::Gt => Ok(self.typ.to_string() > other.typ.to_string()),
+            CompareOp::Ge => Ok(self.typ.to_string() >= other.typ.to_string()),
+        }
     }
     
     #[classmethod]
     fn __len__(_cls: &PyType) -> PyResult<usize> {
         Ok(BaseBondType::iter().count())
     }
     
@@ -42,28 +52,25 @@
     // is way too complicated in pyo3 rn
     #[staticmethod]
     fn members() -> Vec<BondType> {
         BaseBondType::iter().map(|item: BaseBondType| BondType{typ: item} ).collect()
     }
 
     #[classattr]
-    #[allow(non_snake_case)]
     fn Corporate() -> BondType {
         BondType {
             typ: BaseBondType::Corporate
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn Government() -> BondType {
         BondType {
             typ: BaseBondType::Government
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn Municipal() -> BondType {
         BondType {
             typ: BaseBondType::Municipal
         }
     }
 }
```

### Comparing `finance_enums-0.2.1/src/security/commodity.rs` & `finance_enums-0.2.2/src/security/commodity.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+#![allow(non_snake_case)]
+
 use pyo3::prelude::*;
+use pyo3::class::basic::CompareOp;
 use pyo3::types::PyType;
 use strum::IntoEnumIterator;
 use std::str::FromStr;
 
 use finance_enums::{CommodityType as BaseCommodityType};
 
 #[pyclass]
@@ -24,46 +27,50 @@
     fn __str__(&self) -> PyResult<String>   {
         Ok(format!("{}", self.typ.to_string()))
     }
     
     fn __repr__(&self) -> PyResult<String>   {
         Ok(format!("CommodityType<{}>", self.typ.to_string()))
     }
-    
-    fn __eq__(&self, other: &Self) -> bool   {
-        self.typ == other.typ
-    }
+
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Lt => Ok(self.typ.to_string() < other.typ.to_string()),
+            CompareOp::Le => Ok(self.typ.to_string() <= other.typ.to_string()),
+            CompareOp::Eq => Ok(self.typ == other.typ),
+            CompareOp::Ne => Ok(self.typ != other.typ),
+            CompareOp::Gt => Ok(self.typ.to_string() > other.typ.to_string()),
+            CompareOp::Ge => Ok(self.typ.to_string() >= other.typ.to_string()),
+        }
+    }    
     
     #[classmethod]
     fn __len__(_cls: &PyType) -> PyResult<usize> {
         Ok(BaseCommodityType::iter().count())
     }
     
     // TODO figure out how to make a class iterator,
     // is way too complicated in pyo3 rn
     #[staticmethod]
     fn members() -> Vec<CommodityType> {
         BaseCommodityType::iter().map(|item: BaseCommodityType| CommodityType{typ: item} ).collect()
     }
 
     #[classattr]
-    #[allow(non_snake_case)]
     fn Energy() -> CommodityType {
         CommodityType {
             typ: BaseCommodityType::Energy
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn Metals() -> CommodityType {
         CommodityType {
             typ: BaseCommodityType::Metals
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn Agriculture() -> CommodityType {
         CommodityType {
             typ: BaseCommodityType::Agriculture
         }
     }
 }
```

### Comparing `finance_enums-0.2.1/src/trading/mod.rs` & `finance_enums-0.2.2/src/trading/mod.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,17 @@
+#![allow(non_snake_case)]
+
 use pyo3::prelude::*;
+use pyo3::class::basic::CompareOp;
 use pyo3::types::PyType;
 use strum::IntoEnumIterator;
 use std::str::FromStr;
 
 use finance_enums::{OrderType as BaseOrderType, Side as BaseSide, TimeInForce as BaseTimeInForce, OrderFlag as BaseOrderFlag};
 
-// pub enum TimeInForce {
-//     Day,
-//     GTC,
-// }
-
-// pub enum OrderFlag {
-//     None,
-//     FillOrKill,
-//     ImmediateOrCancel,
-//     AllOrNone,
-// }
-
-
 
 #[pyclass]
 pub struct OrderType {
     pub typ: BaseOrderType
 }
 
 #[pymethods]
@@ -38,17 +28,25 @@
     fn __str__(&self) -> PyResult<String>   {
         Ok(format!("{}", self.typ.to_string()))
     }
     
     fn __repr__(&self) -> PyResult<String>   {
         Ok(format!("OrderType<{}>", self.typ.to_string()))
     }
-    
-    fn __eq__(&self, other: &Self) -> bool   {
-        self.typ == other.typ
+
+
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Lt => Ok(self.typ.to_string() < other.typ.to_string()),
+            CompareOp::Le => Ok(self.typ.to_string() <= other.typ.to_string()),
+            CompareOp::Eq => Ok(self.typ == other.typ),
+            CompareOp::Ne => Ok(self.typ != other.typ),
+            CompareOp::Gt => Ok(self.typ.to_string() > other.typ.to_string()),
+            CompareOp::Ge => Ok(self.typ.to_string() >= other.typ.to_string()),
+        }
     }
     
     #[classmethod]
     fn __len__(_cls: &PyType) -> PyResult<usize> {
         Ok(BaseOrderType::iter().count())
     }
     
@@ -56,29 +54,26 @@
     // is way too complicated in pyo3 rn
     #[staticmethod]
     fn members() -> Vec<OrderType> {
         BaseOrderType::iter().map(|item: BaseOrderType| OrderType{typ: item} ).collect()
     }
 
     #[classattr]
-    #[allow(non_snake_case)]
     fn Market() -> OrderType {
         OrderType {
             typ: BaseOrderType::Market
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn Limit() -> OrderType {
         OrderType {
             typ: BaseOrderType::Limit
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn Stop() -> OrderType {
         OrderType {
             typ: BaseOrderType::Stop
         }
     }
 }
 
@@ -103,39 +98,44 @@
         Ok(format!("{}", self.typ.to_string()))
     }
     
     fn __repr__(&self) -> PyResult<String>   {
         Ok(format!("Side<{}>", self.typ.to_string()))
     }
     
-    fn __eq__(&self, other: &Self) -> bool   {
-        self.typ == other.typ
-    }
-    
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Lt => Ok(self.typ.to_string() < other.typ.to_string()),
+            CompareOp::Le => Ok(self.typ.to_string() <= other.typ.to_string()),
+            CompareOp::Eq => Ok(self.typ == other.typ),
+            CompareOp::Ne => Ok(self.typ != other.typ),
+            CompareOp::Gt => Ok(self.typ.to_string() > other.typ.to_string()),
+            CompareOp::Ge => Ok(self.typ.to_string() >= other.typ.to_string()),
+        }
+    }    
+
     #[classmethod]
     fn __len__(_cls: &PyType) -> PyResult<usize> {
         Ok(BaseSide::iter().count())
     }
     
     // TODO figure out how to make a class iterator,
     // is way too complicated in pyo3 rn
     #[staticmethod]
     fn members() -> Vec<Side> {
         BaseSide::iter().map(|item: BaseSide| Side{typ: item} ).collect()
     }
 
     #[classattr]
-    #[allow(non_snake_case)]
     fn Buy() -> Side {
         Side {
             typ: BaseSide::Buy
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn Sell() -> Side {
         Side {
             typ: BaseSide::Sell
         }
     }
 }
 
@@ -160,39 +160,44 @@
         Ok(format!("{}", self.typ.to_string()))
     }
     
     fn __repr__(&self) -> PyResult<String>   {
         Ok(format!("TimeInForce<{}>", self.typ.to_string()))
     }
     
-    fn __eq__(&self, other: &Self) -> bool   {
-        self.typ == other.typ
-    }
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Lt => Ok(self.typ.to_string() < other.typ.to_string()),
+            CompareOp::Le => Ok(self.typ.to_string() <= other.typ.to_string()),
+            CompareOp::Eq => Ok(self.typ == other.typ),
+            CompareOp::Ne => Ok(self.typ != other.typ),
+            CompareOp::Gt => Ok(self.typ.to_string() > other.typ.to_string()),
+            CompareOp::Ge => Ok(self.typ.to_string() >= other.typ.to_string()),
+        }
+    }    
     
     #[classmethod]
     fn __len__(_cls: &PyType) -> PyResult<usize> {
         Ok(BaseTimeInForce::iter().count())
     }
     
     // TODO figure out how to make a class iterator,
     // is way too complicated in pyo3 rn
     #[staticmethod]
     fn members() -> Vec<TimeInForce> {
         BaseTimeInForce::iter().map(|item: BaseTimeInForce| TimeInForce{typ: item} ).collect()
     }
 
     #[classattr]
-    #[allow(non_snake_case)]
     fn Day() -> TimeInForce {
         TimeInForce {
             typ: BaseTimeInForce::Day
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn GTC() -> TimeInForce {
         TimeInForce {
             typ: BaseTimeInForce::GTC
         }
     }
 }
 
@@ -218,16 +223,23 @@
         Ok(format!("{}", self.typ.to_string()))
     }
     
     fn __repr__(&self) -> PyResult<String>   {
         Ok(format!("OrderFlag<{}>", self.typ.to_string()))
     }
     
-    fn __eq__(&self, other: &Self) -> bool   {
-        self.typ == other.typ
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Lt => Ok(self.typ.to_string() < other.typ.to_string()),
+            CompareOp::Le => Ok(self.typ.to_string() <= other.typ.to_string()),
+            CompareOp::Eq => Ok(self.typ == other.typ),
+            CompareOp::Ne => Ok(self.typ != other.typ),
+            CompareOp::Gt => Ok(self.typ.to_string() > other.typ.to_string()),
+            CompareOp::Ge => Ok(self.typ.to_string() >= other.typ.to_string()),
+        }
     }
     
     #[classmethod]
     fn __len__(_cls: &PyType) -> PyResult<usize> {
         Ok(BaseOrderFlag::iter().count())
     }
     
@@ -236,35 +248,31 @@
     #[staticmethod]
     fn members() -> Vec<OrderFlag> {
         BaseOrderFlag::iter().map(|item: BaseOrderFlag| OrderFlag{typ: item} ).collect()
     }
 
 
     #[classattr]
-    #[allow(non_snake_case)]
     fn None() -> OrderFlag {
         OrderFlag {
             typ: BaseOrderFlag::None
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn FillOrKill() -> OrderFlag {
         OrderFlag {
             typ: BaseOrderFlag::FillOrKill
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn ImmediateOrCancel() -> OrderFlag {
         OrderFlag {
             typ: BaseOrderFlag::ImmediateOrCancel
         }
     }
     #[classattr]
-    #[allow(non_snake_case)]
     fn AllOrNone() -> OrderFlag {
         OrderFlag {
             typ: BaseOrderFlag::AllOrNone
         }
     }
 }
```

### Comparing `finance_enums-0.2.1/Cargo.lock` & `finance_enums-0.2.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 dependencies = [
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "finance_enums"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "casey",
  "chrono",
  "num",
  "serde",
  "serde_json",
  "strum",
```

### Comparing `finance_enums-0.2.1/PKG-INFO` & `finance_enums-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finance-enums
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

