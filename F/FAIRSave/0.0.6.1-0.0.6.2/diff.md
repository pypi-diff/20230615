# Comparing `tmp/FAIRSave-0.0.6.1-py3-none-any.whl.zip` & `tmp/FAIRSave-0.0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,26 @@
-Zip file size: 38890 bytes, number of entries: 23
+Zip file size: 42059 bytes, number of entries: 24
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-01 12:17 FAIRSave/__init__.py
 -rw-rw-rw-  2.0 fat     9303 b- defN 23-Mar-01 12:17 FAIRSave/configuration.py
 -rw-rw-rw-  2.0 fat     2872 b- defN 23-Mar-01 12:17 FAIRSave/eln_manager.py
 -rw-rw-rw-  2.0 fat     4454 b- defN 23-Jun-11 18:32 FAIRSave/kadi_download.py
--rw-rw-rw-  2.0 fat     4081 b- defN 23-Mar-01 12:17 FAIRSave/kadi_identifier.py
+-rw-rw-rw-  2.0 fat    18530 b- defN 23-Jun-15 10:48 FAIRSave/kadi_identifier.py
+-rw-rw-rw-  2.0 fat     5391 b- defN 23-Jun-15 08:48 FAIRSave/kadi_identifiers.py
 -rw-rw-rw-  2.0 fat     3613 b- defN 23-Mar-01 12:17 FAIRSave/kadi_instances.py
--rw-rw-rw-  2.0 fat     8198 b- defN 23-May-16 11:02 FAIRSave/kadi_json_writer.py
--rw-rw-rw-  2.0 fat    18172 b- defN 23-Jun-12 13:18 FAIRSave/kadi_record.py
+-rw-rw-rw-  2.0 fat     8448 b- defN 23-Jun-14 07:09 FAIRSave/kadi_json_writer.py
+-rw-rw-rw-  2.0 fat    14471 b- defN 23-Jun-15 13:52 FAIRSave/kadi_record.py
 -rw-rw-rw-  2.0 fat    12066 b- defN 23-Jun-12 15:20 FAIRSave/kadi_search.py
 -rw-rw-rw-  2.0 fat     1351 b- defN 23-Mar-01 12:17 FAIRSave/kadi_template.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-01 12:17 FAIRSave/tools/__init__.py
 -rw-rw-rw-  2.0 fat     9443 b- defN 23-Mar-01 12:17 FAIRSave/tools/comparison.py
 -rw-rw-rw-  2.0 fat    16743 b- defN 23-Mar-01 12:17 FAIRSave/tools/difference.py
 -rw-rw-rw-  2.0 fat     6976 b- defN 23-Mar-01 12:17 FAIRSave/tools/json_reader.py
 -rw-rw-rw-  2.0 fat    10754 b- defN 23-Mar-01 12:17 FAIRSave/tools/key.py
 -rw-rw-rw-  2.0 fat     9861 b- defN 23-Mar-01 12:17 FAIRSave/tools/metadata.py
 -rw-rw-rw-  2.0 fat     2536 b- defN 23-Mar-01 12:17 FAIRSave/tools/surftheowl_json.py
 -rw-rw-rw-  2.0 fat     4495 b- defN 23-Mar-01 12:17 FAIRSave/tools/validation.py
--rw-rw-rw-  2.0 fat    11734 b- defN 23-Jun-12 15:22 FAIRSave-0.0.6.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3827 b- defN 23-Jun-12 15:22 FAIRSave-0.0.6.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 15:22 FAIRSave-0.0.6.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-12 15:22 FAIRSave-0.0.6.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1889 b- defN 23-Jun-12 15:22 FAIRSave-0.0.6.1.dist-info/RECORD
-23 files, 142469 bytes uncompressed, 35844 bytes compressed:  74.8%
+-rw-rw-rw-  2.0 fat    11734 b- defN 23-Jun-15 14:09 FAIRSave-0.0.6.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3827 b- defN 23-Jun-15 14:09 FAIRSave-0.0.6.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-15 14:09 FAIRSave-0.0.6.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-15 14:09 FAIRSave-0.0.6.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1975 b- defN 23-Jun-15 14:09 FAIRSave-0.0.6.2.dist-info/RECORD
+24 files, 158944 bytes uncompressed, 38881 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: FAIRSave/kadi_download.py
 Comment: 
 
 Filename: FAIRSave/kadi_identifier.py
 Comment: 
 
+Filename: FAIRSave/kadi_identifiers.py
+Comment: 
+
 Filename: FAIRSave/kadi_instances.py
 Comment: 
 
 Filename: FAIRSave/kadi_json_writer.py
 Comment: 
 
 Filename: FAIRSave/kadi_record.py
@@ -48,23 +51,23 @@
 
 Filename: FAIRSave/tools/surftheowl_json.py
 Comment: 
 
 Filename: FAIRSave/tools/validation.py
 Comment: 
 
-Filename: FAIRSave-0.0.6.1.dist-info/LICENSE
+Filename: FAIRSave-0.0.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: FAIRSave-0.0.6.1.dist-info/METADATA
+Filename: FAIRSave-0.0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: FAIRSave-0.0.6.1.dist-info/WHEEL
+Filename: FAIRSave-0.0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: FAIRSave-0.0.6.1.dist-info/top_level.txt
+Filename: FAIRSave-0.0.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: FAIRSave-0.0.6.1.dist-info/RECORD
+Filename: FAIRSave-0.0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## FAIRSave/kadi_identifier.py

