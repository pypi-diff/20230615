# Comparing `tmp/netexp-0.1.9.tar.gz` & `tmp/netexp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netexp-0.1.9.tar", last modified: Wed Mar 23 22:49:53 2022, max compression
+gzip compressed data, was "netexp-0.2.0.tar", last modified: Thu Jun 15 17:14:43 2023, max compression
```

## Comparing `netexp-0.1.9.tar` & `netexp-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-23 22:49:53.802138 netexp-0.1.9/
--rw-r--r--   0 hfreitas (20477) users      (100)     1799 2022-02-17 02:03:25.000000 netexp-0.1.9/.gitignore
--rw-r--r--   0 hfreitas (20477) users      (100)     1518 2022-02-17 02:03:25.000000 netexp-0.1.9/LICENSE
--rw-r--r--   0 hfreitas (20477) users      (100)     1425 2022-03-23 22:49:53.802138 netexp-0.1.9/PKG-INFO
--rw-r--r--   0 hfreitas (20477) users      (100)      210 2022-03-10 18:15:40.000000 netexp-0.1.9/README.md
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-23 22:49:53.802138 netexp-0.1.9/netexp/
--rw-r--r--   0 hfreitas (20477) users      (100)       77 2022-03-23 22:47:59.000000 netexp-0.1.9/netexp/__init__.py
--rw-r--r--   0 hfreitas (20477) users      (100)    12418 2022-03-22 00:03:09.000000 netexp-0.1.9/netexp/helpers.py
--rw-r--r--   0 hfreitas (20477) users      (100)      737 2022-03-16 19:40:28.000000 netexp-0.1.9/netexp/pcap.py
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-23 22:49:53.802138 netexp-0.1.9/netexp/pktgen/
--rw-r--r--   0 hfreitas (20477) users      (100)      829 2022-03-16 18:48:02.000000 netexp-0.1.9/netexp/pktgen/__init__.py
--rw-r--r--   0 hfreitas (20477) users      (100)    12899 2022-03-18 00:52:26.000000 netexp-0.1.9/netexp/pktgen/dpdk.py
--rw-r--r--   0 hfreitas (20477) users      (100)      124 2022-03-18 18:00:48.000000 netexp-0.1.9/netexp/pktgen/norman.py
--rw-r--r--   0 hfreitas (20477) users      (100)     6926 2022-03-10 16:13:18.000000 netexp-0.1.9/netexp/pktgen/zhipeng_fpga.py
--rw-r--r--   0 hfreitas (20477) users      (100)     2332 2022-03-21 18:20:33.000000 netexp-0.1.9/netexp/throughput.py
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-23 22:49:53.802138 netexp-0.1.9/netexp.egg-info/
--rw-r--r--   0 hfreitas (20477) users      (100)     1425 2022-03-23 22:49:53.000000 netexp-0.1.9/netexp.egg-info/PKG-INFO
--rw-r--r--   0 hfreitas (20477) users      (100)      401 2022-03-23 22:49:53.000000 netexp-0.1.9/netexp.egg-info/SOURCES.txt
--rw-r--r--   0 hfreitas (20477) users      (100)        1 2022-03-23 22:49:53.000000 netexp-0.1.9/netexp.egg-info/dependency_links.txt
--rw-r--r--   0 hfreitas (20477) users      (100)       14 2022-03-23 22:49:53.000000 netexp-0.1.9/netexp.egg-info/requires.txt
--rw-r--r--   0 hfreitas (20477) users      (100)        7 2022-03-23 22:49:53.000000 netexp-0.1.9/netexp.egg-info/top_level.txt
--rw-r--r--   0 hfreitas (20477) users      (100)       56 2022-02-17 02:15:10.000000 netexp-0.1.9/pytest.ini
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-23 22:49:53.802138 netexp-0.1.9/scripts/
--rwxr-xr-x   0 hfreitas (20477) users      (100)      103 2022-03-10 23:43:49.000000 netexp-0.1.9/scripts/publish.sh
--rw-r--r--   0 hfreitas (20477) users      (100)      104 2022-03-23 22:49:53.802138 netexp-0.1.9/setup.cfg
--rw-r--r--   0 hfreitas (20477) users      (100)     2071 2022-03-10 18:10:56.000000 netexp-0.1.9/setup.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-15 17:14:43.913977 netexp-0.2.0/
+-rw-r--r--   0 hugo       (501) staff       (20)     1799 2022-02-17 02:03:25.000000 netexp-0.2.0/.gitignore
+-rw-r--r--   0 hugo       (501) staff       (20)     1518 2022-02-17 02:03:25.000000 netexp-0.2.0/LICENSE
+-rw-r--r--   0 hugo       (501) staff       (20)     1130 2023-06-15 17:14:43.914056 netexp-0.2.0/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)      210 2022-03-10 18:15:40.000000 netexp-0.2.0/README.md
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-15 17:14:43.912581 netexp-0.2.0/netexp/
+-rw-r--r--   0 hugo       (501) staff       (20)       76 2023-06-15 17:14:25.000000 netexp-0.2.0/netexp/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)    24821 2023-04-12 17:44:45.000000 netexp-0.2.0/netexp/helpers.py
+-rw-r--r--   0 hugo       (501) staff       (20)      857 2023-04-11 22:46:46.000000 netexp-0.2.0/netexp/pcap.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-15 17:14:43.913704 netexp-0.2.0/netexp/pktgen/
+-rw-r--r--   0 hugo       (501) staff       (20)      828 2023-03-13 19:54:04.000000 netexp-0.2.0/netexp/pktgen/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)    13145 2023-06-15 17:06:33.000000 netexp-0.2.0/netexp/pktgen/dpdk.py
+-rw-r--r--   0 hugo       (501) staff       (20)      120 2023-03-13 19:56:35.000000 netexp-0.2.0/netexp/pktgen/enso.py
+-rw-r--r--   0 hugo       (501) staff       (20)     7248 2023-03-16 15:46:14.000000 netexp-0.2.0/netexp/pktgen/zhipeng_fpga.py
+-rw-r--r--   0 hugo       (501) staff       (20)     2491 2023-04-09 16:41:46.000000 netexp-0.2.0/netexp/throughput.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-15 17:14:43.913186 netexp-0.2.0/netexp.egg-info/
+-rw-r--r--   0 hugo       (501) staff       (20)     1130 2023-06-15 17:14:43.000000 netexp-0.2.0/netexp.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)      399 2023-06-15 17:14:43.000000 netexp-0.2.0/netexp.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (501) staff       (20)        1 2023-06-15 17:14:43.000000 netexp-0.2.0/netexp.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       14 2023-06-15 17:14:43.000000 netexp-0.2.0/netexp.egg-info/requires.txt
+-rw-r--r--   0 hugo       (501) staff       (20)        7 2023-06-15 17:14:43.000000 netexp-0.2.0/netexp.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       56 2022-02-17 02:15:10.000000 netexp-0.2.0/pytest.ini
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-15 17:14:43.913842 netexp-0.2.0/scripts/
+-rwxr-xr-x   0 hugo       (501) staff       (20)      125 2023-04-10 14:10:34.000000 netexp-0.2.0/scripts/publish.sh
+-rw-r--r--   0 hugo       (501) staff       (20)      104 2023-06-15 17:14:43.914281 netexp-0.2.0/setup.cfg
+-rw-r--r--   0 hugo       (501) staff       (20)     1827 2023-03-13 19:54:04.000000 netexp-0.2.0/setup.py
```

### Comparing `netexp-0.1.9/.gitignore` & `netexp-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `netexp-0.1.9/LICENSE` & `netexp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netexp-0.1.9/netexp/pktgen/__init__.py` & `netexp-0.2.0/netexp/pktgen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from abc import ABCMeta, abstractmethod
 
 
 class Pktgen(metaclass=ABCMeta):
     @abstractmethod
     def set_params(self, pkt_size, nb_src, nb_dst) -> None:
         pass
```

