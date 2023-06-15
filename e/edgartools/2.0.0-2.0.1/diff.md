# Comparing `tmp/edgartools-2.0.0.tar.gz` & `tmp/edgartools-2.0.1.tar.gz`

## Comparing `edgartools-2.0.0.tar` & `edgartools-2.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/__about__.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/__init__.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/_codes.py
--rw-r--r--   0        0        0    29821 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/_companies.py
--rw-r--r--   0        0        0    60694 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/_filings.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/_gaap.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/_markdown.py
--rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/_party.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/_rich.py
--rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/_xbrl.py
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/_xml.py
--rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/core.py
--rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/effect.py
--rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/financials.py
--rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/form144.py
--rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/forms.py
--rw-r--r--   0        0        0    35794 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/fundreports.py
--rw-r--r--   0        0        0    41031 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/muniadvisors.py
--rw-r--r--   0        0        0    21603 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/offerings.py
--rw-r--r--   0        0        0    27294 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/ownership.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/search.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/shelfofferings.py
--rw-r--r--   0        0        0  1609032 2020-02-02 00:00:00.000000 edgartools-2.0.0/edgar/data/GAAP_Taxonomy_2022.csv
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 edgartools-2.0.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edgartools-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0    19354 2020-02-02 00:00:00.000000 edgartools-2.0.0/README.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 edgartools-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    20144 2020-02-02 00:00:00.000000 edgartools-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/__about__.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/__init__.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_codes.py
+-rw-r--r--   0        0        0    29821 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_companies.py
+-rw-r--r--   0        0        0    61226 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_filings.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_gaap.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_markdown.py
+-rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_party.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_rich.py
+-rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_xbrl.py
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_xml.py
+-rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/core.py
+-rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/effect.py
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/financials.py
+-rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/form144.py
+-rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/forms.py
+-rw-r--r--   0        0        0    35794 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/fundreports.py
+-rw-r--r--   0        0        0    41031 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/muniadvisors.py
+-rw-r--r--   0        0        0    21603 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/offerings.py
+-rw-r--r--   0        0        0    27294 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/ownership.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/search.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/shelfofferings.py
+-rw-r--r--   0        0        0  1609032 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/data/GAAP_Taxonomy_2022.csv
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 edgartools-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edgartools-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0    19354 2020-02-02 00:00:00.000000 edgartools-2.0.1/README.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 edgartools-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    20144 2020-02-02 00:00:00.000000 edgartools-2.0.1/PKG-INFO
```

### Comparing `edgartools-2.0.0/edgar/__init__.py` & `edgartools-2.0.1/edgar/__init__.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/_codes.py` & `edgartools-2.0.1/edgar/_codes.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/_companies.py` & `edgartools-2.0.1/edgar/_companies.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/_filings.py` & `edgartools-2.0.1/edgar/_filings.py`

 * *Files 0% similar despite different names*

```diff
@@ -594,14 +594,23 @@
 
 # Restricted stock sales
 get_restricted_stock_filings = partial(get_filings, form=[144])
 
 # Insider transaction filings
 get_insider_transaction_filings = partial(get_filings, form=[3, 4, 5])
 
+@lru_cache(maxsize=8)
+def _get_cached_filings(year: Years = None,
+                        quarter: Quarters = None,
+                        form: Union[str, List[IntString]] = None,
+                        amendments: bool = True,
+                        filing_date: str = None,
+                        index="form") -> Filings:
+    # Get the filings but cache the result
+    return get_filings(year=year,quarter=quarter,form=form,amendments=amendments,filing_date=filing_date,index=index)
 
 def parse_filing_header(content):
     data = {}
     current_key = None
 
     lines = content.split('\n')
     for line in lines:
@@ -1497,21 +1506,22 @@
     return (data
             .filter(["Seq", "Document", "Description", "Size"])
             .assign(Size=data.Size.apply(display_size))
             .set_index("Seq")
             )
 
 
+@lru_cache(maxsize=16)
 def get_by_accession_number(accession_number: str):
     """Find the filing using the accession number"""
     assert re.match(r"\d{10}-\d{2}-\d{6}", accession_number), \
         f"{accession_number} is not a valid accession number .. should be 10digits-2digits-6digits"
     year = int("19" + accession_number[11:13]) if accession_number[11] == 9 else int("20" + accession_number[11:13])
     for quarter in range(1, 5):
-        filings = get_filings(year=year, quarter=quarter)
+        filings = _get_cached_filings(year=year, quarter=quarter)
         if filings:
             filing = filings.get(accession_number)
             if filing:
                 return filing
 
 
 def form_with_amendments(*forms: str):
```

### Comparing `edgartools-2.0.0/edgar/_gaap.py` & `edgartools-2.0.1/edgar/_gaap.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/_markdown.py` & `edgartools-2.0.1/edgar/_markdown.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/_party.py` & `edgartools-2.0.1/edgar/_party.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/_rich.py` & `edgartools-2.0.1/edgar/_rich.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/_xbrl.py` & `edgartools-2.0.1/edgar/_xbrl.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/_xml.py` & `edgartools-2.0.1/edgar/_xml.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/core.py` & `edgartools-2.0.1/edgar/core.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/effect.py` & `edgartools-2.0.1/edgar/effect.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/financials.py` & `edgartools-2.0.1/edgar/financials.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/form144.py` & `edgartools-2.0.1/edgar/form144.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/forms.py` & `edgartools-2.0.1/edgar/forms.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/fundreports.py` & `edgartools-2.0.1/edgar/fundreports.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/muniadvisors.py` & `edgartools-2.0.1/edgar/muniadvisors.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/offerings.py` & `edgartools-2.0.1/edgar/offerings.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/ownership.py` & `edgartools-2.0.1/edgar/ownership.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/search.py` & `edgartools-2.0.1/edgar/search.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/edgar/data/GAAP_Taxonomy_2022.csv` & `edgartools-2.0.1/edgar/data/GAAP_Taxonomy_2022.csv`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/LICENSE.txt` & `edgartools-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/README.md` & `edgartools-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/pyproject.toml` & `edgartools-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.0/PKG-INFO` & `edgartools-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgartools
-Version: 2.0.0
+Version: 2.0.1
 Summary: One of the nicest looking EDGAR libraries out there
 Project-URL: Documentation, https://dgunning.github.io/edgartools/
 Project-URL: Issues, https://github.com/dgunning/edgartools/issues
 Project-URL: Source, https://github.com/dgunning/edgartools
 Author-email: Dwight Gunning <dgunning@gmail.com>
 License-File: LICENSE.txt
 Keywords: company,edgar,filings,finance,financial,python,reports,sec
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: edgartools Version: 2.0.0 Summary: One of the
+Metadata-Version: 2.1 Name: edgartools Version: 2.0.1 Summary: One of the
 nicest looking EDGAR libraries out there Project-URL: Documentation, https://
 dgunning.github.io/edgartools/ Project-URL: Issues, https://github.com/
 dgunning/edgartools/issues Project-URL: Source, https://github.com/dgunning/
 edgartools Author-email: Dwight Gunning
 gmail.com> License-File: LICENSE.txt Keywords:
 company,edgar,filings,finance,financial,python,reports,sec Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
```

