# Comparing `tmp/nsqdriver-0.3.3-cp39-cp39-win_amd64.whl.zip` & `tmp/nsqdriver-0.4.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,25 @@
-Zip file size: 213527 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat     8137 b- defN 23-Jun-12 02:16 nsqdriver/NS_CST.py
--rw-rw-rw-  2.0 fat    20055 b- defN 23-Jun-12 02:16 nsqdriver/NS_MCI.py
--rw-rw-rw-  2.0 fat    23950 b- defN 23-Jun-12 02:16 nsqdriver/NS_QSYNC.py
--rw-rw-rw-  2.0 fat      381 b- defN 23-Jun-12 02:16 nsqdriver/__init__.py
--rw-rw-rw-  2.0 fat      519 b- defN 23-Jun-12 02:16 nsqdriver/common.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-12 02:16 nsqdriver/compiler/__init__.py
--rw-rw-rw-  2.0 fat   209920 b- defN 23-Jun-12 02:18 nsqdriver/compiler/ns_wave.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3991 b- defN 23-Jun-12 02:16 nsqdriver/compiler/ns_wave.pyi
--rw-rw-rw-  2.0 fat   228864 b- defN 23-Jun-12 02:18 nsqdriver/compiler/py_wave_asm.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      763 b- defN 23-Jun-12 02:16 nsqdriver/compiler/py_wave_asm.pyi
--rw-rw-rw-  2.0 fat    19745 b- defN 23-Jun-12 02:16 nsqdriver/wrapper/AWG_ADC.py
--rw-rw-rw-  2.0 fat    12555 b- defN 23-Jun-12 02:16 nsqdriver/wrapper/BD_NSMCI.py
--rw-rw-rw-  2.0 fat     6533 b- defN 23-Jun-12 02:16 nsqdriver/wrapper/ND_NSMCI.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-12 02:16 nsqdriver/wrapper/__init__.py
--rw-rw-rw-  2.0 fat     4418 b- defN 23-Jun-12 02:18 nsqdriver-0.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-12 02:18 nsqdriver-0.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-12 02:17 nsqdriver-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1506 b- defN 23-Jun-12 02:18 nsqdriver-0.3.3.dist-info/RECORD
-18 files, 541447 bytes uncompressed, 211061 bytes compressed:  61.0%
+Zip file size: 1293873 bytes, number of entries: 23
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 14:28 nsqdriver/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 14:28 nsqdriver-0.4.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 14:28 nsqdriver.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 14:28 nsqdriver/wrapper/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 14:28 nsqdriver/compiler/
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-15 14:28 nsqdriver/__init__.py
+-rw-r--r--  2.0 unx    19589 b- defN 23-Jun-15 14:28 nsqdriver/NS_MCI.py
+-rw-r--r--  2.0 unx     7877 b- defN 23-Jun-15 14:28 nsqdriver/NS_CST.py
+-rw-r--r--  2.0 unx    23281 b- defN 23-Jun-15 14:28 nsqdriver/NS_QSYNC.py
+-rw-r--r--  2.0 unx      499 b- defN 23-Jun-15 14:28 nsqdriver/common.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 14:28 nsqdriver/wrapper/__init__.py
+-rw-r--r--  2.0 unx    12245 b- defN 23-Jun-15 14:28 nsqdriver/wrapper/BD_NSMCI.py
+-rw-r--r--  2.0 unx     6288 b- defN 23-Jun-15 14:28 nsqdriver/wrapper/ND_NSMCI.py
+-rw-r--r--  2.0 unx    19211 b- defN 23-Jun-15 14:28 nsqdriver/wrapper/AWG_ADC.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 14:28 nsqdriver/compiler/__init__.py
+-rw-r--r--  2.0 unx     3824 b- defN 23-Jun-15 14:28 nsqdriver/compiler/ns_wave.pyi
+-rwxr-xr-x  2.0 unx  1729248 b- defN 23-Jun-15 14:28 nsqdriver/compiler/py_wave_asm.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      633 b- defN 23-Jun-15 14:28 nsqdriver/compiler/py_wave_asm.pyi
+-rwxr-xr-x  2.0 unx  1567184 b- defN 23-Jun-15 14:28 nsqdriver/compiler/ns_wave.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     4361 b- defN 23-Jun-15 14:28 nsqdriver-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-15 14:28 nsqdriver-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-15 14:28 nsqdriver-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1550 b- defN 23-Jun-15 14:28 nsqdriver-0.4.0.dist-info/RECORD
+23 files, 3396319 bytes uncompressed, 1290803 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -1,55 +1,70 @@
-Filename: nsqdriver/NS_CST.py
+Filename: nsqdriver/
 Comment: 
 
-Filename: nsqdriver/NS_MCI.py
+Filename: nsqdriver-0.4.0.dist-info/
 Comment: 
 
-Filename: nsqdriver/NS_QSYNC.py
+Filename: nsqdriver.libs/
 Comment: 
 
-Filename: nsqdriver/__init__.py
+Filename: nsqdriver/wrapper/
 Comment: 
 
-Filename: nsqdriver/common.py
+Filename: nsqdriver/compiler/
 Comment: 
 
-Filename: nsqdriver/compiler/__init__.py
+Filename: nsqdriver/__init__.py
 Comment: 
 
-Filename: nsqdriver/compiler/ns_wave.cp39-win_amd64.pyd
+Filename: nsqdriver/NS_MCI.py
 Comment: 
 
-Filename: nsqdriver/compiler/ns_wave.pyi
+Filename: nsqdriver/NS_CST.py
 Comment: 
 
-Filename: nsqdriver/compiler/py_wave_asm.cp39-win_amd64.pyd
+Filename: nsqdriver/NS_QSYNC.py
 Comment: 
 
-Filename: nsqdriver/compiler/py_wave_asm.pyi
+Filename: nsqdriver/common.py
 Comment: 
 
-Filename: nsqdriver/wrapper/AWG_ADC.py
+Filename: nsqdriver/wrapper/__init__.py
 Comment: 
 
 Filename: nsqdriver/wrapper/BD_NSMCI.py
 Comment: 
 
 Filename: nsqdriver/wrapper/ND_NSMCI.py
 Comment: 
 
-Filename: nsqdriver/wrapper/__init__.py
+Filename: nsqdriver/wrapper/AWG_ADC.py
+Comment: 
+
+Filename: nsqdriver/compiler/__init__.py
+Comment: 
+
+Filename: nsqdriver/compiler/ns_wave.pyi
+Comment: 
+
+Filename: nsqdriver/compiler/py_wave_asm.cpython-39-x86_64-linux-gnu.so
+Comment: 
+
+Filename: nsqdriver/compiler/py_wave_asm.pyi
+Comment: 
+
+Filename: nsqdriver/compiler/ns_wave.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: nsqdriver-0.3.3.dist-info/METADATA
+Filename: nsqdriver-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: nsqdriver-0.3.3.dist-info/WHEEL
+Filename: nsqdriver-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: nsqdriver-0.3.3.dist-info/top_level.txt
+Filename: nsqdriver-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: nsqdriver-0.3.3.dist-info/RECORD
+Filename: nsqdriver-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## nsqdriver/NS_CST.py

 * *Ordering differences only*

```diff
@@ -1,260 +1,260 @@
-import socket
-import struct
-import time
-from functools import lru_cache, wraps
-from typing import Union, TYPE_CHECKING, Tuple, Iterable
-
-try:
-    from .common import BaseDriver, Quantity
-except ImportError as e:
-    class BaseDriver:
-        def __init__(self, addr, timeout, **kw):
-            self.addr = addr
-            self.timeout = timeout
-
-
-    class Quantity(object):
-        def __init__(self, name: str, value=None, ch: int = 1, unit: str = ''):
-            self.name = name
-            self.default = dict(value=value, ch=ch, unit=unit)
-
-
-DEBUG_PRINT = False
-
-
-def print_debug(*args, **kwargs):
-    if DEBUG_PRINT:
-        print(*args, **kwargs)
-
-
-def retry(times):
-    def decorator(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            _times = times - 1
-            while not func(*args, **kwargs) and _times > 0:
-                _times -= 1
-            return _times != 0
-
-        return wrapper
-
-    return decorator
-
-
-class Driver(BaseDriver):
-    icd_head_mode = 0x51000009
-    icd_head_open = 0x5100000A
-    CHs = list(range(1, 17))
-
-    quants = [
-        Quantity('SAMode', value='manual'),  # set/get, 运行模式manual为手动，根据指令切换开关
-        Quantity('Strobe', value=1, ch=1),  # set/get, 选通开关通道，value为开关矩阵in口，ch为out口
-    ]
-
-    SystemParameter = {
-        'SAMode': 'manual',  # 运行模式manual为手动，根据指令切换开关
-        'StrobeList': [1, 9],
-    }
-
-    def __init__(self, addr: str = '', timeout: float = 10.0, **kw):
-        super().__init__(addr, timeout, **kw)
-        self.handle = None
-        self.model = 'NS_CST'  # 默认为设备名字
-        self.srate = None
-        self.gen_trig_num = 0
-        self.addr = addr
-
-        self.param = {'SAMode': 'manual'}
-        print_debug(f'CST: 实例化成功{addr}')
-
-    def open(self, **kw):
-        """!
-        输入IP打开设备，配置默认超时时间为5秒
-        打开设备时配置RFSoC采样时钟，采样时钟以参数定义
-        @param kw:
-        @return:
-        """
-        # 配置系统初始值
-        system_parameter = kw.get('system_parameter', {})
-        values = self.SystemParameter.copy()
-        values.update(system_parameter)
-        for name, value in values.items():
-            if value is not None:
-                self.set(name, value, 1)
-
-    def close(self, **kw):
-        """
-        关闭设备
-        """
-        # self.handle.release_dma()
-        # self.handle.close()
-        ...
-
-    def write(self, name: str, value, **kw):
-        channel = kw.get('ch', 1)
-        return self.set(name, value, channel)
-
-    def read(self, name: str, **kw):
-        channel = kw.get('ch', 1)
-        result = self.get(name, channel)
-        return result
-
-    def set(self, name, value=None, channel=1):
-        """!
-        设置设备属性
-        @param name:
-        @param value:
-        @param channel:
-        @return:
-        """
-        print_debug(f'CST: set操作被调用{name}')
-        if name == 'SAMode':
-            data = self.__fmt_cst_mode(
-                value
-            )
-            self._send_command(data, connect_timeout=2)
-        elif name == 'Strobe':
-            config = self.param['StrobeList']
-            if value not in [1, 2]:
-                raise ValueError(f'IN通道超界，不应为{value}，需要为1或2')
-            config[value-1] = channel
-            data = self.__fmt_cst_strobe(
-                config
-            )
-            self._send_command(data, connect_timeout=2)
-        elif name == 'UpdateFirmware':
-            self.update_firmware(value)
-
-        else:
-            self.param[name] = value
-
-    def get(self, name, channel=1, value=0):
-        """!
-        查询设备属性，获取数据
-        @param name:
-        @param channel:
-        @param value:
-        @return:
-        """
-        print_debug(f'CST: get操作被调用{name}')
-        return self.param.get(name, None)
-
-    def update_firmware(self, file_path, boards=None):
-        """!
-        固件更新
-
-        @param file_path: 固件路径
-        @param boards:
-        @return:
-        """
-        import os
-        if not os.path.exists(file_path):
-            raise ValueError(f'文件路径: {file_path} 不存在')
-        with open(file_path, 'rb') as fp:
-            cmd_data = self.__fmt_update_firmware(fp.read())
-        if not self._send_command(cmd_data):
-            print(f'qsync: 固件更新 执行失败')
-
-    def _connect(self, addr=None, port=5001, timeout=None):
-        """!
-        获取到指定ip的tcp连接
-
-        @param addr:
-        @param port:
-        @return:
-        """
-        timeout = self.timeout if timeout is None else timeout
-        addr = self.addr if addr is None else addr
-        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        sock.settimeout(timeout)
-        sock.connect((addr, port))
-        return sock
-
-    @retry(3)
-    def _send_command(self, data: Union[str, bytes], wait=0, addr=None, port=5001,
-                      check_feedback=True, return_fdk=False, connect_timeout=10):
-        """!
-        发送指定内容到后端
-
-        @param data: 指令内容
-        @param wait: 指令发送完成后，等待一段时间再接收反馈，阻塞式等待
-        @param addr: 后端IP
-        @param port: 后端端口
-        @param check_feedback: 是否解析反馈
-        @param connect_timeout:
-        @return:
-        """
-        command_bak = data
-        try:
-            sock = self._connect(addr=addr, port=port, timeout=connect_timeout)
-        except Exception as e:
-            print(f'device: {addr}无法连接 {e}')
-            return False
-
-        try:
-            sock.sendall(memoryview(data))
-
-            time.sleep(wait)
-            _feedback = sock.recv(20)
-            if check_feedback:
-                if not _feedback.startswith(b'\xcf\xcf\xcf\xcf'):
-                    print('返回指令包头错误')
-                    return False
-                if command_bak[4:8] != _feedback[4:8]:
-                    print(f'返回指令ID错误')
-                    return False
-                _feedback = struct.unpack('=IIIII', _feedback)
-                if _feedback[4] != 0:
-                    print('指令成功下发，但执行失败')
-                    return False
-        except Exception as e:
-            print(f'device: {addr}指令{command_bak[:4]}发送失败 {e}')
-            return False
-        finally:
-            sock.close()
-        return True
-
-    @lru_cache(maxsize=32)
-    def __fmt_cst_mode(self, mode):
-        cmd_pack = (
-            0x5F5F5F5F,
-            self.icd_head_mode,
-            0x00000000,
-            20,
-            0 if mode == 'manual' else 1
-        )
-
-        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack)
-
-    @lru_cache(maxsize=32)
-    def __fmt_cst_strobe(self, out_ch):
-        if out_ch[0] > 8:
-            raise ValueError(f'不能将IN1通道选通到OUT9~16')
-        if out_ch[1] <= 8:
-            raise ValueError(f'不能将IN2通道选通到OUT1~8')
-        cmd_pack = (
-            0x5F5F5F5F,
-            self.icd_head_open,
-            0x00000000,
-            20,
-            (1 << (out_ch[0] - 1)) + (1 << (out_ch[1]-1))
-        )
-
-        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack)
-
-    @staticmethod
-    def __fmt_update_firmware(file_data):
-        cmd_pack = (
-            0x5F5F5F5F,
-            0x31000006,
-            0x00000000,
-            16 + len(file_data),
-        )
-        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack) + file_data
-
-
-if __name__ == '__main__':
-    driver = Driver('192.168.1.241')
-    driver.open()
-    driver.set('Strobe', 1, 3)   # I1选通到OUT3，所有通道编号从1计数
-    driver.set('Strobe', 2, 9)   # I2选通到OUT9，OUT9为第二个模块的OUT1
+import socket
+import struct
+import time
+from functools import lru_cache, wraps
+from typing import Union, TYPE_CHECKING, Tuple, Iterable
+
+try:
+    from .common import BaseDriver, Quantity
+except ImportError as e:
+    class BaseDriver:
+        def __init__(self, addr, timeout, **kw):
+            self.addr = addr
+            self.timeout = timeout
+
+
+    class Quantity(object):
+        def __init__(self, name: str, value=None, ch: int = 1, unit: str = ''):
+            self.name = name
+            self.default = dict(value=value, ch=ch, unit=unit)
+
+
+DEBUG_PRINT = False
+
+
+def print_debug(*args, **kwargs):
+    if DEBUG_PRINT:
+        print(*args, **kwargs)
+
+
+def retry(times):
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            _times = times - 1
+            while not func(*args, **kwargs) and _times > 0:
+                _times -= 1
+            return _times != 0
+
+        return wrapper
+
+    return decorator
+
+
+class Driver(BaseDriver):
+    icd_head_mode = 0x51000009
+    icd_head_open = 0x5100000A
+    CHs = list(range(1, 17))
+
+    quants = [
+        Quantity('SAMode', value='manual'),  # set/get, 运行模式manual为手动，根据指令切换开关
+        Quantity('Strobe', value=1, ch=1),  # set/get, 选通开关通道，value为开关矩阵in口，ch为out口
+    ]
+
+    SystemParameter = {
+        'SAMode': 'manual',  # 运行模式manual为手动，根据指令切换开关
+        'StrobeList': [1, 9],
+    }
+
+    def __init__(self, addr: str = '', timeout: float = 10.0, **kw):
+        super().__init__(addr, timeout, **kw)
+        self.handle = None
+        self.model = 'NS_CST'  # 默认为设备名字
+        self.srate = None
+        self.gen_trig_num = 0
+        self.addr = addr
+
+        self.param = {'SAMode': 'manual'}
+        print_debug(f'CST: 实例化成功{addr}')
+
+    def open(self, **kw):
+        """!
+        输入IP打开设备，配置默认超时时间为5秒
+        打开设备时配置RFSoC采样时钟，采样时钟以参数定义
+        @param kw:
+        @return:
+        """
+        # 配置系统初始值
+        system_parameter = kw.get('system_parameter', {})
+        values = self.SystemParameter.copy()
+        values.update(system_parameter)
+        for name, value in values.items():
+            if value is not None:
+                self.set(name, value, 1)
+
+    def close(self, **kw):
+        """
+        关闭设备
+        """
+        # self.handle.release_dma()
+        # self.handle.close()
+        ...
+
+    def write(self, name: str, value, **kw):
+        channel = kw.get('ch', 1)
+        return self.set(name, value, channel)
+
+    def read(self, name: str, **kw):
+        channel = kw.get('ch', 1)
+        result = self.get(name, channel)
+        return result
+
+    def set(self, name, value=None, channel=1):
+        """!
+        设置设备属性
+        @param name:
+        @param value:
+        @param channel:
+        @return:
+        """
+        print_debug(f'CST: set操作被调用{name}')
+        if name == 'SAMode':
+            data = self.__fmt_cst_mode(
+                value
+            )
+            self._send_command(data, connect_timeout=2)
+        elif name == 'Strobe':
+            config = self.param['StrobeList']
+            if value not in [1, 2]:
+                raise ValueError(f'IN通道超界，不应为{value}，需要为1或2')
+            config[value-1] = channel
+            data = self.__fmt_cst_strobe(
+                config
+            )
+            self._send_command(data, connect_timeout=2)
+        elif name == 'UpdateFirmware':
+            self.update_firmware(value)
+
+        else:
+            self.param[name] = value
+
+    def get(self, name, channel=1, value=0):
+        """!
+        查询设备属性，获取数据
+        @param name:
+        @param channel:
+        @param value:
+        @return:
+        """
+        print_debug(f'CST: get操作被调用{name}')
+        return self.param.get(name, None)
+
+    def update_firmware(self, file_path, boards=None):
+        """!
+        固件更新
+
+        @param file_path: 固件路径
+        @param boards:
+        @return:
+        """
+        import os
+        if not os.path.exists(file_path):
+            raise ValueError(f'文件路径: {file_path} 不存在')
+        with open(file_path, 'rb') as fp:
+            cmd_data = self.__fmt_update_firmware(fp.read())
+        if not self._send_command(cmd_data):
+            print(f'qsync: 固件更新 执行失败')
+
+    def _connect(self, addr=None, port=5001, timeout=None):
+        """!
+        获取到指定ip的tcp连接
+
+        @param addr:
+        @param port:
+        @return:
+        """
+        timeout = self.timeout if timeout is None else timeout
+        addr = self.addr if addr is None else addr
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        sock.settimeout(timeout)
+        sock.connect((addr, port))
+        return sock
+
+    @retry(3)
+    def _send_command(self, data: Union[str, bytes], wait=0, addr=None, port=5001,
+                      check_feedback=True, return_fdk=False, connect_timeout=10):
+        """!
+        发送指定内容到后端
+
+        @param data: 指令内容
+        @param wait: 指令发送完成后，等待一段时间再接收反馈，阻塞式等待
+        @param addr: 后端IP
+        @param port: 后端端口
+        @param check_feedback: 是否解析反馈
+        @param connect_timeout:
+        @return:
+        """
+        command_bak = data
+        try:
+            sock = self._connect(addr=addr, port=port, timeout=connect_timeout)
+        except Exception as e:
+            print(f'device: {addr}无法连接 {e}')
+            return False
+
+        try:
+            sock.sendall(memoryview(data))
+
+            time.sleep(wait)
+            _feedback = sock.recv(20)
+            if check_feedback:
+                if not _feedback.startswith(b'\xcf\xcf\xcf\xcf'):
+                    print('返回指令包头错误')
+                    return False
+                if command_bak[4:8] != _feedback[4:8]:
+                    print(f'返回指令ID错误')
+                    return False
+                _feedback = struct.unpack('=IIIII', _feedback)
+                if _feedback[4] != 0:
+                    print('指令成功下发，但执行失败')
+                    return False
+        except Exception as e:
+            print(f'device: {addr}指令{command_bak[:4]}发送失败 {e}')
+            return False
+        finally:
+            sock.close()
+        return True
+
+    @lru_cache(maxsize=32)
+    def __fmt_cst_mode(self, mode):
+        cmd_pack = (
+            0x5F5F5F5F,
+            self.icd_head_mode,
+            0x00000000,
+            20,
+            0 if mode == 'manual' else 1
+        )
+
+        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack)
+
+    @lru_cache(maxsize=32)
+    def __fmt_cst_strobe(self, out_ch):
+        if out_ch[0] > 8:
+            raise ValueError(f'不能将IN1通道选通到OUT9~16')
+        if out_ch[1] <= 8:
+            raise ValueError(f'不能将IN2通道选通到OUT1~8')
+        cmd_pack = (
+            0x5F5F5F5F,
+            self.icd_head_open,
+            0x00000000,
+            20,
+            (1 << (out_ch[0] - 1)) + (1 << (out_ch[1]-1))
+        )
+
+        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack)
+
+    @staticmethod
+    def __fmt_update_firmware(file_data):
+        cmd_pack = (
+            0x5F5F5F5F,
+            0x31000006,
+            0x00000000,
+            16 + len(file_data),
+        )
+        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack) + file_data
+
+
+if __name__ == '__main__':
+    driver = Driver('192.168.1.241')
+    driver.open()
+    driver.set('Strobe', 1, 3)   # I1选通到OUT3，所有通道编号从1计数
+    driver.set('Strobe', 2, 9)   # I2选通到OUT9，OUT9为第二个模块的OUT1
```

## nsqdriver/NS_MCI.py