### Comparing `netexp-0.1.9/netexp/pktgen/dpdk.py` & `netexp-0.2.0/netexp/pktgen/dpdk.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-
 import ipaddress
 import time
 
 from typing import Any, Optional, Iterable, Union
 
 from netexp.pktgen import Pktgen
-from netexp.helpers import get_ssh_client, posix_shell, remote_command, \
-    run_console_commands, watch_command
+from netexp.helpers import (
+    get_ssh_client,
+    posix_shell,
+    remote_command,
+    run_console_commands,
+    watch_command,
+)
 
 
 class DpdkConfig:
     """Represent DPDK command-line options.
 
     Attributes:
         cores: List of cores to run on.
@@ -47,29 +51,37 @@
     Examples:
         Obtaining the DPDK configuration in command-line option format:
 
         >>> dpdk_config = DpdkConfig([0, 2], 4, pci_allow_list='05:00.0')
         >>> str(dpdk_config)
         '-l 0,2 -n 4 -a 05:00.0'
     """
-    def __init__(self, cores: Iterable[int], mem_channels: int,
-                 drivers: Optional[Iterable[str]] = None,
-                 mem_alloc: Optional[int] = None,
-                 mem_ranks: Optional[int] = None, xen_dom0: bool = False,
-                 syslog: bool = False,
-                 socket_mem: Optional[Iterable[int]] = None,
-                 huge_dir: Optional[str] = None,
-                 proc_type: Optional[str] = None,
-                 file_prefix: Optional[str] = None,
-                 pci_block_list: Optional[Iterable[str]] = None,
-                 pci_allow_list: Optional[Iterable[str]] = None,
-                 vdev: Optional[str] = None, vmware_tsc_map: bool = False,
-                 base_virtaddr: Optional[str] = None,
-                 vfio_intr: Optional[str] = None, create_uio_dev: bool = False,
-                 extra_opt: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        cores: Iterable[int],
+        mem_channels: int,
+        drivers: Optional[Iterable[str]] = None,
+        mem_alloc: Optional[int] = None,
+        mem_ranks: Optional[int] = None,
+        xen_dom0: bool = False,
+        syslog: bool = False,
+        socket_mem: Optional[Iterable[int]] = None,
+        huge_dir: Optional[str] = None,
+        proc_type: Optional[str] = None,
+        file_prefix: Optional[str] = None,
+        pci_block_list: Optional[Iterable[str]] = None,
+        pci_allow_list: Optional[Iterable[str]] = None,
+        vdev: Optional[str] = None,
+        vmware_tsc_map: bool = False,
+        base_virtaddr: Optional[str] = None,
+        vfio_intr: Optional[str] = None,
+        create_uio_dev: bool = False,
+        extra_opt: Optional[str] = None,
+    ) -> None:
         self.cores = cores
         self.mem_channels = mem_channels
         self.drivers = drivers
         self.mem_alloc = mem_alloc
         self.mem_ranks = mem_ranks
         self.xen_dom0 = xen_dom0
         self.syslog = syslog
