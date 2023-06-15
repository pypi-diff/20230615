# Comparing `tmp/easydock-0.2.0.tar.gz` & `tmp/easydock-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easydock-0.2.0.tar", last modified: Sat May 20 10:07:24 2023, max compression
+gzip compressed data, was "dist/easydock-0.2.1.tar", last modified: Thu Jun 15 18:20:59 2023, max compression
```

## Comparing `easydock-0.2.0.tar` & `easydock-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-20 10:07:24.000000 easydock-0.2.0/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8167 2023-05-20 10:07:24.000000 easydock-0.2.0/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-05-20 10:07:24.000000 easydock-0.2.0/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-20 10:07:24.000000 easydock-0.2.0/easydock/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    21139 2023-05-17 14:24:22.000000 easydock-0.2.0/easydock/preparation_for_docking.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    13440 2023-05-16 09:01:52.000000 easydock-0.2.0/easydock/run_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3382 2023-05-16 09:01:52.000000 easydock-0.2.0/easydock/vina_dock_cli.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7491 2023-05-16 09:01:52.000000 easydock-0.2.0/easydock/read_input.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2023-05-20 10:00:51.000000 easydock-0.2.0/easydock/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5962 2023-05-16 19:41:28.000000 easydock-0.2.0/easydock/get_sdf_from_dock_db.py
--rwxrwxr-x   0 pavel     (1000) pavel     (1000)     5288 2023-05-16 09:01:52.000000 easydock-0.2.0/easydock/vina_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2713 2023-05-16 09:01:52.000000 easydock-0.2.0/easydock/gnina_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6176 2023-05-20 10:02:12.000000 easydock-0.2.0/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-20 10:07:24.000000 easydock-0.2.0/easydock.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8167 2023-05-20 10:07:24.000000 easydock-0.2.0/easydock.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      427 2023-05-20 10:07:24.000000 easydock-0.2.0/easydock.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      111 2023-05-20 10:07:24.000000 easydock-0.2.0/easydock.egg-info/entry_points.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2023-05-20 10:07:24.000000 easydock-0.2.0/easydock.egg-info/top_level.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-05-20 10:07:24.000000 easydock-0.2.0/easydock.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-05-20 10:07:24.000000 easydock-0.2.0/easydock.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1155 2023-05-16 09:01:52.000000 easydock-0.2.0/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-15 18:20:59.000000 easydock-0.2.1/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1516 2019-11-25 13:17:56.000000 easydock-0.2.1/LICENSE.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8857 2023-06-15 18:20:59.000000 easydock-0.2.1/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-06-15 18:20:59.000000 easydock-0.2.1/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-15 18:20:59.000000 easydock-0.2.1/easydock/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    21656 2023-06-15 18:00:36.000000 easydock-0.2.1/easydock/preparation_for_docking.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    13642 2023-06-15 14:29:36.000000 easydock-0.2.1/easydock/run_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3382 2023-05-16 09:01:52.000000 easydock-0.2.1/easydock/vina_dock_cli.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7491 2023-05-16 09:01:52.000000 easydock-0.2.1/easydock/read_input.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2023-06-15 18:16:50.000000 easydock-0.2.1/easydock/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5965 2023-05-30 12:11:29.000000 easydock-0.2.1/easydock/get_sdf_from_dock_db.py
+-rwxrwxr-x   0 pavel     (1000) pavel     (1000)     5288 2023-05-16 09:01:52.000000 easydock-0.2.1/easydock/vina_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2713 2023-05-16 09:01:52.000000 easydock-0.2.1/easydock/gnina_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6802 2023-06-15 18:18:52.000000 easydock-0.2.1/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-15 18:20:59.000000 easydock-0.2.1/easydock.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8857 2023-06-15 18:20:59.000000 easydock-0.2.1/easydock.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      439 2023-06-15 18:20:59.000000 easydock-0.2.1/easydock.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      111 2023-06-15 18:20:59.000000 easydock-0.2.1/easydock.egg-info/entry_points.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2023-06-15 18:20:59.000000 easydock-0.2.1/easydock.egg-info/top_level.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-06-15 18:20:59.000000 easydock-0.2.1/easydock.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-06-15 18:20:59.000000 easydock-0.2.1/easydock.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1155 2023-05-16 09:01:52.000000 easydock-0.2.1/setup.py
```

### Comparing `easydock-0.2.0/PKG-INFO` & `easydock-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydock
-Version: 0.2.0
+Version: 0.2.1
 Summary: EasyDock Python module to facilitate molecular docking
 Home-page: https://github.com/ci-lab-cz/easydock
 Author: Pavel Polishchuk, Guzel Minibaeva, Aleksandra Ivanova
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # EasyDock - Python module to automate molecular docking
         