```diff
@@ -1,513 +1,517 @@
-import pickle
-import socket
-import atexit
-import struct
-import xmlrpc.client
-from xmlrpc.client import Transport
-from multiprocessing import shared_memory
-from functools import wraps
-
-import numpy as np
-import waveforms
-
-try:
-    from .common import BaseDriver, Quantity, get_coef
-except ImportError as e:
-    class BaseDriver:
-        def __init__(self, addr, timeout, **kw):
-            self.addr = addr
-            self.timeout = timeout
-
-
-    class Quantity(object):
-        def __init__(self, name: str, value=None, ch: int = 1, unit: str = ''):
-            self.name = name
-            self.default = dict(value=value, ch=ch, unit=unit)
-
-
-    def get_coef(*args):
-        return '', '', '', ''
-
-DEBUG_PRINT = False
-
-
-def print_debug(*args, **kwargs):
-    if DEBUG_PRINT:
-        print(*args, **kwargs)
-
-
-@atexit.register
-def global_system_exit():
-    """
-    关闭共享内存
-
-    :return:
-    """
-    SHARED_DEVICE_MEM.close()
-    SHARED_DEVICE_MEM.unlink()
-
-
-def solve_rpc_exception(func):
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        try:
-            return func(*args, **kwargs)
-        except xmlrpc.client.Fault as e:
-            print(f'************{args[0].__class__}: {args[0].addr}************')
-            print(f'远程函数报错: {e.faultString}')
-            print(args[0].handle.get_all_status())
-            print(f'远程函数报错: {e.faultString}')
-            print('*****************************')
-        except TimeoutError as e:
-            print(f'************{args[0].__class__}: {args[0].addr}************')
-            print(f'Driver报错: 无法连接到 {args[0].addr}\n请检查网络、设备开机状态、设备是否正在程序更新等')
-            print(f'{e}')
-            print('*****************************')
-            raise e
-        except socket.timeout as e:
-            print(f'************{args[0].__class__}: {args[0].addr}************')
-            print(f'Driver报错: 获取数据超时 {e}')
-            print(args[0].handle.get_all_status())
-            print('*****************************')
-
-    return wrapper
-
-
-class Driver(BaseDriver):
-    CHs = list(range(1, 25))
-
-    quants = [
-        Quantity('ReInit', value={}, ch=1),  # set/get, 设备重新初始化
-        # 采集运行参数
-        Quantity('Shot', value=1024, ch=1),  # set/get,运行次数
-        Quantity('PointNumber', value=16384, unit='point'),  # set/get,AD采样点数
-        Quantity('TriggerDelay', value=0, ch=1, unit='s'),  # set/get,AD采样延时
-        Quantity('FrequencyList', value=[], ch=1, unit='Hz'),  # set/get,解调频率列表，list，单位Hz
-        Quantity('PhaseList', value=[], ch=1, unit='Hz'),  # set/get,解调频率列表，list，单位Hz
-        Quantity('Coefficient', value=None, ch=1),
-        Quantity('DemodulationParam', value=None, ch=1),
-        Quantity('CaptureMode'),
-        Quantity('StartCapture'),  # set,开启采集（执行前复位）
-        Quantity('TraceIQ', ch=1),  # get,获取原始时域数据
-        # 返回：array(shot, point)
-        Quantity('IQ', ch=1),  # get,获取解调后数据,默认复数返回
-        # 系统参数，宏定义修改，open时下发
-        # 复数返回：array(shot,frequency)
-        # 实数返回：array(IQ,shot,frequency)
-
-        # 任意波形发生器
-        Quantity('Waveform', value=np.array([]), ch=1),  # set/get,下发原始波形数据
-        Quantity('Delay', value=0, ch=1),  # set/get,播放延时
-        Quantity('KeepAmp', value=0),  # set, 电平是否维持在波形最后一个值, 0：波形播放完成后归0，1：保持波形最后一个值，2:保持波形第一个值
-        Quantity('Biasing', value=0, ch=1),  # set, 播放延迟
-        Quantity('LinSpace', value=[0, 30e-6, 1000], ch=1),  # set/get, np.linspace函数，用于生成timeline
-        Quantity('Output', value=True, ch=1),  # set/get,播放通道开关设置
-        Quantity('GenWave', value=waveforms.Waveform(), ch=1),  # set/get, 设备接收waveform对象，根据waveform对象直接生成波形
-        # set/get, 设备接收IQ分离的waveform对象列表，根据waveform对象列表直接生成波形
-        Quantity('GenWaveIQ', value=[waveforms.Waveform(), waveforms.Waveform()], ch=1),
-        Quantity('MultiGenWave', value={1: np.ndarray([])}),  # 多通道波形同时下发
-        Quantity('EnableWaveCache', value=False),  # 是否开启waveform缓存
-        Quantity('PushWaveCache'),  # 使waveform缓存中的波形数据生效
-        # 混频相关配置
-        Quantity('EnableDAMixer', value=False, ch=1),  # DA通道混频模式开关
-        Quantity('MixingWave',),  # 修改完混频相关参数后，运行混频器
-        Quantity('DAIQRate', value=1e9, ch=1),  # 基带信号采样率
-        Quantity('DALOFreq', value=100e6, ch=1),  # 中频信号频率
-        Quantity('DALOPhase', value=0, ch=1),  # 基带信号相位，弧度制
-        Quantity('DASideband', value='lower', ch=1),  # 混频后取的边带
-        Quantity('DAWindow', value=None, ch=1),
-        # 基带信号升采样率时所使用的窗函数，默认不使用任何窗，
-        # 可选：None、boxcar、triang、blackman、hamming、hann、bartlett、flattop、parzen、bohman、blackmanharris、nuttall、
-        # barthann、cosine、exponential、tukey、taylor
-
-        # 内触发
-        Quantity('GenerateTrig', value=1e7, unit='ns'),  # set/get,触发周期单位ns，触发数量=shot
-        Quantity('UpdateFirmware', value='', ch=1),  # qsync固件更新
-    ]
-
-    SystemParameter = {
-        'MixMode': 2,  # Mix模式，1：第一奈奎斯特去； 2：第二奈奎斯特区
-        'PLLFreq': 100e6,  # 参考时钟频率, 单位为Hz
-        'RefClock': 'out',  # 参考时钟选择： ‘out’：外参考时钟；‘in’：内参考时钟
-        'ADrate': 4e9,  # AD采样率，单位Hz
-        'DArate': 6e9,  # DA采样率，单位Hz
-        'KeepAmp': 0,  # DA波形发射完毕后，保持最后一个值
-        'Delay': 0,  # 配置DA的原生Delay
-        'SegmentSampling': [],  # 配置分段采样
-        # 'EnableDAMixer': False,  # 默认关闭DA混频器
-        # 'DASideband': 'lower',  # da混频默认使用下边带
-    }
-
-    def __init__(self, addr: str = '', timeout: float = 10.0, **kw):
-        super().__init__(addr, timeout, **kw)
-        self.fast_rpc = None
-        self.handle = None
-        self.model = 'NS_MCI'  # 默认为设备名字
-        self.srate = 6.4e9
-        self.device_online = True
-        self.has_start_capture = False
-        self.backend_version = (0, 0, 0)
-        print_debug(f'Driver: 实例化成功{addr}')
-
-    @solve_rpc_exception
-    def open(self, **kw):
-        """
-        输入IP打开设备，配置默认超时时间为5秒
-        打开设备时配置RFSoC采样时钟，采样时钟以参数定义
-        """
-        tran = Transport(use_builtin_types=True)
-        tran.accept_gzip_encoding = False
-        self.handle = xmlrpc.client.ServerProxy(f'http://{self.addr}:10801', transport=tran, allow_none=True,
-                                                use_builtin_types=True)
-        self.fast_rpc = FastRPC(self.addr, self.timeout)
-        debug = kw.get('debug', False)
-        if debug:
-            return
-        print_debug('Driver: RPC句柄建立成功')
-        # 检查目标设备是否在位设备
-        result = self.init_device(**kw)
-        if result:
-            # 在共享内存中注册本设备的ip
-            SHARED_DEVICE_MEM.ip = self.addr
-            self._show_system_status()
-            print(f'{self.addr}开启成功')
-        elif result is None:
-            ...
-        else:
-            print(self.handle.get_all_status())
-
-    def init_device(self, **kw):
-        try:
-            self._connect(self.addr, timeout=1).close()
-        except:
-            print(f'Driver: {self.addr}不在位，请检查网络重新open')
-            self.device_online = False
-            return
-        # 此时会连接rfsoc的指令接收tcp server
-        result = True
-        result &= self.handle.start_command(self.timeout)
-        print_debug('Driver: 后端rfs网络连接成功')
-
-        # 配置系统初始值
-        system_parameter = kw.get('system_parameter', {})
-        values = self.SystemParameter.copy()
-        values.update(system_parameter)
-        for name, value in values.items():
-            if value is not None:
-                self.handle.rpc_set(name, value, 0, False)
-        print_debug('Driver: 后端参数配置成功')
-
-        # 系统开启前必须进行过一次初始化
-        result &= self.__init_system()
-        print_debug('Driver: 后端RF配置成功')
-        result &= self.handle.rpc_set('Reset')
-        print_debug('Driver: 后端缓存配置成功')
-        return result
-
-    @solve_rpc_exception
-    def close(self, **kw):
-        """
-        关闭设备
-        """
-        if getattr(self, 'handle', None) is not None:
-            self.handle.close()
-            self.handle = None
-        if getattr(self, 'fast_rpc', None) is not None:
-            self.fast_rpc = None
-
-    def write(self, name: str, value, **kw):
-        channel = kw.get('ch', 1)
-        if name in {'Coefficient'}:
-            data, f_list, numberOfPoints, phases = get_coef(value, 4e9)
-            self.set('DemodulationParam', data, channel)
-        elif name in {'CaptureMode', 'SystemSync', 'ResetTrig', 'TrigPeriod', 'TrigFrom'}:
-            pass
-        else:
-            return self.set(name, value, channel)
-
-    def read(self, name: str, **kw):
-        channel = kw.get('ch', 1)
-        result = self.get(name, channel)
-        return result
-
-    @solve_rpc_exception
-    def set(self, name, value=0, channel=1):
-        """
-        设置设备属性
-
-        :param name: 属性名
-                "Waveform"| "Amplitude" | "Offset"| "Output"
-        :param value: 属性值
-                "Waveform" --> 1d np.ndarray & -1 <= value <= 1
-                "Amplitude"| "Offset"| "Phase" --> float    dB | dB | °
-                “PRFNum”   采用内部PRF时，可以通过这个参数控制开启后prf的数量
-                "Output" --> bool
-        :param channel：通道号
-        """
-        if not self.device_online:
-            return
-        print_debug(f'Driver: set操作被调用{name}')
-        if name in {'UpdateFirmware'}:
-            self.update_firmware(value)
-            return
-        elif name in {'ReInit'}:
-            if not isinstance(value, dict):
-                value = {}
-            self.init_device(system_parameter=value)
-            return
-        elif name in {'CaptureMode', 'SystemSync', 'ResetTrig', 'TrigPeriod', 'TrigFrom'}:
-            return
-
-        value = RPCValueParser.dump(value)
-        if name in {'Waveform', 'GenWave', 'MultiGenWave', 'GenWaveIQ', 'DemodulationParam', 'Coefficient'}:
-            func = self.fast_rpc.rpc_set
-            name = 'GenWave' if name == 'Waveform' and value[0] == RPCValueParser.dump_tag_waveform else name
-        else:
-            func = self.handle.rpc_set
-
-        if self.has_start_capture and name == 'StartCapture':
-            return
-        self.has_start_capture = name == 'StartCapture'
-
-        if not func(name, value, channel):
-            raise xmlrpc.client.Fault(400, f'指令{name}执行失败, 请重新open板卡')
-
-    @solve_rpc_exception
-    def get(self, name, channel=1, value=0):
-        """
-        查询设备属性，获取数据
-
-        """
-        if not self.device_online:
-            return
-        print_debug(f'Driver: get操作被调用{name}')
-        self.has_start_capture = False
-
-        func = self.fast_rpc.rpc_get
-        tmp = func(name, channel, value)
-        tmp = RPCValueParser.load(tmp)
-        return tmp
-
-    def update_firmware(self, file_path, target='all'):
-        if not self.device_online:
-            return
-        import os
-        if not os.path.exists(file_path):
-            raise ValueError(f'文件路径: {file_path} 不存在')
-        with open(file_path, 'rb') as fp:
-            result = self.handle.update_rfs_firmware(fp.read(), target)
-        if result:
-            print(f'设备{self.addr} 固件更新成功，3s后设备自动重启')
-        else:
-            print(f'设备{self.addr} 固件更新失败')
-        return result
-
-    def __init_system(self):
-        version = self.get('Version')
-        if isinstance(version, dict):
-            for key in version:
-                key: str
-                if key.endswith('version'):
-                    version = version[key][1:].split('-')[0]
-                    version = tuple(int(v) for v in version.split('.'))
-                else:
-                    version = (0, 0, 0)
-        self.backend_version = version
-        if version >= (1, 2, 7):
-            return self.set('InitSystem')
-        else:
-            return self.__exec_command('初始化')
-
-    def __exec_command(self, button_name: str,
-                       need_feedback=True, file_name=None, check_feedback=True,
-                       callback=lambda *args: True, wait: int = 0):
-        flag = self.handle.execute_command(button_name, need_feedback, file_name, check_feedback)
-        if not flag:
-            print(f'设备{self.addr}-指令{button_name}执行失败')
-        return flag
-
-    def _connect(self, addr=None, port=5001, timeout=None):
-        """
-        获取到指定ip的tcp连接
-
-        :param addr:
-        :param port:
-        :return:
-        """
-        timeout = self.timeout if timeout is None else timeout
-        addr = self.addr if addr is None else addr
-        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        sock.settimeout(timeout)
-        sock.connect((addr, port))
-        return sock
-
-    def _show_system_status(self):
-        import json
-        keys = ['device_type', 'backend_version', 'ad_num', 'da_num', 'cpu_temp', 'memory_use']
-        status: dict = self.handle.get_all_status(False)
-        _string = [f'*********设备{self.addr}开启成功*********']
-        for key in keys:
-            _string.append(f'{key}: {status.get(key, "nan")}')
-        # for i in range(len(status['rfsoc_addr'])):
-        #     _string.append(f'sub_device{status["rfsoc_addr"][i]}: '
-        #                    f'{status["ref_clock_lock"][i]}{status["ref_clock_from"][i]}')
-        print('\n'.join(_string))
-
-
-class FastRPC:
-    def __init__(self, address, timeout):
-        self.addr = address
-        self.timeout = timeout
-
-    def connect(self):
-        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        sock.connect((self.addr, 10800))
-        sock.settimeout(self.timeout)
-        # sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, True)
-        # sock.ioctl(socket.SIO_KEEPALIVE_VALS, (1, 60 * 1000, 30 * 1000))
-        # sock.close()
-        return sock
-
-    def rpc_set(self, *param):
-        sock = self.connect()
-        a = pickle.dumps(param)
-        head = struct.pack('=IIII', *[0x5F5F5F5F, 0x32000001, 0, 16 + len(a)])
-        sock.sendall(head)
-        sock.sendall(a)
-        head = struct.unpack("=IIIII", sock.recv(20))
-        # print(head)
-        data = sock.recv(head[3] - 20)
-        data = pickle.loads(data)
-        if head[4]:
-            print(data)
-            return False
-        sock.close()
-        return data
-
-    def rpc_get(self, *param):
-        sock = self.connect()
-        a = pickle.dumps(param)
-        head = struct.pack('=IIII', *[0x5F5F5F5F, 0x32000002, 0, 16 + len(a)])
-        sock.sendall(head)
-        sock.sendall(a)
-        head = struct.unpack("=IIIII", sock.recv(20))
-        length = head[3] - 20
-        data = []
-        while length > 0:
-            _data = sock.recv(length)
-            length -= len(_data)
-            data.append(_data)
-        data = pickle.loads(b''.join(data))
-        if head[4]:
-            raise xmlrpc.client.Fault(400, data)
-        sock.close()
-        return data
-
-    def debug_param(self, *param):
-        sock = self.connect()
-        a = pickle.dumps(param)
-        head = struct.pack('=IIII', *[0x5F5F5F5F, 0x32000003, 0, 16 + len(a)])
-        sock.sendall(head)
-        sock.sendall(a)
-        head = struct.unpack("=IIIII", sock.recv(20))
-        length = head[3] - 20
-        data = []
-        while length > 0:
-            _data = sock.recv(length)
-            length -= len(_data)
-            data.append(_data)
-        data = pickle.loads(b''.join(data))
-        if head[4]:
-            print(data)
-            return False
-        sock.close()
-        return data
-
-
-class RPCValueParser:
-    """
-    rpc调用格式化工具集
-
-    """
-    dump_tag_waveform = 'waveform.Waveforms'
-    dump_tag_ndarray = 'numpy.ndarray'
-    dump_tag_complex = 'complex'
-
-    @staticmethod
-    def dump(value):
-        if isinstance(value, np.ndarray):
-            value = [RPCValueParser.dump_tag_ndarray, value.tobytes(), str(value.dtype), value.shape]
-        elif isinstance(value, float):
-            value = float(value)
-        elif isinstance(value, int):
-            value = int(value)
-        elif isinstance(value, np.uint):
-            value = int(value)
-        elif isinstance(value, complex):
-            value = [RPCValueParser.dump_tag_complex, value.real, value.imag]
-        elif isinstance(value, waveforms.Waveform):
-            value = [RPCValueParser.dump_tag_waveform, pickle.dumps(value)]
-        elif isinstance(value, (list, tuple)):
-            value = [RPCValueParser.dump(_v) for _v in value]
-
-        return value
-
-    @staticmethod
-    def load(value):
-        if isinstance(value, list) and len(value) >= 2:
-            if value[0] == RPCValueParser.dump_tag_ndarray:
-                data = np.frombuffer(value[1], dtype=value[2])
-                value = data.reshape(value[3])
-            # elif: value[0] == 'numpy.float'
-            elif value[0] == RPCValueParser.dump_tag_waveform:
-                value = pickle.loads(value[1])
-            elif value[0] == RPCValueParser.dump_tag_complex:
-                value = complex(value[1], value[2])
-            else:
-                value = [RPCValueParser.load(_v) for _v in value]
-        elif isinstance(value, (list, tuple)):
-            value = [RPCValueParser.load(_v) for _v in value]
-        return value
-
-
-class InfoSharedList:
-    memory_name = 'NS_DEVICE_MEMORY'
-    memory_size = 1024 ** 2
-    head_size = 32  # memory中前head_size的长度为头部预留信息
-
-    def __init__(self):
-        try:
-            self._memory = shared_memory.SharedMemory(name=self.memory_name, create=True, size=self.memory_size)
-        except FileExistsError:
-            self._memory = shared_memory.SharedMemory(name=self.memory_name, create=False, size=self.memory_size)
-
-    def clear_ip(self):
-        _exit_pkl = pickle.dumps(self.ip)
-        self._memory.buf[self.head_size:len(_exit_pkl) + self.head_size] = b'\x00' * len(_exit_pkl)
-
-    @property
-    def ip(self):
-        try:
-            return pickle.loads(self._memory.buf[self.head_size:])
-        except pickle.UnpicklingError:
-            return []
-
-    @ip.setter
-    def ip(self, value):
-        ips = self.ip
-        ips.append(value)
-        ips = list(set(ips))
-        _pkl = pickle.dumps(ips)
-        self._memory.buf[self.head_size:len(_pkl) + self.head_size] = _pkl
-
-    def close(self):
-        self._memory.close()
-
-    def unlink(self):
-        try:
-            self._memory.unlink()
-        except FileNotFoundError as e:
-            pass
-
-
-SHARED_DEVICE_MEM = InfoSharedList()
+import pickle
+import socket
+import atexit
+import struct
+import xmlrpc.client
+from xmlrpc.client import Transport
+from multiprocessing import shared_memory
+from functools import wraps
+
+import numpy as np
+try:
+    import waveforms
+    HAS_WAVEFORMS = True
+except ImportError as e:
+    HAS_WAVEFORMS = False
+
+try:
+    from .common import BaseDriver, Quantity, get_coef
+except ImportError as e:
+    class BaseDriver:
+        def __init__(self, addr, timeout, **kw):
+            self.addr = addr
+            self.timeout = timeout
+
+
+    class Quantity(object):
+        def __init__(self, name: str, value=None, ch: int = 1, unit: str = ''):
+            self.name = name
+            self.default = dict(value=value, ch=ch, unit=unit)
+
+
+    def get_coef(*args):
+        return '', '', '', ''
+
+DEBUG_PRINT = False
+
+
+def print_debug(*args, **kwargs):
+    if DEBUG_PRINT:
+        print(*args, **kwargs)
+
+
+@atexit.register
+def global_system_exit():
+    """
+    关闭共享内存
+
+    :return:
+    """
+    SHARED_DEVICE_MEM.close()
+    SHARED_DEVICE_MEM.unlink()
+
+
+def solve_rpc_exception(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except xmlrpc.client.Fault as e:
+            print(f'************{args[0].__class__}: {args[0].addr}************')
+            print(f'远程函数报错: {e.faultString}')
+            print(args[0].handle.get_all_status())
+            print(f'远程函数报错: {e.faultString}')
+            print('*****************************')
+        except TimeoutError as e:
+            print(f'************{args[0].__class__}: {args[0].addr}************')
+            print(f'Driver报错: 无法连接到 {args[0].addr}\n请检查网络、设备开机状态、设备是否正在程序更新等')
+            print(f'{e}')
+            print('*****************************')
+            raise e
+        except socket.timeout as e:
+            print(f'************{args[0].__class__}: {args[0].addr}************')
+            print(f'Driver报错: 获取数据超时 {e}')
+            print(args[0].handle.get_all_status())
+            print('*****************************')
+
+    return wrapper
+
+
+class Driver(BaseDriver):
+    CHs = list(range(1, 25))
+
+    quants = [
+        Quantity('ReInit', value={}, ch=1),  # set/get, 设备重新初始化
+        # 采集运行参数
+        Quantity('Shot', value=1024, ch=1),  # set/get,运行次数
+        Quantity('PointNumber', value=16384, unit='point'),  # set/get,AD采样点数
+        Quantity('TriggerDelay', value=0, ch=1, unit='s'),  # set/get,AD采样延时
+        Quantity('FrequencyList', value=[], ch=1, unit='Hz'),  # set/get,解调频率列表，list，单位Hz
+        Quantity('PhaseList', value=[], ch=1, unit='Hz'),  # set/get,解调频率列表，list，单位Hz
+        Quantity('Coefficient', value=None, ch=1),
+        Quantity('DemodulationParam', value=None, ch=1),
+        Quantity('CaptureMode'),
+        Quantity('StartCapture'),  # set,开启采集（执行前复位）
+        Quantity('TraceIQ', ch=1),  # get,获取原始时域数据
+        # 返回：array(shot, point)
+        Quantity('IQ', ch=1),  # get,获取解调后数据,默认复数返回
+        # 系统参数，宏定义修改，open时下发
+        # 复数返回：array(shot,frequency)
+        # 实数返回：array(IQ,shot,frequency)
+
+        # 任意波形发生器
+        Quantity('Waveform', value=np.array([]), ch=1),  # set/get,下发原始波形数据
+        Quantity('Delay', value=0, ch=1),  # set/get,播放延时
+        Quantity('KeepAmp', value=0),  # set, 电平是否维持在波形最后一个值, 0：波形播放完成后归0，1：保持波形最后一个值，2:保持波形第一个值
+        Quantity('Biasing', value=0, ch=1),  # set, 播放延迟
+        Quantity('LinSpace', value=[0, 30e-6, 1000], ch=1),  # set/get, np.linspace函数，用于生成timeline
+        Quantity('Output', value=True, ch=1),  # set/get,播放通道开关设置
+        Quantity('GenWave', value=None, ch=1),  # set/get, 设备接收waveform对象，根据waveform对象直接生成波形
+        # set/get, 设备接收IQ分离的waveform对象列表，根据waveform对象列表直接生成波形
+        Quantity('GenWaveIQ', value=None, ch=1),
+        Quantity('MultiGenWave', value={1: np.ndarray([])}),  # 多通道波形同时下发
+        Quantity('EnableWaveCache', value=False),  # 是否开启waveform缓存
+        Quantity('PushWaveCache'),  # 使waveform缓存中的波形数据生效
+        # 混频相关配置
+        Quantity('EnableDAMixer', value=False, ch=1),  # DA通道混频模式开关
+        Quantity('MixingWave',),  # 修改完混频相关参数后，运行混频器
+        Quantity('DAIQRate', value=1e9, ch=1),  # 基带信号采样率
+        Quantity('DALOFreq', value=100e6, ch=1),  # 中频信号频率
+        Quantity('DALOPhase', value=0, ch=1),  # 基带信号相位，弧度制
+        Quantity('DASideband', value='lower', ch=1),  # 混频后取的边带
+        Quantity('DAWindow', value=None, ch=1),
+        # 基带信号升采样率时所使用的窗函数，默认不使用任何窗，
+        # 可选：None、boxcar、triang、blackman、hamming、hann、bartlett、flattop、parzen、bohman、blackmanharris、nuttall、
+        # barthann、cosine、exponential、tukey、taylor
+
+        # 内触发
+        Quantity('GenerateTrig', value=1e7, unit='ns'),  # set/get,触发周期单位ns，触发数量=shot
+        Quantity('UpdateFirmware', value='', ch=1),  # qsync固件更新
+    ]
+
+    SystemParameter = {
+        'MixMode': 2,  # Mix模式，1：第一奈奎斯特去； 2：第二奈奎斯特区
+        'PLLFreq': 100e6,  # 参考时钟频率, 单位为Hz
+        'RefClock': 'out',  # 参考时钟选择： ‘out’：外参考时钟；‘in’：内参考时钟
+        'ADrate': 4e9,  # AD采样率，单位Hz
+        'DArate': 6e9,  # DA采样率，单位Hz
+        'KeepAmp': 0,  # DA波形发射完毕后，保持最后一个值
+        'Delay': 0,  # 配置DA的原生Delay
+        'SegmentSampling': [],  # 配置分段采样
+        # 'EnableDAMixer': False,  # 默认关闭DA混频器
+        # 'DASideband': 'lower',  # da混频默认使用下边带
+    }
+
+    def __init__(self, addr: str = '', timeout: float = 10.0, **kw):
+        super().__init__(addr, timeout, **kw)
+        self.fast_rpc = None
+        self.handle = None
+        self.model = 'NS_MCI'  # 默认为设备名字
+        self.srate = 6.4e9
+        self.device_online = True
+        self.has_start_capture = False
+        self.backend_version = (0, 0, 0)
+        print_debug(f'Driver: 实例化成功{addr}')
+
+    @solve_rpc_exception
+    def open(self, **kw):
+        """
+        输入IP打开设备，配置默认超时时间为5秒
+        打开设备时配置RFSoC采样时钟，采样时钟以参数定义
+        """
+        tran = Transport(use_builtin_types=True)
+        tran.accept_gzip_encoding = False
+        self.handle = xmlrpc.client.ServerProxy(f'http://{self.addr}:10801', transport=tran, allow_none=True,
+                                                use_builtin_types=True)
+        self.fast_rpc = FastRPC(self.addr, self.timeout)
+        debug = kw.get('debug', False)
+        if debug:
+            return
+        print_debug('Driver: RPC句柄建立成功')
+        # 检查目标设备是否在位设备
+        result = self.init_device(**kw)
+        if result:
+            # 在共享内存中注册本设备的ip
+            SHARED_DEVICE_MEM.ip = self.addr
+            self._show_system_status()
+            print(f'{self.addr}开启成功')
+        elif result is None:
+            ...
+        else:
+            print(self.handle.get_all_status())
+
+    def init_device(self, **kw):
+        try:
+            self._connect(self.addr, timeout=1).close()
+        except:
+            print(f'Driver: {self.addr}不在位，请检查网络重新open')
+            self.device_online = False
+            return
+        # 此时会连接rfsoc的指令接收tcp server
+        result = True
+        result &= self.handle.start_command(self.timeout)
+        print_debug('Driver: 后端rfs网络连接成功')
+
+        # 配置系统初始值
+        system_parameter = kw.get('system_parameter', {})
+        values = self.SystemParameter.copy()
+        values.update(system_parameter)
+        for name, value in values.items():
+            if value is not None:
+                self.handle.rpc_set(name, value, 0, False)
+        print_debug('Driver: 后端参数配置成功')
+
+        # 系统开启前必须进行过一次初始化
+        result &= self.__init_system()
+        print_debug('Driver: 后端RF配置成功')
+        result &= self.handle.rpc_set('Reset')
+        print_debug('Driver: 后端缓存配置成功')
+        return result
+
+    @solve_rpc_exception
+    def close(self, **kw):
+        """
+        关闭设备
+        """
+        if getattr(self, 'handle', None) is not None:
+            self.handle.close()
+            self.handle = None
+        if getattr(self, 'fast_rpc', None) is not None:
+            self.fast_rpc = None
+
+    def write(self, name: str, value, **kw):
+        channel = kw.get('ch', 1)
+        if name in {'Coefficient'}:
+            data, f_list, numberOfPoints, phases = get_coef(value, 4e9)
+            self.set('DemodulationParam', data, channel)
+        elif name in {'CaptureMode', 'SystemSync', 'ResetTrig', 'TrigPeriod', 'TrigFrom'}:
+            pass
+        else:
+            return self.set(name, value, channel)
+
+    def read(self, name: str, **kw):
+        channel = kw.get('ch', 1)
+        result = self.get(name, channel)
+        return result
+
+    @solve_rpc_exception
+    def set(self, name, value=0, channel=1):
+        """
+        设置设备属性
+
+        :param name: 属性名
+                "Waveform"| "Amplitude" | "Offset"| "Output"
+        :param value: 属性值
+                "Waveform" --> 1d np.ndarray & -1 <= value <= 1
+                "Amplitude"| "Offset"| "Phase" --> float    dB | dB | °
+                “PRFNum”   采用内部PRF时，可以通过这个参数控制开启后prf的数量
+                "Output" --> bool
+        :param channel：通道号
+        """
+        if not self.device_online:
+            return
+        print_debug(f'Driver: set操作被调用{name}')
+        if name in {'UpdateFirmware'}:
+            self.update_firmware(value)
+            return
+        elif name in {'ReInit'}:
+            if not isinstance(value, dict):
+                value = {}
+            self.init_device(system_parameter=value)
+            return
+        elif name in {'CaptureMode', 'SystemSync', 'ResetTrig', 'TrigPeriod', 'TrigFrom'}:
+            return
+
+        value = RPCValueParser.dump(value)
+        if name in {'Waveform', 'GenWave', 'MultiGenWave', 'GenWaveIQ', 'DemodulationParam', 'Coefficient'}:
+            func = self.fast_rpc.rpc_set
+            name = 'GenWave' if name == 'Waveform' and value[0] == RPCValueParser.dump_tag_waveform else name
+        else:
+            func = self.handle.rpc_set
+
+        if self.has_start_capture and name == 'StartCapture':
+            return
+        self.has_start_capture = name == 'StartCapture'
+
+        if not func(name, value, channel):
+            raise xmlrpc.client.Fault(400, f'指令{name}执行失败, 请重新open板卡')
+
+    @solve_rpc_exception
+    def get(self, name, channel=1, value=0):
+        """
+        查询设备属性，获取数据
+
+        """
+        if not self.device_online:
+            return
+        print_debug(f'Driver: get操作被调用{name}')
+        self.has_start_capture = False
+
+        func = self.fast_rpc.rpc_get
+        tmp = func(name, channel, value)
+        tmp = RPCValueParser.load(tmp)
+        return tmp
+
+    def update_firmware(self, file_path, target='all'):
+        if not self.device_online:
+            return
+        import os
+        if not os.path.exists(file_path):
+            raise ValueError(f'文件路径: {file_path} 不存在')
+        with open(file_path, 'rb') as fp:
+            result = self.handle.update_rfs_firmware(fp.read(), target)
+        if result:
+            print(f'设备{self.addr} 固件更新成功，3s后设备自动重启')
+        else:
+            print(f'设备{self.addr} 固件更新失败')
+        return result
+
+    def __init_system(self):
+        version = self.get('Version')
+        if isinstance(version, dict):
+            for key in version:
+                key: str
+                if key.endswith('version'):
+                    version = version[key][1:].split('-')[0]
+                    version = tuple(int(v) for v in version.split('.'))
+                else:
+                    version = (0, 0, 0)
+        self.backend_version = version
+        if version >= (1, 2, 7):
+            return self.set('InitSystem')
+        else:
+            return self.__exec_command('初始化')
+
+    def __exec_command(self, button_name: str,
+                       need_feedback=True, file_name=None, check_feedback=True,
+                       callback=lambda *args: True, wait: int = 0):
+        flag = self.handle.execute_command(button_name, need_feedback, file_name, check_feedback)
+        if not flag:
+            print(f'设备{self.addr}-指令{button_name}执行失败')
+        return flag
+
+    def _connect(self, addr=None, port=5001, timeout=None):
+        """
+        获取到指定ip的tcp连接
+
+        :param addr:
+        :param port:
+        :return:
+        """
+        timeout = self.timeout if timeout is None else timeout
+        addr = self.addr if addr is None else addr
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        sock.settimeout(timeout)
+        sock.connect((addr, port))
+        return sock
+
+    def _show_system_status(self):
+        import json
+        keys = ['device_type', 'backend_version', 'ad_num', 'da_num', 'cpu_temp', 'memory_use']
+        status: dict = self.handle.get_all_status(False)
+        _string = [f'*********设备{self.addr}开启成功*********']
+        for key in keys:
+            _string.append(f'{key}: {status.get(key, "nan")}')
+        # for i in range(len(status['rfsoc_addr'])):
+        #     _string.append(f'sub_device{status["rfsoc_addr"][i]}: '
+        #                    f'{status["ref_clock_lock"][i]}{status["ref_clock_from"][i]}')
+        print('\n'.join(_string))
+
+
+class FastRPC:
+    def __init__(self, address, timeout):
+        self.addr = address
+        self.timeout = timeout
+
+    def connect(self):
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        sock.connect((self.addr, 10800))
+        sock.settimeout(self.timeout)
+        # sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, True)
+        # sock.ioctl(socket.SIO_KEEPALIVE_VALS, (1, 60 * 1000, 30 * 1000))
+        # sock.close()
+        return sock
+
+    def rpc_set(self, *param):
+        sock = self.connect()
+        a = pickle.dumps(param)
+        head = struct.pack('=IIII', *[0x5F5F5F5F, 0x32000001, 0, 16 + len(a)])
+        sock.sendall(head)
+        sock.sendall(a)
+        head = struct.unpack("=IIIII", sock.recv(20))
+        # print(head)
+        data = sock.recv(head[3] - 20)
+        data = pickle.loads(data)
+        if head[4]:
+            print(data)
+            return False
+        sock.close()
+        return data
+
+    def rpc_get(self, *param):
+        sock = self.connect()
+        a = pickle.dumps(param)
+        head = struct.pack('=IIII', *[0x5F5F5F5F, 0x32000002, 0, 16 + len(a)])
+        sock.sendall(head)
+        sock.sendall(a)
+        head = struct.unpack("=IIIII", sock.recv(20))
+        length = head[3] - 20
+        data = []
+        while length > 0:
+            _data = sock.recv(length)
+            length -= len(_data)
+            data.append(_data)
+        data = pickle.loads(b''.join(data))
+        if head[4]:
+            raise xmlrpc.client.Fault(400, data)
+        sock.close()
+        return data
+
+    def debug_param(self, *param):
+        sock = self.connect()
+        a = pickle.dumps(param)
+        head = struct.pack('=IIII', *[0x5F5F5F5F, 0x32000003, 0, 16 + len(a)])
+        sock.sendall(head)
+        sock.sendall(a)
+        head = struct.unpack("=IIIII", sock.recv(20))
+        length = head[3] - 20
+        data = []
+        while length > 0:
+            _data = sock.recv(length)
+            length -= len(_data)
+            data.append(_data)
+        data = pickle.loads(b''.join(data))
+        if head[4]:
+            print(data)
+            return False
+        sock.close()
+        return data
+
+
+class RPCValueParser:
+    """
+    rpc调用格式化工具集
+
+    """
+    dump_tag_waveform = 'waveform.Waveforms'
+    dump_tag_ndarray = 'numpy.ndarray'
+    dump_tag_complex = 'complex'
+
+    @staticmethod
+    def dump(value):
+        if isinstance(value, np.ndarray):
+            value = [RPCValueParser.dump_tag_ndarray, value.tobytes(), str(value.dtype), value.shape]
+        elif isinstance(value, float):
+            value = float(value)
+        elif isinstance(value, int):
+            value = int(value)
+        elif isinstance(value, np.uint):
+            value = int(value)
+        elif isinstance(value, complex):
+            value = [RPCValueParser.dump_tag_complex, value.real, value.imag]
+        elif HAS_WAVEFORMS and isinstance(value, waveforms.Waveform):
+            value = [RPCValueParser.dump_tag_waveform, pickle.dumps(value)]
+        elif isinstance(value, (list, tuple)):
+            value = [RPCValueParser.dump(_v) for _v in value]
+
+        return value
+
+    @staticmethod
+    def load(value):
+        if isinstance(value, list) and len(value) >= 2:
+            if value[0] == RPCValueParser.dump_tag_ndarray:
+                data = np.frombuffer(value[1], dtype=value[2])
+                value = data.reshape(value[3])
+            # elif: value[0] == 'numpy.float'
+            elif value[0] == RPCValueParser.dump_tag_waveform:
+                value = pickle.loads(value[1])
+            elif value[0] == RPCValueParser.dump_tag_complex:
+                value = complex(value[1], value[2])
+            else:
+                value = [RPCValueParser.load(_v) for _v in value]
+        elif isinstance(value, (list, tuple)):
+            value = [RPCValueParser.load(_v) for _v in value]
+        return value
+
+
+class InfoSharedList:
+    memory_name = 'NS_DEVICE_MEMORY'
+    memory_size = 1024 ** 2
+    head_size = 32  # memory中前head_size的长度为头部预留信息
+
+    def __init__(self):
+        try:
+            self._memory = shared_memory.SharedMemory(name=self.memory_name, create=True, size=self.memory_size)
+        except FileExistsError:
+            self._memory = shared_memory.SharedMemory(name=self.memory_name, create=False, size=self.memory_size)
+
+    def clear_ip(self):
+        _exit_pkl = pickle.dumps(self.ip)
+        self._memory.buf[self.head_size:len(_exit_pkl) + self.head_size] = b'\x00' * len(_exit_pkl)
+
+    @property
+    def ip(self):
+        try:
+            return pickle.loads(self._memory.buf[self.head_size:])
+        except pickle.UnpicklingError:
+            return []
+
+    @ip.setter
+    def ip(self, value):
+        ips = self.ip
+        ips.append(value)
+        ips = list(set(ips))
+        _pkl = pickle.dumps(ips)
+        self._memory.buf[self.head_size:len(_pkl) + self.head_size] = _pkl
+
+    def close(self):
+        self._memory.close()
+
+    def unlink(self):
+        try:
+            self._memory.unlink()
+        except FileNotFoundError as e:
+            pass
+
+
+SHARED_DEVICE_MEM = InfoSharedList()
```