```diff
@@ -1,91 +1,426 @@
 from kadi_apy import KadiManager
-import uuid
 from FAIRSave.kadi_search import search_item_id_kadi
-import math
 import itertools
-from typing import Optional, List
+from typing import Optional, Union
+import os
+from pathlib import Path
+import itertools
+import string
+import requests
 import re
+import math
+
 
+def title_id_identifier_tuples_kadi(instance: str,
+                                        item: str,
+                                        collection_id: Optional[int] = None,
+                                        collection: Optional[str] = None,
+                                        child_collections: Optional[bool] = True,
+                                        visibility: Optional[str] = 'private'):
+    """Outputs a list of tuples with title, id and identifier for records of a collection.
+
+    Args:
+        instance (str): The name of the instance to use in combination with a config file.
+        item (str): Item whose identifiers should be listed
+        collection_id (Optional[int], optional): Id of collection to search in. Defaults to None.
+        collection (Optional[str], optional): Title of colleciton to search in. Defaults to None.
+        child_collections (Optional[bool], optional): Should child collecitons be included? Defaults to True.
+        visibility (Optional[str], optional): Visibility option for records. Defaults to 'private'.
+    """
+    
+    if collection is not None:
+        collection_id = search_item_id_kadi(instance,
+                                            title=collection,
+                                            item='collection')
+        
+    sr = KadiManager(instance).search_resource()
+    search_results = (sr.search_items(  item=item,
+                                        visibility=visibility,
+                                        collection=collection_id,
+                                        child_collections=child_collections,
+                                        per_page=100))
+    pages = search_results.json()['_pagination'].get('total_pages')
+
+    item_tuples = []
+    for page in range(1, pages+1):
+        var = sr.search_items(  item=item,
+                                visibility=visibility,
+                                collection=collection_id,
+                                child_collections=child_collections,
+                                per_page=100,
+                                page=page).json().get('items')
+        if item == "record":
+            item_tuples += [(x['title'], x['id'], x['identifier'][-11:-6]) for x in var]
+        elif item == "collection":
+            item_tuples += [(x['title'], x['id'], x['identifier']) for x in var]
+        
+    item_tuples = sorted(item_tuples, key=lambda x: x[2])
+    
+    item_tuples_string = ''.join(['\t'.join(str(s) for s in item) + '\n' for item in item_tuples])
+    
+    manager = KadiManager(instance)
+    record = manager.record(id=18224)
+    record.upload_string_to_file(item_tuples_string,"Used_identifiers.csv",force=True)
+
+def get_vocpopuli_id(top_level_term: str,
+                    Gitlab_PAT: str,
+                    project_id: Optional[int] = 41732562):
+    """Search in Gitlab for top-level term ID of vocabulary
+
+    Args:
+        top_level_term (str): Top-level-term from VocPopuli.
+        Gitlab_PAT (str): Access token for Gitlab.
+        project_id (Optional[int], optional): Gitlab project id for vocabulary. Defaults to 41732562.
+
+    Returns:
+        str: Local id of top-level term in VocPopuli.
+    """
+    
+    issues_ep = f"projects/{project_id}/issues"
+
+    params = {'private_token': Gitlab_PAT,
+              'scope': 'all',
+              'order_by': 'created_at',
+              'sort': 'desc',
+              'per_page': 100,
+              'search': top_level_term}
+
+    # get all repository issues
+    issues_response = requests.get(f"https://gitlab.com/api/v4/{issues_ep}",
+                                   params=params)
+    issues_dict_list = issues_response.json()
+
+    # handle pagination
+    for page in range(2, 1 + int(issues_response.headers.get('X-Total-Pages', 0))):
+        params['page'] = page
+        next_page = requests.get(f"https://gitlab.com/api/v4/{issues_ep}",
+                                 params=params)
+        issues_dict_list += next_page.json()
+
+    for issue in issues_dict_list:
+        title = issue['title']
+        label = title.split(' | ')[0].split('] ')[1]
+        if top_level_term == label:
+            global_t_id = title.split(' | ')[1]
+            break
+
+    repo_tree_ep = f"projects/{project_id}/repository/tree"
+    params = {'private_token': Gitlab_PAT,
+              'path': 'approved_terms',
+              'per_page': 100,
+              'ref': 'main'}
+
+    repo_files = []
+    repo_files_response = requests.get(f"https://gitlab.com/api/v4/{repo_tree_ep}",
+                                       params=params)
+
+    repo_files += repo_files_response.json()
+
+    # handle pagination
+    if 'rel="next"' in repo_files_response.headers['Link']:
+        more_pages_left = True
+    else:
+        more_pages_left = False
 
-def is_valid_identifier(identifier_to_test: str) -> bool:
-    pattern = "[a-z]{3}-[a-z]{3}-[0-9a-z]{4}-[0-9a-z]{8}-[0-9a-z]{4}-4[0-9a-z]{3}-[89ab][0-9a-z]{3}-[0-9a-z]{12}"
-    prog = re.compile(pattern)
+    while more_pages_left:
+        # get all pagination links
+        pagination_links = (repo_files_response.headers['Link']
+                            .split(', '))
+        # get the link to the next page
+        next_page_link = [x
+                          for x in pagination_links
+                          if 'rel="next"' in x][0]
+        # strip 'rel="next"'
+        next_page_link = next_page_link.split(';')[0]
+        # remove leading < and trailing >
+        next_page_link = next_page_link[1:-1]
+        repo_files_response = requests.get(next_page_link, params=params)
+        repo_files += repo_files_response.json()
+
+        # breaking condition
+        if any([f'{global_t_id}.json' == x['name'] for x in repo_files]):
+            more_pages_left = False
+        elif 'rel="next"' in repo_files_response.headers['Link']:
+            more_pages_left = True
+        else:
+            more_pages_left = False
+
+    file_dict = [x
+                 for x in repo_files
+                 if x['name'] == f'{global_t_id}.json'][0]
+
+    file_path = (file_dict['path']
+                 .replace('approved_terms/', 'approved_terms%2F')
+                 .replace('.json', '%2Ejson'))
+
+    file_ep = f"projects/{project_id}/repository/files/{file_path}/raw"
+    params = {'private_token': Gitlab_PAT,
+              'ref': 'main'}
+    file = requests.get(f"https://gitlab.com/api/v4/{file_ep}",
+                        params=params)
+    metadata = file.json().get('metadata')
+    id_t_local = metadata.get('id_t_local')
+    
+    return id_t_local
+
+def new_identifier_kadi(instance: str,
+                        top_level_term: str,
+                        Gitlab_PAT: str,
+                        project_id: Optional[int] = 41732562):
+    """Creates a new Kadi4Mat record identifier.
+
+    Args:
+        instance (str): The name of the instance to use in combination with a config file.
+        top_level_term (str): Top-level-term from VocPopuli.
+        Gitlab_PAT (str): Access token for Gitlab.
+        project_id (Optional[int], optional): Gitlab project id for vocabulary. Defaults to 41732562.
+
+    Returns:
+        str: Record identifier
+    """
+    
+    # manager = KadiManager(instance)
+    # record = manager.record(id=18224)
+    # file_id = record.get_file_id(file_name="Used_identifiers.csv")
+    # file = Path(os.path.dirname(os.path.abspath(__file__)),"Used_identifiers.csv")
+    # record.download_file(file_id, file)
+    # with open(file, "r") as f:
+    #     string_of_tuples = f.read()
+    
+    # list_of_tuples = []
+    # # Store string of tuples as list of tuples
+    # list_of_strings = string_of_tuples.split('\n')
+    # for string in list_of_strings:
+    #     list_of_tuples.append(tuple(map(str, string.split('\t'))))
+    
+    sr = KadiManager(instance).search_resource()
+    search_results = (sr.search_items(  item='record',
+                                        visibility='private',
+                                        collection=1141,
+                                        child_collections=True,
+                                        per_page=100))
+    pages = search_results.json()['_pagination'].get('total_pages')
+
+    item_tuples = []
+    for page in range(1, pages+1):
+        var = sr.search_items(  item='record',
+                                visibility='private',
+                                collection=1141,
+                                child_collections=True,
+                                per_page=100,
+                                page=page).json().get('items')
+        item_tuples += [(x['title'], x['id'], x['identifier'][-11:-6]) for x in var]
+        
+    item_tuples = sorted(item_tuples, key=lambda x: x[2])
+
+    ## Search for next higher free idenifier
+    list_of_identifiers = [x[2] for x in item_tuples[1:-1]]
+    unused = False
+    identifier = "aaaaa"
+    while unused is False:
+        if identifier in list_of_identifiers:
+            alphabet = ["a", "b", "c", "d", "e", "f", "g", "h",
+                    "i", "j", "k", "l", "m", "n", "o", "p",
+                    "q", "r", "s", "t", "u", "v", "w", "x",
+                    "y", "z"]
+            if identifier[1:5] == "zzzz":
+                identifier = alphabet[alphabet.index(identifier[0])+1] + "aaaa"
+            elif identifier[2:5] == "zzz":
+                identifier = identifier[:1] + alphabet[alphabet.index(identifier[1])+1] + "aaa"
+            elif identifier[3:5] == "zz":
+                identifier = identifier[:2] + alphabet[alphabet.index(identifier[2])+1] + "aa"
+            elif identifier[4] == "z":
+                identifier = identifier[:3] + alphabet[alphabet.index(identifier[3])+1] + "a"
+            else:
+                identifier = identifier[:4] + alphabet[alphabet.index(identifier[4])+1]
+        else:
+            unused = True
+            
+    id_t_local = get_vocpopuli_id(top_level_term,Gitlab_PAT,project_id)
+    kadi_identifier = id_t_local + '-' + identifier + '-kitmt'
+    
+    # Update used identifiers list
+    title_id_identifier_tuples_kadi(instance,'record')
+    
+    return kadi_identifier
+
+def unused_identifiers_kadi(instance: str):
+    manager = KadiManager(instance)
+    record = manager.record(id=18224)
+    file_id = record.get_file_id(file_name="Used_identifiers.csv")
+    file = Path(os.path.dirname(os.path.abspath(__file__)),"Used_identifiers.csv")
+    record.download_file(file_id, file)
+    with open(file, "r") as f:
+        string_of_tuples = f.read()
+    
+    list_of_tuples = []
+    # Store string of tuples as list of tuples
+    list_of_strings = string_of_tuples.split('\n')
+    for string_ in list_of_strings:
+        list_of_tuples.append(tuple(map(str, string_.split('\t'))))
+
+    ## Search for next higher free idenifier
+    list_of_identifiers = [x[2] for x in list_of_tuples[1:-1]]
+    used_identifiers = set(list_of_identifiers)
+
+    all_identifiers = set(''.join(identifier) for identifier in itertools.product(string.ascii_uppercase, repeat=5))
+    available_identifiers = all_identifiers - used_identifiers
+    available_identifiers = sorted(available_identifiers)
+    available_identifiers_string = '\n'.join(available_identifiers)
+    record.upload_string_to_file(available_identifiers_string,"Unused_identifiers.csv",force=True)
+
+def is_valid_identifier_kadi(identifier_to_test):
+    """Checks identifier validation.
+
+    Args:
+        identifier_to_test (str): Identifier that should be validated.
+
+    Returns:
+        bool: Validation of identifier.
+    """
+    regex_pattern = "[a-z0-9]{32}-vp-[a-z0-9]{5}-kitmt"  
+    prog = re.compile(regex_pattern)
     if prog.match(identifier_to_test):
         return True
     else:
         return False
 
+def Kadi_invalid_identifiers(instance, collection=None, collection_id=None):
+    """Returns list of invalid identifiers tuples in Kadi4Mat.
 
-def Kadi_not_UUID_identifiers(*args, **kwargs):
-    import warnings
-    warnings.simplefilter('always', DeprecationWarning)
-    warnings.warn('Warning! "Kadi_not_UUID_identifiers" will be renamed to '
-                  '"get_non_uuid_identifiers_kadi" in a future release!',
-                  DeprecationWarning)
-    return get_non_uuid_identifiers_kadi(*args, **kwargs)
-
-
-def get_non_uuid_identifiers_kadi(instance: str,
-                                  collection_title: Optional[str] = None,
-                                  collection_id: Optional[str] = None) -> List:
-    """This function should find all identifiers that are not UUID."""
-
-    if collection_title is not None:
-        collection_id = search_item_id_kadi(instance=instance,
-                                            title=collection_title,
-                                            item='collection')
+    Args:
+        instance (str): The name of the instance to use in combination with a config file.
+        collection (_type_, optional): Title of colleciton to search in. Defaults to None.
+        collection_id (_type_, optional): ID of colleciton to search in. Defaults to None.
+
+    Returns:
+        List: List of tuples with titles, invalid identifiers and ids.
+    """
+
+    if collection != None:
+        collection_id = search_item_id_kadi(instance, collection, 'collection')
 
     searchresource = KadiManager(instance=instance).search_resource()
-    search_results = searchresource.search_items(item='record',
-                                                 collection=collection_id,
-                                                 per_page=100)
+    search_results = (searchresource.search_items(item='record',collection=collection_id,child_collections=True,visibility="private",per_page =100))
     total_items = search_results.json()['_pagination'].get('total_items')
     per_page = search_results.json()['_pagination'].get('per_page')
-
+    
     tuples = []
     for n in range(math.ceil(total_items / per_page)):
-        var = searchresource.search_items(item='record',
-                                          collection=collection_id,
-                                          per_page=100,
-                                          page=n+1).json().get('items')
-        identifier_id_tuple = [(x['title'], x['identifier'], x['id'])
-                               for x in var
-                               if not is_valid_identifier(x['identifier'])]
+        var = searchresource.search_items(item='record',collection=collection_id,per_page =100,child_collections=True,visibility="private", page=n+1).json().get('items')
+        identifier_id_tuple = [(x['title'], x['identifier'], x['id']) for x in var if not is_valid_identifier_kadi(x['identifier'])]
         tuples.append(identifier_id_tuple)
 
     list_of_tuples = list(itertools.chain.from_iterable(tuples))
-
     return list_of_tuples
 
+def Kadi_replace_invalid_identifier(instance: str, Gitlab_PAT: str, collection: Union[int, str] = 1141):
+    """Replaces all invalid identifiers in collection
 
-def Kadi_replace_identifier_with_UUID(*args, **kwargs):
-    import warnings
-    warnings.simplefilter('always', DeprecationWarning)
-    warnings.warn('Warning! "Kadi_replace_identifier_with_UUID" will be renamed to '
-                  '"replace_identifier_uuid_kadi" in a future release!',
-                  DeprecationWarning)
-    return replace_identifier_uuid_kadi(*args, **kwargs)
-
-
-def replace_identifier_uuid_kadi(instance: str,
-                                 collection_title: Optional[str] = None,
-                                 collection_id: Optional[str] = None):
-    if collection_title is not None:
-        collection_id = search_item_id_kadi(instance=instance,
-                                            title=collection_title,
-                                            item='collection')
-
-    identifier_id_tuples = get_non_uuid_identifiers_kadi(instance=instance,
-                                                         collection_id=collection_id)
-
+    Args:
+        instance (str):  The name of the instance to use in combination with a config file.
+        Gitlab_PAT (str): Access token for Gitlab.
+        collection (Union[int, str], optional): Title or ID of collection to search in. Defaults to 1141.
+    """
+
+    if type(collection) == str:
+        collection = search_item_id_kadi(instance, collection, 'collection')
+        
+    identifier_id_tuples = Kadi_invalid_identifiers('Malte Flachmann', collection_id=collection)
+    
     for title, identifier, id in identifier_id_tuples:
-        record = KadiManager(instance=instance).record(id=id)
-        identifier_uuid = str(uuid.uuid4())
-
-        # First two words in record title are shortened to 3 chars
-        record_name_words = title.split(' ')[:2]
-        identifier_text = '-'.join((record_name_word[:3]
-                                    for record_name_word in record_name_words))
-        record_number = title[-4:]
-        new_identifier = (identifier_text + '-' + record_number + '-' + identifier_uuid).lower()
-        record.edit(identifier=new_identifier).json()
+        manager = KadiManager(instance)
+        
+        top_level_term = []
+        if 'Tribological Experiment' in title:
+            top_level_term = 'Tribological Experiment'
+        elif 'Data Processing' in title:
+            top_level_term = 'Data Processing'
+        elif 'Data Publication' in title:
+            top_level_term = "Data Publication"
+            pass
+        elif 'Preprocessing' in title:
+            top_level_term = 'Data Processing'
+        elif 'Comparison' in title:
+            top_level_term = 'Data Processing'
+        elif 'Gwyddion' in title:
+            top_level_term = 'Data Processing'
+        elif 'Block Specimen' in title:
+            top_level_term = 'Block Specimen'
+        elif 'Thesis' in title or "Poster" in title:
+            top_level_term = 'Publication'
+        elif 'Band Saw' in title:
+            top_level_term = 'Band Saw'
+        elif 'Wire Saw' in title:
+            top_level_term = 'Wire Saw'
+        elif 'Furnace' in title:
+            top_level_term = 'Furnace'
+        elif 'Heat Treatment' in title:
+            top_level_term = 'Heat Treatment'
+        elif 'Electrolyte' in title:
+            top_level_term = 'Electrolyte'
+        elif 'Optical Surface Profilometer' in title:
+            top_level_term = 'Optical Surface Profilometer'
+        elif 'MATLAB' in title:
+            top_level_term = 'Software'
+        elif 'Scanning Electron Microscope' in title:
+            top_level_term = 'Scanning Electron Microscope'
+        elif 'Light Microscopy' in title:
+            top_level_term = 'Light Microscopy'
+        elif 'Light Microscope' in title:
+            top_level_term = 'Light Microscope'
+        elif 'Electron Microscopy' in title:
+            top_level_term = 'Electron Microscopy'
+        elif 'Optical Surface Profilometry' in title:
+            top_level_term = 'Optical Surface Profilometry'
+        elif 'Tactile Surface Profilometry' in title:
+            top_level_term = 'Tactile Surface Profilometry'
+        elif 'Optical Surface Profilometer' in title:
+            top_level_term = 'Optical Surface Profilometer'
+        elif 'Tactile Surface Profilometer' in title:
+            top_level_term = 'Tactile Surface Profilometer'
+        elif 'Specimen Cleaning' in title:
+            top_level_term = 'Specimen Cleaning'
+        elif 'Hardness Measurement' in title:
+            top_level_term = 'Hardness Measurement'
+        elif 'Demagnitization' in title:
+            top_level_term = 'Demagnitization'
+        elif 'Commercial Machining' in title:
+            top_level_term = 'Commercial Machining'
+        elif 'Electrolyte' in title:
+            top_level_term = 'Electrolyte'
+        elif 'Lubricant for Polishing' in title:
+            top_level_term = 'Lubricant for Polishing'
+        elif 'Polishing Medium' in title:
+            top_level_term = 'Polishing Medium'
+        elif 'Grinding Machine' in title:
+            top_level_term = 'Grinding Machine'
+        elif 'Electropolishing Machine' in title:
+            top_level_term = 'Electropolishing Machine'
+        elif 'Polishing Machine' in title:
+            top_level_term = 'Polishing Machine'
+        elif 'Ultrasonic Cleaner' in title:
+            top_level_term = 'Ultrasonic Cleaner'
+        elif 'Tribometer' in title:
+            top_level_term = 'Tribometer'
+        elif 'Demagnitizing Plate' in title:
+            top_level_term = 'Demagnitizing Plate'
+        elif 'Cup Grinding Machine' in title:
+            top_level_term = 'Cup Grinding Machine'
+        elif 'Metal Sawing' or 'Band Sawing' or 'Wire Sawing' in title:
+            top_level_term = 'Metal Sawing'
+        elif 'Electropolishing' in title:
+            top_level_term = 'Electropolishing'
+        elif 'Polishing' in title:
+            top_level_term = 'Polishing'
+        elif 'Cup Grinding' in title:
+            top_level_term = 'Cup Grinding'
+        elif 'Grinding' in title:
+            top_level_term = 'Grinding'
+
+        if top_level_term != []:
+            print(title, top_level_term)
+
+            identifier = new_identifier_kadi(instance,top_level_term,Gitlab_PAT)
+            print(identifier)
+            print(manager.record(id = id).edit(identifier = identifier))
```