@@ -23,18 +23,20 @@
         from conda
         ```
         conda install -c conda-forge python=3.9 numpy=1.20 rdkit scipy dask distributed
         ```
         
         from pypi
         ```
-        pip install vina meeko
+        pip install meeko
         ```
         
-        Installation of gnina is described at https://github.com/gnina/gnina
+        Installation of `vina`. There is a strict recommendation to install `vina` from sources https://github.com/ccsb-scripps/AutoDock-Vina, because version 1.2.3 (available from pip) contains a bug which result in very unstable docking scores. The fix will be included in later releases.
+        
+        Installation of `gnina` is described at https://github.com/gnina/gnina
         
         ### Description
         
         Fully automatic pipeline for molecular docking.  
         
         Features:
         - the major script `run_dock` supports docking with `vina` and `gnina` (`gnina` also supports `smina` and its custom scoring functions)
@@ -162,14 +164,20 @@
         
         ##### Customization
         
         To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
         
         ### Changelog
         
+        **0.2.1**
+        - fix treatment of molecule ids in get_sdf_from_dock_db
+        - change installation instructions, vina must be installed from sources
+        - add argument no_tautomerization to disable tautomerization during protonation
+        - (critical) fix conversion of PDBQT to Mol which could not assign bond orders and returned molecules with only single bonds 
+        
         **0.2.0**
         - the stable version with multiple fixes and updates
         - dask library was fully integrated and tested
         - API was redesigned
         - docking of boron-containing compounds was implemented (Vina, smina)
         - a function to predict docking runtime was introduced
```

### Comparing `easydock-0.2.0/easydock/preparation_for_docking.py` & `easydock-0.2.1/easydock/preparation_for_docking.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,23 @@
 def mol_from_smi_or_molblock(ligand_string):
     mol = Chem.MolFromMolBlock(ligand_string)
     if mol is None:
         mol = Chem.MolFromSmiles(ligand_string)
     return mol
 
 
-def add_protonation(db_fname, table_name='mols', add_sql=''):
+def add_protonation(db_fname, tautomerize=True, table_name='mols', add_sql=''):
     '''
     Protonate SMILES by Chemaxon cxcalc utility to get molecule ionization states at pH 7.4.
     Parse console output and update db.
     :param db_fname:
+    :param tautomerize: get a major tautomer at protonation
     :param table_name: table name with molecules to protonate
     :param add_sql: additional SQL query to be appended to the SQL query to retrieve molecules for protonation,
-                    e.g. "AND iteration=MAX(iteration)".
+                    e.g. "AND id IN ('MOL1', 'MOL2')" or "AND iteration=(SELECT MAX(iteration) FROM mols)".
     :return:
     '''
     conn = sqlite3.connect(db_fname)
 
     try:
         cur = conn.cursor()
 
@@ -84,15 +85,16 @@
         with tempfile.NamedTemporaryFile(suffix='.sdf', mode='w', encoding='utf-8') as tmp:
             fd, output = tempfile.mkstemp()  # use output file to avoid overflow of stdout in extreme cases
             try:
                 for _, mol_block, _ in data_list:
                     tmp.write(mol_block)
                     tmp.write('\n$$$$\n')
                 tmp.flush()