@@ -92,68 +104,68 @@
         if pci_allow_list is not None and not isinstance(pci_allow_list, list):
             self.pci_allow_list = [self.pci_allow_list]
 
         if pci_block_list is not None and not isinstance(pci_block_list, list):
             self.pci_block_list = [self.pci_block_list]
 
     def __str__(self) -> str:
-        opts = '-l ' + ','.join(str(c) for c in self.cores)
-        opts += f' -n {self.mem_channels}'
+        opts = "-l " + ",".join(str(c) for c in self.cores)
+        opts += f" -n {self.mem_channels}"
 
         if self.drivers is not None:
             for driver in self.drivers:
-                opts += f' -d {driver}'
+                opts += f" -d {driver}"
 
         if self.mem_alloc is not None:
-            opts += f' -m {self.mem_alloc}'
+            opts += f" -m {self.mem_alloc}"
 
         if self.mem_ranks is not None:
-            opts += f' -r {self.mem_ranks}'
+            opts += f" -r {self.mem_ranks}"
 
         if self.xen_dom0:
-            opts += ' --xen-dom0'
+            opts += " --xen-dom0"
 
         if self.syslog:
-            opts += ' --syslog'
+            opts += " --syslog"
 
         if self.socket_mem is not None:
-            opt = ','.join(str(sm) for sm in self.socket_mem)
-            opts += f' --socket-mem {opt}'
+            opt = ",".join(str(sm) for sm in self.socket_mem)
+            opts += f" --socket-mem {opt}"
 
         if self.huge_dir is not None:
-            opts += f' --huge-dir {self.huge_dir}'
+            opts += f" --huge-dir {self.huge_dir}"
 
         if self.proc_type is not None:
-            opts += f' --proc-type {self.proc_type}'
+            opts += f" --proc-type {self.proc_type}"
 
         if self.file_prefix is not None:
-            opts += f' --file-prefix {self.file_prefix}'
+            opts += f" --file-prefix {self.file_prefix}"
 
         if self.pci_block_list is not None:
             for pci_block_list in self.pci_block_list:
-                opts += f' -b {pci_block_list}'
+                opts += f" -b {pci_block_list}"
 
         if self.pci_allow_list is not None:
             for pci_allow_list in self.pci_allow_list:
-                opts += f' -a {pci_allow_list}'
+                opts += f" -a {pci_allow_list}"
 
         if self.vdev is not None:
-            opts += f' --vdev {self.vdev}'
+            opts += f" --vdev {self.vdev}"
 
         if self.vmware_tsc_map:
-            opts += ' --vmware-tsc-map'
+            opts += " --vmware-tsc-map"
 
         if self.base_virtaddr is not None:
-            opts += f' --base-virt-addr {self.base_virtaddr}'
+            opts += f" --base-virt-addr {self.base_virtaddr}"
 
         if self.vfio_intr is not None:
-            opts += f' --vfio-intr {self.vfio_intr}'
+            opts += f" --vfio-intr {self.vfio_intr}"
 
         if self.create_uio_dev:
-            opts += ' --create-uio-dev'
+            opts += " --create-uio-dev"
 
         if self.extra_opt is not None:
             opts += self.extra_opt
 
         return opts
 
 
@@ -165,181 +177,211 @@
     `meson build -Denable_lua=true`).
 
     Attributes:
         pktgen_server: The remote host to run DPDK Pktgen on.
         dpdk_config: CLI config to pass to DPDK.
         port_map: Port map using DPDK Pktgen port map syntax.
         max_throughput: Maximum throughput supported by the NIC.