## FAIRSave/kadi_json_writer.py

```diff
@@ -34,16 +34,17 @@
                 dict_for_list['value'].pop(-1)
 
         elif isinstance(value.get(j), dict) and word_in_list('@id', list(value.get(j).keys())):
             dict_for_list['value'].append(create_list_from_list(j,
                                                                 value.get(j)))
 
         elif isinstance(value.get(j), dict):
-            dict_for_list['value'].append(create_list_from_dict(j,
-                                                                value.get(j)))
+            list_from_dict = create_list_from_dict(j,value.get(j))
+            if list_from_dict.get('value') != []:
+                dict_for_list['value'].append(list_from_dict)
 
         elif isinstance(value.get(j), list):
             dict_for_list['value'].append(create_list_from_list(j,
                                                                 value.get(j)))
 
         else:
             if type(value.get(j)).__name__ == 'NoneType':
@@ -80,29 +81,29 @@
     :return: dict_of_element
     :rtype: dict
     """
     if bool(list(attr.keys())) is True:
         if isinstance(ast.literal_eval(value), int):
             if value == '0' and (key == 'Relative_Starting_Position_Setpoint' or key == 'Targeted_Normal_Load'):
                 pass
-            elif attr.get('unit') == "": 
+            elif attr.get('unit') == "" and value == '0': 
                 pass
             else:
                 dict_of_element = {'key': key,
                                    'type': type(ast.literal_eval(value)).__name__, list(attr.keys())[0]: attr.get('unit'),
                                    'value': int(value)}
                 return dict_of_element
         else:
             dict_of_element = {'key': key,
                                'type': type(ast.literal_eval(value)).__name__, list(attr.keys())[0]: attr.get('unit'),
                                'value': float(value)}
 
             return dict_of_element
 
-    elif key == 'Setup_Starting_Time' or key == 'Experiment_Starting_Time' or key == 'Experiment_Ending_Time':
+    elif key == 'Setup_Starting_Time' or key == 'Experiment_Starting_Time' or key == 'Experiment_Ending_Time' or key == 'Time_of_Last_Self_Calibration':
         dict_of_element = {'key': key,
                            'type': 'date',
                            'value': value}
         return dict_of_element
 
     else:
         # Floor and Room need to be str
@@ -147,26 +148,30 @@
             try:
                 k.pop('@id')
             except:
                 pass
             dict_list = []
             for m in k.keys():
                 if type(k.get(m)).__name__ == 'dict' and word_in_list('@unit', list(k.get(m).keys())):
+                    key = m
+                    value = k.get(m).get('#text')
                     attr = {'unit': k.get(m).get('@unit')}
-                    dict_list.append(create_dict_from_element(m, k.get(m).get('#text'), attr))
+                    if attr.get('unit') == "" and value == '0': 
+                        pass
+                    else:
+                        dict_list.append(create_dict_from_element(key, value, attr))
                 elif type(k.get(m)).__name__ == 'dict':
                     try:
                         dict_list.append(create_list_from_dict(m, k.get(m).get('#text')))
                     except:
                         dict_list.append(create_list_from_dict(m, k.get(m)))
                 elif isinstance(k.get(m), list):
                     dict_list.append(create_list_from_list(m, k.get(m)))
                 else:
                     if type(k.get(m)).__name__ == 'NoneType':
-                        print(key)
                         continue
                     else:
                         dict_list.append(create_dict_from_element(m, k.get(m), {}))
             dict_for_list['value'].append({'type': 'dict', 'value': dict_list})
     # List with only one element is not detected as list
     else:
         dict_for_list = {'key': key,
```