-                cmd_run = f"cxcalc -S majormicrospecies -H 7.4 -M -K '{tmp.name}' > '{output}'"
+                cmd_run = f"cxcalc -S --ignore-error majormicrospecies -H 7.4 " \
+                          f"{'-M' if tautomerize else ''} -K '{tmp.name}' > '{output}'"
                 subprocess.call(cmd_run, shell=True)
                 sdf_protonated = Chem.SDMolSupplier(output)
                 for mol in sdf_protonated:
                     mol_name = mol.GetProp('_Name')
                     smi = mol.GetPropsAsDict().get('MAJORMS', None)
                     if smi is not None:
                         cansmi = Chem.CanonSmiles(smi)
@@ -273,28 +275,27 @@
     :return: a single string with a MOL block, if conversion failed returns None
     """
     mol_block = None
     fixed = False
     while mol_block is None:
         mol = Chem.MolFromPDBBlock('\n'.join([i[:66] for i in pdbqt_block.split('\n')]), removeHs=False, sanitize=False)
         try:
-            mol = boron_reduction(template_mol, mol)
-        except ValueError:
-            try:
+            if 5 in [atom.GetAtomicNum() for atom in template_mol.GetAtoms()]:
+                mol = boron_reduction(template_mol, mol)
+            else:
                 mol = assign_bonds_from_template(template_mol, mol)
-            except ValueError:
-                if fixed:  # if a molecule was already fixed and the error persists - simply break and return None
-                    sys.stderr.write(f'Parsing PDB was failed (fixing did not help): {mol_id}\n')
-                    break
-                sys.stderr.write(f'Could not assign bond orders while parsing PDB: {mol_id}. Trying to fix.\n')
-                pdbqt_block = fix_pdbqt(pdbqt_block)
-                fixed = True
-                continue
-        mol.SetProp('_Name', mol_id)
-        mol_block = Chem.MolToMolBlock(mol)
+            mol.SetProp('_Name', mol_id)
+            mol_block = Chem.MolToMolBlock(mol)
+        except ValueError:
+            if fixed:  # if a molecule was already fixed and the error persists - simply break and return None
+                sys.stderr.write(f'Parsing PDB was failed (fixing did not help): {mol_id}\n')
+                break
+            sys.stderr.write(f'Could not assign bond orders while parsing PDB: {mol_id}. Trying to fix.\n')
+            pdbqt_block = fix_pdbqt(pdbqt_block)
+            fixed = True
     return mol_block
 
 
 def create_db(db_fname, args, args_to_save=(), config_args_to_save=('protein', 'protein_setup')):
     """
     Create empty database structure and the setup table, which is filled with values. To setup table two fields are
     always stored: yaml file with all input args of the docking script and yaml file with docking config
@@ -465,28 +466,31 @@
             db_conn.commit()
 
 
 def insert_db(db_fname, data, cols=None, table_name='mols'):
     """
 
     :param db_fname:
-    :param data: list of values to insert
+    :param data: list of values to insert or a list of lists to insert multiple records
     :param cols: list of corresponding column names in the same order
     :param table_name:
     :return:
     """
     conn = sqlite3.connect(db_fname)
     if data:
+        # transform data to list of lists to perform executemany and be compatible with data if it is lists of lists
+        if not isinstance(data[0], (list, tuple)):
+            data = [data]
         cur = conn.cursor()
-        ncols = len(data)
+        ncols = len(data[0])
         if cols is None:
-            cur.execute(f"INSERT OR IGNORE INTO {table_name} VAlUES({','.join('?' * ncols)})", data)
+            cur.executemany(f"INSERT OR IGNORE INTO {table_name} VAlUES({','.join('?' * ncols)})", data)
         else:
             cols = ', '.join(cols)