## nsqdriver/NS_QSYNC.py

 * *Ordering differences only*

```diff
@@ -1,669 +1,669 @@
-import atexit
-import socket
-import struct
-import threading
-import time
-import enum
-import pickle
-from concurrent.futures import ThreadPoolExecutor
-from concurrent.futures import wait as wait_futures
-from multiprocessing import shared_memory
-from functools import lru_cache, wraps
-from typing import Union, TYPE_CHECKING, Tuple, Iterable
-
-try:
-    from .common import BaseDriver, Quantity, QInteger
-except ImportError as e:
-    class BaseDriver:
-        def __init__(self, addr, timeout, **kw):
-            self.addr = addr
-            self.timeout = timeout
-
-
-    class Quantity(object):
-        def __init__(self, name: str, value=None, ch: int = 1, unit: str = ''):
-            self.name = name
-            self.default = dict(value=value, ch=ch, unit=unit)
-
-
-    class QInteger:
-        def __init__(self, name, value=None, unit='', ch=None,
-                     get_cmd='', set_cmd='', ):
-            self.name = name
-
-
-if TYPE_CHECKING:
-    from backend.board_parser import MCIBoard
-    from concurrent.futures import Future
-
-THREAD_POOL = ThreadPoolExecutor(max_workers=10)
-_scanning_lock = threading.Lock()
-_scanning_stop_event = threading.Event()
-DEVICE_SET = set()
-
-DEBUG_PRINT = False
-
-
-def print_debug(*args, **kwargs):
-    if DEBUG_PRINT:
-        print(*args, **kwargs)
-
-
-@atexit.register
-def global_system_exit():
-    THREAD_POOL.shutdown(wait=False)
-    SHARED_DEVICE_MEM.close()
-    try:
-        SHARED_DEVICE_MEM.unlink()
-    except FileNotFoundError as e:
-        pass
-
-
-def retry(times):
-    def decorator(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            _times = times-1
-            while not func(*args, **kwargs) and _times > 0:
-                _times -= 1
-            return _times != 0
-        return wrapper
-    return decorator
-
-
-class Driver(BaseDriver):
-    class ScannMode(enum.IntEnum):
-        """!
-        @detail QC/QR等被同步设备的发现方式，'local': 本地共享内存扫描， 'remote': 网络udp扫描
-        """
-        local = 0
-        """local: 本地共享内存扫描
-
-        - NS_MCI中的Driver每实例化一次，就会在SharedMemory中记录一次自己的ip
-        - 系统进行同步时，会对SharedMemory中记录的QC/QR设备ip进行同步
-        - 只有程序整体退出的时候才会清空这片缓存
-        """
-        remote = 1
-        """remote: 网络udp扫描
-
-        - import 本文件后，会建立一个独立线程间断广播UDP包，扫描局域网内的QC/QR设备，记录被扫描到的设备ip
-        - 系统进行同步时，会对扫描到的QC/QR设备ip进行同步
-        - 注意：这种方式比较粗暴，会影响局域网内正在运行的设备
-        """
-        alone = 2
-        """alone: 单机运行模式
-
-        - QC/QR设备单独运行时使用本模式，默认使用QC/QR设备板内的QSYNC做设备内的系统同步
-        - 系统进行同步时，会判断QSYNC Driver的ip是否为QC/QR设备的ip
-        """
-
-    _scanning_lock = _scanning_lock
-    _device_set = DEVICE_SET
-
-    icd_head_reset = 0x41000002
-    icd_head_status = 0x4100000E
-    icd_head_cmd_2 = 0x31000015
-    icd_head_cmd_3 = 0x410000B1
-    icd_head_cmd_4 = 0x31000013
-    icd_head_cmd_5 = 0x410000B2
-    icd_head_cmd_6 = 0x3100001A
-    icd_head_cmd_7 = 0x410000B3
-    CHs = list(range(1, 17))
-
-    quants = [
-        QInteger('TRIG'),
-        Quantity('SystemSync', value=None, ch=1),  # set/get,运行次数
-        Quantity('GenerateTrig', value=None, unit='s'),  # set/get,触发周期单位s，触发数量=shot
-        Quantity('ResetTrig', value=None),
-        Quantity('Shot', value=1024, ch=1),  # set/get, 运行次数
-        Quantity('TrigPeriod', value=200e-6, ch=1),  # set/get, 触发周期
-        Quantity('TrigWidth', value=800e-9, ch=1),  # set/get, 触发周期
-        Quantity('TrigDelay', value=0, ch=1),  # set/get, 触发周期
-        Quantity('TrigFrom', value=0, ch=1),  # Trig来源： 0：内部产生；1：外部输入
-        Quantity('RefClock', value='out', ch=1),  # 参考时钟选择： ‘out’：外参考时钟；‘in’：内参考时钟
-        Quantity('DiscoveryMode', value=ScannMode.local, ch=1),  # QC/QR等被同步设备的发现方式，见DiscoveryMode说明
-        Quantity('UpdateFirmware', value='', ch=1),  # qsync固件更新
-    ]
-
-    SystemParameter = {
-        'RefClock': 'out',  # 参考时钟选择： ‘out’：外参考时钟；‘in’：内参考时钟
-        'TrigFrom': 0,  # Trig来源： 0：内部产生；1：外部输入
-        'TrigPeriod': 200e-6,  # 触发信号重复周期
-        'TrigWidth': 800e-9,  # 触发信号高电平宽度 单位s
-        'TrigDelay': 0,  # 触发信号相对开启通知的延迟
-        'DiscoveryMode': ScannMode.local,  # QC/QR等被同步设备的发现方式，见DiscoveryMode说明
-    }
-
-    def __init__(self, addr: str = '', timeout: float = 10.0, **kw):
-        super().__init__(addr, timeout, **kw)
-        self.handle = None
-        self.model = 'NS_QSYNC'  # 默认为设备名字
-        self.srate = None
-        self.gen_trig_num = 0
-        self.addr = addr
-
-        self.param = {'Shot': 1024, 'period': 200e-6, 'MixMode': 2}
-        print_debug(f'QSYNC: 实例化成功{addr}')
-
-    @property
-    def device_set(self):
-        mode = self.param.get('DiscoveryMode', self.ScannMode.local)
-        if mode is self.ScannMode.local:
-            return set(SHARED_DEVICE_MEM.ip)
-        elif mode is self.ScannMode.alone:
-            if self.addr in SHARED_DEVICE_MEM.ip:
-                return {self.addr}
-            else:
-                raise RuntimeError('qsync处于alone模式下，只能控制QC/QR内的qsync，请确认对应QC/QR设备是否已经open成功')
-        elif mode is self.ScannMode.remote:
-            return self._device_set.copy()
-        else:
-            return set()
-
-    def open(self, **kw):
-        """!
-        输入IP打开设备，配置默认超时时间为5秒
-        打开设备时配置RFSoC采样时钟，采样时钟以参数定义
-        @param kw:
-        @return:
-        """
-        # 配置系统初始值
-        system_parameter = kw.get('system_parameter', {})
-        values = self.SystemParameter.copy()
-        values.update(system_parameter)
-        for name, value in values.items():
-            if value is not None:
-                self.set(name, value, 1)
-
-        # self.sync_system()
-        status = self.get('Status')
-        print(f'*********QSYNC{self.addr}开启成功*********\n'
-              f'core_temp: {status[0]}℃\n'
-              f'10M_locked: {status[1] if len(status) > 1 else "nan"}')
-        print(f'qsync {self.addr} opened successfully')
-
-    def close(self, **kw):
-        """
-        关闭设备
-        """
-        # self.handle.release_dma()
-        # self.handle.close()
-        ...
-
-    def write(self, name: str, value, **kw):
-        channel = kw.get('ch', 1)
-        return self.set(name, value, channel)
-
-    def read(self, name: str, **kw):
-        channel = kw.get('ch', 1)
-        result = self.get(name, channel)
-        return result
-
-    def set(self, name, value=None, channel=1):
-        """!
-        设置设备属性
-        @param name:
-        @param value:
-        @param channel:
-        @return:
-        """
-        print_debug(f'QSYNC: set操作被调用{name}')
-        if name in {'SystemSync', 'ReInit'}:
-            self.sync_system()
-        elif name == 'TRIG':
-            value = self.param['TrigPeriod']
-            data = self.__fmt_qsync_start(
-                self.param['TrigFrom'], value, self.param['Shot'],
-                self.param['TrigWidth'], self.param['TrigDelay']
-            )
-            self._send_command(data, connect_timeout=2)
-            self.gen_trig_num += 1
-        elif name == 'GenerateTrig':
-            value = self.param['TrigPeriod'] if value is None else value
-            data = self.__fmt_qsync_start(
-                self.param['TrigFrom'], value, self.param['Shot'],
-                self.param['TrigWidth'], self.param['TrigDelay']
-            )
-            self._send_command(data, connect_timeout=2)
-            self.gen_trig_num += 1
-        elif name == 'ResetTrig':
-            data = self.__fmt_qsync_common(self.icd_head_reset)
-            self._send_command(data)
-        elif name == 'RefClock':
-            self.change_ref(value)
-        elif name == 'UpdateFirmware':
-            self.update_firmware(value)
-
-        else:
-            self.param[name] = value
-
-    def get(self, name, channel=1, value=0):
-        """!
-        查询设备属性，获取数据
-        @param name:
-        @param channel:
-        @param value:
-        @return:
-        """
-        print_debug(f'QSYNC: get操作被调用{name}')
-        if name == 'Status':
-            cmd_data = self.__fmt_qsync_common(self.icd_head_status)
-            data = DeviceCmdHandle.send_command(cmd_data, addr=self.addr, return_fdk=True)
-            data = struct.unpack('I' * (len(data) // 4), data)
-            return data
-        return self.param.get(name, None)
-
-    def sync_system(self):
-        """
-        全系统同步流程
-
-        :return:
-        """
-        if Driver._scanning_lock.acquire(timeout=10):
-            Driver._scanning_lock.release()
-        if len(self.device_set) == 0:
-            return
-
-        data = self.__fmt_qsync_common(self.icd_head_reset)
-        self._send_command(data)
-
-        result = True
-        if self.param.get('DiscoveryMode', self.ScannMode.local) != self.ScannMode.alone:
-            data = self.__fmt_qsync_common(self.icd_head_reset)
-            result &= self._sendto_fake_qsync(data)
-            data = self.__fmt_qsync_ref_from('out')
-            result &= self._sendto_fake_qsync(data)
-        result &= self._sendto_device(self.icd_head_cmd_2)
-        result &= self._sendto_qsync(self.icd_head_cmd_3)
-        result &= self._sendto_device(self.icd_head_cmd_4)
-        result &= self._sendto_qsync(self.icd_head_cmd_5)
-        result &= self._sendto_device(self.icd_head_cmd_6, 30)
-        result &= self._sendto_qsync(self.icd_head_cmd_7)
-
-        print(f'System synchronization {"succeeded" if result else "FAILED"}')
-
-    def change_ref(self, value='out'):
-        self.param['RefClock'] = value
-        self.set('ResetTrig')
-        data = self.__fmt_qsync_ref_from(value)
-        self._send_command(data)
-
-    def _sendto_device(self, cmd_head, timeout=2):
-        """!
-        将指令发送给设备
-        @param cmd_head:
-        @param timeout:
-        @return:
-        """
-        cmd_data = self.__fmt_qsync_common(cmd_head)
-        devices = list(self.device_set)
-        futures = [
-            THREAD_POOL.submit(DeviceCmdHandle.send_command, cmd_data, 0, addr, 5000, True, False, timeout)
-            for addr in devices
-        ]
-        wait_futures(futures)
-        result = all(future.result() for future in futures)
-        for idx, future in enumerate(futures):
-            if not future.result():
-                print(f'device: {devices[idx]}系统同步过程 {hex(cmd_head)} 执行失败')
-        return result
-
-    def _sendto_fake_qsync(self, cmd_data, timeout=2):
-        devices = list(self.device_set)
-        futures = [
-            THREAD_POOL.submit(self._send_command, cmd_data, 0, addr, 5001, True, False, timeout)
-            for addr in devices if addr != self.addr
-        ]
-        wait_futures(futures)
-        result = all(future.result() for future in futures)
-        for idx, future in enumerate(futures):
-            if not future.result():
-                print(f'device: {devices[idx]}系统同步过程 {cmd_data[4:12]} 执行失败')
-        return result
-
-    def _sendto_qsync(self, cmd_head: int):
-        """!
-        将指令发送给qsync
-
-        @param cmd_head:
-        @return:
-        """
-        cmd_data = self.__fmt_qsync_common(cmd_head)
-        if not self._send_command(cmd_data, connect_timeout=2):
-            print(f'qsync: 系统同步过程 {hex(cmd_head)} 执行失败')
-            return False
-        return True
-
-    def update_firmware(self, file_path, boards=None):
-        """!
-        固件更新
-
-        @param file_path: 固件路径
-        @param boards:
-        @return:
-        """
-        import os
-        if not os.path.exists(file_path):
-            raise ValueError(f'文件路径: {file_path} 不存在')
-        with open(file_path, 'rb') as fp:
-            cmd_data = self.__fmt_update_firmware(fp.read())
-        if not self._send_command(cmd_data):
-            print(f'qsync: 固件更新 执行失败')
-
-    def _connect(self, addr=None, port=5001, timeout=None):
-        """!
-        获取到指定ip的tcp连接
-
-        @param addr:
-        @param port:
-        @return:
-        """
-        timeout = self.timeout if timeout is None else timeout
-        addr = self.addr if addr is None else addr
-        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        sock.settimeout(timeout)
-        sock.connect((addr, port))
-        return sock
-
-    @retry(3)
-    def _send_command(self, data: Union[str, bytes], wait=0, addr=None, port=5001,
-                      check_feedback=True, return_fdk=False, connect_timeout=10):
-        """!
-        发送指定内容到后端
-
-        @param data: 指令内容
-        @param wait: 指令发送完成后，等待一段时间再接收反馈，阻塞式等待
-        @param addr: 后端IP
-        @param port: 后端端口
-        @param check_feedback: 是否解析反馈
-        @param connect_timeout:
-        @return:
-        """
-        command_bak = data
-        try:
-            sock = self._connect(addr=addr, port=port, timeout=connect_timeout)
-        except Exception as e:
-            print(f'device: {addr}无法连接 {e}')
-            return False
-
-        try:
-            sock.sendall(memoryview(data))
-
-            time.sleep(wait)
-            _feedback = sock.recv(20)
-            if check_feedback:
-                if not _feedback.startswith(b'\xcf\xcf\xcf\xcf'):
-                    print('返回指令包头错误')
-                    return False
-                if command_bak[4:8] != _feedback[4:8]:
-                    print('返回指令ID错误')
-                    return False
-                # print(_feedback)
-                _feedback = struct.unpack('=IIIII', _feedback)
-                if _feedback[4] != 0:
-                    print('指令成功下发，但执行失败')
-                    return False
-        except Exception as e:
-            print(f'device: {addr}指令{command_bak[:4]}发送失败 {e}')
-            return False
-        finally:
-            sock.close()
-        return True
-
-    @lru_cache(maxsize=32)
-    def __fmt_qsync_common(self, head):
-        cmd_pack = (
-            0x5F5F5F5F,
-            head,
-            0x00000000,
-            16,
-        )
-
-        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack)
-
-    @lru_cache(maxsize=16)
-    def __fmt_qsync_ref_from(self, _from):
-        if _from == 'in':
-            _from = 0
-        elif _from == 'out':
-            _from = 1
-        else:
-            _from = 0
-        cmd_pack = (
-            0x5F5F5F5F,
-            0x4100000F,
-            0x00000000,
-            20,
-            _from
-        )
-
-        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack)
-
-    @lru_cache(maxsize=32)
-    def __fmt_qsync_start(self, src, period, shots, width, delay):
-        cmd_pack = (
-            0x5F5F5F5F,
-            0x41000001,
-            0x00000000,
-            36,
-            int(src),
-            int(period * 1e9) & 0xFFFFFFFF,
-            int(shots),
-            int(width * 1e9) & 0xFFFFFFFF,
-            int(delay * 1e9) & 0xFFFFFFFF
-        )
-
-        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack)
-
-    @staticmethod
-    def __fmt_update_firmware(file_data):
-        cmd_pack = (
-            0x5F5F5F5F,
-            0x31000006,
-            0x00000000,
-            16 + len(file_data),
-        )
-        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack) + file_data
-
-    # DG645兼容
-    def Trigger_singleshot(self):
-        self.set('GenerateTrig')
-
-    def Convention_init(self, rate=5000, **kwds):
-        self.set('ResetTrig')
-        self.set('Shot', 0xFFFFFFFF)
-        self.set('TrigPeriod', 1 / rate)
-        self.set('GenerateTrig')
-
-    def BurstMode_init(self, count=2048, delay=200e-6, period=200e-6, source=0, **kwds):
-        self.set('ResetTrig')
-        self.set('Shot', count)
-        self.set('TrigPeriod', period)
-        self.set('TrigDelay', delay)
-        self.set('TrigFrom', source)
-
-    def startGun(self):
-        self.Trigger_singleshot()
-
-
-def do_scanning():
-    """
-    扫描板卡
-
-    :return:
-    """
-    while True:
-        dest = ('<broadcast>', 5003)
-        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        s.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
-        addrs = socket.getaddrinfo(socket.gethostname(), None)
-        addr = [addr[4][0] for addr in addrs if addr[4][0].startswith('192.168.1.')]
-        _bind = False
-        _port = 15000
-        with _scanning_lock:
-            while not _bind:
-                try:
-                    s.bind((addr[0], _port))
-                    _bind = True
-                except Exception as e:
-                    _port += 1
-                    if _port >= 30000:
-                        raise e
-            s.sendto(b"____\x20\x00\x002\x00\x00\x00\x00\x14\x00\x00\x00\x00\x00\x00\x00", dest)
-            s.settimeout(3)
-
-            try:
-                while True:
-                    (feedback, _addr) = s.recvfrom(20)
-                    if feedback:
-                        DEVICE_SET.add(_addr[0])
-            except Exception as e:
-                s.close()
-        time.sleep(5)
-
-
-class DeviceCmdHandle:
-    """!
-    @brief 封装与QC/QR设备间的交互
-    """
-    error_map = {b'\x1a\x00\x001': {1: '指令Resync执行失败',
-                                    2: 'REFCLK not Detected',
-                                    3: 'Clock Maybe unstable, DAC Settings Error',
-                                    4: 'Clock Maybe unstable, ADC Settings Error',
-                                    5: 'SYSREF(External TRIG) not Detected, MTS failed / Sample Rate not Support',
-                                    7: 'ADC Calibration Failed'}
-                 }
-
-    @staticmethod
-    def packing_result(boards: Iterable["MCIBoard"],
-                       futures: Iterable["Future"],
-                       cmd_data: memoryview,
-                       head: bytes) -> Tuple[bytes, list]:
-        res = []
-        errors = []
-        for board, future in zip(boards, futures):
-            if board.has_ip and board.has_dma:
-                _id = (board.dma_id & 0xFF) << 24
-                _res = struct.unpack('IIIII', future.result())[-1] & 0xFFFFFF
-                if _res:
-                    errors.append(f'指令{cmd_data[4:8].tobytes()}向{board.board_ip}转发失败\n')
-                res.append(_id + _res)
-        return b''.join((head, cmd_data[4:12], struct.pack('=I' + 'I' * len(res), 16 + len(res) * 4, *res))), errors
-
-    @staticmethod
-    def packing_fake_result(boards: Iterable["MCIBoard"], cmd_data: memoryview, head: bytes) -> bytes:
-        res = []
-        for board in boards:
-            if board.has_ip and board.has_dma:
-                _id = (board.dma_id & 0xFF) << 24
-                res.append(_id + 0)
-        return b''.join((head, cmd_data[4:12], struct.pack('=I' + 'I' * len(res), 16 + len(res) * 4, *res)))
-
-    @classmethod
-    def unpacking_result(cls, _feedback, _res, command_bak, addr):
-        cmd_id = command_bak[4:8]
-        if not _feedback.startswith(b'\xcf\xcf\xcf\xcf'):
-            print(f'设备{addr}-指令{cmd_id}-返回指令包头错误')
-            return False
-        if cmd_id != _feedback[4:8]:
-            print(f'设备{addr}-指令{cmd_id}-返回指令ID错误{_feedback[4:8]}')
-            return False
-        if len(_res) % 4 != 0:
-            print(f'设备{addr}-指令{cmd_id}-返回结果{_res}长度错误')
-            return False
-        command_status = True
-        results = struct.unpack('I' * (len(_res) // 4), _res)
-        for result in results:
-            board_id = (result & 0xFF000000) >> 24
-            board_res = result & 0xFFFFFF
-            error_map = cls.error_map.get(command_bak[4:8], {})
-            if board_res:
-                print(f'设备{addr}-板卡{board_id}-指令{cmd_id}-{error_map.get(board_res, "执行失败")}')
-                command_status &= False
-        return command_status
-
-    @classmethod
-    def send_command(cls, data: Union[str, bytes], wait=0, addr=None, port=5001,
-                     check_feedback=True, return_fdk=False, connect_timeout=None):
-        """!
-        发送指定内容到后端
-
-        @param data: 指令内容
-        @param wait: 指令发送完成后，等待一段时间再接收反馈，阻塞式等待
-        @param addr: 后端IP
-        @param port: 后端端口
-        @param check_feedback:
-        @param return_fdk:
-        @param connect_timeout:
-        @return:
-        """
-        command_bak = data
-        try:
-            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            sock.settimeout(connect_timeout)
-            sock.connect((addr, port))
-        except Exception as e:
-            print(e)
-            return False
-
-        try:
-            sock.sendall(memoryview(data))
-
-            time.sleep(wait)
-            _feedback = sock.recv(16)
-            if check_feedback:
-                _res = sock.recv(struct.unpack('I', _feedback[12:16])[0] - 16)
-                if return_fdk:
-                    return _res
-                else:
-                    return cls.unpacking_result(_feedback, _res, command_bak, addr)
-        except Exception as e:
-            print(e)
-            return False
-        finally:
-            sock.close()
-        return True
-
-
-class InfoSharedList:
-    memory_name = 'NS_DEVICE_MEMORY'
-    memory_size = 1024 ** 2
-    head_size = 32  # memory中前head_size的长度为头部预留信息
-
-    def __init__(self):
-        try:
-            self._memory = shared_memory.SharedMemory(name=self.memory_name, create=True, size=self.memory_size)
-        except FileExistsError:
-            self._memory = shared_memory.SharedMemory(name=self.memory_name, create=False, size=self.memory_size)
-
-    def clear_ip(self):
-        _exit_pkl = pickle.dumps(self.ip)
-        self._memory.buf[self.head_size:len(_exit_pkl) + self.head_size] = b'\x00' * len(_exit_pkl)
-
-    @property
-    def ip(self):
-        try:
-            return pickle.loads(self._memory.buf[self.head_size:])
-        except pickle.UnpicklingError:
-            return []
-
-    @ip.setter
-    def ip(self, value):
-        ips = self.ip
-        ips.append(value)
-        ips = list(set(ips))
-        _pkl = pickle.dumps(ips)
-        self._memory.buf[self.head_size:len(_pkl) + self.head_size] = _pkl
-
-    def close(self):
-        self._memory.close()
-
-    def unlink(self):
-        try:
-            self._memory.unlink()
-        except FileNotFoundError as e:
-            pass
-
-
-# threading.Thread(target=do_scanning, daemon=True, name='qsync_scanning_device').start()
-SHARED_DEVICE_MEM = InfoSharedList()
+import atexit
+import socket
+import struct
+import threading
+import time
+import enum
+import pickle
+from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import wait as wait_futures
+from multiprocessing import shared_memory
+from functools import lru_cache, wraps
+from typing import Union, TYPE_CHECKING, Tuple, Iterable
+
+try:
+    from .common import BaseDriver, Quantity, QInteger
+except ImportError as e:
+    class BaseDriver:
+        def __init__(self, addr, timeout, **kw):
+            self.addr = addr
+            self.timeout = timeout
+
+
+    class Quantity(object):
+        def __init__(self, name: str, value=None, ch: int = 1, unit: str = ''):
+            self.name = name
+            self.default = dict(value=value, ch=ch, unit=unit)
+
+
+    class QInteger:
+        def __init__(self, name, value=None, unit='', ch=None,
+                     get_cmd='', set_cmd='', ):
+            self.name = name
+
+
+if TYPE_CHECKING:
+    from backend.board_parser import MCIBoard
+    from concurrent.futures import Future
+
+THREAD_POOL = ThreadPoolExecutor(max_workers=10)
+_scanning_lock = threading.Lock()
+_scanning_stop_event = threading.Event()
+DEVICE_SET = set()
+
+DEBUG_PRINT = False
+
+
+def print_debug(*args, **kwargs):
+    if DEBUG_PRINT:
+        print(*args, **kwargs)
+
+
+@atexit.register
+def global_system_exit():
+    THREAD_POOL.shutdown(wait=False)
+    SHARED_DEVICE_MEM.close()
+    try:
+        SHARED_DEVICE_MEM.unlink()
+    except FileNotFoundError as e:
+        pass
+
+
+def retry(times):
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            _times = times-1
+            while not func(*args, **kwargs) and _times > 0:
+                _times -= 1
+            return _times != 0
+        return wrapper
+    return decorator
+
+
+class Driver(BaseDriver):
+    class ScannMode(enum.IntEnum):
+        """!
+        @detail QC/QR等被同步设备的发现方式，'local': 本地共享内存扫描， 'remote': 网络udp扫描
+        """
+        local = 0
+        """local: 本地共享内存扫描
+
+        - NS_MCI中的Driver每实例化一次，就会在SharedMemory中记录一次自己的ip
+        - 系统进行同步时，会对SharedMemory中记录的QC/QR设备ip进行同步
+        - 只有程序整体退出的时候才会清空这片缓存
+        """
+        remote = 1
+        """remote: 网络udp扫描
+
+        - import 本文件后，会建立一个独立线程间断广播UDP包，扫描局域网内的QC/QR设备，记录被扫描到的设备ip
+        - 系统进行同步时，会对扫描到的QC/QR设备ip进行同步
+        - 注意：这种方式比较粗暴，会影响局域网内正在运行的设备
+        """
+        alone = 2
+        """alone: 单机运行模式
+
+        - QC/QR设备单独运行时使用本模式，默认使用QC/QR设备板内的QSYNC做设备内的系统同步
+        - 系统进行同步时，会判断QSYNC Driver的ip是否为QC/QR设备的ip
+        """
+
+    _scanning_lock = _scanning_lock
+    _device_set = DEVICE_SET
+
+    icd_head_reset = 0x41000002
+    icd_head_status = 0x4100000E
+    icd_head_cmd_2 = 0x31000015
+    icd_head_cmd_3 = 0x410000B1
+    icd_head_cmd_4 = 0x31000013
+    icd_head_cmd_5 = 0x410000B2
+    icd_head_cmd_6 = 0x3100001A
+    icd_head_cmd_7 = 0x410000B3
+    CHs = list(range(1, 17))
+
+    quants = [
+        QInteger('TRIG'),
+        Quantity('SystemSync', value=None, ch=1),  # set/get,运行次数
+        Quantity('GenerateTrig', value=None, unit='s'),  # set/get,触发周期单位s，触发数量=shot
+        Quantity('ResetTrig', value=None),
+        Quantity('Shot', value=1024, ch=1),  # set/get, 运行次数
+        Quantity('TrigPeriod', value=200e-6, ch=1),  # set/get, 触发周期
+        Quantity('TrigWidth', value=800e-9, ch=1),  # set/get, 触发周期
+        Quantity('TrigDelay', value=0, ch=1),  # set/get, 触发周期
+        Quantity('TrigFrom', value=0, ch=1),  # Trig来源： 0：内部产生；1：外部输入
+        Quantity('RefClock', value='out', ch=1),  # 参考时钟选择： ‘out’：外参考时钟；‘in’：内参考时钟
+        Quantity('DiscoveryMode', value=ScannMode.local, ch=1),  # QC/QR等被同步设备的发现方式，见DiscoveryMode说明
+        Quantity('UpdateFirmware', value='', ch=1),  # qsync固件更新
+    ]
+
+    SystemParameter = {
+        'RefClock': 'out',  # 参考时钟选择： ‘out’：外参考时钟；‘in’：内参考时钟
+        'TrigFrom': 0,  # Trig来源： 0：内部产生；1：外部输入
+        'TrigPeriod': 200e-6,  # 触发信号重复周期
+        'TrigWidth': 800e-9,  # 触发信号高电平宽度 单位s
+        'TrigDelay': 0,  # 触发信号相对开启通知的延迟
+        'DiscoveryMode': ScannMode.local,  # QC/QR等被同步设备的发现方式，见DiscoveryMode说明
+    }
+
+    def __init__(self, addr: str = '', timeout: float = 10.0, **kw):
+        super().__init__(addr, timeout, **kw)
+        self.handle = None
+        self.model = 'NS_QSYNC'  # 默认为设备名字
+        self.srate = None
+        self.gen_trig_num = 0
+        self.addr = addr
+
+        self.param = {'Shot': 1024, 'period': 200e-6, 'MixMode': 2}
+        print_debug(f'QSYNC: 实例化成功{addr}')
+
+    @property
+    def device_set(self):
+        mode = self.param.get('DiscoveryMode', self.ScannMode.local)
+        if mode is self.ScannMode.local:
+            return set(SHARED_DEVICE_MEM.ip)
+        elif mode is self.ScannMode.alone:
+            if self.addr in SHARED_DEVICE_MEM.ip:
+                return {self.addr}
+            else:
+                raise RuntimeError('qsync处于alone模式下，只能控制QC/QR内的qsync，请确认对应QC/QR设备是否已经open成功')
+        elif mode is self.ScannMode.remote:
+            return self._device_set.copy()
+        else:
+            return set()
+
+    def open(self, **kw):
+        """!
+        输入IP打开设备，配置默认超时时间为5秒
+        打开设备时配置RFSoC采样时钟，采样时钟以参数定义
+        @param kw:
+        @return:
+        """
+        # 配置系统初始值
+        system_parameter = kw.get('system_parameter', {})
+        values = self.SystemParameter.copy()
+        values.update(system_parameter)
+        for name, value in values.items():
+            if value is not None:
+                self.set(name, value, 1)
+
+        # self.sync_system()
+        status = self.get('Status')
+        print(f'*********QSYNC{self.addr}开启成功*********\n'
+              f'core_temp: {status[0]}℃\n'
+              f'10M_locked: {status[1] if len(status) > 1 else "nan"}')
+        print(f'qsync {self.addr} opened successfully')
+
+    def close(self, **kw):
+        """
+        关闭设备
+        """
+        # self.handle.release_dma()
+        # self.handle.close()
+        ...
+
+    def write(self, name: str, value, **kw):
+        channel = kw.get('ch', 1)
+        return self.set(name, value, channel)
+
+    def read(self, name: str, **kw):
+        channel = kw.get('ch', 1)
+        result = self.get(name, channel)
+        return result
+
+    def set(self, name, value=None, channel=1):
+        """!
+        设置设备属性
+        @param name:
+        @param value:
+        @param channel:
+        @return:
+        """
+        print_debug(f'QSYNC: set操作被调用{name}')
+        if name in {'SystemSync', 'ReInit'}:
+            self.sync_system()
+        elif name == 'TRIG':
+            value = self.param['TrigPeriod']
+            data = self.__fmt_qsync_start(
+                self.param['TrigFrom'], value, self.param['Shot'],
+                self.param['TrigWidth'], self.param['TrigDelay']
+            )
+            self._send_command(data, connect_timeout=2)
+            self.gen_trig_num += 1
+        elif name == 'GenerateTrig':
+            value = self.param['TrigPeriod'] if value is None else value
+            data = self.__fmt_qsync_start(
+                self.param['TrigFrom'], value, self.param['Shot'],
+                self.param['TrigWidth'], self.param['TrigDelay']
+            )
+            self._send_command(data, connect_timeout=2)
+            self.gen_trig_num += 1
+        elif name == 'ResetTrig':
+            data = self.__fmt_qsync_common(self.icd_head_reset)
+            self._send_command(data)
+        elif name == 'RefClock':
+            self.change_ref(value)
+        elif name == 'UpdateFirmware':
+            self.update_firmware(value)
+
+        else:
+            self.param[name] = value
+
+    def get(self, name, channel=1, value=0):
+        """!
+        查询设备属性，获取数据
+        @param name:
+        @param channel:
+        @param value:
+        @return:
+        """
+        print_debug(f'QSYNC: get操作被调用{name}')
+        if name == 'Status':
+            cmd_data = self.__fmt_qsync_common(self.icd_head_status)
+            data = DeviceCmdHandle.send_command(cmd_data, addr=self.addr, return_fdk=True)
+            data = struct.unpack('I' * (len(data) // 4), data)
+            return data
+        return self.param.get(name, None)
+
+    def sync_system(self):
+        """
+        全系统同步流程
+
+        :return:
+        """
+        if Driver._scanning_lock.acquire(timeout=10):
+            Driver._scanning_lock.release()
+        if len(self.device_set) == 0:
+            return
+
+        data = self.__fmt_qsync_common(self.icd_head_reset)
+        self._send_command(data)
+
+        result = True
+        if self.param.get('DiscoveryMode', self.ScannMode.local) != self.ScannMode.alone:
+            data = self.__fmt_qsync_common(self.icd_head_reset)
+            result &= self._sendto_fake_qsync(data)
+            data = self.__fmt_qsync_ref_from('out')
+            result &= self._sendto_fake_qsync(data)
+        result &= self._sendto_device(self.icd_head_cmd_2)
+        result &= self._sendto_qsync(self.icd_head_cmd_3)
+        result &= self._sendto_device(self.icd_head_cmd_4)
+        result &= self._sendto_qsync(self.icd_head_cmd_5)
+        result &= self._sendto_device(self.icd_head_cmd_6, 30)
+        result &= self._sendto_qsync(self.icd_head_cmd_7)
+
+        print(f'System synchronization {"succeeded" if result else "FAILED"}')
+
+    def change_ref(self, value='out'):
+        self.param['RefClock'] = value
+        self.set('ResetTrig')
+        data = self.__fmt_qsync_ref_from(value)
+        self._send_command(data)
+
+    def _sendto_device(self, cmd_head, timeout=2):
+        """!
+        将指令发送给设备
+        @param cmd_head:
+        @param timeout:
+        @return:
+        """
+        cmd_data = self.__fmt_qsync_common(cmd_head)
+        devices = list(self.device_set)
+        futures = [
+            THREAD_POOL.submit(DeviceCmdHandle.send_command, cmd_data, 0, addr, 5000, True, False, timeout)
+            for addr in devices
+        ]
+        wait_futures(futures)
+        result = all(future.result() for future in futures)
+        for idx, future in enumerate(futures):
+            if not future.result():
+                print(f'device: {devices[idx]}系统同步过程 {hex(cmd_head)} 执行失败')
+        return result
+
+    def _sendto_fake_qsync(self, cmd_data, timeout=2):
+        devices = list(self.device_set)
+        futures = [
+            THREAD_POOL.submit(self._send_command, cmd_data, 0, addr, 5001, True, False, timeout)
+            for addr in devices if addr != self.addr
+        ]
+        wait_futures(futures)
+        result = all(future.result() for future in futures)
+        for idx, future in enumerate(futures):
+            if not future.result():
+                print(f'device: {devices[idx]}系统同步过程 {cmd_data[4:12]} 执行失败')
+        return result
+
+    def _sendto_qsync(self, cmd_head: int):
+        """!
+        将指令发送给qsync
+
+        @param cmd_head:
+        @return:
+        """
+        cmd_data = self.__fmt_qsync_common(cmd_head)
+        if not self._send_command(cmd_data, connect_timeout=2):
+            print(f'qsync: 系统同步过程 {hex(cmd_head)} 执行失败')
+            return False
+        return True
+
+    def update_firmware(self, file_path, boards=None):
+        """!
+        固件更新
+
+        @param file_path: 固件路径
+        @param boards:
+        @return:
+        """
+        import os
+        if not os.path.exists(file_path):
+            raise ValueError(f'文件路径: {file_path} 不存在')
+        with open(file_path, 'rb') as fp:
+            cmd_data = self.__fmt_update_firmware(fp.read())
+        if not self._send_command(cmd_data):
+            print(f'qsync: 固件更新 执行失败')
+
+    def _connect(self, addr=None, port=5001, timeout=None):
+        """!
+        获取到指定ip的tcp连接
+
+        @param addr:
+        @param port:
+        @return:
+        """
+        timeout = self.timeout if timeout is None else timeout
+        addr = self.addr if addr is None else addr
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        sock.settimeout(timeout)
+        sock.connect((addr, port))
+        return sock
+
+    @retry(3)
+    def _send_command(self, data: Union[str, bytes], wait=0, addr=None, port=5001,
+                      check_feedback=True, return_fdk=False, connect_timeout=10):
+        """!
+        发送指定内容到后端
+
+        @param data: 指令内容
+        @param wait: 指令发送完成后，等待一段时间再接收反馈，阻塞式等待
+        @param addr: 后端IP
+        @param port: 后端端口
+        @param check_feedback: 是否解析反馈
+        @param connect_timeout:
+        @return:
+        """
+        command_bak = data
+        try:
+            sock = self._connect(addr=addr, port=port, timeout=connect_timeout)
+        except Exception as e:
+            print(f'device: {addr}无法连接 {e}')
+            return False
+
+        try:
+            sock.sendall(memoryview(data))
+
+            time.sleep(wait)
+            _feedback = sock.recv(20)
+            if check_feedback:
+                if not _feedback.startswith(b'\xcf\xcf\xcf\xcf'):
+                    print('返回指令包头错误')
+                    return False
+                if command_bak[4:8] != _feedback[4:8]:
+                    print('返回指令ID错误')
+                    return False
+                # print(_feedback)
+                _feedback = struct.unpack('=IIIII', _feedback)
+                if _feedback[4] != 0:
+                    print('指令成功下发，但执行失败')
+                    return False
+        except Exception as e:
+            print(f'device: {addr}指令{command_bak[:4]}发送失败 {e}')
+            return False
+        finally:
+            sock.close()
+        return True
+
+    @lru_cache(maxsize=32)
+    def __fmt_qsync_common(self, head):
+        cmd_pack = (
+            0x5F5F5F5F,
+            head,
+            0x00000000,
+            16,
+        )
+
+        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack)
+
+    @lru_cache(maxsize=16)
+    def __fmt_qsync_ref_from(self, _from):
+        if _from == 'in':
+            _from = 0
+        elif _from == 'out':
+            _from = 1
+        else:
+            _from = 0
+        cmd_pack = (
+            0x5F5F5F5F,
+            0x4100000F,
+            0x00000000,
+            20,
+            _from
+        )
+
+        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack)
+
+    @lru_cache(maxsize=32)
+    def __fmt_qsync_start(self, src, period, shots, width, delay):
+        cmd_pack = (
+            0x5F5F5F5F,
+            0x41000001,
+            0x00000000,
+            36,
+            int(src),
+            int(period * 1e9) & 0xFFFFFFFF,
+            int(shots),
+            int(width * 1e9) & 0xFFFFFFFF,
+            int(delay * 1e9) & 0xFFFFFFFF
+        )
+
+        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack)
+
+    @staticmethod
+    def __fmt_update_firmware(file_data):
+        cmd_pack = (
+            0x5F5F5F5F,
+            0x31000006,
+            0x00000000,
+            16 + len(file_data),
+        )
+        return struct.pack('=' + 'I' * len(cmd_pack), *cmd_pack) + file_data
+
+    # DG645兼容
+    def Trigger_singleshot(self):
+        self.set('GenerateTrig')
+
+    def Convention_init(self, rate=5000, **kwds):
+        self.set('ResetTrig')
+        self.set('Shot', 0xFFFFFFFF)
+        self.set('TrigPeriod', 1 / rate)
+        self.set('GenerateTrig')
+
+    def BurstMode_init(self, count=2048, delay=200e-6, period=200e-6, source=0, **kwds):
+        self.set('ResetTrig')
+        self.set('Shot', count)
+        self.set('TrigPeriod', period)
+        self.set('TrigDelay', delay)
+        self.set('TrigFrom', source)
+
+    def startGun(self):
+        self.Trigger_singleshot()
+
+
+def do_scanning():
+    """
+    扫描板卡
+
+    :return:
+    """
+    while True:
+        dest = ('<broadcast>', 5003)
+        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        s.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
+        addrs = socket.getaddrinfo(socket.gethostname(), None)
+        addr = [addr[4][0] for addr in addrs if addr[4][0].startswith('192.168.1.')]
+        _bind = False
+        _port = 15000
+        with _scanning_lock:
+            while not _bind:
+                try:
+                    s.bind((addr[0], _port))
+                    _bind = True
+                except Exception as e:
+                    _port += 1
+                    if _port >= 30000:
+                        raise e
+            s.sendto(b"____\x20\x00\x002\x00\x00\x00\x00\x14\x00\x00\x00\x00\x00\x00\x00", dest)
+            s.settimeout(3)
+
+            try:
+                while True:
+                    (feedback, _addr) = s.recvfrom(20)
+                    if feedback:
+                        DEVICE_SET.add(_addr[0])
+            except Exception as e:
+                s.close()
+        time.sleep(5)
+
+
+class DeviceCmdHandle:
+    """!
+    @brief 封装与QC/QR设备间的交互
+    """
+    error_map = {b'\x1a\x00\x001': {1: '指令Resync执行失败',
+                                    2: 'REFCLK not Detected',
+                                    3: 'Clock Maybe unstable, DAC Settings Error',
+                                    4: 'Clock Maybe unstable, ADC Settings Error',
+                                    5: 'SYSREF(External TRIG) not Detected, MTS failed / Sample Rate not Support',
+                                    7: 'ADC Calibration Failed'}
+                 }
+
+    @staticmethod
+    def packing_result(boards: Iterable["MCIBoard"],
+                       futures: Iterable["Future"],
+                       cmd_data: memoryview,
+                       head: bytes) -> Tuple[bytes, list]:
+        res = []
+        errors = []
+        for board, future in zip(boards, futures):
+            if board.has_ip and board.has_dma:
+                _id = (board.dma_id & 0xFF) << 24
+                _res = struct.unpack('IIIII', future.result())[-1] & 0xFFFFFF
+                if _res:
+                    errors.append(f'指令{cmd_data[4:8].tobytes()}向{board.board_ip}转发失败\n')
+                res.append(_id + _res)
+        return b''.join((head, cmd_data[4:12], struct.pack('=I' + 'I' * len(res), 16 + len(res) * 4, *res))), errors
+
+    @staticmethod
+    def packing_fake_result(boards: Iterable["MCIBoard"], cmd_data: memoryview, head: bytes) -> bytes:
+        res = []
+        for board in boards:
+            if board.has_ip and board.has_dma:
+                _id = (board.dma_id & 0xFF) << 24
+                res.append(_id + 0)
+        return b''.join((head, cmd_data[4:12], struct.pack('=I' + 'I' * len(res), 16 + len(res) * 4, *res)))
+
+    @classmethod
+    def unpacking_result(cls, _feedback, _res, command_bak, addr):
+        cmd_id = command_bak[4:8]
+        if not _feedback.startswith(b'\xcf\xcf\xcf\xcf'):
+            print(f'设备{addr}-指令{cmd_id}-返回指令包头错误')
+            return False
+        if cmd_id != _feedback[4:8]:
+            print(f'设备{addr}-指令{cmd_id}-返回指令ID错误{_feedback[4:8]}')
+            return False
+        if len(_res) % 4 != 0:
+            print(f'设备{addr}-指令{cmd_id}-返回结果{_res}长度错误')
+            return False
+        command_status = True
+        results = struct.unpack('I' * (len(_res) // 4), _res)
+        for result in results:
+            board_id = (result & 0xFF000000) >> 24
+            board_res = result & 0xFFFFFF
+            error_map = cls.error_map.get(command_bak[4:8], {})
+            if board_res:
+                print(f'设备{addr}-板卡{board_id}-指令{cmd_id}-{error_map.get(board_res, "执行失败")}')
+                command_status &= False
+        return command_status
+
+    @classmethod
+    def send_command(cls, data: Union[str, bytes], wait=0, addr=None, port=5001,
+                     check_feedback=True, return_fdk=False, connect_timeout=None):
+        """!
+        发送指定内容到后端
+
+        @param data: 指令内容
+        @param wait: 指令发送完成后，等待一段时间再接收反馈，阻塞式等待
+        @param addr: 后端IP
+        @param port: 后端端口
+        @param check_feedback:
+        @param return_fdk:
+        @param connect_timeout:
+        @return:
+        """
+        command_bak = data
+        try:
+            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            sock.settimeout(connect_timeout)
+            sock.connect((addr, port))
+        except Exception as e:
+            print(e)
+            return False
+
+        try:
+            sock.sendall(memoryview(data))
+
+            time.sleep(wait)
+            _feedback = sock.recv(16)
+            if check_feedback:
+                _res = sock.recv(struct.unpack('I', _feedback[12:16])[0] - 16)
+                if return_fdk:
+                    return _res
+                else:
+                    return cls.unpacking_result(_feedback, _res, command_bak, addr)
+        except Exception as e:
+            print(e)
+            return False
+        finally:
+            sock.close()
+        return True
+
+
+class InfoSharedList:
+    memory_name = 'NS_DEVICE_MEMORY'
+    memory_size = 1024 ** 2
+    head_size = 32  # memory中前head_size的长度为头部预留信息
+
+    def __init__(self):
+        try:
+            self._memory = shared_memory.SharedMemory(name=self.memory_name, create=True, size=self.memory_size)
+        except FileExistsError:
+            self._memory = shared_memory.SharedMemory(name=self.memory_name, create=False, size=self.memory_size)
+
+    def clear_ip(self):
+        _exit_pkl = pickle.dumps(self.ip)
+        self._memory.buf[self.head_size:len(_exit_pkl) + self.head_size] = b'\x00' * len(_exit_pkl)
+
+    @property
+    def ip(self):
+        try:
+            return pickle.loads(self._memory.buf[self.head_size:])
+        except pickle.UnpicklingError:
+            return []
+
+    @ip.setter
+    def ip(self, value):
+        ips = self.ip
+        ips.append(value)
+        ips = list(set(ips))
+        _pkl = pickle.dumps(ips)
+        self._memory.buf[self.head_size:len(_pkl) + self.head_size] = _pkl
+
+    def close(self):
+        self._memory.close()
+
+    def unlink(self):
+        try:
+            self._memory.unlink()
+        except FileNotFoundError as e:
+            pass
+
+
+# threading.Thread(target=do_scanning, daemon=True, name='qsync_scanning_device').start()
+SHARED_DEVICE_MEM = InfoSharedList()
```

