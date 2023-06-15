# Comparing `tmp/tencentcloud-sdk-python-csip-3.0.914.tar.gz` & `tmp/tencentcloud-sdk-python-csip-3.0.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-csip-3.0.914.tar", last modified: Wed Jun 14 00:23:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-csip-3.0.915.tar", last modified: Thu Jun 15 00:22:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-csip-3.0.914.tar` & `tencentcloud-sdk-python-csip-3.0.915.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud_sdk_python_csip.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud_sdk_python_csip.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud_sdk_python_csip.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud_sdk_python_csip.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud_sdk_python_csip.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud/csip/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud/csip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud/csip/v20221121/
--rw-r--r--   0 root         (0) root         (0)     8878 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud/csip/v20221121/csip_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud/csip/v20221121/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud/csip/v20221121/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61284 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud/csip/v20221121/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:23:32.000000 tencentcloud-sdk-python-csip-3.0.914/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud_sdk_python_csip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud_sdk_python_csip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud_sdk_python_csip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud_sdk_python_csip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud_sdk_python_csip.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud/csip/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud/csip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud/csip/v20221121/
+-rw-r--r--   0 root         (0) root         (0)    13590 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud/csip/v20221121/csip_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud/csip/v20221121/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud/csip/v20221121/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   108427 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud/csip/v20221121/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:22:37.000000 tencentcloud-sdk-python-csip-3.0.915/setup.cfg
```

### Comparing `tencentcloud-sdk-python-csip-3.0.914/tencentcloud_sdk_python_csip.egg-info/PKG-INFO` & `tencentcloud-sdk-python-csip-3.0.915/tencentcloud_sdk_python_csip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csip
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Csip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csip-3.0.914/README.rst` & `tencentcloud-sdk-python-csip-3.0.915/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.914/tencentcloud/csip/v20221121/errorcodes.py` & `tencentcloud-sdk-python-csip-3.0.915/tencentcloud/csip/v20221121/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.914/tencentcloud/csip/v20221121/models.py` & `tencentcloud-sdk-python-csip-3.0.915/tencentcloud/csip/v20221121/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -211,14 +211,377 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AssetClusterPod(AbstractModel):
+    """集群pod列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AppId: 租户id
+        :type AppId: int
+        :param Uin: 租户uin
+        :type Uin: str
+        :param Nick: 租户昵称
+        :type Nick: str
+        :param Region: 地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        :param AssetId: pod id
+        :type AssetId: str
+        :param AssetName: pod名称
+        :type AssetName: str
+        :param InstanceCreateTime: pod创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceCreateTime: str
+        :param Namespace: 命名空间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Namespace: str
+        :param Status: 状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: str
+        :param ClusterId: 集群id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterId: str
+        :param ClusterName: 集群名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterName: str
+        :param MachineId: 主机id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MachineId: str
+        :param MachineName: 主机名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MachineName: str
+        :param PodIp: pod ip
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PodIp: str
+        :param ServiceCount: 关联service数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ServiceCount: int
+        :param ContainerCount: 关联容器数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ContainerCount: int
+        :param PublicIp: 公网ip
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PublicIp: str
+        :param PrivateIp: 内网ip
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PrivateIp: str
+        :param IsCore: 是否核心：1:核心，2:非核心
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsCore: int
+        """
+        self.AppId = None
+        self.Uin = None
+        self.Nick = None
+        self.Region = None
+        self.AssetId = None
+        self.AssetName = None
+        self.InstanceCreateTime = None
+        self.Namespace = None
+        self.Status = None
+        self.ClusterId = None
+        self.ClusterName = None
+        self.MachineId = None
+        self.MachineName = None
+        self.PodIp = None
+        self.ServiceCount = None
+        self.ContainerCount = None
+        self.PublicIp = None
+        self.PrivateIp = None
+        self.IsCore = None
+
+
+    def _deserialize(self, params):
+        self.AppId = params.get("AppId")
+        self.Uin = params.get("Uin")
+        self.Nick = params.get("Nick")
+        self.Region = params.get("Region")
+        self.AssetId = params.get("AssetId")
+        self.AssetName = params.get("AssetName")
+        self.InstanceCreateTime = params.get("InstanceCreateTime")
+        self.Namespace = params.get("Namespace")
+        self.Status = params.get("Status")
+        self.ClusterId = params.get("ClusterId")
+        self.ClusterName = params.get("ClusterName")
+        self.MachineId = params.get("MachineId")
+        self.MachineName = params.get("MachineName")
+        self.PodIp = params.get("PodIp")
+        self.ServiceCount = params.get("ServiceCount")
+        self.ContainerCount = params.get("ContainerCount")
+        self.PublicIp = params.get("PublicIp")
+        self.PrivateIp = params.get("PrivateIp")
+        self.IsCore = params.get("IsCore")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AssetViewPortRisk(AbstractModel):
+    """资产视角的端口风险对象
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Port: 端口
+        :type Port: int
+        :param AffectAsset: 影响资产
+        :type AffectAsset: str
+        :param Level: 风险等级
+        :type Level: str
+        :param InstanceType: 资产类型
+        :type InstanceType: str
+        :param Protocol: 协议
+        :type Protocol: str
+        :param Component: 组件
+        :type Component: str
+        :param Service: 服务
+        :type Service: str
+        :param RecentTime: 最近识别时间
+        :type RecentTime: str
+        :param FirstTime: 首次识别时间
+        :type FirstTime: str
+        :param Suggestion: 处置建议,0保持现状、1限制访问、2封禁端口
+        :type Suggestion: int
+        :param Status: 状态，0未处理、1已处置、2已忽略
+        :type Status: int
+        :param Id: 资产唯一id
+        :type Id: str
+        :param Index: 前端索引
+        :type Index: str
+        :param InstanceId: 实例id
+        :type InstanceId: str
+        :param InstanceName: 实例名
+        :type InstanceName: str
+        :param AppId: 用户appid
+        :type AppId: str
+        :param Nick: 用户昵称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Nick: str
+        :param Uin: 用户uin
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Uin: str
+        :param From: 来源
+        :type From: str
+        """
+        self.Port = None
+        self.AffectAsset = None
+        self.Level = None
+        self.InstanceType = None
+        self.Protocol = None
+        self.Component = None
+        self.Service = None
+        self.RecentTime = None
+        self.FirstTime = None
+        self.Suggestion = None
+        self.Status = None
+        self.Id = None
+        self.Index = None
+        self.InstanceId = None
+        self.InstanceName = None
+        self.AppId = None
+        self.Nick = None
+        self.Uin = None
+        self.From = None
+
+
+    def _deserialize(self, params):
+        self.Port = params.get("Port")
+        self.AffectAsset = params.get("AffectAsset")
+        self.Level = params.get("Level")
+        self.InstanceType = params.get("InstanceType")
+        self.Protocol = params.get("Protocol")
+        self.Component = params.get("Component")
+        self.Service = params.get("Service")
+        self.RecentTime = params.get("RecentTime")
+        self.FirstTime = params.get("FirstTime")
+        self.Suggestion = params.get("Suggestion")
+        self.Status = params.get("Status")
+        self.Id = params.get("Id")
+        self.Index = params.get("Index")
+        self.InstanceId = params.get("InstanceId")
+        self.InstanceName = params.get("InstanceName")
+        self.AppId = params.get("AppId")
+        self.Nick = params.get("Nick")
+        self.Uin = params.get("Uin")
+        self.From = params.get("From")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AssetViewVULRisk(AbstractModel):
+    """资产视角的漏洞风险对象
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AffectAsset: 影响资产
+        :type AffectAsset: str
+        :param Level: 风险等级
+        :type Level: str
+        :param InstanceType: 资产类型
+        :type InstanceType: str
+        :param Component: 组件
+        :type Component: str
+        :param Service: 服务
+        :type Service: str
+        :param RecentTime: 最近识别时间
+        :type RecentTime: str
+        :param FirstTime: 首次识别时间
+        :type FirstTime: str
+        :param Status: 状态，0未处理、1已处置、2已忽略
+        :type Status: int
+        :param Id: 资产唯一id
+        :type Id: str
+        :param Index: 前端索引
+        :type Index: str
+        :param InstanceId: 实例id
+        :type InstanceId: str
+        :param InstanceName: 实例名
+        :type InstanceName: str
+        :param AppId: 用户appid
+        :type AppId: str
+        :param Nick: 用户昵称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Nick: str
+        :param Uin: 用户uin
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Uin: str
+        :param VULType: 漏洞类型
+        :type VULType: str
+        :param Port: 端口
+        :type Port: str
+        :param Describe: 描述
+        :type Describe: str
+        :param AppName: 版本名
+        :type AppName: str
+        :param References: 相关信息
+        :type References: str
+        :param AppVersion: 版本
+        :type AppVersion: str
+        :param VULURL: 漏洞url
+        :type VULURL: str
+        :param VULName: 漏洞名称
+        :type VULName: str
+        :param CVE: cve
+        :type CVE: str
+        :param Fix: 修复建议
+        :type Fix: str
+        :param POCId: pocid
+        :type POCId: str
+        :param From: 来源
+        :type From: str
+        :param CWPVersion: 主机版本
+        :type CWPVersion: int
+        :param IsSupportRepair: 是否支持修复
+        :type IsSupportRepair: bool
+        :param IsSupportDetect: 是否支持扫描
+        :type IsSupportDetect: bool
+        :param InstanceUUID: 实例uuid
+        :type InstanceUUID: str
+        :param Payload: 负载
+        :type Payload: str
+        :param EMGCVulType: 应急漏洞类型，1-应急漏洞，0-非应急漏洞
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EMGCVulType: int
+        """
+        self.AffectAsset = None
+        self.Level = None
+        self.InstanceType = None
+        self.Component = None
+        self.Service = None
+        self.RecentTime = None
+        self.FirstTime = None
+        self.Status = None
+        self.Id = None
+        self.Index = None
+        self.InstanceId = None
+        self.InstanceName = None
+        self.AppId = None
+        self.Nick = None
+        self.Uin = None
+        self.VULType = None
+        self.Port = None
+        self.Describe = None
+        self.AppName = None
+        self.References = None
+        self.AppVersion = None
+        self.VULURL = None
+        self.VULName = None
+        self.CVE = None
+        self.Fix = None
+        self.POCId = None
+        self.From = None
+        self.CWPVersion = None
+        self.IsSupportRepair = None
+        self.IsSupportDetect = None
+        self.InstanceUUID = None
+        self.Payload = None
+        self.EMGCVulType = None
+
+
+    def _deserialize(self, params):
+        self.AffectAsset = params.get("AffectAsset")
+        self.Level = params.get("Level")
+        self.InstanceType = params.get("InstanceType")
+        self.Component = params.get("Component")
+        self.Service = params.get("Service")
+        self.RecentTime = params.get("RecentTime")
+        self.FirstTime = params.get("FirstTime")
+        self.Status = params.get("Status")
+        self.Id = params.get("Id")
+        self.Index = params.get("Index")
+        self.InstanceId = params.get("InstanceId")
+        self.InstanceName = params.get("InstanceName")
+        self.AppId = params.get("AppId")
+        self.Nick = params.get("Nick")
+        self.Uin = params.get("Uin")
+        self.VULType = params.get("VULType")
+        self.Port = params.get("Port")
+        self.Describe = params.get("Describe")
+        self.AppName = params.get("AppName")
+        self.References = params.get("References")
+        self.AppVersion = params.get("AppVersion")
+        self.VULURL = params.get("VULURL")
+        self.VULName = params.get("VULName")
+        self.CVE = params.get("CVE")
+        self.Fix = params.get("Fix")
+        self.POCId = params.get("POCId")
+        self.From = params.get("From")
+        self.CWPVersion = params.get("CWPVersion")
+        self.IsSupportRepair = params.get("IsSupportRepair")
+        self.IsSupportDetect = params.get("IsSupportDetect")
+        self.InstanceUUID = params.get("InstanceUUID")
+        self.Payload = params.get("Payload")
+        self.EMGCVulType = params.get("EMGCVulType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CVMAssetVO(AbstractModel):
     """主机资产信息
 
     """
 
     def __init__(self):
         r"""
@@ -365,14 +728,17 @@
         :type MemberId: str
         :param Os: os全称
 注意：此字段可能返回 null，表示取不到有效值。
         :type Os: str
         :param RiskExposure: 风险服务暴露
 注意：此字段可能返回 null，表示取不到有效值。
         :type RiskExposure: int
+        :param BASAgentStatus: 模拟攻击工具状态。0代表未安装，1代表已安装，2代表已离线
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BASAgentStatus: int
         """
         self.AssetId = None
         self.AssetName = None
         self.AssetType = None
         self.Region = None
         self.CWPStatus = None
         self.AssetCreateTime = None
@@ -415,14 +781,15 @@
         self.VulnerabilityRisk = None
         self.ConfigurationRisk = None
         self.ScanTask = None
         self.Tag = None
         self.MemberId = None
         self.Os = None
         self.RiskExposure = None
+        self.BASAgentStatus = None
 
 
     def _deserialize(self, params):
         self.AssetId = params.get("AssetId")
         self.AssetName = params.get("AssetName")
         self.AssetType = params.get("AssetType")
         self.Region = params.get("Region")
@@ -472,14 +839,15 @@
             for item in params.get("Tag"):
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tag.append(obj)
         self.MemberId = params.get("MemberId")
         self.Os = params.get("Os")
         self.RiskExposure = params.get("RiskExposure")
+        self.BASAgentStatus = params.get("BASAgentStatus")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -937,14 +1305,106 @@
             for item in params.get("OsList"):
                 obj = FilterDataObject()
                 obj._deserialize(item)
                 self.OsList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeClusterPodAssetsRequest(AbstractModel):
+    """DescribeClusterPodAssets请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Filter: 过滤
+        :type Filter: :class:`tencentcloud.csip.v20221121.models.Filter`
+        """
+        self.Filter = None
+
+
+    def _deserialize(self, params):
+        if params.get("Filter") is not None:
+            self.Filter = Filter()
+            self.Filter._deserialize(params.get("Filter"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeClusterPodAssetsResponse(AbstractModel):
+    """DescribeClusterPodAssets返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 列表
+        :type Data: list of AssetClusterPod
+        :param TotalCount: 总数
+        :type TotalCount: int
+        :param PodStatusList: 集群pod状态枚举
+        :type PodStatusList: list of FilterDataObject
+        :param NamespaceList: 命名空间枚举
+        :type NamespaceList: list of FilterDataObject
+        :param RegionList: 地域枚举
+        :type RegionList: list of FilterDataObject
+        :param AppIdList: 租户枚举
+        :type AppIdList: list of FilterDataObject
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.TotalCount = None
+        self.PodStatusList = None
+        self.NamespaceList = None
+        self.RegionList = None
+        self.AppIdList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self.Data = []
+            for item in params.get("Data"):
+                obj = AssetClusterPod()
+                obj._deserialize(item)
+                self.Data.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        if params.get("PodStatusList") is not None:
+            self.PodStatusList = []
+            for item in params.get("PodStatusList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.PodStatusList.append(obj)
+        if params.get("NamespaceList") is not None:
+            self.NamespaceList = []
+            for item in params.get("NamespaceList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.NamespaceList.append(obj)
+        if params.get("RegionList") is not None:
+            self.RegionList = []
+            for item in params.get("RegionList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.RegionList.append(obj)
+        if params.get("AppIdList") is not None:
+            self.AppIdList = []
+            for item in params.get("AppIdList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.AppIdList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDbAssetInfoRequest(AbstractModel):
     """DescribeDbAssetInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1083,14 +1543,431 @@
             for item in params.get("AppIdList"):
                 obj = FilterDataObject()
                 obj._deserialize(item)
                 self.AppIdList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDomainAssetsRequest(AbstractModel):
+    """DescribeDomainAssets请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Filter: -
+        :type Filter: :class:`tencentcloud.csip.v20221121.models.Filter`
+        """
+        self.Filter = None
+
+
+    def _deserialize(self, params):
+        if params.get("Filter") is not None:
+            self.Filter = Filter()
+            self.Filter._deserialize(params.get("Filter"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDomainAssetsResponse(AbstractModel):
+    """DescribeDomainAssets返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Total: -
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Total: int
+        :param Data: -
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Data: list of DomainAssetVO
+        :param DefenseStatusList: 防护状态列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DefenseStatusList: list of FilterDataObject
+        :param AssetLocationList: 资产归属地列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetLocationList: list of FilterDataObject
+        :param SourceTypeList: 资产类型列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SourceTypeList: list of FilterDataObject
+        :param RegionList: 地域列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RegionList: list of FilterDataObject
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Total = None
+        self.Data = None
+        self.DefenseStatusList = None
+        self.AssetLocationList = None
+        self.SourceTypeList = None
+        self.RegionList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Total = params.get("Total")
+        if params.get("Data") is not None:
+            self.Data = []
+            for item in params.get("Data"):
+                obj = DomainAssetVO()
+                obj._deserialize(item)
+                self.Data.append(obj)
+        if params.get("DefenseStatusList") is not None:
+            self.DefenseStatusList = []
+            for item in params.get("DefenseStatusList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.DefenseStatusList.append(obj)
+        if params.get("AssetLocationList") is not None:
+            self.AssetLocationList = []
+            for item in params.get("AssetLocationList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.AssetLocationList.append(obj)
+        if params.get("SourceTypeList") is not None:
+            self.SourceTypeList = []
+            for item in params.get("SourceTypeList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.SourceTypeList.append(obj)
+        if params.get("RegionList") is not None:
+            self.RegionList = []
+            for item in params.get("RegionList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.RegionList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribePublicIpAssetsRequest(AbstractModel):
+    """DescribePublicIpAssets请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Filter: filte过滤条件
+        :type Filter: :class:`tencentcloud.csip.v20221121.models.Filter`
+        """
+        self.Filter = None
+
+
+    def _deserialize(self, params):
+        if params.get("Filter") is not None:
+            self.Filter = Filter()
+            self.Filter._deserialize(params.get("Filter"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribePublicIpAssetsResponse(AbstractModel):
+    """DescribePublicIpAssets返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Data: list of IpAssetListVO
+        :param Total: 总数
+        :type Total: int
+        :param AssetLocationList: 资产归属地
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetLocationList: list of FilterDataObject
+        :param IpTypeList: ip列表枚举
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpTypeList: list of FilterDataObject
+        :param RegionList: 地域列表枚举
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RegionList: list of FilterDataObject
+        :param DefenseStatusList: 防护枚举
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DefenseStatusList: list of FilterDataObject
+        :param AssetTypeList: 资产类型枚举
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetTypeList: list of FilterDataObject
+        :param AppIdList: AppId枚举
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppIdList: list of FilterDataObject
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.Total = None
+        self.AssetLocationList = None
+        self.IpTypeList = None
+        self.RegionList = None
+        self.DefenseStatusList = None
+        self.AssetTypeList = None
+        self.AppIdList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self.Data = []
+            for item in params.get("Data"):
+                obj = IpAssetListVO()
+                obj._deserialize(item)
+                self.Data.append(obj)
+        self.Total = params.get("Total")
+        if params.get("AssetLocationList") is not None:
+            self.AssetLocationList = []
+            for item in params.get("AssetLocationList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.AssetLocationList.append(obj)
+        if params.get("IpTypeList") is not None:
+            self.IpTypeList = []
+            for item in params.get("IpTypeList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.IpTypeList.append(obj)
+        if params.get("RegionList") is not None:
+            self.RegionList = []
+            for item in params.get("RegionList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.RegionList.append(obj)
+        if params.get("DefenseStatusList") is not None:
+            self.DefenseStatusList = []
+            for item in params.get("DefenseStatusList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.DefenseStatusList.append(obj)
+        if params.get("AssetTypeList") is not None:
+            self.AssetTypeList = []
+            for item in params.get("AssetTypeList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.AssetTypeList.append(obj)
+        if params.get("AppIdList") is not None:
+            self.AppIdList = []
+            for item in params.get("AppIdList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.AppIdList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeRiskCenterAssetViewPortRiskListRequest(AbstractModel):
+    """DescribeRiskCenterAssetViewPortRiskList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Filter: 过滤内容
+        :type Filter: :class:`tencentcloud.csip.v20221121.models.Filter`
+        """
+        self.Filter = None
+
+
+    def _deserialize(self, params):
+        if params.get("Filter") is not None:
+            self.Filter = Filter()
+            self.Filter._deserialize(params.get("Filter"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeRiskCenterAssetViewPortRiskListResponse(AbstractModel):
+    """DescribeRiskCenterAssetViewPortRiskList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 总条数
+        :type TotalCount: int
+        :param Data: 资产视角的配置风险列表
+        :type Data: list of AssetViewPortRisk
+        :param StatusLists: 状态列表
+        :type StatusLists: list of FilterDataObject
+        :param LevelLists: 危险等级列表
+        :type LevelLists: list of FilterDataObject
+        :param SuggestionLists: 建议列表
+        :type SuggestionLists: list of FilterDataObject
+        :param InstanceTypeLists: 资产类型列表
+        :type InstanceTypeLists: list of FilterDataObject
+        :param FromLists: 来源列表
+        :type FromLists: list of FilterDataObject
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.Data = None
+        self.StatusLists = None
+        self.LevelLists = None
+        self.SuggestionLists = None
+        self.InstanceTypeLists = None
+        self.FromLists = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("Data") is not None:
+            self.Data = []
+            for item in params.get("Data"):
+                obj = AssetViewPortRisk()
+                obj._deserialize(item)
+                self.Data.append(obj)
+        if params.get("StatusLists") is not None:
+            self.StatusLists = []
+            for item in params.get("StatusLists"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.StatusLists.append(obj)
+        if params.get("LevelLists") is not None:
+            self.LevelLists = []
+            for item in params.get("LevelLists"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.LevelLists.append(obj)
+        if params.get("SuggestionLists") is not None:
+            self.SuggestionLists = []
+            for item in params.get("SuggestionLists"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.SuggestionLists.append(obj)
+        if params.get("InstanceTypeLists") is not None:
+            self.InstanceTypeLists = []
+            for item in params.get("InstanceTypeLists"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.InstanceTypeLists.append(obj)
+        if params.get("FromLists") is not None:
+            self.FromLists = []
+            for item in params.get("FromLists"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.FromLists.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeRiskCenterAssetViewVULRiskListRequest(AbstractModel):
+    """DescribeRiskCenterAssetViewVULRiskList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Filter: 过滤内容
+        :type Filter: :class:`tencentcloud.csip.v20221121.models.Filter`
+        """
+        self.Filter = None
+
+
+    def _deserialize(self, params):
+        if params.get("Filter") is not None:
+            self.Filter = Filter()
+            self.Filter._deserialize(params.get("Filter"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeRiskCenterAssetViewVULRiskListResponse(AbstractModel):
+    """DescribeRiskCenterAssetViewVULRiskList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 总条数
+        :type TotalCount: int
+        :param Data: 资产视角的漏洞风险列表
+        :type Data: list of AssetViewVULRisk
+        :param StatusLists: 状态列表
+        :type StatusLists: list of FilterDataObject
+        :param LevelLists: 危险等级列表
+        :type LevelLists: list of FilterDataObject
+        :param FromLists: 来源列表
+        :type FromLists: list of FilterDataObject
+        :param VULTypeLists: 漏洞类型列表
+        :type VULTypeLists: list of FilterDataObject
+        :param InstanceTypeLists: 资产类型列表
+        :type InstanceTypeLists: list of FilterDataObject
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.Data = None
+        self.StatusLists = None
+        self.LevelLists = None
+        self.FromLists = None
+        self.VULTypeLists = None
+        self.InstanceTypeLists = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("Data") is not None:
+            self.Data = []
+            for item in params.get("Data"):
+                obj = AssetViewVULRisk()
+                obj._deserialize(item)
+                self.Data.append(obj)
+        if params.get("StatusLists") is not None:
+            self.StatusLists = []
+            for item in params.get("StatusLists"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.StatusLists.append(obj)
+        if params.get("LevelLists") is not None:
+            self.LevelLists = []
+            for item in params.get("LevelLists"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.LevelLists.append(obj)
+        if params.get("FromLists") is not None:
+            self.FromLists = []
+            for item in params.get("FromLists"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.FromLists.append(obj)
+        if params.get("VULTypeLists") is not None:
+            self.VULTypeLists = []
+            for item in params.get("VULTypeLists"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.VULTypeLists.append(obj)
+        if params.get("InstanceTypeLists") is not None:
+            self.InstanceTypeLists = []
+            for item in params.get("InstanceTypeLists"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.InstanceTypeLists.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeScanReportListRequest(AbstractModel):
     """DescribeScanReportList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1320,14 +2197,204 @@
             for item in params.get("AppIdList"):
                 obj = FilterDataObject()
                 obj._deserialize(item)
                 self.AppIdList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DomainAssetVO(AbstractModel):
+    """域名资产
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AssetId: 资产id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetId: list of str
+        :param AssetName: 资产名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetName: list of str
+        :param AssetType: 资产类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetType: list of str
+        :param Region: 地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: list of str
+        :param WAFStatus: Waf状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WAFStatus: int
+        :param AssetCreateTime: 资产创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetCreateTime: str
+        :param AppId: Appid
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppId: int
+        :param Uin: 账号id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Uin: str
+        :param NickName: 账号名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NickName: str
+        :param IsCore: 是否核心
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsCore: int
+        :param IsCloud: 是否云上资产
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsCloud: int
+        :param Attack: 网络攻击
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Attack: int
+        :param Access: 网络访问
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Access: int
+        :param Intercept: 网络拦截
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Intercept: int
+        :param InBandwidth: 入站峰值带宽
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InBandwidth: str
+        :param OutBandwidth: 出站峰值带宽
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutBandwidth: str
+        :param InFlow: 入站累计流量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InFlow: str
+        :param OutFlow: 出站累计流量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutFlow: str
+        :param LastScanTime: 最近扫描时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LastScanTime: str
+        :param PortRisk: 端口风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PortRisk: int
+        :param VulnerabilityRisk: 漏洞风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VulnerabilityRisk: int
+        :param ConfigurationRisk: 配置风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConfigurationRisk: int
+        :param ScanTask: 扫描任务
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScanTask: int
+        :param SubDomain: 域名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubDomain: str
+        :param SeverIp: 解析ip
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SeverIp: list of str
+        :param BotCount: boi访问数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BotCount: int
+        :param WeakPassword: 弱口令风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WeakPassword: int
+        :param WebContentRisk: 内容风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WebContentRisk: int
+        :param Tag: tag标签
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tag: list of Tag
+        :param SourceType: 关联实例类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SourceType: str
+        :param MemberId: memberiD
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MemberId: str
+        :param CCAttack: cc攻击
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CCAttack: int
+        :param WebAttack: web攻击
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WebAttack: int
+        """
+        self.AssetId = None
+        self.AssetName = None
+        self.AssetType = None
+        self.Region = None
+        self.WAFStatus = None
+        self.AssetCreateTime = None
+        self.AppId = None
+        self.Uin = None
+        self.NickName = None
+        self.IsCore = None
+        self.IsCloud = None
+        self.Attack = None
+        self.Access = None
+        self.Intercept = None
+        self.InBandwidth = None
+        self.OutBandwidth = None
+        self.InFlow = None
+        self.OutFlow = None
+        self.LastScanTime = None
+        self.PortRisk = None
+        self.VulnerabilityRisk = None
+        self.ConfigurationRisk = None
+        self.ScanTask = None
+        self.SubDomain = None
+        self.SeverIp = None
+        self.BotCount = None
+        self.WeakPassword = None
+        self.WebContentRisk = None
+        self.Tag = None
+        self.SourceType = None
+        self.MemberId = None
+        self.CCAttack = None
+        self.WebAttack = None
+
+
+    def _deserialize(self, params):
+        self.AssetId = params.get("AssetId")
+        self.AssetName = params.get("AssetName")
+        self.AssetType = params.get("AssetType")
+        self.Region = params.get("Region")
+        self.WAFStatus = params.get("WAFStatus")
+        self.AssetCreateTime = params.get("AssetCreateTime")
+        self.AppId = params.get("AppId")
+        self.Uin = params.get("Uin")
+        self.NickName = params.get("NickName")
+        self.IsCore = params.get("IsCore")
+        self.IsCloud = params.get("IsCloud")
+        self.Attack = params.get("Attack")
+        self.Access = params.get("Access")
+        self.Intercept = params.get("Intercept")
+        self.InBandwidth = params.get("InBandwidth")
+        self.OutBandwidth = params.get("OutBandwidth")
+        self.InFlow = params.get("InFlow")
+        self.OutFlow = params.get("OutFlow")
+        self.LastScanTime = params.get("LastScanTime")
+        self.PortRisk = params.get("PortRisk")
+        self.VulnerabilityRisk = params.get("VulnerabilityRisk")
+        self.ConfigurationRisk = params.get("ConfigurationRisk")
+        self.ScanTask = params.get("ScanTask")
+        self.SubDomain = params.get("SubDomain")
+        self.SeverIp = params.get("SeverIp")
+        self.BotCount = params.get("BotCount")
+        self.WeakPassword = params.get("WeakPassword")
+        self.WebContentRisk = params.get("WebContentRisk")
+        if params.get("Tag") is not None:
+            self.Tag = []
+            for item in params.get("Tag"):
+                obj = Tag()
+                obj._deserialize(item)
+                self.Tag.append(obj)
+        self.SourceType = params.get("SourceType")
+        self.MemberId = params.get("MemberId")
+        self.CCAttack = params.get("CCAttack")
+        self.WebAttack = params.get("WebAttack")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Filter(AbstractModel):
     """列表查询接口采用新filter 接口，直接传给后台供后台查询过滤
 
     """
 
     def __init__(self):
         r"""
@@ -1399,14 +2466,204 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class IpAssetListVO(AbstractModel):
+    """ip列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AssetId: 资产id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetId: str
+        :param AssetName: 资产name
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetName: str
+        :param AssetType: 资产类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetType: str
+        :param Region: 地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        :param CFWStatus: 云防状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CFWStatus: int
+        :param AssetCreateTime: 资产创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetCreateTime: str
+        :param PublicIp: 公网ip
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PublicIp: str
+        :param PublicIpType: 公网ip类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PublicIpType: int
+        :param VpcId: vpc
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
+        :param VpcName: vpc名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcName: str
+        :param AppId: appid
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppId: int
+        :param Uin: 用户uin
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Uin: str
+        :param NickName: 名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NickName: str
+        :param IsCore: 核心
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsCore: int
+        :param IsCloud: 云上
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsCloud: int
+        :param Attack: 网络攻击
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Attack: int
+        :param Access: 网络访问
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Access: int
+        :param Intercept: 网络拦截
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Intercept: int
+        :param InBandwidth: 入向带宽
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InBandwidth: str
+        :param OutBandwidth: 出向带宽
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutBandwidth: str
+        :param InFlow: 入向流量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InFlow: str
+        :param OutFlow: 出向流量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutFlow: str
+        :param LastScanTime: 最近扫描时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LastScanTime: str
+        :param PortRisk: 端口风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PortRisk: int
+        :param VulnerabilityRisk: 漏洞风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VulnerabilityRisk: int
+        :param ConfigurationRisk: 配置风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConfigurationRisk: int
+        :param ScanTask: 扫描任务
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScanTask: int
+        :param WeakPassword: 弱口令
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WeakPassword: int
+        :param WebContentRisk: 内容风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WebContentRisk: int
+        :param Tag: 标签
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tag: list of Tag
+        :param AddressId: eip主键
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AddressId: str
+        :param MemberId: memberid信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MemberId: str
+        :param RiskExposure: 风险服务暴露
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RiskExposure: int
+        """
+        self.AssetId = None
+        self.AssetName = None
+        self.AssetType = None
+        self.Region = None
+        self.CFWStatus = None
+        self.AssetCreateTime = None
+        self.PublicIp = None
+        self.PublicIpType = None
+        self.VpcId = None
+        self.VpcName = None
+        self.AppId = None
+        self.Uin = None
+        self.NickName = None
+        self.IsCore = None
+        self.IsCloud = None
+        self.Attack = None
+        self.Access = None
+        self.Intercept = None
+        self.InBandwidth = None
+        self.OutBandwidth = None
+        self.InFlow = None
+        self.OutFlow = None
+        self.LastScanTime = None
+        self.PortRisk = None
+        self.VulnerabilityRisk = None
+        self.ConfigurationRisk = None
+        self.ScanTask = None
+        self.WeakPassword = None
+        self.WebContentRisk = None
+        self.Tag = None
+        self.AddressId = None
+        self.MemberId = None
+        self.RiskExposure = None
+
+
+    def _deserialize(self, params):
+        self.AssetId = params.get("AssetId")
+        self.AssetName = params.get("AssetName")
+        self.AssetType = params.get("AssetType")
+        self.Region = params.get("Region")
+        self.CFWStatus = params.get("CFWStatus")
+        self.AssetCreateTime = params.get("AssetCreateTime")
+        self.PublicIp = params.get("PublicIp")
+        self.PublicIpType = params.get("PublicIpType")
+        self.VpcId = params.get("VpcId")
+        self.VpcName = params.get("VpcName")
+        self.AppId = params.get("AppId")
+        self.Uin = params.get("Uin")
+        self.NickName = params.get("NickName")
+        self.IsCore = params.get("IsCore")
+        self.IsCloud = params.get("IsCloud")
+        self.Attack = params.get("Attack")
+        self.Access = params.get("Access")
+        self.Intercept = params.get("Intercept")
+        self.InBandwidth = params.get("InBandwidth")
+        self.OutBandwidth = params.get("OutBandwidth")
+        self.InFlow = params.get("InFlow")
+        self.OutFlow = params.get("OutFlow")
+        self.LastScanTime = params.get("LastScanTime")
+        self.PortRisk = params.get("PortRisk")
+        self.VulnerabilityRisk = params.get("VulnerabilityRisk")
+        self.ConfigurationRisk = params.get("ConfigurationRisk")
+        self.ScanTask = params.get("ScanTask")
+        self.WeakPassword = params.get("WeakPassword")
+        self.WebContentRisk = params.get("WebContentRisk")
+        if params.get("Tag") is not None:
+            self.Tag = []
+            for item in params.get("Tag"):
+                obj = Tag()
+                obj._deserialize(item)
+                self.Tag.append(obj)
+        self.AddressId = params.get("AddressId")
+        self.MemberId = params.get("MemberId")
+        self.RiskExposure = params.get("RiskExposure")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class ScanTaskInfo(AbstractModel):
     """扫描任务详情
 
     """
```

### Comparing `tencentcloud-sdk-python-csip-3.0.914/tencentcloud/__init__.py` & `tencentcloud-sdk-python-csip-3.0.915/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.914'
+__version__ = '3.0.915'
```

### Comparing `tencentcloud-sdk-python-csip-3.0.914/PKG-INFO` & `tencentcloud-sdk-python-csip-3.0.915/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csip
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Csip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csip-3.0.914/setup.py` & `tencentcloud-sdk-python-csip-3.0.915/setup.py`

 * *Files identical despite different names*