-            cur.execute(f"INSERT OR IGNORE INTO {table_name} ({cols}) VAlUES({','.join('?' * ncols)})", data)
+            cur.executemany(f"INSERT OR IGNORE INTO {table_name} ({cols}) VAlUES({','.join('?' * ncols)})", data)
         conn.commit()
 
 
 def save_sdf(db_fname):
     sdf_fname = os.path.splitext(db_fname)[0] + '.sdf'
     with open(sdf_fname, 'wt') as w:
         conn = sqlite3.connect(db_fname)
@@ -504,15 +508,15 @@
 
 def select_mols_to_dock(db_conn, table_name='mols', add_sql=None):
     """
     Select molecules for docking from a given table using additional selection conditions
     :param db_conn:
     :param table_name:
     :param add_sql: additional SQL query which is appended the SQL query which returns molecules for docking,
-                    e.g. "AND iteration=MAX(iteration)"
+                    e.g. "AND id IN ('MOL1', 'MOL2')" or "AND iteration=(SELECT MAX(iteration) FROM mols)"
     :return: list of tuples (mol_id, smi) or (mol_id, mol_block). They can be mixed if the DB is not consistently
              filled, but this is not an issue if use proper parsing function
     """
     protonation_status = get_protonation_arg_value(db_conn)
     cur = db_conn.cursor()
     smi_field_name = 'smi_protonated' if protonation_status else 'smi'
     mol_field_name = 'source_mol_block_protonated' if protonation_status else 'source_mol_block'
```

### Comparing `easydock-0.2.0/easydock/run_dock.py` & `easydock-0.2.1/easydock/run_dock.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,16 @@
                              'exhaustiveness: 8\n'
                              'n_poses: 10\n'
                              'seed: -1\n'
                              'gnina.yml\n')
     parser.add_argument('--no_protonation', action='store_true', default=False,
                         help='disable protonation of molecules before docking. Protonation requires installed '
                              'cxcalc chemaxon utility.')
+    parser.add_argument('--no_tautomerization', action='store_true', default=False,
+                        help='disable tautomerization of molecules during protonation.')
     parser.add_argument('--sdf', action='store_true', default=False,
                         help='save best docked poses to SDF file with the same name as output DB.')
     parser.add_argument('--hostfile', metavar='FILENAME', required=False, type=filepath_type, default=None,
                         help='text file with addresses of nodes of dask SSH cluster. The most typical, it can be '
                              'passed as $PBS_NODEFILE variable from inside a PBS script. The first line in this file '
                              'will be the address of the scheduler running on the standard port 8786. If omitted, '
                              'calculations will run on a single machine as usual.')
@@ -183,15 +185,15 @@
                 hosts = [line.strip() for line in f]
             dask_client = Client(hosts[0] + ':8786', connection_limit=2048)
             # dask_client = Client()   # to test dask locally
         else:
             dask_client = None
 
         if not args.no_protonation:
-            add_protonation(args.output)
+            add_protonation(args.output, not args.no_tautomerization)
 
         if args.program == 'vina':
             from easydock.vina_dock import mol_dock, pred_dock_time
         elif args.program == 'gnina':
             from easydock.gnina_dock import mol_dock
             from easydock.vina_dock import pred_dock_time
         else:
```

### Comparing `easydock-0.2.0/easydock/vina_dock_cli.py` & `easydock-0.2.1/easydock/vina_dock_cli.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.0/easydock/read_input.py` & `easydock-0.2.1/easydock/read_input.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.0/easydock/get_sdf_from_dock_db.py` & `easydock-0.2.1/easydock/get_sdf_from_dock_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                         help='list of pose numbers to retrieve, starting from 1. If specified, poses will be retrieved '
                              'from PDB block and a trailing pose id will be added to each molecule name.')
 
     args = parser.parse_args()
 
     if args.ids is None:
         ids = tuple()
-    elif os.path.isfile(args.ids):
+    elif os.path.isfile(args.ids[0]):
         with open(args.ids) as f:
             ids = [line.strip() for line in f]
     else:
         ids = args.ids
 
     conn = sqlite3.connect(args.input)
     cur = conn.cursor()