-        port: Default port to use, only relevant when using multiple interfaces.
+        port: Default port to use, only relevant with multiple interfaces.
         pcap: Path to pcap file.
         config_file: DPDK Pktgen configuration file.
         log_file: Log file.
         promiscuous: Enable promiscuous mode (accept all packets that arrive at
           the interface).
         numa_support: Enable NUMA support.
         extra_opt: Extra DPDK pktgen command-line options.
     """
-    def __init__(self, pktgen_server: str, dpdk_config: Union[str, DpdkConfig],
-                 port_map: str, max_throughput: float, port: int = 0,
-                 pcap: Optional[str] = None, config_file: Optional[str] = None,
-                 log_file: Optional[str] = None, promiscuous=False,
-                 numa_support=False, extra_opt: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        pktgen_server: str,
+        dpdk_config: Union[str, DpdkConfig],
+        port_map: str,
+        max_throughput: float,
+        rx_port: int = 0,
+        tx_port: int = 0,
+        pcap: Optional[str] = None,
+        config_file: Optional[str] = None,
+        log_file: Optional[str] = None,
+        promiscuous: bool = False,
+        numa_support: bool = False,
+        extra_opt: Optional[str] = None,
+    ) -> None:
         self.pktgen_ssh_client = get_ssh_client(pktgen_server)
         pktgen_options = f'-m "{port_map}"'
         self.max_throughput = max_throughput
-        self.port = port
+        self.rx_port = rx_port
+        self.tx_port = tx_port
 
         if pcap is not None:
-            pktgen_options += f' -s 0:{pcap}'
+            pktgen_options += f" -s 0:{pcap}"
             self.use_pcap = True
         else:
             self.use_pcap = False
 
         if config_file is not None:
-            pktgen_options += f' -f {config_file}'
+            pktgen_options += f" -f {config_file}"
 
         if log_file is not None:
-            pktgen_options += f' -l {log_file}'
+            pktgen_options += f" -l {log_file}"
 
         if promiscuous:
-            pktgen_options += ' -P'
+            pktgen_options += " -P"
 
         if numa_support:
-            pktgen_options += ' -N'
+            pktgen_options += " -N"
 
         if extra_opt is not None:
             pktgen_options += extra_opt
 
-        remote_cmd = f'sudo pktgen {dpdk_config} -- {pktgen_options}'
-        self.pktgen = remote_command(self.pktgen_ssh_client, remote_cmd,
-                                     pty=True, print_command=True)
+        remote_cmd = f"sudo pktgen {dpdk_config} -- {pktgen_options}"
+        self.pktgen = remote_command(
+            self.pktgen_ssh_client, remote_cmd, pty=True, print_command=True
+        )
         self.remote_cmd = remote_cmd
         self.target_pkt_tx = 0
 
         self.ready = False
 
     def wait_ready(self, stdout: bool = True, stderr: bool = True) -> None:
-        watch_command(self.pktgen, keyboard_int=self.pktgen.close,
-                      stop_pattern='Pktgen:/>', stdout=stdout, stderr=stderr)
+        watch_command(
+            self.pktgen,
+            keyboard_int=self.pktgen.close,
+            stop_pattern="Pktgen:/>",
+            stdout=stdout,
+            stderr=stderr,
+        )
         self.ready = True
 
     def commands(self, cmds, timeout: float = 0.5) -> None:
-        run_console_commands(self.pktgen, cmds, timeout=timeout,
-                             console_pattern='\r\nPktgen:/> ')
+        run_console_commands(
+            self.pktgen,
+            cmds,
+            timeout=timeout,
+            console_pattern="\r\nPktgen:/> ",
+        )
 
-    def set_params(self, pkt_size: int, nb_src: int, nb_dst: int,
-                   init_ip: Any = None, init_port: int = 0,
-                   port: Optional[int] = None) -> None:
-        init_ip = init_ip or '192.168.0.0'
+    def set_params(
+        self,
+        pkt_size: int,
+        nb_src: int,
+        nb_dst: int,
+        init_ip: Any = None,
+        init_port: int = 0,
+        tx_port: Optional[int] = None,
+    ) -> None:
+        init_ip = init_ip or "192.168.0.0"
         max_src_ip = ipaddress.ip_address(init_ip) + nb_src - 1
         max_dst_ip = ipaddress.ip_address(init_ip) + nb_dst - 1
 
-        if port is None:
-            port = self.port
+        if tx_port is None:
+            tx_port = self.tx_port
 
         if not self.ready:
             self.wait_ready(stdout=False, stderr=False)
 
         commands = [
-            f'range {port} dst port start {init_port}',
-            f'range {port} src ip max {max_src_ip}',
-            f'range {port} dst ip max {max_dst_ip}',
-            f'range {port} size start {pkt_size}',
-            f'range {port} size min {pkt_size}',
-            f'range {port} size max {pkt_size}',
+            f"range {tx_port} dst port start {init_port}",
+            f"range {tx_port} src ip max {max_src_ip}",
+            f"range {tx_port} dst ip max {max_dst_ip}",
+            f"range {tx_port} size start {pkt_size}",
+            f"range {tx_port} size min {pkt_size}",
+            f"range {tx_port} size max {pkt_size}",
         ]
         self.commands(commands)
 
-    def start(self, throughput: float, nb_pkts: int,
-              port: Optional[int] = None) -> None:
-        port = port or self.port
+    def start(
+        self, throughput: float, nb_pkts: int, tx_port: Optional[int] = None
+    ) -> None:
+        tx_port = tx_port or self.tx_port
 
         if not self.ready:
             self.wait_ready(stdout=False, stderr=False)
 
         commands = []
         if self.use_pcap:
-            commands += [f'enable {port} pcap']
+            commands += [f"enable {tx_port} pcap"]
 
-        rate = (throughput / self.max_throughput * 100)
+        rate = throughput / self.max_throughput * 100
 
         self.target_pkt_tx = self.get_nb_tx_pkts() + nb_pkts
 
         commands += [
-            f'set {port} count {nb_pkts}',
-            f'set {port} rate {rate}',
-            f'start {port}',
+            f"set {tx_port} count {nb_pkts}",
+            f"set {tx_port} rate {rate}",
+            f"start {tx_port}",
         ]
         self.commands(commands)
 
     def wait_transmission_done(self) -> None:
         pkts_tx = 0
         while pkts_tx < self.target_pkt_tx:
             time.sleep(1)
 
             old_pkt_tx = pkts_tx
             pkts_tx = self.get_nb_tx_pkts()
 
             if old_pkt_tx == pkts_tx:
-                raise RuntimeError('Pktgen is not making progress')
+                raise RuntimeError("Pktgen is not making progress")
 
-    def stop(self, port: Optional[int] = None) -> None:
-        self.commands(f'stop {port or self.port}')
+    def stop(self, tx_port: Optional[int] = None) -> None:
+        self.commands(f"stop {tx_port or self.tx_port}")
 
     def clear(self) -> None:
-        self.pktgen.send('clr\n')
+        self.pktgen.send("clr\n")
         self.wait_ready()
 
     def clean_stats(self) -> None:
         return self.clear()
 
     def close(self) -> None:
-        self.pktgen.send('quit\n')
+        self.pktgen.send("quit\n")
         time.sleep(0.1)
         self.pktgen_ssh_client.close()
 
     def _get_stats(self, subtype: str, stat_name: str, port: int) -> int:
         self.pktgen.send(
             f'\nlua \'print(pktgen.portStats("all", "{subtype}")[{port}].'
-            f'{stat_name})\'\n'
+            f"{stat_name})'\n"
         )
         output = watch_command(
-            self.pktgen, keyboard_int=lambda: self.pktgen.send('\x03'),
-            stop_pattern='\r\n\\d+\r\n'
+            self.pktgen,
+            keyboard_int=lambda: self.pktgen.send("\x03"),
+            stop_pattern="\r\n\\d+\r\n",
         )
-        lines = output.split('\r\n')
+        lines = output.split("\r\n")
         lines = [ln for ln in lines if ln.isdigit()]
 
         return int(lines[-1])
 
     def get_pkts_rx_rate(self, port: Optional[int] = None) -> int:
-        return self._get_stats('rate', 'pkts_rx', port or self.port)
+        return self._get_stats("rate", "pkts_rx", port or self.rx_port)
 
     def get_pkts_tx_rate(self, port: Optional[int] = None) -> int:
-        return self._get_stats('rate', 'pkts_tx', port or self.port)
+        return self._get_stats("rate", "pkts_tx", port or self.tx_port)
 
     def get_mbits_rx(self, port: Optional[int] = None) -> int:
-        return self._get_stats('rate', 'mbits_rx', port or self.port)
+        return self._get_stats("rate", "mbits_rx", port or self.rx_port)
 
     def get_mbits_tx(self, port: Optional[int] = None) -> int:
-        return self._get_stats('rate', 'mbits_rx', port or self.port)
+        return self._get_stats("rate", "mbits_rx", port or self.tx_port)
 
     def get_nb_rx_pkts(self, port: Optional[int] = None) -> int:
-        return self._get_stats('port', 'ipackets', port or self.port)
+        return self._get_stats("port", "ipackets", port or self.rx_port)
 
     def get_nb_tx_pkts(self, port: Optional[int] = None) -> int:
-        return self._get_stats('port', 'opackets', port or self.port)
+        return self._get_stats("port", "opackets", port or self.tx_port)
 
     def get_rx_throughput(self, port: Optional[int] = None) -> int:
-        return self.get_mbits_rx(self.port) * 1_000_000
+        return self.get_mbits_rx(self.rx_port) * 1_000_000
 
     def get_tx_throughput(self, port: Optional[int] = None) -> int:
-        return self.get_mbits_tx(self.port) * 1_000_000
+        return self.get_mbits_tx(self.tx_port) * 1_000_000
 
     def enter_interactive(self) -> None:
         posix_shell(self.pktgen)
 
     def __del__(self) -> None:
-        self.commands('quit')
+        self.commands("quit")
         del self.pktgen
         self.pktgen_ssh_client.close()
         del self.pktgen_ssh_client
```

### Comparing `netexp-0.1.9/netexp/pktgen/zhipeng_fpga.py` & `netexp-0.2.0/netexp/pktgen/zhipeng_fpga.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,221 +1,239 @@
-
-from netexp.helpers import RemoteIntelFpga, remote_command, upload_file, \
-    watch_command
+from netexp.helpers import (
+    IntelFpga,
+    remote_command,
+    upload_file,
+    watch_command,
+)
 from netexp.pktgen import Pktgen
 
 import math
 import sys
 
 from pathlib import Path
 
 
-PARSE_OUTPUT_CMD = 'rtl_sim/input_gen/run.sh'
-INPUT_GEN_CMD = 'hardware_test/hwtest/input_gen.py'
-PCAP_GEN_CMD = 'frontend/generate_synthetic_trace.py'
-PCAP_DEST = Path('hardware_test/hwtest')
+PARSE_OUTPUT_CMD = "rtl_sim/input_gen/run.sh"
+INPUT_GEN_CMD = "hardware_test/hwtest/input_gen.py"
+PCAP_GEN_CMD = "frontend/generate_synthetic_trace.py"
+PCAP_DEST = Path("hardware_test/hwtest")
+
+LOAD_BITSTREAM_CMD = "hardware_test/load_bitstream.sh"
+RUN_CONSOLE_CMD = "hardware_test/run_console.sh"
 
 MAX_NB_PCAP_FLITS = 16384
 
 
 class FpgaPktgen(Pktgen):
     def __init__(self, server, fpga_id, remote_dir, load_bitstream=True):
         self._rate = 0
         self._nb_flits_in_pcap = 0
         self._rx_window = 0
         self._tx_window = 0
         self._nb_pcap_iters = 0  # 0 means forever
-        self.fpga = RemoteIntelFpga(server, fpga_id, remote_dir,
-                                    load_bitstream=load_bitstream)
+
+        load_bitstream_cmd = f"{remote_dir}/{LOAD_BITSTREAM_CMD}"
+        run_console_cmd = f"{remote_dir}/{RUN_CONSOLE_CMD}"
+
+        self.fpga = IntelFpga(
+            fpga_id,
+            run_console_cmd,
+            load_bitstream_cmd,
+            host_name=server,
+            load_bitstream=load_bitstream,
+        )
 
         # make sure it is not running and registers are clear
         if not load_bitstream:
             self.stop()
             self.clear()
 
     def run_and_watch_cmd(self, cmd, dir=None):
         app = remote_command(self.ssh_client, cmd, pty=True, dir=dir)
-        watch_command(app, keyboard_int=lambda: app.send('\x03'))
+        watch_command(app, keyboard_int=lambda: app.send("\x03"))
         status = app.recv_exit_status()
         return status
 
     def set_params(self, pkt_size, nb_src, nb_dst):
         nb_pkts = nb_src * nb_dst
 
         pkt_size_in_flits = int(math.ceil(pkt_size / 64))
         total_nb_flits = nb_pkts * pkt_size_in_flits
 
         if total_nb_flits > MAX_NB_PCAP_FLITS:
-            sys.stderr.write('pcap size exceeds maximum number of flits')
+            sys.stderr.write("pcap size exceeds maximum number of flits")
             raise RuntimeError()
 
         remote_dir_path = Path(self.fpga.remote_dir)
         pcap_dst = remote_dir_path / PCAP_DEST
         pcap_gen_cmd = remote_dir_path / Path(PCAP_GEN_CMD)
-        pcap_gen_cmd = f'{pcap_gen_cmd} {nb_pkts} {pkt_size} {nb_src} {nb_dst}'
+        pcap_gen_cmd = f"{pcap_gen_cmd} {nb_pkts} {pkt_size} {nb_src} {nb_dst}"
         self.run_and_watch_cmd(pcap_gen_cmd, dir=pcap_dst)
 
-        out_pcap = '_'.join(str(x) for x in (nb_pkts, pkt_size, nb_src, nb_dst))
-        out_pcap += '.pcap'
+        out_pcap = "_".join(
+            str(x) for x in (nb_pkts, pkt_size, nb_src, nb_dst)
+        )
+        out_pcap += ".pcap"
 
         self.parse_pcap(out_pcap)
         self.reload_pcap()
 
     def parse_pcap(self, pcap_name):
         pcap_name = Path(pcap_name)
         remote_dir_path = Path(self.fpga.remote_dir)
         pcap_dst = remote_dir_path / PCAP_DEST
-        pkt_dest = pcap_dst / pcap_name.with_suffix('.pkt').name
+        pkt_dest = pcap_dst / pcap_name.with_suffix(".pkt").name
 
         parse_cmd = remote_dir_path / Path(PARSE_OUTPUT_CMD)
-        parse_cmd = f'{parse_cmd} {pcap_dst / pcap_name} {pkt_dest}'
+        parse_cmd = f"{parse_cmd} {pcap_dst / pcap_name} {pkt_dest}"
 
         in_gen_cmd = remote_dir_path / Path(INPUT_GEN_CMD)
-        in_gen_cmd = f'{in_gen_cmd} {pkt_dest}'
+        in_gen_cmd = f"{in_gen_cmd} {pkt_dest}"
 
         self.run_and_watch_cmd(parse_cmd, dir=pcap_dst)
         self.run_and_watch_cmd(in_gen_cmd, dir=pcap_dst)
 
     def load_pcap(self, pcap_file_name, local=True):
         """Load local pcap in remote FPGA."""
         pcap_path = Path(pcap_file_name)
         remote_dir_path = Path(self.fpga.remote_dir)
         pcap_dst = remote_dir_path / PCAP_DEST
 
         if local:
             upload_file(pcap_path, self.fpga.server, pcap_dst)
         else:
-            cmd = f'cp {pcap_path} {pcap_dst}'
+            cmd = f"cp {pcap_path} {pcap_dst}"
             if self.run_and_watch_cmd(cmd, dir=pcap_dst):
                 raise RuntimeError()
 
         self.parse_pcap(pcap_path.name)
         self.reload_pcap()
 
     def reload_pcap(self):
         """Reload last loaded pcap."""
         remote_dir_path = Path(self.fpga.remote_dir)
         pcap_dst = remote_dir_path / PCAP_DEST
-        app = remote_command(self.fpga.ssh_client, 'wc -l < meta.txt', pty=True,
-                             dir=pcap_dst)
-        output = watch_command(app, keyboard_int=lambda: app.send('\x03'))
+        app = remote_command(
+            self.fpga.ssh_client, "wc -l < meta.txt", pty=True, dir=pcap_dst
+        )
+        output = watch_command(app, keyboard_int=lambda: app.send("\x03"))
         nb_flits = int(output)
-        print(f'pcap has {nb_flits} flits')
+        print(f"pcap has {nb_flits} flits")
 
         self.nb_flits_in_pcap = nb_flits
         self.load_mem()
         self.load_meta()
 
         self.clear()
 
     @property
     def rate(self):
         return self._rate
 
     @rate.setter
     def rate(self, rate):
         self._rate = rate
-        self.fpga.run_jtag_commands(f'set_rate {rate}')
+        self.fpga.run_jtag_commands(f"set_rate {rate}")
 
     def load_mem(self):
-        self.fpga.run_jtag_commands('load_mem')
+        self.fpga.run_jtag_commands("load_mem")
 
     def load_meta(self):
-        self.fpga.run_jtag_commands('load_meta')
+        self.fpga.run_jtag_commands("load_meta")
 
     @property
     def nb_flits_in_pcap(self):
         return self._nb_flits_in_pcap
 
     @nb_flits_in_pcap.setter
     def nb_flits_in_pcap(self, nb_flits_in_pcap):
         self._nb_flits_in_pcap = nb_flits_in_pcap
-        self.fpga.run_jtag_commands(f'set_flit_size {nb_flits_in_pcap}')
+        self.fpga.run_jtag_commands(f"set_flit_size {nb_flits_in_pcap}")
 
     @property
     def rx_window(self):
         return self._rx_window
 
     @rx_window.setter
     def rx_window(self, rx_window):
         self._rx_window = rx_window
-        self.fpga.run_jtag_commands(f'set_rx_pkt_win {rx_window}')
+        self.fpga.run_jtag_commands(f"set_rx_pkt_win {rx_window}")
 
     @property
     def tx_window(self):
         return self._tx_window
 
     @tx_window.setter
     def tx_window(self, tx_window):
         self._tx_window = tx_window
-        self.fpga.run_jtag_commands(f'set_tx_pkt_win {tx_window}')
+        self.fpga.run_jtag_commands(f"set_tx_pkt_win {tx_window}")
 
     @property
     def nb_pcap_iters(self):
         return self._nb_pcap_iters
 
     @nb_pcap_iters.setter
     def nb_pcap_iters(self, nb_pcap_iters):
         self._nb_pcap_iters = nb_pcap_iters
-        self.fpga.run_jtag_commands(f'set_pkt_num {nb_pcap_iters}')
+        self.fpga.run_jtag_commands(f"set_pkt_num {nb_pcap_iters}")
 
     def get_top_stats(self):
-        self.fpga.jtag_console.send('get_top_stats\n')
+        self.fpga.jtag_console.send("get_top_stats\n")
         output = watch_command(
             self.fpga.jtag_console,
-            keyboard_int=lambda: self.fpga.jtag_console.send('\x03'),
-            stop_pattern='REG_OUT_PKT_23_FLIT'
+            keyboard_int=lambda: self.fpga.jtag_console.send("\x03"),
+            stop_pattern="REG_OUT_PKT_23_FLIT",
         )
 
-        lines = output.split('\n')
+        lines = output.split("\n")
 
         stats = {}
         for line in lines:
-            if ':' in line:
-                key, value = line.split(':')
-                if key.startswith('\x1b[?1l\x1b>\x1b[?2004l'):
-                    key = key.split('\x1b[?1l\x1b>\x1b[?2004l')[1]
+            if ":" in line:
+                key, value = line.split(":")
+                if key.startswith("\x1b[?1l\x1b>\x1b[?2004l"):
+                    key = key.split("\x1b[?1l\x1b>\x1b[?2004l")[1]
                 stats[key] = int(value)
 
         return stats
 
     def _get_single_xput(self, xput_type):
-        self.fpga.jtag_console.send(f'get_{xput_type}_xput\n')
+        self.fpga.jtag_console.send(f"get_{xput_type}_xput\n")
         output = watch_command(
             self.fpga.jtag_console,
-            keyboard_int=lambda: self.fpga.jtag_console.send('\x03'),
-            stop_pattern='\r\n% '
+            keyboard_int=lambda: self.fpga.jtag_console.send("\x03"),
+            stop_pattern="\r\n% ",
         )
 
-        lines = output.split('\n')
+        lines = output.split("\n")
         value = 0.0
 
         for line in lines:
-            if 'Gbps' in line:
-                if line.startswith('\x1b[?1l\x1b>\x1b[?2004l'):
-                    line = line.split('\x1b[?1l\x1b>\x1b[?2004l')[1]
-                value = float(line.split('Gbps')[0])
+            if "Gbps" in line:
+                if line.startswith("\x1b[?1l\x1b>\x1b[?2004l"):
+                    line = line.split("\x1b[?1l\x1b>\x1b[?2004l")[1]
+                value = float(line.split("Gbps")[0])
                 break
 
         return value
 
     def get_tx_xput(self):
-        return self._get_single_xput('tx')
+        return self._get_single_xput("tx")
 
     def get_rx_xput(self):
-        return self._get_single_xput('rx')
+        return self._get_single_xput("rx")
 
     def start(self):
-        self.fpga.run_jtag_commands('start')
+        self.fpga.run_jtag_commands("start")
 
     def stop(self):
-        self.fpga.run_jtag_commands('stop')
+        self.fpga.run_jtag_commands("stop")
 
     def clear(self):
-        self.fpga.run_jtag_commands('set_clear')
+        self.fpga.run_jtag_commands("set_clear")
 
         # need to reset config after clear
         self.rate = self._rate
         self.nb_flits_in_pcap = self._nb_flits_in_pcap
         self.rx_window = self._rx_window
         self.tx_window = self._tx_window
         self.nb_pcap_iters = self._nb_pcap_iters
```

### Comparing `netexp-0.1.9/netexp/throughput.py` & `netexp-0.2.0/netexp/throughput.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-
 from netexp.pktgen import Pktgen
+from typing import TextIO, Union
+
+import sys
 
 
-def zero_loss_throughput(pktgen: Pktgen, mean_pkt_size: int,
-                         max_throughput: int = 100_000_000_000,
-                         precision: int = 1_000_000_000,
-                         target_duration: int = 5) -> int:
+def zero_loss_throughput(
+    pktgen: Pktgen,
+    mean_pkt_size: int,
+    max_throughput: int = 100_000_000_000,
+    precision: int = 1_000_000_000,
+    target_duration: int = 5,
+    log_file: Union[bool, TextIO] = False,
+) -> int:
     """Find zero-loss throughput using a binary search.
 
     This assumes that the DUT is connected to the packet generator and ready to
     receive packets. The DUT should try to send back all packets that it
     receives and should not introduce new ones. The DUT is allowed to drop
     packets if it cannot keep up with the input throughput.
 