## FAIRSave/kadi_record.py

```diff
@@ -5,14 +5,15 @@
 import shutil
 from FAIRSave.kadi_search import search_item_id_kadi
 import requests
 import time
 from typing import Optional, Union, Dict
 import re
 from FAIRSave.kadi_instances import read_operator_config
+from FAIRSave.kadi_identifier import new_identifier_kadi, get_vocpopuli_id
 
 
 def Record_Create(*args, **kwargs):
     import warnings
     warnings.simplefilter('always', DeprecationWarning)
     warnings.warn('Warning! "Record_Create" will be renamed to '
                   '"create_record_kadi" in a future release!',
@@ -34,151 +35,23 @@
         top_level_term: Top Level term of the vocabulary.
         GITLAB_PAT: Personal access token to Gitlab.
 
     Returns:
     tuple: Tuple of id and identifier of newly crated record.
     """
 
-    # Search in Gitlab for top-level term ID of vocabulary
-    issues_ep = f"projects/{project_id}/issues"
-
-    params = {'private_token': Gitlab_PAT,
-              'scope': 'all',
-              'order_by': 'created_at',
-              'sort': 'desc',
-              'per_page': 100,
-              'search': top_level_term}
-
-    # get all repository issues
-    issues_response = requests.get(f"https://gitlab.com/api/v4/{issues_ep}",
-                                   params=params)
-    issues_dict_list = issues_response.json()
-
-    # handle pagination
-    for page in range(2, 1 + int(issues_response.headers.get('X-Total-Pages', 0))):
-        params['page'] = page
-        next_page = requests.get(f"https://gitlab.com/api/v4/{issues_ep}",
-                                 params=params)
-        issues_dict_list += next_page.json()
-
-    for issue in issues_dict_list:
-        title = issue['title']
-        label = title.split(' | ')[0].split('] ')[1]
-        if top_level_term == label:
-            global_t_id = title.split(' | ')[1]
-            break
-
-    repo_tree_ep = f"projects/{project_id}/repository/tree"
-    params = {'private_token': Gitlab_PAT,
-              'path': 'approved_terms',
-              'per_page': 100,
-              'ref': 'main'}
-
-    repo_files = []
-    repo_files_response = requests.get(f"https://gitlab.com/api/v4/{repo_tree_ep}",
-                                       params=params)
-
-    repo_files += repo_files_response.json()
-
-    # handle pagination
-    if 'rel="next"' in repo_files_response.headers['Link']:
-        more_pages_left = True
-    else:
-        more_pages_left = False
-
-    while more_pages_left:
-        # get all pagination links
-        pagination_links = (repo_files_response.headers['Link']
-                            .split(', '))
-        # get the link to the next page
-        next_page_link = [x
-                          for x in pagination_links
-                          if 'rel="next"' in x][0]
-        # strip 'rel="next"'
-        next_page_link = next_page_link.split(';')[0]
-        # remove leading < and trailing >
-        next_page_link = next_page_link[1:-1]
-        repo_files_response = requests.get(next_page_link, params=params)
-        repo_files += repo_files_response.json()
-
-        # breaking condition
-        if any([f'{global_t_id}.json' == x['name'] for x in repo_files]):
-            more_pages_left = False
-        elif 'rel="next"' in repo_files_response.headers['Link']:
-            more_pages_left = True
-        else:
-            more_pages_left = False
-
-    file_dict = [x
-                 for x in repo_files
-                 if x['name'] == f'{global_t_id}.json'][0]
-
-    file_path = (file_dict['path']
-                 .replace('approved_terms/', 'approved_terms%2F')
-                 .replace('.json', '%2Ejson'))
-
-    file_ep = f"projects/{project_id}/repository/files/{file_path}/raw"
-    params = {'private_token': Gitlab_PAT,
-              'ref': 'main'}
-    file = requests.get(f"https://gitlab.com/api/v4/{file_ep}",
-                        params=params)
-    metadata = file.json().get('metadata')
-    id_t_local = metadata.get('id_t_local')
-
     # Access Manager with Configuration Instance
     manager = KadiManager(instance=instance)
 
-    # Create a record for the processed data in Kadi4Mat
-
-    # Basic info for the new record
-    title = record_name
-
-    # Search identifiers in Kadi4Mat to check new identifiers uniqueness
-    search_results = (manager
-                      .search_resource()
-                      .search_items(item='record', per_page=100))
-
-    pages = search_results.json()['_pagination'].get('total_pages')
-
-    identifier_list = []
-    pattern = re.compile("[a-z0-9]{32}-vp-[a-z0-9]{5}-kitmt")
-    for page in range(1, pages+1):
-        results = (manager
-                   .search_resource()
-                   .search_items(item='record', per_page=100, page=page)
-                   .json().get('items'))
-        for record in results:
-            identifier_to_test = record.get('identifier')
-            if pattern.match(identifier_to_test):
-                identifier_list.append(record.get('identifier')[-11:-6])
-    identifier_list.sort()
-    highest_identifier = identifier_list[-1]
-
-    # Create unique_identifier
-    alphabet = ["a", "b", "c", "d", "e", "f", "g", "h",
-                "i", "j", "k", "l", "m", "n", "o", "p",
-                "q", "r", "s", "t", "u", "v", "w", "x",
-                "y", "z"]
-    if highest_identifier[1:5] == "zzzz":
-        unique_identifier = alphabet[alphabet.index(highest_identifier[0])+1] + "aaaa"
-    elif highest_identifier[2:5] == "zzz":
-        unique_identifier = highest_identifier[:1] + alphabet[alphabet.index(highest_identifier[1])+1] + "aaa"
-    elif highest_identifier[3:5] == "zz":
-        unique_identifier = highest_identifier[:2] + alphabet[alphabet.index(highest_identifier[2])+1] + "aa"
-    elif highest_identifier[4] == "z":
-        unique_identifier = highest_identifier[:3] + alphabet[alphabet.index(highest_identifier[3])+1] + "a"
-    else:
-        unique_identifier = highest_identifier[:4] + alphabet[alphabet.index(highest_identifier[4])+1]
-
     # Create identifier from local_id and unique identifier for external applications
-    identifier = id_t_local + '-' + unique_identifier + '-kitmt'
+    identifier = new_identifier_kadi(instance,top_level_term,Gitlab_PAT,project_id)
 
     # This creates a new record if none with the given identifier exists yet.
     # If one exists, but we cannot access it, an exception will be raised.
-    record = manager.record(identifier=identifier, title=title, create=True)
+    record = manager.record(identifier=identifier, title=record_name, create=True)
     return (record.id, identifier)
 
 def Record_Add_Links_and_Edit(*args, **kwargs):
     import warnings
     warnings.simplefilter('always', DeprecationWarning)
     warnings.warn('Warning! "Record_Add_Links_and_Edit" will be renamed to '
                   '"record_add_links_and_edit_kadi" in a future release!',
@@ -407,24 +280,44 @@
     elif file_list is None:
         file_list = os.listdir(files_path)
 
     if files_path is not None:
         # Add metadata from files
         for file in file_list:
             file_id = []
-            file_metadata = {'Array of Produced File Metadata': []}
             if isfile(files_path + '\\' + file):
                 record.upload_file(files_path + '\\' + file, force=True)
                 file_id = record.get_file_id(file)
-                file_MD = {'File(s) Purpose': file_purpose}
-                file_metadata['Array of Produced File Metadata'].append(file_MD)
+                file_info = record.get_file_info(file_id).json()
+                file_size = file_info.get('size')
+                file_name = file_info.get('name')
+                file_MD = {"type": "dict","value":[
+                                {"key": "File Name", "type": "str", "value": file_name},
+                                {"key": "File Persistent ID", "type": "str", "value": file_id},
+                                {"key": "File Size", "type": "float", "unit": "kB", "value": file_size},
+                                {"key": "File(s) Purpose", "type": "str", "value": file_purpose}]}
             elif isdir(files_path + '\\' + file):
                 zip_file = shutil.make_archive(files_path + '/' + file,
                                                'zip',
                                                files_path + '/' + file,
                                                files_path)
                 record.upload_file(zip_file, force=True)
                 file_id = record.get_file_id(file + '.zip')
-                file_MD = {'File(s) Purpose': file_purpose}
-                file_metadata['Array of Produced File Metadata'].append(file_MD)
-
-            record.edit_file(file_id=file_id, description=str(file_metadata))
+                file_info = record.get_file_info(file_id).json()
+                file_size = file_info.get('size')
+                file_name = file_info.get('name')
+                file_MD = {"type": "dict","value":[
+                                {"key": "File Name", "type": "str", "value": file_name},
+                                {"key": "File Persistent ID", "type": "str", "value": file_id},
+                                {"key": "File Size", "type": "float", "unit": "kB", "value": file_size},
+                                {"key": "File(s) Purpose", "type": "str", "value": file_purpose}]}
+
+            record_MD = record.meta.get('extras')
+            if record_MD[-1].get('key') == "Array Produced File Metadata":
+                # record.remove_metadatum("Array Produced File Metadata")
+                file_MD_array = record_MD[-1]
+                file_MD_array['value'].append(file_MD)
+            else:
+                file_metadata = {"key": "Array Produced File Metadata", "type": "list", "value": []}
+                file_metadata['value'].append(file_MD)
+                file_MD_array = file_metadata
+            record.add_metadata(file_MD_array, force=True)
```