```

### Comparing `easydock-0.2.0/easydock/vina_dock.py` & `easydock-0.2.1/easydock/vina_dock.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.0/easydock/gnina_dock.py` & `easydock-0.2.1/easydock/gnina_dock.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.0/README.md` & `easydock-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 from conda
 ```
 conda install -c conda-forge python=3.9 numpy=1.20 rdkit scipy dask distributed
 ```
 
 from pypi
 ```
-pip install vina meeko
+pip install meeko
 ```
 
-Installation of gnina is described at https://github.com/gnina/gnina
+Installation of `vina`. There is a strict recommendation to install `vina` from sources https://github.com/ccsb-scripps/AutoDock-Vina, because version 1.2.3 (available from pip) contains a bug which result in very unstable docking scores. The fix will be included in later releases.
+
+Installation of `gnina` is described at https://github.com/gnina/gnina
 
 ### Description
 
 Fully automatic pipeline for molecular docking.  
 
 Features:
 - the major script `run_dock` supports docking with `vina` and `gnina` (`gnina` also supports `smina` and its custom scoring functions)
@@ -154,14 +156,20 @@
 
 ##### Customization
 
 To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
 
 ### Changelog
 
+**0.2.1**
+- fix treatment of molecule ids in get_sdf_from_dock_db
+- change installation instructions, vina must be installed from sources
+- add argument no_tautomerization to disable tautomerization during protonation
+- (critical) fix conversion of PDBQT to Mol which could not assign bond orders and returned molecules with only single bonds 
+
 **0.2.0**
 - the stable version with multiple fixes and updates
 - dask library was fully integrated and tested
 - API was redesigned
 - docking of boron-containing compounds was implemented (Vina, smina)
 - a function to predict docking runtime was introduced
```

### Comparing `easydock-0.2.0/easydock.egg-info/PKG-INFO` & `easydock-0.2.1/easydock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydock
-Version: 0.2.0
+Version: 0.2.1
 Summary: EasyDock Python module to facilitate molecular docking
 Home-page: https://github.com/ci-lab-cz/easydock
 Author: Pavel Polishchuk, Guzel Minibaeva, Aleksandra Ivanova
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # EasyDock - Python module to automate molecular docking
         
@@ -23,18 +23,20 @@
         from conda
         ```
         conda install -c conda-forge python=3.9 numpy=1.20 rdkit scipy dask distributed
         ```
         
         from pypi
         ```
-        pip install vina meeko
+        pip install meeko
         ```
         
-        Installation of gnina is described at https://github.com/gnina/gnina
+        Installation of `vina`. There is a strict recommendation to install `vina` from sources https://github.com/ccsb-scripps/AutoDock-Vina, because version 1.2.3 (available from pip) contains a bug which result in very unstable docking scores. The fix will be included in later releases.
+        
+        Installation of `gnina` is described at https://github.com/gnina/gnina
         
         ### Description
         
         Fully automatic pipeline for molecular docking.  
         
         Features:
         - the major script `run_dock` supports docking with `vina` and `gnina` (`gnina` also supports `smina` and its custom scoring functions)
@@ -162,14 +164,20 @@
         
         ##### Customization
         
         To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
         
         ### Changelog
         
+        **0.2.1**
+        - fix treatment of molecule ids in get_sdf_from_dock_db
+        - change installation instructions, vina must be installed from sources
+        - add argument no_tautomerization to disable tautomerization during protonation
+        - (critical) fix conversion of PDBQT to Mol which could not assign bond orders and returned molecules with only single bonds 
+        
         **0.2.0**
         - the stable version with multiple fixes and updates
         - dask library was fully integrated and tested
         - API was redesigned
         - docking of boron-containing compounds was implemented (Vina, smina)
         - a function to predict docking runtime was introduced
```

### Comparing `easydock-0.2.0/setup.py` & `easydock-0.2.1/setup.py`

 * *Files identical despite different names*