## nsqdriver/__init__.py

```diff
@@ -1,10 +1,10 @@
-from .NS_MCI import Driver as MCIDriver
-from .NS_QSYNC import Driver as QSYNCDriver
-from .NS_CST import Driver as CSTDriver
-from .compiler.ns_wave import InsChannel
-from .compiler.py_wave_asm import nsw_config, AssemblyError
-
-version_pack = (0, 3, 3)
-
-__version__ = '.'.join(str(_) for _ in version_pack)
-__all__ = ['MCIDriver', 'QSYNCDriver', 'CSTDriver', 'InsChannel']
+from .NS_MCI import Driver as MCIDriver
+from .NS_QSYNC import Driver as QSYNCDriver
+from .NS_CST import Driver as CSTDriver
+from .compiler.ns_wave import InsChannel
+from .compiler.py_wave_asm import nsw_config, AssemblyError
+
+version_pack = (0, 4, 0)
+
+__version__ = '.'.join(str(_) for _ in version_pack)
+__all__ = ['MCIDriver', 'QSYNCDriver', 'CSTDriver', 'InsChannel']
```

## nsqdriver/common.py

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
-class Quantity(object):
-    def __init__(self, name: str, value=None, ch: int = 1, unit: str = ''):
-        self.name = name
-        self.default = dict(value=value, ch=ch, unit=unit)
-
-
-class QInteger:
-    def __init__(self, name, value=None, unit='', ch=None,
-                 get_cmd='', set_cmd='',):
-        self.name = name
-
-
-class BaseDriver:
-    def __init__(self, addr, timeout, **kw):
-        self.addr = addr
-        self.timeout = timeout
-
-
-def get_coef(*args):
-    return '', '', '', ''
+class Quantity(object):
+    def __init__(self, name: str, value=None, ch: int = 1, unit: str = ''):
+        self.name = name
+        self.default = dict(value=value, ch=ch, unit=unit)
+
+
+class QInteger:
+    def __init__(self, name, value=None, unit='', ch=None,
+                 get_cmd='', set_cmd='',):
+        self.name = name
+
+
+class BaseDriver:
+    def __init__(self, addr, timeout, **kw):
+        self.addr = addr
+        self.timeout = timeout
+
+
+def get_coef(*args):
+    return '', '', '', ''
```

## nsqdriver/compiler/ns_wave.pyi

```diff
@@ -1,151 +1,151 @@
-import numpy as np
-import waveforms as wf
-
-from enum import IntEnum
-from typing import Union, List, Dict
-from nsqdriver.compiler.py_wave_asm import *
-
-
-class QInsPlaceholder(NSQCommand):
-    ...
-
-
-class Wave(GenTagMixin):
-    class Tag(IntEnum): ...
-
-    def __init__(self, ins_obj: "InstructionQ", ins_id: dict): ...
-
-class Frame(Wave):
-    def __init__(self, ins_obj: "InstructionQ", ins_id: int, freq: float): ...
-
-    @property
-    def freq(self) -> float: ...
-
-    @freq.setter
-    def freq(self, value: float): ...
-
-    def __mul__(self, other: Wave) -> Signal: ...
-
-    def format(self) -> "QInsFrame": ...
-
-
-class Envelope(Wave):
-    def __init__(self, ins_obj: "InstructionQ", ins_id: int, content: "Union[wf.Waveform, np.ndarray]"): ...
-
-    @property
-    def content(self) -> "Union[wf.Waveform, np.ndarray]": ...
-
-    @content.setter
-    def content(self, value: "Union[wf.Waveform, np.ndarray]"): ...
-
-    def __mul__(self, other: Wave) -> Signal: ...
-
-    def format(self) -> "QInsEnvelop": ...
-
-
-class Signal(Wave):
-    def __init__(self, ins_obj: "InstructionQ", ins_id: dict): ...
-
-
-class InstructionQ(GenTagMixin):
-    """!
-    包含各种具体的指令
-    """
-
-    def __init__(self, freqs=None, envelopes=None):
-        self.i_set: "List[Union[NSQCommand, InstructionQ]]" = []
-        self.f_set: "Dict[int, Frame]" = {}
-        self.e_set: "Dict[int, Envelope]" = {}
-        self.symbol_set: Dict[str, int] = {}
-        self.symbol_idx: int = -1
-        self.is_first_trig: bool = True
-        self.last_ins: NSQCommand
-
-    def clear(self) -> None: ...
-
-    @property
-    def length(self) -> int: ...
-
-    def ins_frame(self, freq, idx=None) -> Frame: ...
-
-    def ins_envelope(self, envelope: "Union[np.ndarray, wf.Waveform, str]", idx=None) -> Envelope: ...
-
-    def evlp_gaussian(self, width: float) -> Envelope: ...
-
-    def evlp_cospulse(self, width: float) -> Envelope: ...
-
-    def evlp_square(self, width: float) -> Envelope: ...
-
-    def _append_ins(self, cmd: "Union[NSQCommand, InstructionQ]"): ...
-
-    def _map_var(self, var: str) -> int: ...
-
-    def wait_for_trigger(self) -> QInsWaitTrig: ...
-
-    def ins_variable(self, reg: str, value: int): ...
-
-    def ins_add(self, reg: str, value: int): ...
-
-    def ins_reset_frame(self, flag: str, frame: "Frame"): ...
-
-    def inc_phase(self, frame: "Frame", phase: float): ...
-
-    def play_wave(self, wave: Signal, amp=1, freq=0, phase=0): ...
-
-    def play_zero(self, width: float): ...
-
-    def wait(self): ...
-
-    def end(self): ...
-
-    def capture(self, width: float, delay=0.): ...
-
-
-class InsChannel(InstructionQ):
-    def __init__(self, freqs=None, envelopes=None):
-        self.if_stack: "List[InsIF]" = []
-        self.looping = False
-
-    def ins_if(self, formula: str) -> "InsIF": ...
-
-    def ins_else(self) -> "InsElse": ...
-
-    def ins_loop(self, times: int) -> "InsLoop": ...
-
-
-class InsIF(InsChannel):
-    ch_judge_name = {f'FREQ_{i}': 1<<i for i in range(6)}
-
-    def __init__(self, freqs=None, envelopes=None):
-        self.channel: "InsChannel" = None
-        self.key_ins: "NSQCommand" = None
-        self.ins_else = None
-
-    @classmethod
-    def from_channel(cls, channel :InsChannel) -> InsIF: ...
-
-    @property
-    def formula(self): ...
-
-    @formula.setter
-    def formula(self, formula: str): ...
-
-
-class InsElse(InsChannel):
-    def __init__(self, freqs=None, envelopes=None): ...
-
-    @classmethod
-    def from_channel(cls, channel: InsChannel) -> InsElse: ...
-
-    def capture(self, width: float, delay=0): ...
-
-
-class InsLoop(InsChannel):
-    def __init__(self, freqs: float=None, envelopes: "Union[wf.Waveform, np.ndarray]"=None): ...
-
-    @classmethod
-    def from_channel(cls, channel: InsChannel) -> InsLoop: ...
-
-    def capture(self, width: float, delay=0): ...
-
-    def _compile(self) -> "List[NSQCommand]": ...
+import numpy as np
+import waveforms as wf
+
+from enum import IntEnum
+from typing import Union, List, Dict
+from nsqdriver.compiler.py_wave_asm import *
+
+
+class QInsPlaceholder(NSQCommand):
+    ...
+
+
+class Wave(GenTagMixin):
+    class Tag(IntEnum): ...
+
+    def __init__(self, ins_obj: "InstructionQ", ins_id: dict): ...
+
+class Frame(Wave):
+    def __init__(self, ins_obj: "InstructionQ", ins_id: int, freq: float): ...
+
+    @property
+    def freq(self) -> float: ...
+
+    @freq.setter
+    def freq(self, value: float): ...
+
+    def __mul__(self, other: Wave) -> Signal: ...
+
+    def format(self) -> "NSQCommand": ...
+
+
+class Envelope(Wave):
+    def __init__(self, ins_obj: "InstructionQ", ins_id: int, content: "Union[wf.Waveform, np.ndarray]"): ...
+
+    @property
+    def content(self) -> "Union[wf.Waveform, np.ndarray]": ...
+
+    @content.setter
+    def content(self, value: "Union[wf.Waveform, np.ndarray]"): ...
+
+    def __mul__(self, other: Wave) -> Signal: ...
+
+    def format(self) -> "NSQCommand": ...
+
+
+class Signal(Wave):
+    def __init__(self, ins_obj: "InstructionQ", ins_id: dict): ...
+
+
+class InstructionQ(GenTagMixin):
+    """!
+    包含各种具体的指令
+    """
+
+    def __init__(self, freqs=None, envelopes=None):
+        self.i_set: "List[Union[NSQCommand, InstructionQ]]" = []
+        self.f_set: "Dict[int, Frame]" = {}
+        self.e_set: "Dict[int, Envelope]" = {}
+        self.symbol_set: Dict[str, int] = {}
+        self.symbol_idx: int = -1
+        self.is_first_trig: bool = True
+        self.last_ins: NSQCommand
+
+    def clear(self) -> None: ...
+
+    @property
+    def length(self) -> int: ...
+
+    def ins_frame(self, freq, idx=None) -> Frame: ...
+
+    def ins_envelope(self, envelope: "Union[np.ndarray, wf.Waveform, str]", idx=None) -> Envelope: ...
+
+    def evlp_gaussian(self, width: float) -> Envelope: ...
+
+    def evlp_cospulse(self, width: float) -> Envelope: ...
+
+    def evlp_square(self, width: float) -> Envelope: ...
+
+    def _append_ins(self, cmd: "Union[NSQCommand, InstructionQ]"): ...
+
+    def _map_var(self, var: str) -> int: ...
+
+    def wait_for_trigger(self): ...
+
+    def ins_variable(self, reg: str, value: int): ...
+
+    def ins_add(self, reg: str, value: int): ...
+
+    def ins_reset_frame(self, flag: str, frame: "Frame"): ...
+
+    def inc_phase(self, frame: "Frame", phase: float): ...
+
+    def play_wave(self, wave: Signal, amp=1, freq=0, phase=0): ...
+
+    def play_zero(self, width: float): ...
+
+    def wait(self): ...
+
+    def end(self): ...
+
+    def capture(self, width: float, delay=0.): ...
+
+
+class InsChannel(InstructionQ):
+    def __init__(self, freqs=None, envelopes=None):
+        self.if_stack: "List[InsIF]" = []
+        self.looping = False
+
+    def ins_if(self, formula: str) -> "InsIF": ...
+
+    def ins_else(self) -> "InsElse": ...
+
+    def ins_loop(self, times: int) -> "InsLoop": ...
+
+
+class InsIF(InsChannel):
+    ch_judge_name = {f'FREQ_{i}': 1<<i for i in range(6)}
+
+    def __init__(self, freqs=None, envelopes=None):
+        self.channel: "InsChannel" = None
+        self.key_ins: "NSQCommand" = None
+        self.ins_else = None
+
+    @classmethod
+    def from_channel(cls, channel :InsChannel) -> InsIF: ...
+
+    @property
+    def formula(self): ...
+
+    @formula.setter
+    def formula(self, formula: str): ...
+
+
+class InsElse(InsChannel):
+    def __init__(self, freqs=None, envelopes=None): ...
+
+    @classmethod
+    def from_channel(cls, channel: InsChannel) -> InsElse: ...
+
+    def capture(self, width: float, delay=0): ...
+
+
+class InsLoop(InsChannel):
+    def __init__(self, freqs: float=None, envelopes: "Union[wf.Waveform, np.ndarray]"=None): ...
+
+    @classmethod
+    def from_channel(cls, channel: InsChannel) -> InsLoop: ...
+
+    def capture(self, width: float, delay=0): ...
+
+    def _compile(self) -> "List[NSQCommand]": ...
```

## nsqdriver/compiler/py_wave_asm.pyi

```diff
@@ -1,27 +1,26 @@
-import struct
-import copy
-import uuid
-from typing import Union, List, Tuple, Any
-from dataclasses import dataclass
-from collections import ChainMap
-
-import numpy as np
-import waveforms as wf
-
-
-global_config = {
-    'play_zero_step': 4e-9,
-    'OUTSrate': 8e9,
-    'envelope_dtype': np.int16,  # 描述包络每个点的数据类型
-    'envelope_step': 64,  # 包络步进粒度，单位为bytes
-    'envelope_quant': 16383,  # 包络量化范围
-    'envelope_cache': 204800,  # 包络缓存大小，单位bytes
-    'envelope_head': np.array([2, 0, 0, 4096, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=np.int16),   # 包络更新包头
-}
-
-
-def nsw_config(name: str, value: Any) -> None: ...
-
-
-class AssemblyError(RuntimeError):
-    ...
+from typing import Any
+
+import numpy as np
+
+
+global_config = {
+    'play_zero_step': 4e-9,
+    'OUTSrate': 8e9,
+    'envelope_dtype': np.int16,  # 描述包络每个点的数据类型
+    'envelope_step': 64,  # 包络步进粒度，单位为bytes
+    'envelope_quant': 16383,  # 包络量化范围
+    'envelope_cache': 204800,  # 包络缓存大小，单位bytes
+    'envelope_head': np.array([2, 0, 0, 4096, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=np.int16),   # 包络更新包头
+}
+
+
+def nsw_config(name: str, value: Any) -> None: ...
+
+
+class AssemblyError(RuntimeError): ...
+
+
+class GenTagMixin: ...
+
+
+class NSQCommand: ...
```

## nsqdriver/wrapper/AWG_ADC.py

 * *Ordering differences only*

```diff
@@ -1,534 +1,534 @@
-import enum
-import abc
-import dataclasses
-from typing import List, Union, Dict, Iterable, Sized
-from functools import wraps
-
-import numpy as np
-from ..NS_MCI import Driver as MCIDriver
-from ..NS_QSYNC import Driver as QSYNCDriver
-
-MIX_BIT_WIDTH = 32767
-SEGMENT_ENABLE = False
-
-
-@dataclasses.dataclass
-class DAChannelData:
-    seg_waves: "Sized|Iterable[np.ndarray]" = tuple()
-    delays: "Sized|Iterable[float]" = tuple()
-    data: np.ndarray = np.array([0])
-    updated: bool = False
-
-    @property
-    def right(self) -> bool:
-        return len(self.seg_waves) == len(self.delays)
-
-    def compute_data(self, rate):
-        """计算最后可下发给设备的data
-
-        :param rate: DA采样率，单位Hz
-        :return:
-        """
-        if not self.updated:
-            return
-        # if not self.right:
-        #     print(f'警告：波形片段数{len(self.seg_waves)}与波形延迟数{len(self.delays)}不匹配')
-        #     return
-        data = []
-        for seg, delay in zip(self.seg_waves, self.delays):
-            seg = seg / MIX_BIT_WIDTH
-            data.append(np.zeros((round(float(delay) * rate),)))
-            data.append(seg)
-        self.data = np.hstack(data)
-
-
-class ChannelDataPara(DAChannelData):
-    def __check_waveform(self, wave):
-        if wave.stop is None:
-            raise ValueError('waveform.stop为None，应为一确定波形时宽')
-        wave.start = 0 if wave.start is None else wave.start
-
-    def compute_data(self, rate):
-        import waveforms
-        if not self.updated:
-            return
-        if not self.right:
-            print(f'警告：波形片段数{len(self.seg_waves)}与波形延迟数{len(self.delays)}不匹配')
-            return
-        data = waveforms.zero()
-        wave_width = 0
-        for seg, delay in zip(self.seg_waves, self.delays):
-            seg: waveforms.Waveform
-            self.__check_waveform(seg)
-            wave_width += delay
-            window = waveforms.square(seg.stop - seg.start) >> seg.start
-            data += ((window*seg) >> wave_width)
-            wave_width += (seg.stop - seg.start)
-        self.data = np.array(data)
-
-
-@dataclasses.dataclass
-class ADConfig:
-    mixer_table: "np.ndarray" = np.zeros((1, 4096, 12, 2))
-    delays: "List[float]" = tuple()
-    updated: bool = False
-    coff_param: "Union[np.ndarray, List[np.ndarray]]" = (np.zeros((12, 4096), dtype=np.complex64), )
-    seg_conf: "List[List[float]]" = tuple()
-
-    @property
-    def right(self) -> bool:
-        return self.mixer_table.shape[0] == len(self.delays)
-
-    def compute_conf(self, rate):
-        """计算最后可下发给设备的采集conf
-
-        :param rate: AD采样率，单位Hz
-        :return:
-        """
-        if not self.updated:
-            return
-        if not self.right:
-            print(f'警告：mixer table片段数{len(self.mixer_table.shape[0])}与波形延迟数{len(self.delays)}不匹配')
-            return
-        coff_param = []
-        seg_conf = []
-        delay_count = 0
-        seg_length = self.mixer_table.shape[1]/rate
-        for idx, (table, delay) in enumerate(zip(self.mixer_table, self.delays)):
-            table: "np.ndarray"
-            table = table[:, :, 0] + table[:, :, 1]*1j
-            coff_param.append(table.T)
-            seg_conf.append([seg_length, delay_count])
-            delay_count += seg_length+delay if idx != 0 else seg_length
-        self.coff_param = coff_param
-        self.seg_conf = seg_conf
-
-
-class _BaseDriver(abc.ABC):
-    class DARunMode(enum.IntEnum):
-        TRIGGER_MODE = 1
-        """触发模式"""
-        CONTINUOUS_MODE = 2
-        """连续模式"""
-
-    class ADRunMode(enum.IntEnum):
-        ALGORITHMIC_MODE = 1
-        """算法采集模式"""
-        TRACE_MODE = 2
-        """时域采集模式"""
-
-    mode_map = {}
-
-    def __init__(self, *args):
-        self.driver: "MCIDriver" = MCIDriver()
-        self.sys_param = {
-            'MixMode': 2,  # Mix模式，1：第一奈奎斯特去； 2：第二奈奎斯特区
-            'PLLFreq': 100e6,  # 参考时钟频率, 单位为Hz
-            'RefClock': 'out',  # 参考时钟选择： ‘out’：外参考时钟；‘in’：内参考时钟
-            'ADrate': 4e9,  # AD采样率，单位Hz
-            'DArate': 6e9,  # DA采样率，单位Hz
-            'KeepAmp': 0,  # DA波形发射完毕后，保持最后一个值
-            'Delay': 0,  # 配置DA的原生Delay
-            'SegmentSampling': []  # 配置分段采样
-        }
-        self.connected = False
-
-        self.run_mode = None
-        self.run_count = 1024
-
-    def connect(self, address, *args) -> bool:
-        """连接设备
-
-        :param address: 设备ip
-        :param args:
-        :return:
-        """
-        if self.connected and self.driver.addr != address:
-            raise ValueError(f'系统已连接到{self.driver.addr}')
-        self.driver = MCIDriver(address)
-        self.driver.open()
-        return self.init_system(*args)
-
-    def disconnect(self, address, *args):
-        if self.connected and self.driver.addr != address:
-            raise ValueError(f'系统已连接到{self.driver.addr}，不可与{address}断开连接')
-        self.connected = False
-
-    @staticmethod
-    def with_connected(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            self: "_BaseDriver" = args[0]
-            if not self.connected:
-                raise RuntimeError(f'系统未连接，不可调用{self.__class__.__name__}.{func.__name__}')
-            return func(*args, **kwargs)
-
-        return wrapper
-
-    def update_sys_parm(self, _input):
-        if len(_input) > 0 and isinstance(_input[0], dict):
-            self.sys_param.update(_input[0])
-
-    def init_system(self, *args) -> bool:
-        self.update_sys_parm(args)
-        self.connected = self.driver.init_device(system_parameter=self.sys_param)
-        return self.connected
-
-    def setRunMode(self, mode):
-        """设置运行模式
-
-        :param mode:
-        :return:
-        """
-        self.run_mode = self.mode_map.get(mode, 1)
-
-    # @with_connected
-    def setCount(self, N):
-        self.driver.set('Shot', N)
-        self.run_count = N
-
-    @abc.abstractmethod
-    def start(self, channels):
-        ...
-
-    def stop(self, channels):  # 停止channels里面指定的通道的运行
-        ...
-
-
-class DAC(_BaseDriver):
-    with_connected = _BaseDriver.with_connected
-    mode_map = {
-        2: _BaseDriver.DARunMode.CONTINUOUS_MODE,
-        1: _BaseDriver.DARunMode.TRIGGER_MODE
-    }
-
-    def __init__(self, *args):
-        super(DAC, self).__init__(*args)
-        self.run_mode = self.DARunMode.TRIGGER_MODE
-        self.run_wave_points = 0
-        self.run_da_seg_cache: "Dict[int, DAChannelData]" = {}
-
-    def initDAC(self):
-        self.init_system()
-        self.driver.set('EnableWaveCache', True)
-
-    @with_connected
-    def write_wave(self, waves, channeli):
-        """
-        给其中一个通道写波形，waves:[wave0,wave1,wave2,...]
-        其中wave0,wave1,...为能直接写入fpga的int数组或uint数组，这里可以写一段或多段波形，
-        触发模式下，仪器接收一个触发信号后，每段波形依次运行，波形之间的延迟可以通过setTriggerDelays函数设置
-        注意，对于每一个触发信号，waves里的波形都会被运行
-
-        :param waves: List[np.array]  int16
-        :param channeli: int
-        :return:
-        """
-        da_data = self.run_da_seg_cache.get(channeli, DAChannelData())
-        da_data.seg_waves = waves
-        da_data.updated = True
-        self.run_da_seg_cache[channeli] = da_data
-        # self._upload_wave([channeli])
-
-    @with_connected
-    def setTriggerDelays(self, delays, channeli):
-        """
-        设置trigger和发出波形之间的delays,只用于trig的运行模式，接收到trig后会前后相继的运行写入的[wave0,wave1,wave2,...]
-        delays=[delay0,delay1,delay2,....]一一对应于[wave0,wave1,wave2,...]
-        delay0为trig信号和wave0的起始时刻之间的延迟，delay1为wave0的末尾时刻和wave1的起始时刻之间的延迟，依次类推
-
-        :param delays: List[float]
-        :param channeli:
-        :return:
-        """
-        da_data = self.run_da_seg_cache.get(channeli, DAChannelData())
-        da_data.delays = delays
-        da_data.updated = True
-        self.run_da_seg_cache[channeli] = da_data
-        self._upload_wave([channeli])
-
-    @with_connected
-    def write_param_waveform(self, wave, channeli):
-        """发送要求wave为waveforms的Waveform对象
-
-        :param wave:
-        :param channeli:
-        :return:
-        """
-        self.driver.set('GenWave', wave, channeli)
-
-    @with_connected
-    def start(self, channels):
-        """当前后台仅能支持配置过波形的所有通道一起播放，后续支持
-
-        :param channels:
-        :return:
-        """
-        # 生效缓存的数据。支持ping-pang模式
-        self.driver.set('PushWaveCache')
-        if self.run_mode is self.DARunMode.CONTINUOUS_MODE:
-            period = self.run_wave_points / self.sys_param['DArate']
-            self.driver.set('GenerateTrig', period)
-
-    def _upload_wave(self, channels=None):
-        """按需计算要下发的data，并将缓存中“updated”的数据更新到设备中
-
-        :param channels:
-        :return:
-        """
-        channels = self.run_da_seg_cache.keys() if channels is None else channels
-        rate = self.sys_param['DArate']
-        for chnl in channels:
-            if chnl not in self.run_da_seg_cache:
-                continue
-            da_data = self.run_da_seg_cache[chnl]
-            da_data.compute_data(rate)
-            if not da_data.updated:
-                continue
-            self.driver.set('Waveform', da_data.data, chnl)
-            da_data.updated = False
-
-
-class ADC(_BaseDriver):
-    with_connected = _BaseDriver.with_connected
-    mode_map = {
-        1: _BaseDriver.ADRunMode.TRACE_MODE,
-        2: _BaseDriver.ADRunMode.ALGORITHMIC_MODE
-    }
-
-    def __init__(self, *args):
-        super(ADC, self).__init__(*args)
-        self.run_mode = self.ADRunMode.ALGORITHMIC_MODE
-        self.chnl_id = 0 if len(args) == 0 else args[0]
-        self.run_ad_chnl_conf: "Dict[int, ADConfig]" = {}
-
-    def initADC(self):
-        """连接ADC后进行初始化
-
-        :return:
-        """
-        self.init_system()
-
-    @with_connected
-    def write_mixerTable(self, mixData, channeli=None):
-        """算法采集模式下，事先把要用于算法采集模式的权重数据写入ADC
-
-        :param mixData: 如果ADC可以采集Y段波形，M为解模频点数，每段波形要在M个频率点做解模，时域波形一共L个点，
-                        那mixData的shape为:(Y,L,M,2),类型为int数组 或uint数组  np.array  int16
-        :param channeli:
-        :return:
-        """
-        channeli = self.chnl_id if channeli is None else channeli
-        ad_conf = self.run_ad_chnl_conf.get(channeli, ADConfig())
-        ad_conf.mixer_table = mixData
-        ad_conf.updated = True
-        self.run_ad_chnl_conf[channeli] = ad_conf
-
-    @with_connected
-    def setTriggerDelays(self, delays, channeli=None):
-        """设置trigger和采集波形之间的delays,接收到trig后会前后相继的采集waveDatas=[waveData0,waveData1,waveData2,...]
-            delays = [delay0,delay1,delay2,....]一一对应于[waveData0,waveData1,waveData2,...]
-            delay0为trig信号和waveData0的起始时刻之间的延迟，delay1为waveData0的末尾时刻和waveData1的起始时刻之间的延迟，依次类推
-
-        :param delays: List[float]
-        :param channeli:
-        :return:
-        """
-        channeli = self.chnl_id if channeli is None else channeli
-        ad_conf = self.run_ad_chnl_conf.get(channeli, ADConfig())
-        ad_conf.delays = delays
-        ad_conf.updated = True
-        self.run_ad_chnl_conf[channeli] = ad_conf
-
-    @with_connected
-    def collectWaveData(self, channeli=None):
-        """采集波形数据，waveDatas=[waveData0,waveData1,waveData2,...]，waveData? 为int数组，每接收一个trig，采集一次waveDatas
-            时域采集模式下,waveData0为第一段时域波形数据,shape为（N,L）,N为采集波形的次数，算法采集模式下，waveData0为解模后的数据，shape为（N，M）
-            ！注意该命令应该能在波形运行的过程中能采集，如果计划要采集N次，不能AWG的波形运行N次之后才采集，而是AWG边运行边采集，以加快速度
-
-        :return:
-        """
-        try:
-            channeli = self.chnl_id if channeli is None else channeli
-            if channeli not in self.run_ad_chnl_conf:
-                raise ValueError(f'未配置通道{channeli}的相关采集信息')
-            ad_conf = self.run_ad_chnl_conf[channeli]
-            seg_num = len(ad_conf.seg_conf)
-            if self.run_mode is self.ADRunMode.TRACE_MODE:
-                data = self.driver.get('TraceIQ', channeli)
-                seg_length = data.shape[1]//seg_num
-                data = [data[:, i:i+seg_length] for i in range(seg_num)]
-            else:
-                data = self.driver.get('IQ', channeli)
-                print(data)
-                if SEGMENT_ENABLE:
-                    data = [data[i] for i in range(seg_num)]
-            return data
-        except Exception as e:
-            print(e)
-
-    def clearBuf(self):
-        """清理ADC缓存的命令，假设上次运行报错，ADC能清理掉上次报错前所采集到的波形数据
-
-        :return:
-        """
-        self.driver.write('ResetCollect', None)
-
-    @with_connected
-    def start(self, channels):
-        """启动ADC的运行
-
-        :param channels: QMAC有4个ad通道编号为 [1, 2, 3, 4]
-        :return:
-        """
-        self._upload_collect_conf(channels)
-        self.driver.set('StartCapture')
-
-    def _upload_collect_conf(self, channels=None):
-        """按需计算要下发的data，并将缓存中“updated”的数据更新到设备中
-
-        :param channels:
-        :return:
-        """
-        channels = self.run_ad_chnl_conf.keys() if channels is None else channels
-        rate = self.sys_param['ADrate']
-        for chnl in channels:
-            if chnl not in self.run_ad_chnl_conf:
-                continue
-            ad_conf = self.run_ad_chnl_conf[chnl]
-            ad_conf.compute_conf(rate)
-            if not ad_conf.updated:
-                continue
-            self.driver.set('TriggerDelay', float(ad_conf.delays[0]), int(chnl))
-            if SEGMENT_ENABLE:
-                self.driver.set('SegmentSampling', ad_conf.seg_conf, int(chnl))
-                self.driver.set('DemodulationParam', ad_conf.coff_param, int(chnl))
-            else:
-                self.driver.set('SegmentSampling', [], int(chnl))
-                self.driver.set('DemodulationParam', ad_conf.coff_param[0], int(chnl))
-            ad_conf.updated = False
-
-class Trig(_BaseDriver):
-    class RunMode(enum.IntEnum):
-        INSIDE_MODE = 1
-        """内部触发模式"""
-        EXTERNAL_MODE = 2
-        """外部触发模式"""
-
-    mode_map = {
-        1: RunMode.INSIDE_MODE,
-        2: RunMode.EXTERNAL_MODE
-    }
-    with_connected = _BaseDriver.with_connected
-
-    def __init__(self, *args):
-        super(Trig, self).__init__(*args)
-        self.sys_param = {
-            'RefClock': 'in',  # 参考时钟选择： ‘out’：外参考时钟；‘in’：内参考时钟
-            'TrigFrom': 0,  # Trig来源： 0：内部产生；1：外部输入
-            'TrigPeriod': 200e-6,
-            'DiscoveryMode': QSYNCDriver.ScannMode.local,  # QC/QR等被同步设备的发现方式，见DiscoveryMode说明
-        }
-        self.run_mode = self.RunMode.INSIDE_MODE
-        self.driver: "QSYNCDriver" = QSYNCDriver()
-
-    def connect(self, address, *args):
-        self.driver = QSYNCDriver(address)
-        self.update_sys_parm(args)
-        self.driver.open(system_parameter=self.sys_param)
-        self.connected = True
-
-    @with_connected
-    def initTrig(self):
-        self.driver.set('ResetTrig')
-        self.driver.sync_system()
-
-    @with_connected
-    def setClock(self, **kws):
-        """设置时钟运行相关参数,比如外部或内部时钟，时钟频率等等
-
-        :param kws: 参考信号 RefClock，TrigFrom
-        :return:
-        """
-        self.update_sys_parm((kws, ))
-        self.driver.open(system_parameter=self.sys_param)
-
-    def checkStatus(self):  # 查看相关状态，比如时钟是多少MHz，是外部接入还是内部产生，trig信号的间隔，宽度，每个通道发出trig信号的延迟
-        print(self.sys_param)
-
-    @with_connected
-    def setTrigOffset(self, time, channel):  # 设置通道channel的trigger信号的延迟
-        self.driver.set('TrigOffset', time)
-
-    @with_connected
-    def setIntervalTime(self, time):  # 设置触发
-        """
-        :param time: 秒
-        """
-        self.driver.set('TrigPeriod', time)
-
-    def setIntervalShape(self, width, amplitude):  # 设置触发信号宽度和高度
-        self.driver.set('TrigWidth', width)
-
-    def start(self, channels):  # 启动trig信号的运行
-        if self.run_mode is self.RunMode.INSIDE_MODE:
-            self.driver.set('GenerateTrig')
-
-    def stop(self, channels):  # 停止trig信号的运行
-        if self.run_mode is self.RunMode.INSIDE_MODE:
-            self.driver.set('ResetTrig')
-
-
-trig = Trig
-
-
-if __name__ == '__main__':
-    from waveforms import *
-
-    sample_rate = 6e9
-    width = 20e-9
-    time_line = np.linspace(0, width*10, int(width * 10 * sample_rate))
-    waves = {
-        'poly': poly([1, -1 / 2, 1 / 6, -1 / 12]),
-        'cos': cos(2 * pi * 5.2e9),
-        'sin': sin(2 * pi * 5.2e9),
-        'gaussian': gaussian(width) >> (width * 2),
-        'sinc': sinc(6e8),
-        'square': square(width) >> (width * 2),
-        'cosPulse': cosPulse(width) >> (width * 2),
-        'chirp_linear': chirp(1e9, 1.5e9, width * 10, type='linear'),
-        'chirp_exponential': chirp(1e9, 1.5e9, width * 10, type='exponential'),
-        'chirp_hyperbolic': chirp(1e9, 1.5e9, width * 10, type='hyperbolic'),
-        'cos*gaussian': cos(2 * pi * 5.2e9) * gaussian(width) >> (width * 2),
-        'cos*cosPulse': cos(2 * pi * 5.2e9) * cosPulse(width) >> (width * 2),
-        'gaussian_with_window': (gaussian(10) >> width * 2) + square(width, edge=5, type='linear') * cos(
-            2 * pi * 5.2e9),
-    }
-
-    ip = '192.168.1.141'
-    trig = Trig()
-    adc = ADC()
-    dac = DAC()
-
-    trig.connect(ip, {'RefClock': 'in'})
-    adc.connect(ip)
-    dac.connect(ip)
-    adc.initADC()
-    dac.initDAC()
-    trig.initTrig()
-
-    dac.write_wave([MIX_BIT_WIDTH*waves['cos*gaussian'](time_line), MIX_BIT_WIDTH*waves['chirp_linear'](time_line)], 1)
-    dac.setTriggerDelays([100e-9, 200e-9], 1)
-    dac.setCount(1024)
-    dac.start([1])
-
-    adc.setCount(1024)
-    adc.write_mixerTable(np.ones((1, 16384, 1, 2)), 1)
-    adc.setTriggerDelays([0], 1)
-    adc.start([1])
-
-    trig.setIntervalTime(200e-6)
-    trig.setCount(1024)
-    trig.start([])
-
-    data = adc.collectWaveData(1)
+import enum
+import abc
+import dataclasses
+from typing import List, Union, Dict, Iterable, Sized
+from functools import wraps
+
+import numpy as np
+from ..NS_MCI import Driver as MCIDriver
+from ..NS_QSYNC import Driver as QSYNCDriver
+
+MIX_BIT_WIDTH = 32767
+SEGMENT_ENABLE = False
+
+
+@dataclasses.dataclass
+class DAChannelData:
+    seg_waves: "Sized|Iterable[np.ndarray]" = tuple()
+    delays: "Sized|Iterable[float]" = tuple()
+    data: np.ndarray = np.array([0])
+    updated: bool = False
+
+    @property
+    def right(self) -> bool:
+        return len(self.seg_waves) == len(self.delays)
+
+    def compute_data(self, rate):
+        """计算最后可下发给设备的data
+
+        :param rate: DA采样率，单位Hz
+        :return:
+        """
+        if not self.updated:
+            return
+        # if not self.right:
+        #     print(f'警告：波形片段数{len(self.seg_waves)}与波形延迟数{len(self.delays)}不匹配')
+        #     return
+        data = []
+        for seg, delay in zip(self.seg_waves, self.delays):
+            seg = seg / MIX_BIT_WIDTH
+            data.append(np.zeros((round(float(delay) * rate),)))
+            data.append(seg)
+        self.data = np.hstack(data)
+
+
+class ChannelDataPara(DAChannelData):
+    def __check_waveform(self, wave):
+        if wave.stop is None:
+            raise ValueError('waveform.stop为None，应为一确定波形时宽')
+        wave.start = 0 if wave.start is None else wave.start
+
+    def compute_data(self, rate):
+        import waveforms
+        if not self.updated:
+            return
+        if not self.right:
+            print(f'警告：波形片段数{len(self.seg_waves)}与波形延迟数{len(self.delays)}不匹配')
+            return
+        data = waveforms.zero()
+        wave_width = 0
+        for seg, delay in zip(self.seg_waves, self.delays):
+            seg: waveforms.Waveform
+            self.__check_waveform(seg)
+            wave_width += delay
+            window = waveforms.square(seg.stop - seg.start) >> seg.start
+            data += ((window*seg) >> wave_width)
+            wave_width += (seg.stop - seg.start)
+        self.data = np.array(data)
+
+
+@dataclasses.dataclass
+class ADConfig:
+    mixer_table: "np.ndarray" = np.zeros((1, 4096, 12, 2))
+    delays: "List[float]" = tuple()
+    updated: bool = False
+    coff_param: "Union[np.ndarray, List[np.ndarray]]" = (np.zeros((12, 4096), dtype=np.complex64), )
+    seg_conf: "List[List[float]]" = tuple()
+
+    @property
+    def right(self) -> bool:
+        return self.mixer_table.shape[0] == len(self.delays)
+
+    def compute_conf(self, rate):
+        """计算最后可下发给设备的采集conf
+
+        :param rate: AD采样率，单位Hz
+        :return:
+        """
+        if not self.updated:
+            return
+        if not self.right:
+            print(f'警告：mixer table片段数{len(self.mixer_table.shape[0])}与波形延迟数{len(self.delays)}不匹配')
+            return
+        coff_param = []
+        seg_conf = []
+        delay_count = 0
+        seg_length = self.mixer_table.shape[1]/rate
+        for idx, (table, delay) in enumerate(zip(self.mixer_table, self.delays)):
+            table: "np.ndarray"
+            table = table[:, :, 0] + table[:, :, 1]*1j
+            coff_param.append(table.T)
+            seg_conf.append([seg_length, delay_count])
+            delay_count += seg_length+delay if idx != 0 else seg_length
+        self.coff_param = coff_param
+        self.seg_conf = seg_conf
+
+
+class _BaseDriver(abc.ABC):
+    class DARunMode(enum.IntEnum):
+        TRIGGER_MODE = 1
+        """触发模式"""
+        CONTINUOUS_MODE = 2
+        """连续模式"""
+
+    class ADRunMode(enum.IntEnum):
+        ALGORITHMIC_MODE = 1
+        """算法采集模式"""
+        TRACE_MODE = 2
+        """时域采集模式"""
+
+    mode_map = {}
+
+    def __init__(self, *args):
+        self.driver: "MCIDriver" = MCIDriver()
+        self.sys_param = {
+            'MixMode': 2,  # Mix模式，1：第一奈奎斯特去； 2：第二奈奎斯特区
+            'PLLFreq': 100e6,  # 参考时钟频率, 单位为Hz
+            'RefClock': 'out',  # 参考时钟选择： ‘out’：外参考时钟；‘in’：内参考时钟
+            'ADrate': 4e9,  # AD采样率，单位Hz
+            'DArate': 6e9,  # DA采样率，单位Hz
+            'KeepAmp': 0,  # DA波形发射完毕后，保持最后一个值
+            'Delay': 0,  # 配置DA的原生Delay
+            'SegmentSampling': []  # 配置分段采样
+        }
+        self.connected = False
+
+        self.run_mode = None
+        self.run_count = 1024
+
+    def connect(self, address, *args) -> bool:
+        """连接设备
+
+        :param address: 设备ip
+        :param args:
+        :return:
+        """
+        if self.connected and self.driver.addr != address:
+            raise ValueError(f'系统已连接到{self.driver.addr}')
+        self.driver = MCIDriver(address)
+        self.driver.open()
+        return self.init_system(*args)
+
+    def disconnect(self, address, *args):
+        if self.connected and self.driver.addr != address:
+            raise ValueError(f'系统已连接到{self.driver.addr}，不可与{address}断开连接')
+        self.connected = False
+
+    @staticmethod
+    def with_connected(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            self: "_BaseDriver" = args[0]
+            if not self.connected:
+                raise RuntimeError(f'系统未连接，不可调用{self.__class__.__name__}.{func.__name__}')
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    def update_sys_parm(self, _input):
+        if len(_input) > 0 and isinstance(_input[0], dict):
+            self.sys_param.update(_input[0])
+
+    def init_system(self, *args) -> bool:
+        self.update_sys_parm(args)
+        self.connected = self.driver.init_device(system_parameter=self.sys_param)
+        return self.connected
+
+    def setRunMode(self, mode):
+        """设置运行模式
+
+        :param mode:
+        :return:
+        """
+        self.run_mode = self.mode_map.get(mode, 1)
+
+    # @with_connected
+    def setCount(self, N):
+        self.driver.set('Shot', N)
+        self.run_count = N
+
+    @abc.abstractmethod
+    def start(self, channels):
+        ...
+
+    def stop(self, channels):  # 停止channels里面指定的通道的运行
+        ...
+
+
+class DAC(_BaseDriver):
+    with_connected = _BaseDriver.with_connected
+    mode_map = {
+        2: _BaseDriver.DARunMode.CONTINUOUS_MODE,
+        1: _BaseDriver.DARunMode.TRIGGER_MODE
+    }
+
+    def __init__(self, *args):
+        super(DAC, self).__init__(*args)
+        self.run_mode = self.DARunMode.TRIGGER_MODE
+        self.run_wave_points = 0
+        self.run_da_seg_cache: "Dict[int, DAChannelData]" = {}
+
+    def initDAC(self):
+        self.init_system()
+        self.driver.set('EnableWaveCache', True)
+
+    @with_connected
+    def write_wave(self, waves, channeli):
+        """
+        给其中一个通道写波形，waves:[wave0,wave1,wave2,...]
+        其中wave0,wave1,...为能直接写入fpga的int数组或uint数组，这里可以写一段或多段波形，
+        触发模式下，仪器接收一个触发信号后，每段波形依次运行，波形之间的延迟可以通过setTriggerDelays函数设置
+        注意，对于每一个触发信号，waves里的波形都会被运行
+
+        :param waves: List[np.array]  int16
+        :param channeli: int
+        :return:
+        """
+        da_data = self.run_da_seg_cache.get(channeli, DAChannelData())
+        da_data.seg_waves = waves
+        da_data.updated = True
+        self.run_da_seg_cache[channeli] = da_data
+        # self._upload_wave([channeli])
+
+    @with_connected
+    def setTriggerDelays(self, delays, channeli):
+        """
+        设置trigger和发出波形之间的delays,只用于trig的运行模式，接收到trig后会前后相继的运行写入的[wave0,wave1,wave2,...]
+        delays=[delay0,delay1,delay2,....]一一对应于[wave0,wave1,wave2,...]
+        delay0为trig信号和wave0的起始时刻之间的延迟，delay1为wave0的末尾时刻和wave1的起始时刻之间的延迟，依次类推
+
+        :param delays: List[float]
+        :param channeli:
+        :return:
+        """
+        da_data = self.run_da_seg_cache.get(channeli, DAChannelData())
+        da_data.delays = delays
+        da_data.updated = True
+        self.run_da_seg_cache[channeli] = da_data
+        self._upload_wave([channeli])
+
+    @with_connected
+    def write_param_waveform(self, wave, channeli):
+        """发送要求wave为waveforms的Waveform对象
+
+        :param wave:
+        :param channeli:
+        :return:
+        """
+        self.driver.set('GenWave', wave, channeli)
+
+    @with_connected
+    def start(self, channels):
+        """当前后台仅能支持配置过波形的所有通道一起播放，后续支持
+
+        :param channels:
+        :return:
+        """
+        # 生效缓存的数据。支持ping-pang模式
+        self.driver.set('PushWaveCache')
+        if self.run_mode is self.DARunMode.CONTINUOUS_MODE:
+            period = self.run_wave_points / self.sys_param['DArate']
+            self.driver.set('GenerateTrig', period)
+
+    def _upload_wave(self, channels=None):
+        """按需计算要下发的data，并将缓存中“updated”的数据更新到设备中
+
+        :param channels:
+        :return:
+        """
+        channels = self.run_da_seg_cache.keys() if channels is None else channels
+        rate = self.sys_param['DArate']
+        for chnl in channels:
+            if chnl not in self.run_da_seg_cache:
+                continue
+            da_data = self.run_da_seg_cache[chnl]
+            da_data.compute_data(rate)
+            if not da_data.updated:
+                continue
+            self.driver.set('Waveform', da_data.data, chnl)
+            da_data.updated = False
+
+
+class ADC(_BaseDriver):
+    with_connected = _BaseDriver.with_connected
+    mode_map = {
+        1: _BaseDriver.ADRunMode.TRACE_MODE,
+        2: _BaseDriver.ADRunMode.ALGORITHMIC_MODE
+    }
+
+    def __init__(self, *args):
+        super(ADC, self).__init__(*args)
+        self.run_mode = self.ADRunMode.ALGORITHMIC_MODE
+        self.chnl_id = 0 if len(args) == 0 else args[0]
+        self.run_ad_chnl_conf: "Dict[int, ADConfig]" = {}
+
+    def initADC(self):
+        """连接ADC后进行初始化
+
+        :return:
+        """
+        self.init_system()
+
+    @with_connected
+    def write_mixerTable(self, mixData, channeli=None):
+        """算法采集模式下，事先把要用于算法采集模式的权重数据写入ADC
+
+        :param mixData: 如果ADC可以采集Y段波形，M为解模频点数，每段波形要在M个频率点做解模，时域波形一共L个点，
+                        那mixData的shape为:(Y,L,M,2),类型为int数组 或uint数组  np.array  int16
+        :param channeli:
+        :return:
+        """
+        channeli = self.chnl_id if channeli is None else channeli
+        ad_conf = self.run_ad_chnl_conf.get(channeli, ADConfig())
+        ad_conf.mixer_table = mixData
+        ad_conf.updated = True
+        self.run_ad_chnl_conf[channeli] = ad_conf
+
+    @with_connected
+    def setTriggerDelays(self, delays, channeli=None):
+        """设置trigger和采集波形之间的delays,接收到trig后会前后相继的采集waveDatas=[waveData0,waveData1,waveData2,...]
+            delays = [delay0,delay1,delay2,....]一一对应于[waveData0,waveData1,waveData2,...]
+            delay0为trig信号和waveData0的起始时刻之间的延迟，delay1为waveData0的末尾时刻和waveData1的起始时刻之间的延迟，依次类推
+
+        :param delays: List[float]
+        :param channeli:
+        :return:
+        """
+        channeli = self.chnl_id if channeli is None else channeli
+        ad_conf = self.run_ad_chnl_conf.get(channeli, ADConfig())
+        ad_conf.delays = delays
+        ad_conf.updated = True
+        self.run_ad_chnl_conf[channeli] = ad_conf
+
+    @with_connected
+    def collectWaveData(self, channeli=None):
+        """采集波形数据，waveDatas=[waveData0,waveData1,waveData2,...]，waveData? 为int数组，每接收一个trig，采集一次waveDatas
+            时域采集模式下,waveData0为第一段时域波形数据,shape为（N,L）,N为采集波形的次数，算法采集模式下，waveData0为解模后的数据，shape为（N，M）
+            ！注意该命令应该能在波形运行的过程中能采集，如果计划要采集N次，不能AWG的波形运行N次之后才采集，而是AWG边运行边采集，以加快速度
+
+        :return:
+        """
+        try:
+            channeli = self.chnl_id if channeli is None else channeli
+            if channeli not in self.run_ad_chnl_conf:
+                raise ValueError(f'未配置通道{channeli}的相关采集信息')
+            ad_conf = self.run_ad_chnl_conf[channeli]
+            seg_num = len(ad_conf.seg_conf)
+            if self.run_mode is self.ADRunMode.TRACE_MODE:
+                data = self.driver.get('TraceIQ', channeli)
+                seg_length = data.shape[1]//seg_num
+                data = [data[:, i:i+seg_length] for i in range(seg_num)]
+            else:
+                data = self.driver.get('IQ', channeli)
+                print(data)
+                if SEGMENT_ENABLE:
+                    data = [data[i] for i in range(seg_num)]
+            return data
+        except Exception as e:
+            print(e)
+
+    def clearBuf(self):
+        """清理ADC缓存的命令，假设上次运行报错，ADC能清理掉上次报错前所采集到的波形数据
+
+        :return:
+        """
+        self.driver.write('ResetCollect', None)
+
+    @with_connected
+    def start(self, channels):
+        """启动ADC的运行
+
+        :param channels: QMAC有4个ad通道编号为 [1, 2, 3, 4]
+        :return:
+        """
+        self._upload_collect_conf(channels)
+        self.driver.set('StartCapture')
+
+    def _upload_collect_conf(self, channels=None):
+        """按需计算要下发的data，并将缓存中“updated”的数据更新到设备中
+
+        :param channels:
+        :return:
+        """
+        channels = self.run_ad_chnl_conf.keys() if channels is None else channels
+        rate = self.sys_param['ADrate']
+        for chnl in channels:
+            if chnl not in self.run_ad_chnl_conf:
+                continue
+            ad_conf = self.run_ad_chnl_conf[chnl]
+            ad_conf.compute_conf(rate)
+            if not ad_conf.updated:
+                continue
+            self.driver.set('TriggerDelay', float(ad_conf.delays[0]), int(chnl))
+            if SEGMENT_ENABLE:
+                self.driver.set('SegmentSampling', ad_conf.seg_conf, int(chnl))
+                self.driver.set('DemodulationParam', ad_conf.coff_param, int(chnl))
+            else:
+                self.driver.set('SegmentSampling', [], int(chnl))
+                self.driver.set('DemodulationParam', ad_conf.coff_param[0], int(chnl))
+            ad_conf.updated = False
+
+class Trig(_BaseDriver):
+    class RunMode(enum.IntEnum):
+        INSIDE_MODE = 1
+        """内部触发模式"""
+        EXTERNAL_MODE = 2
+        """外部触发模式"""
+
+    mode_map = {
+        1: RunMode.INSIDE_MODE,
+        2: RunMode.EXTERNAL_MODE
+    }
+    with_connected = _BaseDriver.with_connected
+
+    def __init__(self, *args):
+        super(Trig, self).__init__(*args)
+        self.sys_param = {
+            'RefClock': 'in',  # 参考时钟选择： ‘out’：外参考时钟；‘in’：内参考时钟
+            'TrigFrom': 0,  # Trig来源： 0：内部产生；1：外部输入
+            'TrigPeriod': 200e-6,
+            'DiscoveryMode': QSYNCDriver.ScannMode.local,  # QC/QR等被同步设备的发现方式，见DiscoveryMode说明
+        }
+        self.run_mode = self.RunMode.INSIDE_MODE
+        self.driver: "QSYNCDriver" = QSYNCDriver()
+
+    def connect(self, address, *args):
+        self.driver = QSYNCDriver(address)
+        self.update_sys_parm(args)
+        self.driver.open(system_parameter=self.sys_param)
+        self.connected = True
+
+    @with_connected
+    def initTrig(self):
+        self.driver.set('ResetTrig')
+        self.driver.sync_system()
+
+    @with_connected
+    def setClock(self, **kws):
+        """设置时钟运行相关参数,比如外部或内部时钟，时钟频率等等
+
+        :param kws: 参考信号 RefClock，TrigFrom
+        :return:
+        """
+        self.update_sys_parm((kws, ))
+        self.driver.open(system_parameter=self.sys_param)
+
+    def checkStatus(self):  # 查看相关状态，比如时钟是多少MHz，是外部接入还是内部产生，trig信号的间隔，宽度，每个通道发出trig信号的延迟
+        print(self.sys_param)
+
+    @with_connected
+    def setTrigOffset(self, time, channel):  # 设置通道channel的trigger信号的延迟
+        self.driver.set('TrigOffset', time)
+
+    @with_connected
+    def setIntervalTime(self, time):  # 设置触发
+        """
+        :param time: 秒
+        """
+        self.driver.set('TrigPeriod', time)
+
+    def setIntervalShape(self, width, amplitude):  # 设置触发信号宽度和高度
+        self.driver.set('TrigWidth', width)
+
+    def start(self, channels):  # 启动trig信号的运行
+        if self.run_mode is self.RunMode.INSIDE_MODE:
+            self.driver.set('GenerateTrig')
+
+    def stop(self, channels):  # 停止trig信号的运行
+        if self.run_mode is self.RunMode.INSIDE_MODE:
+            self.driver.set('ResetTrig')
+
+
+trig = Trig
+
+
+if __name__ == '__main__':
+    from waveforms import *
+
+    sample_rate = 6e9
+    width = 20e-9
+    time_line = np.linspace(0, width*10, int(width * 10 * sample_rate))
+    waves = {
+        'poly': poly([1, -1 / 2, 1 / 6, -1 / 12]),
+        'cos': cos(2 * pi * 5.2e9),
+        'sin': sin(2 * pi * 5.2e9),
+        'gaussian': gaussian(width) >> (width * 2),
+        'sinc': sinc(6e8),
+        'square': square(width) >> (width * 2),
+        'cosPulse': cosPulse(width) >> (width * 2),
+        'chirp_linear': chirp(1e9, 1.5e9, width * 10, type='linear'),
+        'chirp_exponential': chirp(1e9, 1.5e9, width * 10, type='exponential'),
+        'chirp_hyperbolic': chirp(1e9, 1.5e9, width * 10, type='hyperbolic'),
+        'cos*gaussian': cos(2 * pi * 5.2e9) * gaussian(width) >> (width * 2),
+        'cos*cosPulse': cos(2 * pi * 5.2e9) * cosPulse(width) >> (width * 2),
+        'gaussian_with_window': (gaussian(10) >> width * 2) + square(width, edge=5, type='linear') * cos(
+            2 * pi * 5.2e9),
+    }
+
+    ip = '192.168.1.141'
+    trig = Trig()
+    adc = ADC()
+    dac = DAC()
+
+    trig.connect(ip, {'RefClock': 'in'})
+    adc.connect(ip)
+    dac.connect(ip)
+    adc.initADC()
+    dac.initDAC()
+    trig.initTrig()
+
+    dac.write_wave([MIX_BIT_WIDTH*waves['cos*gaussian'](time_line), MIX_BIT_WIDTH*waves['chirp_linear'](time_line)], 1)
+    dac.setTriggerDelays([100e-9, 200e-9], 1)
+    dac.setCount(1024)
+    dac.start([1])
+
+    adc.setCount(1024)
+    adc.write_mixerTable(np.ones((1, 16384, 1, 2)), 1)
+    adc.setTriggerDelays([0], 1)
+    adc.start([1])
+
+    trig.setIntervalTime(200e-6)
+    trig.setCount(1024)
+    trig.start([])
+
+    data = adc.collectWaveData(1)
```

## nsqdriver/wrapper/BD_NSMCI.py

 * *Ordering differences only*

```diff
@@ -1,310 +1,310 @@
-import time
-from typing import Dict, Any, List
-
-import numpy as np
-
-from nsqdriver import MCIDriver, QSYNCDriver
-
-
-try:
-    import Instrument
-except ImportError as e:
-    class Instrument(object):
-        ...
-
-
-class NSInstrument(Instrument):
-    """ Instrument for GuoDun devices """
-    ParameterMC = {
-        'OUTSrate': 8e9,      # 配置OUT通道采样率
-        'OUTMix': 2,          # 设置OUT通道增强第二奈奎斯特区信号
-        'INZone': 'zone3'     # 设置IN通道输入为Zone4，即要IN通道要采集的信号范围为6~8G
-    }
-    ParameterZ = {
-        'OUTSrate': 2e9,      # 配置OUT通道采样率
-        'OUTMix': 1,          # 设置OUT通道增强第一奈奎斯特区信号
-        'KeepAmp': 2          # 开启Z通道的保持电平模式，2为保持drive信号电平
-    }
-    ParameterQSYNC = {
-        'RefClock': 'in'      # MC112的100M参考信号来源，机箱上的100M IN没有接的情况下，选择为in，反之选out
-    }
-
-    def __init__(self):
-        """ Initialization """
-        super(NSInstrument, self).__init__()
-
-        # 设备驱动
-        self.driver_mc: MCIDriver = MCIDriver('192.168.111.152')
-        self.driver_z: MCIDriver = MCIDriver('192.168.111.132')
-        self.qsync: QSYNCDriver = QSYNCDriver('192.168.111.152')
-
-        # 参数
-        self.waves = dict()
-        self.roFreq = dict()
-        self.roQubits = dict()
-        self.roLength = dict()
-        self.roDADelay = dict()
-        self.zpdc = dict()
-        self.group = dict()
-        self.roLines = dict()
-        self.connectDict = dict()
-        self.deviceDict = dict()
-        self.qubitROChannels = dict()
-        self.integrationDelay = dict()
-        self.inputRange = dict()
-        self.outputRange = dict()
-        self.devices = {
-            'awg': self.driver_mc,
-            'dc': self.driver_z,
-            'qa': self.driver_mc,
-        }  # type: Dict[str, Any]
-        self.shots = 1000
-        self.devicesList = {
-            'awg': [],
-            'dc': [],
-            'qa': []
-        }  # type: Dict[str, Any]
-
-    def connectDevices(self, *args, **kwargs):
-        """ Connect and initialize devices """
-        if 'devices' not in kwargs.keys():
-            raise ValueError('Parameter `devices` does not exist in connectDevices().')
-        if 'connect' not in kwargs.keys():
-            raise ValueError('Parameter `connect` does not exist in connectDevices().')
-        if 'roLines' not in kwargs.keys():
-            raise ValueError('Parameter `roLines` does not exist in connectDevices().')
-
-        self.roLines = kwargs['roLines']
-        """
-        The readout line dict. Example:
-        {"r1":["q01","q02","q03","q04","q05"], "r2": ["q06","q07","q08","q09","q10"], ...}
-        """
-
-        self.deviceDict = kwargs['devices']
-        """
-        The dict for all devices. Example:
-        {
-            "XY":["mc_1", ...],
-            "Z":["z_1", ...],
-            "ZDC":["z_1", ...],
-            "RO":["out01", "out09", ...],
-            "QA":["in01", "in09", ...]
-        }
-        """
-
-        self.connectDict = kwargs['connect']
-        """
-        The mapping between device channels and logical channels. Example:
-        {
-            "QA": {"r1QA": ["in01", "range(20)"], "r2QA": ["in09", "range(20)"], ...},
-            "RO": {"r1RO": ["out01", "range(20)"], "r2RO": ["out09", "range(20)"], ...},
-            "RO_qubits": {"q01RO": "r1RO", "q02RO": "r1RO", "q03RO": "r1RO", ...},
-            "RO_trig": {"r1RO": "AWG5M1", "r2RO": "AWG5M1", ...},
-            "XY": {"q03XY": ["mc_1", "out03"], "q04XY": ["mc_1", "out04"], ...},
-            "Z": {"q03Z": ["z_1", "out01"], "q04Z": ["z_1", "out02"]}
-        }
-
-        """
-
-        # Parse readout channels
-        for _line, _qubits in self.roLines.items():
-            ro_channels = [i for i in eval(self.connectDict['RO'][f'{_line}RO'][1])]
-            if len(ro_channels) != len(_qubits):
-                raise RuntimeError(f'Qubit number in {_line} does not equal to '
-                                   f'the number of channels ({ro_channels}).')
-            for _q, _c in zip(self.roLines[_line], ro_channels):
-                self.qubitROChannels[f'{_q}RO'] = _c
-
-        # Connect device
-        # 在kw参数中寻找系统初始化相关参数
-        qs_sp = self.ParameterQSYNC.copy()
-        qs_sp.update(kwargs.get('qs_param', {}))
-        mc_sp = self.ParameterMC.copy()
-        mc_sp.update(kwargs.get('mc_param', {}))
-        z_sp = self.ParameterZ.copy()
-        z_sp.update(kwargs.get('z_param', {}))
-
-        self.qsync.open(system_parameter=qs_sp)
-        self.driver_mc.open(system_parameter=mc_sp)
-        self.driver_z.open(system_parameter=z_sp)
-        self.qsync.sync_system()
-
-    def _rline2chnl(self, rline):
-        return int(self.connectDict['QA'][f'{rline}QA'][0][-2:])
-
-    def _xy2chnl(self, _key):
-        return int(self.connectDict['XY'][_key][1][-2:])
-
-    def _z2chnl(self, _key):
-        return int(self.connectDict['Z'][_key][1][-2:])
-
-    def _qubit2rline(self, qubit):
-        return self.connectDict['RO_qubits'][f'{qubit}RO'][:2]
-
-    def disconnectDevices(self, *args, **kwargs):
-        """ Initialize devices """
-        ...
-
-    # def expendBatchChannels(self):
-
-    def stopOutput(self, *args, **kwargs):
-        """ Stop the output of waveforms """
-        self.qsync.set('ResetTrig')
-
-    def startOutput(self, *args, **kwargs):
-        """ Stop the output of waveforms """
-        self.qsync.set('GenerateTrig')
-
-    def uploadWaveforms(self, *args, **kwargs):
-        """ Upload waveforms """
-        if 'waves' not in kwargs.keys():
-            raise ValueError('Parameter `waves` does not exist in uploadWaveforms().')
-        if 'zpdc' not in kwargs.keys():
-            raise ValueError('Parameter `zpdc` does not exist in uploadWaveforms().')
-
-        self.setINDemod(**kwargs)
-        self.setRODADelay(**kwargs)
-        self.zpdc = kwargs['zpdc']
-
-        waves = kwargs['waves']
-        waves_map = {}
-        for _key, _wave in waves.items():
-            _devChannel = None
-            if _key in self.connectDict['XY'].keys():
-                _devChannel = self._xy2chnl(_key)
-                self.driver_mc.set('Waveform', _wave, _devChannel)
-            elif _key in self.connectDict['Z'].keys():
-                _devChannel = self._z2chnl(_key)
-                self.driver_mc.set('Waveform', _wave, _devChannel)
-            elif _key in self.qubitROChannels.keys():
-                _devChannel = self._qubit2rline(_key)
-                wave_list = waves_map.get(_devChannel, [])
-                wave_list.append(_wave)
-            if _devChannel is None:
-                raise RuntimeError(f'Channel {_key} does not found.')
-            print(_key, _devChannel, len(_wave))
-
-        # 合并下发probe da波形
-        for _line, wave_list in waves_map.items():
-            max_points = max(_w.size() for _w in wave_list)
-            wave_array = np.zeros((len(self.roLines[_line]), max_points))
-            for idx, _w in enumerate(wave_list):
-                wave_array[idx][:_w.size()] = _w
-            self.driver_mc.set('Waveform', wave_array.mean(axis=0), self._rline2chnl(_line))
-
-        # import matplotlib.pyplot as plt
-        # for _key, _seq in self.waves.items():
-        #     plt.plot(_seq, label=_key)
-        # plt.legend()
-        # plt.show()
-
-    def downloadIQ(self, *args, **kwargs):
-        """ Download IQ data """
-        self.setIntegrationDelay(**kwargs)
-        self.startOutput()
-        st_time = time.time()
-        roChannels = {}
-        print('self.roQubits', self.roQubits)
-        for _r in self.roQubits.keys():
-            roChannels[_r] = [self.qubitROChannels[f'{_q}RO'] for _q in self.roQubits[_r]]
-        print('roChannels', roChannels)
-        full = {
-            _r: self.driver_mc.get('IQ', channel=self._rline2chnl(_r))
-            for _r in self.roQubits.keys()
-        }
-        print('get iq data timing:', time.time() - st_time)
-
-        iqDict = dict()
-        for qubit, iqData in zip(self.roQubits.values(), full.values()):
-            for _q in qubit:
-                iqDict[_q] = iqData[self.qubitROChannels[f'{_q}RO']]
-        return iqDict
-
-    def setINDemod(self, *args, **kwargs):
-        """!
-        配置MC设备的解模系数
-        @param args:
-        @param kwargs:
-        @return:
-        """
-        if 'roQubits' not in kwargs.keys():
-            raise ValueError('Parameter `roQubits` does not exist in uploadWaveforms().')
-        if 'roLength' not in kwargs.keys():
-            raise ValueError('Parameter `roLength` does not exist in uploadWaveforms().')
-        if 'roFreq' not in kwargs.keys():
-            raise ValueError('Parameter `roFreq` does not exist in uploadWaveforms().')
-        self.roQubits = kwargs['roQubits']
-        self.roLength = {_line: [length / 1e9 for length in lengths] for _line, lengths in kwargs['roLength'].items()}
-        self.roFreq = {_line: [freq / 1e9 for freq in freqs] for _line, freqs in kwargs['roFreq'].items()}
-
-        for _line, qubits in self.roQubits.items():
-            freqs = {_q: 1e9 for _q in self.roLines[_line]}
-            lengths = {_q: 512e-9 for _q in self.roLines[_line]}
-            for _q, _freq, _len in zip(qubits, self.roFreq[_line], self.roLength[_line]):
-                freqs[_q] = _freq
-                lengths[_q] = _len
-            print(f'The configured demodulation frequency point is ({freqs})')
-            self.driver_mc.set('TimeWidth', list(lengths.values()), self._rline2chnl(_line))
-            self.driver_mc.set('FreqList', max(freqs.values()), self._rline2chnl(_line))
-
-    def setRODADelay(self, *args, **kwargs):
-        """!
-        配置probe da相对触发的延迟
-        配置粒度为16ns的整倍数
-        @param args:
-        @param kwargs:
-        @return:
-        """
-        if 'roDADelay' in kwargs.keys():
-            for _line, delay in kwargs['roDADelay'].items():
-                self.roDADelay[_line] = delay/1e9
-                self.driver_mc.set('OUTDelay', self.roDADelay[_line], self._rline2chnl(_line))
-        else:
-            raise ValueError('Parameter `roDADelay` does not exist in uploadWaveforms().')
-
-    def setShots(self, *args, **kwargs):
-        """ Set shots """
-        if 'shots' not in kwargs.keys():
-            raise ValueError('Parameter `shots` does not exist in setShots().')
-        shots = kwargs['shots']
-        self.shots = shots
-        self.qsync.set('Shot', shots)
-        self.driver_mc.set('Shot', shots)
-        print("set shots:", shots)
-
-    def setHoldoffTime(self, *args, **kwargs):
-        """ Set hold-off time """
-        if 'interval' not in kwargs.keys():
-            raise ValueError('Parameter `interval` does not exist in setHoldoffTime().')
-        interval = kwargs['interval']
-        self.qsync.set('TrigPeriod', interval / 1e9)  # 单位：s
-
-    def setLO(self, *args, **kwargs):
-        """ Set LO """
-        ...
-
-    def setIntegrationDelay(self, *args, **kwargs):
-        """ Set readout integration delay. """
-        if 'integrationDelay' in kwargs.keys():
-            for _channel, delay in kwargs['integrationDelay'].items():
-                self.integrationDelay[_channel] = delay
-                self.driver_mc.set('INDelay', delay / 1e9, self._rline2chnl(_channel))
-        else:
-            raise ValueError('Parameter `integrationDelay` does not exist in setIntegrationDelay().')
-
-    def setInputRange(self, *args, **kwargs):
-        """ Set input range for output channels """
-        if 'inputRange' in kwargs.keys():
-            for _channel, _value in kwargs['inputRange'].items():
-                devChannel = self.connectDict['QA'][_channel][1]
-                self.inputRange[devChannel] = _value
-        else:
-            raise ValueError('Parameter `inputRange` does not exist in setInputRange().')
-
-    def setOutputRange(self, *args, **kwargs):
-        """ Set output range for output channels """
-        if 'outputRange' in kwargs.keys():
-            for _channel, delay in kwargs['outputRange'].items():
-                self.outputRange[_channel] = delay
-        else:
-            raise ValueError('Parameter `outputRange` does not exist in setOutputRange().')
+import time
+from typing import Dict, Any, List
+
+import numpy as np
+
+from nsqdriver import MCIDriver, QSYNCDriver
+
+
+try:
+    import Instrument
+except ImportError as e:
+    class Instrument(object):
+        ...
+
+
+class NSInstrument(Instrument):
+    """ Instrument for GuoDun devices """
+    ParameterMC = {
+        'OUTSrate': 8e9,      # 配置OUT通道采样率
+        'OUTMix': 2,          # 设置OUT通道增强第二奈奎斯特区信号
+        'INZone': 'zone3'     # 设置IN通道输入为Zone4，即要IN通道要采集的信号范围为6~8G
+    }
+    ParameterZ = {
+        'OUTSrate': 2e9,      # 配置OUT通道采样率
+        'OUTMix': 1,          # 设置OUT通道增强第一奈奎斯特区信号
+        'KeepAmp': 2          # 开启Z通道的保持电平模式，2为保持drive信号电平
+    }
+    ParameterQSYNC = {
+        'RefClock': 'in'      # MC112的100M参考信号来源，机箱上的100M IN没有接的情况下，选择为in，反之选out
+    }
+
+    def __init__(self):
+        """ Initialization """
+        super(NSInstrument, self).__init__()
+
+        # 设备驱动
+        self.driver_mc: MCIDriver = MCIDriver('192.168.111.152')
+        self.driver_z: MCIDriver = MCIDriver('192.168.111.132')
+        self.qsync: QSYNCDriver = QSYNCDriver('192.168.111.152')
+
+        # 参数
+        self.waves = dict()
+        self.roFreq = dict()
+        self.roQubits = dict()
+        self.roLength = dict()
+        self.roDADelay = dict()
+        self.zpdc = dict()
+        self.group = dict()
+        self.roLines = dict()
+        self.connectDict = dict()
+        self.deviceDict = dict()
+        self.qubitROChannels = dict()
+        self.integrationDelay = dict()
+        self.inputRange = dict()
+        self.outputRange = dict()
+        self.devices = {
+            'awg': self.driver_mc,
+            'dc': self.driver_z,
+            'qa': self.driver_mc,
+        }  # type: Dict[str, Any]
+        self.shots = 1000
+        self.devicesList = {
+            'awg': [],
+            'dc': [],
+            'qa': []
+        }  # type: Dict[str, Any]
+
+    def connectDevices(self, *args, **kwargs):
+        """ Connect and initialize devices """
+        if 'devices' not in kwargs.keys():
+            raise ValueError('Parameter `devices` does not exist in connectDevices().')
+        if 'connect' not in kwargs.keys():
+            raise ValueError('Parameter `connect` does not exist in connectDevices().')
+        if 'roLines' not in kwargs.keys():
+            raise ValueError('Parameter `roLines` does not exist in connectDevices().')
+
+        self.roLines = kwargs['roLines']
+        """
+        The readout line dict. Example:
+        {"r1":["q01","q02","q03","q04","q05"], "r2": ["q06","q07","q08","q09","q10"], ...}
+        """
+
+        self.deviceDict = kwargs['devices']
+        """
+        The dict for all devices. Example:
+        {
+            "XY":["mc_1", ...],
+            "Z":["z_1", ...],
+            "ZDC":["z_1", ...],
+            "RO":["out01", "out09", ...],
+            "QA":["in01", "in09", ...]
+        }
+        """
+
+        self.connectDict = kwargs['connect']
+        """
+        The mapping between device channels and logical channels. Example:
+        {
+            "QA": {"r1QA": ["in01", "range(20)"], "r2QA": ["in09", "range(20)"], ...},
+            "RO": {"r1RO": ["out01", "range(20)"], "r2RO": ["out09", "range(20)"], ...},
+            "RO_qubits": {"q01RO": "r1RO", "q02RO": "r1RO", "q03RO": "r1RO", ...},
+            "RO_trig": {"r1RO": "AWG5M1", "r2RO": "AWG5M1", ...},
+            "XY": {"q03XY": ["mc_1", "out03"], "q04XY": ["mc_1", "out04"], ...},
+            "Z": {"q03Z": ["z_1", "out01"], "q04Z": ["z_1", "out02"]}
+        }
+
+        """
+
+        # Parse readout channels
+        for _line, _qubits in self.roLines.items():
+            ro_channels = [i for i in eval(self.connectDict['RO'][f'{_line}RO'][1])]
+            if len(ro_channels) != len(_qubits):
+                raise RuntimeError(f'Qubit number in {_line} does not equal to '
+                                   f'the number of channels ({ro_channels}).')
+            for _q, _c in zip(self.roLines[_line], ro_channels):
+                self.qubitROChannels[f'{_q}RO'] = _c
+
+        # Connect device
+        # 在kw参数中寻找系统初始化相关参数
+        qs_sp = self.ParameterQSYNC.copy()
+        qs_sp.update(kwargs.get('qs_param', {}))
+        mc_sp = self.ParameterMC.copy()
+        mc_sp.update(kwargs.get('mc_param', {}))
+        z_sp = self.ParameterZ.copy()
+        z_sp.update(kwargs.get('z_param', {}))
+
+        self.qsync.open(system_parameter=qs_sp)
+        self.driver_mc.open(system_parameter=mc_sp)
+        self.driver_z.open(system_parameter=z_sp)
+        self.qsync.sync_system()
+
+    def _rline2chnl(self, rline):
+        return int(self.connectDict['QA'][f'{rline}QA'][0][-2:])
+
+    def _xy2chnl(self, _key):
+        return int(self.connectDict['XY'][_key][1][-2:])
+
+    def _z2chnl(self, _key):
+        return int(self.connectDict['Z'][_key][1][-2:])
+
+    def _qubit2rline(self, qubit):
+        return self.connectDict['RO_qubits'][f'{qubit}RO'][:2]
+
+    def disconnectDevices(self, *args, **kwargs):
+        """ Initialize devices """
+        ...
+
+    # def expendBatchChannels(self):
+
+    def stopOutput(self, *args, **kwargs):
+        """ Stop the output of waveforms """
+        self.qsync.set('ResetTrig')
+
+    def startOutput(self, *args, **kwargs):
+        """ Stop the output of waveforms """
+        self.qsync.set('GenerateTrig')
+
+    def uploadWaveforms(self, *args, **kwargs):
+        """ Upload waveforms """
+        if 'waves' not in kwargs.keys():
+            raise ValueError('Parameter `waves` does not exist in uploadWaveforms().')
+        if 'zpdc' not in kwargs.keys():
+            raise ValueError('Parameter `zpdc` does not exist in uploadWaveforms().')
+
+        self.setINDemod(**kwargs)
+        self.setRODADelay(**kwargs)
+        self.zpdc = kwargs['zpdc']
+
+        waves = kwargs['waves']
+        waves_map = {}
+        for _key, _wave in waves.items():
+            _devChannel = None
+            if _key in self.connectDict['XY'].keys():
+                _devChannel = self._xy2chnl(_key)
+                self.driver_mc.set('Waveform', _wave, _devChannel)
+            elif _key in self.connectDict['Z'].keys():
+                _devChannel = self._z2chnl(_key)
+                self.driver_mc.set('Waveform', _wave, _devChannel)
+            elif _key in self.qubitROChannels.keys():
+                _devChannel = self._qubit2rline(_key)
+                wave_list = waves_map.get(_devChannel, [])
+                wave_list.append(_wave)
+            if _devChannel is None:
+                raise RuntimeError(f'Channel {_key} does not found.')
+            print(_key, _devChannel, len(_wave))
+
+        # 合并下发probe da波形
+        for _line, wave_list in waves_map.items():
+            max_points = max(_w.size() for _w in wave_list)
+            wave_array = np.zeros((len(self.roLines[_line]), max_points))
+            for idx, _w in enumerate(wave_list):
+                wave_array[idx][:_w.size()] = _w
+            self.driver_mc.set('Waveform', wave_array.mean(axis=0), self._rline2chnl(_line))
+
+        # import matplotlib.pyplot as plt
+        # for _key, _seq in self.waves.items():
+        #     plt.plot(_seq, label=_key)
+        # plt.legend()
+        # plt.show()
+
+    def downloadIQ(self, *args, **kwargs):
+        """ Download IQ data """
+        self.setIntegrationDelay(**kwargs)
+        self.startOutput()
+        st_time = time.time()
+        roChannels = {}
+        print('self.roQubits', self.roQubits)
+        for _r in self.roQubits.keys():
+            roChannels[_r] = [self.qubitROChannels[f'{_q}RO'] for _q in self.roQubits[_r]]
+        print('roChannels', roChannels)
+        full = {
+            _r: self.driver_mc.get('IQ', channel=self._rline2chnl(_r))
+            for _r in self.roQubits.keys()
+        }
+        print('get iq data timing:', time.time() - st_time)
+
+        iqDict = dict()
+        for qubit, iqData in zip(self.roQubits.values(), full.values()):
+            for _q in qubit:
+                iqDict[_q] = iqData[self.qubitROChannels[f'{_q}RO']]
+        return iqDict
+
+    def setINDemod(self, *args, **kwargs):
+        """!
+        配置MC设备的解模系数
+        @param args:
+        @param kwargs:
+        @return:
+        """
+        if 'roQubits' not in kwargs.keys():
+            raise ValueError('Parameter `roQubits` does not exist in uploadWaveforms().')
+        if 'roLength' not in kwargs.keys():
+            raise ValueError('Parameter `roLength` does not exist in uploadWaveforms().')
+        if 'roFreq' not in kwargs.keys():
+            raise ValueError('Parameter `roFreq` does not exist in uploadWaveforms().')
+        self.roQubits = kwargs['roQubits']
+        self.roLength = {_line: [length / 1e9 for length in lengths] for _line, lengths in kwargs['roLength'].items()}
+        self.roFreq = {_line: [freq / 1e9 for freq in freqs] for _line, freqs in kwargs['roFreq'].items()}
+
+        for _line, qubits in self.roQubits.items():
+            freqs = {_q: 1e9 for _q in self.roLines[_line]}
+            lengths = {_q: 512e-9 for _q in self.roLines[_line]}
+            for _q, _freq, _len in zip(qubits, self.roFreq[_line], self.roLength[_line]):
+                freqs[_q] = _freq
+                lengths[_q] = _len
+            print(f'The configured demodulation frequency point is ({freqs})')
+            self.driver_mc.set('TimeWidth', list(lengths.values()), self._rline2chnl(_line))
+            self.driver_mc.set('FreqList', max(freqs.values()), self._rline2chnl(_line))
+
+    def setRODADelay(self, *args, **kwargs):
+        """!
+        配置probe da相对触发的延迟
+        配置粒度为16ns的整倍数
+        @param args:
+        @param kwargs:
+        @return:
+        """
+        if 'roDADelay' in kwargs.keys():
+            for _line, delay in kwargs['roDADelay'].items():
+                self.roDADelay[_line] = delay/1e9
+                self.driver_mc.set('OUTDelay', self.roDADelay[_line], self._rline2chnl(_line))
+        else:
+            raise ValueError('Parameter `roDADelay` does not exist in uploadWaveforms().')
+
+    def setShots(self, *args, **kwargs):
+        """ Set shots """
+        if 'shots' not in kwargs.keys():
+            raise ValueError('Parameter `shots` does not exist in setShots().')
+        shots = kwargs['shots']
+        self.shots = shots
+        self.qsync.set('Shot', shots)
+        self.driver_mc.set('Shot', shots)
+        print("set shots:", shots)
+
+    def setHoldoffTime(self, *args, **kwargs):
+        """ Set hold-off time """
+        if 'interval' not in kwargs.keys():
+            raise ValueError('Parameter `interval` does not exist in setHoldoffTime().')
+        interval = kwargs['interval']
+        self.qsync.set('TrigPeriod', interval / 1e9)  # 单位：s
+
+    def setLO(self, *args, **kwargs):
+        """ Set LO """
+        ...
+
+    def setIntegrationDelay(self, *args, **kwargs):
+        """ Set readout integration delay. """
+        if 'integrationDelay' in kwargs.keys():
+            for _channel, delay in kwargs['integrationDelay'].items():
+                self.integrationDelay[_channel] = delay
+                self.driver_mc.set('INDelay', delay / 1e9, self._rline2chnl(_channel))
+        else:
+            raise ValueError('Parameter `integrationDelay` does not exist in setIntegrationDelay().')
+
+    def setInputRange(self, *args, **kwargs):
+        """ Set input range for output channels """
+        if 'inputRange' in kwargs.keys():
+            for _channel, _value in kwargs['inputRange'].items():
+                devChannel = self.connectDict['QA'][_channel][1]
+                self.inputRange[devChannel] = _value
+        else:
+            raise ValueError('Parameter `inputRange` does not exist in setInputRange().')
+
+    def setOutputRange(self, *args, **kwargs):
+        """ Set output range for output channels """
+        if 'outputRange' in kwargs.keys():
+            for _channel, delay in kwargs['outputRange'].items():
+                self.outputRange[_channel] = delay
+        else:
+            raise ValueError('Parameter `outputRange` does not exist in setOutputRange().')
```

## nsqdriver/wrapper/ND_NSMCI.py

 * *Ordering differences only*

```diff
@@ -1,245 +1,245 @@
-import numpy as np
-from nsqdriver import MCIDriver, QSYNCDriver
-
-
-class _XYChannel:
-    def __init__(self, mci: "DeviceBase", ch=1):
-        self.mci = mci
-        self.ch = ch
-        self.to_zero = np.zeros((16,))
-        self.to_one = np.ones((16,))
-        self.en = True
-        self.mode = 0
-        self.off = 0
-
-    def wave(self, w):
-        self.wavex(w, self.ch)
-
-    def wavex(self, w, idx):
-        if np.max(np.abs(w)) < 1e-30:
-            wr = np.zeros(16)
-        else:
-            wr = w
-        self.mci.mci_driver.set("Waveform", wr, idx)
-
-    def arm(self, k=None):
-        self.mci.mci_driver.set('PushWaveCache')
-
-    def trig_del(self, delay):
-        ...
-
-    def output_del(self, delay):
-        ...
-
-    def __del__(self):
-        pass
-
-    def output(self, b):
-        self.en = bool(b)
-        if not self.en:
-            self.mci.mci_driver.set("Waveform", self.to_zero, self.ch)
-
-    def mode(self, m_):
-        ...
-
-    def offsetx(self, off, idx):
-        self.mci.mci_driver.set('Waveform', off*self.to_one, idx)
-        self.off = off
-
-    def offset(self, off):
-        self.offsetx(off, self.ch)
-
-    W = {
-        "wave": wave,
-        "output": output,
-        "trig_del": trig_del,
-        "output_del": output_del,
-        "mode": mode,
-        "offset": offset,
-    }
-
-    Q = {"arm": arm}
-
-
-class _ZChannel(_XYChannel):
-    pass
-
-
-class _Probe:
-    def __init__(self, mci: "DeviceBase", ch=1):
-        self.mci = mci
-        self.ch = ch
-        self.freqList = []
-        self.SGS = None  # single shot temp cache
-        self.AVG = None  # average temp cache
-        self.depth = 2000
-        self._width = 1000
-        self.start = 500
-        self.demod = 1
-        self.averaged_I = np.zeros((16384, ))  # 直播直采，相当于只有I路数据
-
-    def depth(self, depth_):
-        self.depth = depth_
-        self.mci.mci_driver.set('PointNumber', depth_, self.ch)
-
-    def demodulation_on(self, demod_):
-        self.demod = int(demod_)
-
-    def start(self, start_):
-        self.start = start_
-        self.mci.mci_driver.set('TriggerDelay', start_, self.ch)
-
-    def width(self, width_):
-        self._width = width_/4e9
-        self.mci.mci_driver.set('PointNumber', width_, self.ch)
-
-    def freqs(self, *freqList_):
-        self.freqList = freqList_
-        self.mci.mci_driver.set('FreqList', freqList_, self.ch)
-
-    def shot(self, _shot):
-        self.mci.mci_driver.set('Shot', _shot)
-
-    def measure(self, k=None):
-        self.mci.mci_driver.set('StartCapture')
-        if self.demod:
-            self.SGS = self.mci.mci_driver.get('IQ', self.ch)
-            self.AVG = np.mean(self.SGS, axis=0)
-        else:
-            self.averaged_I = np.mean(self.mci.mci_driver.get('TraceIQ', self.ch), axis=0)
-
-    def single_shot(self, k=None):
-        return self.SGS
-
-    def average(self, k=None):
-        return self.AVG
-
-    def trace_I(self, k=None):
-        return self.averaged_I
-
-    def trace_Q(self, k=None):
-        return self.averaged_I
-
-    def __del__(self):
-        pass
-
-    W = {
-        "demod": demodulation_on,
-        "depth": depth,
-        "width": width,
-        "start": start,
-        "freqs": freqs,
-        "shot": shot,
-    }
-
-    Q = {
-        "measure": measure,
-        "A": average,
-        "S": single_shot,
-        "traceI": trace_I,
-        "traceQ": trace_Q
-    };
-
-
-# one box need one class
-class DeviceBase:
-    def __init__(self):
-        self.mci_driver = MCIDriver('127.0.0.1')
-        self.qsync_driver = QSYNCDriver('127.0.0.1')
-
-
-class NS_MCI(DeviceBase):
-    def __init__(self, addr, srate=10e9, mixmode=2, ref_clk='in'):
-        """!
-        此类涉及到系统同步，放到最后实例化
-        @param addr: 设备ip
-        @param srate: OUT通道采样率
-        @param mixmode: 为2时开启OUT通道混合模式，增强第二奈奎斯特区输出
-        @param ref_clk: 设备参考信号来源，不接外输出100M时都配置为'in'
-        """
-        super(NS_MCI, self).__init__()
-        self.mci_driver = MCIDriver(addr)
-        self.qsync = QSYNCDriver(addr)
-        self.srate = srate
-        self.mixmode = mixmode
-        self.ref_clk = ref_clk
-        self.connect()
-
-    def connect(self):
-        mci_params = {'DArate': self.srate, 'MixMode': self.mixmode}
-        qsync_params = {'RefClock': self.ref_clk}
-
-        self.qsync.open(system_parameter=qsync_params)
-        self.mci_driver.open(system_parameter=mci_params)
-        self.qsync.sync_system()
-
-        self.mci_driver.set('EnableWaveCache', True)
-
-        for _ch in range(22):
-            xy_ch = _ch+1
-            setattr(self, f'OUT{xy_ch}', _XYChannel(self, xy_ch))
-        for _ch in range(2):
-            probe_ch = _ch+1
-            setattr(self, f'IN{probe_ch}', _Probe(self, probe_ch))
-
-    def trig_interval(self, interval):
-        self.interval = interval
-        self.qsync.set('TrigPeriod', int(interval))
-
-    def trig_count(self, count_):
-        self.qsync.set('Shot', int(count_))
-
-    def trig(self):
-        self.qsync.set('GenerateTrig', self.interval)
-
-    def awg_arm(self):
-        self.mci_driver.set('PushWaveCache')
-
-    def __del__(self):
-        pass
-
-    W = {
-        "trig_interval": trig_interval,
-        "trig_count": trig_count,
-        "connect": connect,
-        "trig": trig,
-        "awg_arm": awg_arm,
-    }
-
-    Q = {
-    }
-
-
-class NS_Z(DeviceBase):
-    def __init__(self, addr, mixmode=2):
-        """!
-        此类负责控制24 Z OUT通道的设备，采样率固定为2Gsps，mixmode固定为1
-        @param addr: 设备ip
-        @param mixmode: 为1时关闭OUT通道混合模式
-        """
-        super(NS_Z, self).__init__()
-        self.mci_driver = MCIDriver(addr)
-        self.qsync = QSYNCDriver(addr)
-        self.srate = 2e9
-        self.mixmode = 1
-        self.connect()
-
-    def connect(self):
-        mci_params = {'DArate': self.srate, 'MixMode': self.mixmode}
-        self.mci_driver.open(system_parameter=mci_params)
-
-        self.mci_driver.set('EnableWaveCache', True)
-
-        for _ch in range(24):
-            xy_ch = _ch+1
-            setattr(self, f'OUT{xy_ch}', _ZChannel(self, xy_ch))
-
-    def awg_arm(self):
-        self.mci_driver.set('PushWaveCache')
-
-    W = {
-        "connect": connect,
-    }
-
-    Q = {
-    }
+import numpy as np
+from nsqdriver import MCIDriver, QSYNCDriver
+
+
+class _XYChannel:
+    def __init__(self, mci: "DeviceBase", ch=1):
+        self.mci = mci
+        self.ch = ch
+        self.to_zero = np.zeros((16,))
+        self.to_one = np.ones((16,))
+        self.en = True
+        self.mode = 0
+        self.off = 0
+
+    def wave(self, w):
+        self.wavex(w, self.ch)
+
+    def wavex(self, w, idx):
+        if np.max(np.abs(w)) < 1e-30:
+            wr = np.zeros(16)
+        else:
+            wr = w
+        self.mci.mci_driver.set("Waveform", wr, idx)
+
+    def arm(self, k=None):
+        self.mci.mci_driver.set('PushWaveCache')
+
+    def trig_del(self, delay):
+        ...
+
+    def output_del(self, delay):
+        ...
+
+    def __del__(self):
+        pass
+
+    def output(self, b):
+        self.en = bool(b)
+        if not self.en:
+            self.mci.mci_driver.set("Waveform", self.to_zero, self.ch)
+
+    def mode(self, m_):
+        ...
+
+    def offsetx(self, off, idx):
+        self.mci.mci_driver.set('Waveform', off*self.to_one, idx)
+        self.off = off
+
+    def offset(self, off):
+        self.offsetx(off, self.ch)
+
+    W = {
+        "wave": wave,
+        "output": output,
+        "trig_del": trig_del,
+        "output_del": output_del,
+        "mode": mode,
+        "offset": offset,
+    }
+
+    Q = {"arm": arm}
+
+
+class _ZChannel(_XYChannel):
+    pass
+
+
+class _Probe:
+    def __init__(self, mci: "DeviceBase", ch=1):
+        self.mci = mci
+        self.ch = ch
+        self.freqList = []
+        self.SGS = None  # single shot temp cache
+        self.AVG = None  # average temp cache
+        self.depth = 2000
+        self._width = 1000
+        self.start = 500
+        self.demod = 1
+        self.averaged_I = np.zeros((16384, ))  # 直播直采，相当于只有I路数据
+
+    def depth(self, depth_):
+        self.depth = depth_
+        self.mci.mci_driver.set('PointNumber', depth_, self.ch)
+
+    def demodulation_on(self, demod_):
+        self.demod = int(demod_)
+
+    def start(self, start_):
+        self.start = start_
+        self.mci.mci_driver.set('TriggerDelay', start_, self.ch)
+
+    def width(self, width_):
+        self._width = width_/4e9
+        self.mci.mci_driver.set('PointNumber', width_, self.ch)
+
+    def freqs(self, *freqList_):
+        self.freqList = freqList_
+        self.mci.mci_driver.set('FreqList', freqList_, self.ch)
+
+    def shot(self, _shot):
+        self.mci.mci_driver.set('Shot', _shot)
+
+    def measure(self, k=None):
+        self.mci.mci_driver.set('StartCapture')
+        if self.demod:
+            self.SGS = self.mci.mci_driver.get('IQ', self.ch)
+            self.AVG = np.mean(self.SGS, axis=0)
+        else:
+            self.averaged_I = np.mean(self.mci.mci_driver.get('TraceIQ', self.ch), axis=0)
+
+    def single_shot(self, k=None):
+        return self.SGS
+
+    def average(self, k=None):
+        return self.AVG
+
+    def trace_I(self, k=None):
+        return self.averaged_I
+
+    def trace_Q(self, k=None):
+        return self.averaged_I
+
+    def __del__(self):
+        pass
+
+    W = {
+        "demod": demodulation_on,
+        "depth": depth,
+        "width": width,
+        "start": start,
+        "freqs": freqs,
+        "shot": shot,
+    }
+
+    Q = {
+        "measure": measure,
+        "A": average,
+        "S": single_shot,
+        "traceI": trace_I,
+        "traceQ": trace_Q
+    };
+
+
+# one box need one class
+class DeviceBase:
+    def __init__(self):
+        self.mci_driver = MCIDriver('127.0.0.1')
+        self.qsync_driver = QSYNCDriver('127.0.0.1')
+
+
+class NS_MCI(DeviceBase):
+    def __init__(self, addr, srate=10e9, mixmode=2, ref_clk='in'):
+        """!
+        此类涉及到系统同步，放到最后实例化
+        @param addr: 设备ip
+        @param srate: OUT通道采样率
+        @param mixmode: 为2时开启OUT通道混合模式，增强第二奈奎斯特区输出
+        @param ref_clk: 设备参考信号来源，不接外输出100M时都配置为'in'
+        """
+        super(NS_MCI, self).__init__()
+        self.mci_driver = MCIDriver(addr)
+        self.qsync = QSYNCDriver(addr)
+        self.srate = srate
+        self.mixmode = mixmode
+        self.ref_clk = ref_clk
+        self.connect()
+
+    def connect(self):
+        mci_params = {'DArate': self.srate, 'MixMode': self.mixmode}
+        qsync_params = {'RefClock': self.ref_clk}
+
+        self.qsync.open(system_parameter=qsync_params)
+        self.mci_driver.open(system_parameter=mci_params)
+        self.qsync.sync_system()
+
+        self.mci_driver.set('EnableWaveCache', True)
+
+        for _ch in range(22):
+            xy_ch = _ch+1
+            setattr(self, f'OUT{xy_ch}', _XYChannel(self, xy_ch))
+        for _ch in range(2):
+            probe_ch = _ch+1
+            setattr(self, f'IN{probe_ch}', _Probe(self, probe_ch))
+
+    def trig_interval(self, interval):
+        self.interval = interval
+        self.qsync.set('TrigPeriod', int(interval))
+
+    def trig_count(self, count_):
+        self.qsync.set('Shot', int(count_))
+
+    def trig(self):
+        self.qsync.set('GenerateTrig', self.interval)
+
+    def awg_arm(self):
+        self.mci_driver.set('PushWaveCache')
+
+    def __del__(self):
+        pass
+
+    W = {
+        "trig_interval": trig_interval,
+        "trig_count": trig_count,
+        "connect": connect,
+        "trig": trig,
+        "awg_arm": awg_arm,
+    }
+
+    Q = {
+    }
+
+
+class NS_Z(DeviceBase):
+    def __init__(self, addr, mixmode=2):
+        """!
+        此类负责控制24 Z OUT通道的设备，采样率固定为2Gsps，mixmode固定为1
+        @param addr: 设备ip
+        @param mixmode: 为1时关闭OUT通道混合模式
+        """
+        super(NS_Z, self).__init__()
+        self.mci_driver = MCIDriver(addr)
+        self.qsync = QSYNCDriver(addr)
+        self.srate = 2e9
+        self.mixmode = 1
+        self.connect()
+
+    def connect(self):
+        mci_params = {'DArate': self.srate, 'MixMode': self.mixmode}
+        self.mci_driver.open(system_parameter=mci_params)
+
+        self.mci_driver.set('EnableWaveCache', True)
+
+        for _ch in range(24):
+            xy_ch = _ch+1
+            setattr(self, f'OUT{xy_ch}', _ZChannel(self, xy_ch))
+
+    def awg_arm(self):
+        self.mci_driver.set('PushWaveCache')
+
+    W = {
+        "connect": connect,
+    }
+
+    Q = {
+    }
```

## Comparing `nsqdriver-0.3.3.dist-info/METADATA` & `nsqdriver-0.4.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,103 +1,104 @@
-Metadata-Version: 2.1
-Name: nsqdriver
-Version: 0.3.3
-Summary: Naishu Q series quantum measurement and control equipment driver interface
-Home-page: https://g2hoyqcmh4.feishu.cn/wiki/wikcnzvyMd82DLZUe2NsI6HxsFc
-Author: Naishu Technology
-Author-email: jilianyi@naishu.tech
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: numpy (>=1.18)
-Requires-Dist: waveforms
-
-```
-  _   _   ____     ___    ____           _                       
- | \ | | / ___|   / _ \  |  _ \   _ __  (_) __   __   ___   _ __ 
- |  \| | \___ \  | | | | | | | | | '__| | | \ \ / /  / _ \ | '__|
- | |\  |  ___) | | |_| | | |_| | | |    | |  \ V /  |  __/ | |   
- |_| \_| |____/   \__\_\ |____/  |_|    |_|   \_/    \___| |_|   
-```
-
-[![Tests](https://github.com/mianyan-echo/UltraMCI/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/mianyan-echo/UltraMCI/)
-***
-
-### 简介
-NSQDriver为一套耐数®量子测控系列设备的Python通用驱动接口。可使用Python作为编程语言，基于此驱动接口可以实现对本公司测控设备的控制，进而完成各种超导量子芯片的表征实验和高保真门操作。
-
-```
-                              +------------------------+
-                              |          Python        |
-                              |     +------------------+
-                              |     |      NSQDriver   |
-                              +------------------------+
-                                     :     :         :
-                           +----------     :         -----+
-                           :               :              :
-                           V               V              V
-                     +-----------+   +-----------+   +-----------+   
-                     |  Device A |   |  Device B |   |   QSYNC   |    
-                     +-----------+   +-----------+   +-----------+   
-```
-
-NSQDriver接口可用于统一控制耐数®生产的Q100、MC、QSYNC等一系列量子测控仪器，可详细控制每台仪器每个OUT、IN通道的播放与采集行为，以及查看设备的运行状态等。在一个多台测控设备组成的多量子比特测控系统中，可以有效的在软件层面实现对系统中每台设备的详细控制。
-
-耐数®量子测控系列设备详细信息参考: [耐数](http://naishu.tech)
-
-***
-### 快速开始
-- 驱动接口的通用流程如下
-```python
-from nsqdriver import MCIDriver, QSYNCDriver
-
-# 实例化设备驱动接口
-driver = MCIDriver('127.0.0.1')
-qsync = QSYNCDriver('127.0.0.1')
-
-# 连接设备
-qsync.open()
-driver.open()
-
-# 初始化系统
-qsync.sync_system()
-
-
-# 相关参数，参数细节相关参考 8.可用参数列表
-driver.set('Shot', 1024)
-```
-
-- NSWave接口
-  - NSWave是一种对于耐数®参数化波形技术的控制接口，参数化波形将量子测控所需的各种门的编辑由主控计算机直接生成波形转化成了设备实时计算
-  - 提供了一套直观的时序编辑接口
-```python
-from nsqdriver import InsChannel
-import numpy as np
-
-ch = InsChannel()                        # 生成参数化波形通道实例
-
-frame_65e9 = ch.ins_frame(6.5e9)         # 生成一个frame
-frame_67e9 = ch.ins_frame(6.7e9)         # 生成一个frame
-
-gaussian = ch.evlp_gaussian(4500e-9)     # 生成一个高斯包络
-square = ch.evlp_square(2500e-9)         # 生成一个方波包络
-
-wave1 = gaussian * frame_67e9            # 生成一段高斯包络的波形
-wave2 = square * frame_65e9              # 生成一段方波包络的波形
-
-ch.ins_reset_frame('phase', frame_65e9)
-ch.ins_reset_frame('phase', frame_67e9)
-ch.wait_for_trigger()                    # 等待触发到来
-# 循环播放200次 3μs延迟+ 7μs波形
-with ch.ins_loop(times=200) as _loop:
-    _loop.play_zero(3000e-9)
-    _loop.inc_phase(frame_65e9, np.pi / 2)
-    _loop.play_wave(wave2)
-    _loop.play_wave(wave1)
-```
+Metadata-Version: 2.1
+Name: nsqdriver
+Version: 0.4.0
+Summary: Naishu Q series quantum measurement and control equipment driver interface
+Home-page: https://g2hoyqcmh4.feishu.cn/wiki/wikcnzvyMd82DLZUe2NsI6HxsFc
+Author: Naishu Technology
+Author-email: jilianyi@naishu.tech
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: numpy (>=1.18)
+Provides-Extra: waveforms
+Requires-Dist: waveforms ; extra == 'waveforms'
+
+```
+  _   _   ____     ___    ____           _                       
+ | \ | | / ___|   / _ \  |  _ \   _ __  (_) __   __   ___   _ __ 
+ |  \| | \___ \  | | | | | | | | | '__| | | \ \ / /  / _ \ | '__|
+ | |\  |  ___) | | |_| | | |_| | | |    | |  \ V /  |  __/ | |   
+ |_| \_| |____/   \__\_\ |____/  |_|    |_|   \_/    \___| |_|   
+```
+***
+
+### 简介
+NSQDriver为一套耐数®量子测控系列设备的Python通用驱动接口。可使用Python作为编程语言，基于此驱动接口可以实现对本公司测控设备的控制，进而完成各种超导量子芯片的表征实验和高保真门操作。
+
+```
+                              +------------------------+
+                              |          Python        |
+                              |     +------------------+
+                              |     |      NSQDriver   |
+                              +------------------------+
+                                     :     :         :
+                           +----------     :         -----+
+                           :               :              :
+                           V               V              V
+                     +-----------+   +-----------+   +-----------+   
+                     |  Device A |   |  Device B |   |   QSYNC   |    
+                     +-----------+   +-----------+   +-----------+   
+```
+
+NSQDriver接口可用于统一控制耐数®生产的Q100、MC、QSYNC等一系列量子测控仪器，可详细控制每台仪器每个OUT、IN通道的播放与采集行为，以及查看设备的运行状态等。在一个多台测控设备组成的多量子比特测控系统中，可以有效的在软件层面实现对系统中每台设备的详细控制。
+
+耐数®量子测控系列设备详细信息参考: [耐数](http://naishu.tech)
+
+***
+### 快速开始
+- 驱动接口的通用流程如下
+```python
+from nsqdriver import MCIDriver, QSYNCDriver
+
+# 实例化设备驱动接口
+driver = MCIDriver('127.0.0.1')
+qsync = QSYNCDriver('127.0.0.1')
+
+# 连接设备
+qsync.open()
+driver.open()
+
+# 初始化系统
+qsync.sync_system()
+
+
+# 相关参数，参数细节相关参考 8.可用参数列表
+driver.set('Shot', 1024)
+```
+
+- NSWave接口
+  - NSWave是一种对于耐数®Sequence序列发生技术的控制接口，Sequence序列发生模式将量子测控所需的各种门的编辑由主控计算机直接生成波形转化成了设备实时计算
+  - 提供了一套直观的时序编辑接口
+  - 如下示例展示了使用nswave控制设备重复播放一段波形200次
+```python
+from nsqdriver import InsChannel
+import numpy as np
+
+ch = InsChannel()                        # 生成参数化波形通道实例
+
+frame_65e9 = ch.ins_frame(6.5e9)         # 生成一个frame
+frame_67e9 = ch.ins_frame(6.7e9)         # 生成一个frame
+
+gaussian = ch.evlp_gaussian(4500e-9)     # 生成一个高斯包络
+square = ch.evlp_square(2500e-9)         # 生成一个方波包络
+
+wave1 = gaussian * frame_67e9            # 生成一段高斯包络的波形
+wave2 = square * frame_65e9              # 生成一段方波包络的波形
+
+ch.ins_reset_frame('phase', frame_65e9)
+ch.ins_reset_frame('phase', frame_67e9)
+ch.wait_for_trigger()                    # 等待触发到来
+# 循环播放200次 3μs延迟+ 7μs波形
+with ch.ins_loop(times=200) as _loop:
+    _loop.play_zero(3000e-9)
+    _loop.inc_phase(frame_65e9, np.pi / 2)
+    _loop.play_wave(wave2)
+    _loop.play_wave(wave1)
+```
```