## Comparing `FAIRSave-0.0.6.1.dist-info/LICENSE` & `FAIRSave-0.0.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `FAIRSave-0.0.6.1.dist-info/METADATA` & `FAIRSave-0.0.6.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FAIRSave
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: Package to run the FAIR-Save toolbox
 Home-page: UNKNOWN
 Author: Malte Flachmann, Floriane Bresser, Ilia Bagov (Karlsruhe Institute of Technology)
 Author-email: malte.flachmann@student.kit.edu
 License: Apache-2.0
 Project-URL: GitLab, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save_Utilities
 Project-URL: Changelog, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save-Utilities/-/blob/main/Changelog.md
```

## Comparing `FAIRSave-0.0.6.1.dist-info/RECORD` & `FAIRSave-0.0.6.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 FAIRSave/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 FAIRSave/configuration.py,sha256=0ehQ_OkseYMsgKhRsdVUclBOXvt4NH1aiobHvN5ziW8,9303
 FAIRSave/eln_manager.py,sha256=dpo3PAS55a_wXGvemiE0eoNr4FsPmCvspezAio-HcX4,2872
 FAIRSave/kadi_download.py,sha256=PWFSppaWx7PjCW1d5W5G4vnisojNoUnZ0qYxp--l9hw,4454
-FAIRSave/kadi_identifier.py,sha256=3OiylNuqzwY3EQgw0Nfov196DOBt495aCEAZUhYdYfY,4081
+FAIRSave/kadi_identifier.py,sha256=TgeXhNcQfYZKs1GZhPUbHgunLZbVVbqZaSB1qCGaHBo,18530
+FAIRSave/kadi_identifiers.py,sha256=Mn2BdW9-3rUk6TvIQTrM-TFi18d6pYpwOgkmjSw1Aus,5391
 FAIRSave/kadi_instances.py,sha256=Xx0dMqouFFHBp9Yo8W4b5dDeX8iss_faGm9fufkVKyQ,3613