@@ -22,14 +28,17 @@
         target_duration: Target experiment duration (in seconds). The number of
           packets to be sent will be adjusted base on this and the current
           attempted throughput.
 
     Returns:
         The zero loss throughput found (in bps).
     """
+    if log_file is True:
+        log_file = sys.stdout
+
     def get_nb_pkts_for_throughput(throughput):
         pps = throughput / ((mean_pkt_size + 20) * 8)
         return int(pps * target_duration)
 
     tpt_lower = 0  # Lower bound.
     tpt_upper = max_throughput  # Upper bound.
 
@@ -37,28 +46,30 @@
     current_throughput = max_throughput
 
     # We iteratively refine the bounds until the difference between them is
     # less than the specified precision.
     while (tpt_upper - tpt_lower) > precision:
         nb_pkts = get_nb_pkts_for_throughput(current_throughput)
 
-        print(f'Trying {current_throughput // 1e6} Mbps with {nb_pkts} pkts.')
+        if log_file:
+            tpt_mbps = current_throughput // 1e6
+            log_file.write(f"Trying {tpt_mbps} Mbps with {nb_pkts} pkts.\n")
 
         pktgen.clean_stats()
         pktgen.start(current_throughput, nb_pkts)
         pktgen.wait_transmission_done()
 
         nb_rx_pkts = pktgen.get_nb_rx_pkts()
 
         if nb_rx_pkts < nb_pkts:
             tpt_upper = current_throughput
         elif nb_rx_pkts == nb_pkts:
             tpt_lower = current_throughput
         else:  # nb_rx_pkts > nb_pkts
             raise RuntimeError(
-                'Received more packets than sent. Measurement is unreliable.'
+                "Received more packets than sent. Measurement is unreliable."
             )
 
         current_throughput = (tpt_upper + tpt_lower) // 2
 
     # Found a rate.
     return tpt_lower
```