-FAIRSave/kadi_json_writer.py,sha256=2ke4ywZNqFYlLrlX30mPkdqnw5QfM0Bs3DjXqYjNh-w,8198
-FAIRSave/kadi_record.py,sha256=-_b38AQcNPPCU4FM_sRVbmK7d9W4fEfTG6tgYMIUNCc,18172
+FAIRSave/kadi_json_writer.py,sha256=5hFDIhcjotLzGci6LmJmJFan7-k-1DrRJFyyIywTg18,8448
+FAIRSave/kadi_record.py,sha256=69OFZlGaMqJ_h8DO7rE1hN5NDMYCsga20D0bDWEF9uc,14471
 FAIRSave/kadi_search.py,sha256=P47wmL8B47qrq5IPwszxzKl1lNMLkZkKTtqlMFOlK-k,12066
 FAIRSave/kadi_template.py,sha256=m0vC4gxy_-liaAe40xlX3VRjxQJXw6pq4s6FDFDzgyk,1351
 FAIRSave/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 FAIRSave/tools/comparison.py,sha256=gQ76mS9glUf9bcS7kWB0mtSx7lZ7WySTz4zCMmdF6zI,9443
 FAIRSave/tools/difference.py,sha256=Drc0LwvT29WUhzyjUgphfM_nuGIi0Oab0138q1PUFKs,16743
 FAIRSave/tools/json_reader.py,sha256=YnE9_3lToaJxU0aVoYOchBcbQh0RoYvuRgtkuwuXRj0,6976
 FAIRSave/tools/key.py,sha256=kspBVidTf54F_GmUdhh6fPT5G7bLHQpjfI2CoUEc-jk,10754
 FAIRSave/tools/metadata.py,sha256=MBtDeQrfrl_uRUSamR7q1JFPoE8JkPN7_UNSi5qdIGs,9861
 FAIRSave/tools/surftheowl_json.py,sha256=Ie9MGa1mXrxaQxynb9daDhR2LFa4kkf4tZ0Hrdb8AgU,2536
 FAIRSave/tools/validation.py,sha256=pQDKRIaoEylU5hPuI_loncMEYAgzgYbZgpm7u7Doat8,4495
-FAIRSave-0.0.6.1.dist-info/LICENSE,sha256=itGSoY4BUSDO1X36lIFXCBlN8XsDnZRP-qdcfnmKazw,11734
-FAIRSave-0.0.6.1.dist-info/METADATA,sha256=w4yQH-55R1gzPFcSm5TkeTCKtKQnCDQsg0HAJ2Anmnw,3827
-FAIRSave-0.0.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-FAIRSave-0.0.6.1.dist-info/top_level.txt,sha256=BemltgO7SU5GOPMbfMCBkSpXowdROrlrsN46O3nTt6A,9
-FAIRSave-0.0.6.1.dist-info/RECORD,,
+FAIRSave-0.0.6.2.dist-info/LICENSE,sha256=itGSoY4BUSDO1X36lIFXCBlN8XsDnZRP-qdcfnmKazw,11734
+FAIRSave-0.0.6.2.dist-info/METADATA,sha256=hwL3N584tL0YtsqFUXgmnO0FWiRK71Pum5HdApBmBZ0,3827
+FAIRSave-0.0.6.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+FAIRSave-0.0.6.2.dist-info/top_level.txt,sha256=BemltgO7SU5GOPMbfMCBkSpXowdROrlrsN46O3nTt6A,9
+FAIRSave-0.0.6.2.dist-info/RECORD,,
```

