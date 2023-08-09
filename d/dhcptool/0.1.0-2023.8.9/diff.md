# Comparing `tmp/dhcptool-0.1.0.tar.gz` & `tmp/dhcptool-2023.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhcptool-0.1.0.tar", max compression
+gzip compressed data, was "dhcptool-2023.8.9.tar", max compression
```

## Comparing `dhcptool-0.1.0.tar` & `dhcptool-2023.8.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-07-28 14:39:44.508079 dhcptool-0.1.0/dhcptool/__init__.py
--rw-r--r--   0        0        0     6125 2023-07-28 16:14:47.115448 dhcptool-0.1.0/dhcptool/dhcp4_controller.py
--rw-r--r--   0        0        0     4650 2023-07-28 16:16:43.091304 dhcptool-0.1.0/dhcptool/dhcp6_controller.py
--rw-r--r--   0        0        0    12898 2023-07-28 16:15:22.074556 dhcptool-0.1.0/dhcptool/dhcp_pkt.py
--rw-r--r--   0        0        0      777 2023-07-28 16:15:41.302427 dhcptool-0.1.0/dhcptool/env_args.py
--rw-r--r--   0        0        0     2216 2023-07-28 16:16:43.111694 dhcptool-0.1.0/dhcptool/extend_tools_controller.py
--rw-r--r--   0        0        0      901 2023-07-24 15:05:42.222000 dhcptool-0.1.0/dhcptool/Logings.py
--rw-r--r--   0        0        0     6272 2023-07-28 16:14:20.728780 dhcptool-0.1.0/dhcptool/main.py
--rw-r--r--   0        0        0     9243 2023-07-28 16:15:57.580666 dhcptool-0.1.0/dhcptool/options.py
--rw-r--r--   0        0        0    10937 2023-07-28 16:16:11.299991 dhcptool-0.1.0/dhcptool/tools.py
--rw-r--r--   0        0        0      490 2023-07-28 16:10:20.340890 dhcptool-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4150 2023-07-28 14:43:26.019930 dhcptool-0.1.0/README.md
--rw-r--r--   0        0        0     4512 1970-01-01 00:00:00.000000 dhcptool-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 02:59:49.447031 dhcptool-2023.8.9/dhcptool/__init__.py
+-rw-r--r--   0        0        0     6125 2023-07-31 02:59:49.447770 dhcptool-2023.8.9/dhcptool/dhcp4_controller.py
+-rw-r--r--   0        0        0     4650 2023-07-31 02:59:49.447770 dhcptool-2023.8.9/dhcptool/dhcp6_controller.py
+-rw-r--r--   0        0        0    12898 2023-08-01 08:31:36.925160 dhcptool-2023.8.9/dhcptool/dhcp_pkt.py
+-rw-r--r--   0        0        0      530 2023-08-04 08:56:37.322190 dhcptool-2023.8.9/dhcptool/env_args.py
+-rw-r--r--   0        0        0     2216 2023-07-31 02:59:49.450317 dhcptool-2023.8.9/dhcptool/extend_tools_controller.py
+-rw-r--r--   0        0        0      901 2023-07-31 02:59:49.446531 dhcptool-2023.8.9/dhcptool/Logings.py
+-rw-r--r--   0        0        0     6272 2023-07-31 02:59:49.451463 dhcptool-2023.8.9/dhcptool/main.py
+-rw-r--r--   0        0        0     9755 2023-08-04 11:00:55.578966 dhcptool-2023.8.9/dhcptool/options.py
+-rw-r--r--   0        0        0    10998 2023-08-04 08:56:19.230423 dhcptool-2023.8.9/dhcptool/tools.py
+-rw-r--r--   0        0        0      495 2023-08-09 02:59:38.969553 dhcptool-2023.8.9/pyproject.toml
+-rw-r--r--   0        0        0     4150 2023-07-31 02:21:29.982053 dhcptool-2023.8.9/README.md
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 dhcptool-2023.8.9/PKG-INFO
```

### Comparing `dhcptool-0.1.0/dhcptool/dhcp4_controller.py` & `dhcptool-2023.8.9/dhcptool/dhcp4_controller.py`

 * *Files identical despite different names*

### Comparing `dhcptool-0.1.0/dhcptool/dhcp6_controller.py` & `dhcptool-2023.8.9/dhcptool/dhcp6_controller.py`

 * *Files identical despite different names*

### Comparing `dhcptool-0.1.0/dhcptool/dhcp_pkt.py` & `dhcptool-2023.8.9/dhcptool/dhcp_pkt.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             Tools.print_formart(pkt, self.args.debug)
             async_sniff_args = {"filter": f'port 67 and src host {self.args.filter}', "count": 1, "timeout": self.timeout}
             self.async_sniff(async_sniff_args, pkt)
         elif self.args.dhcp_server and ip_address(self.args.dhcp_server).version == 4:
             Tools.print_formart(pkt, self.args.debug)
             srp1_args = {"verbose": 0, "timeout": self.timeout}
             response = srp1(pkt, iface=self.args.iface, **srp1_args) if self.args.iface else srp1(pkt, **srp1_args)
-            logs.error('没有接收到返回包！') if response else None
+            None if response else logs.error('没有接收到返回包！')
             return response
         else:
             logs.info("v4发包需要指定IPv4服务器")
 
 
 class Dhcp6Pkt(Pkt):
```

### Comparing `dhcptool-0.1.0/dhcptool/env_args.py` & `dhcptool-2023.8.9/dhcptool/env_args.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,11 +16,8 @@
 pkt_result = {
     "dhcp6_advertise": queue.Queue(),
     "dhcp6_reply": queue.Queue(),
     "dhcp4_offer": queue.Queue(),
     "dhcp4_ack": queue.Queue(),
     "dhcp4_nak": queue.Queue(),
 }
-logs = Logings("DHCP")
-# 应答内容过滤正则
-response_filter_regex = '(\/)|(:dhcpv6_server)|(:bootps)|(DHCP6OptClientId)|(:dhcpv6_client)|(DHCP6OptServerId)|(' \
-                        'DHCP6OptIA_NA)|(DHCP6OptIA_PD)|(DHCP6OptStatusCode)|(DHCP6OptRelayMsg) '
+logs = Logings("DHCP")
```

### Comparing `dhcptool-0.1.0/dhcptool/extend_tools_controller.py` & `dhcptool-2023.8.9/dhcptool/extend_tools_controller.py`

 * *Files identical despite different names*

### Comparing `dhcptool-0.1.0/dhcptool/Logings.py` & `dhcptool-2023.8.9/dhcptool/Logings.py`

 * *Files identical despite different names*

### Comparing `dhcptool-0.1.0/dhcptool/main.py` & `dhcptool-2023.8.9/dhcptool/main.py`

 * *Files identical despite different names*

### Comparing `dhcptool-0.1.0/dhcptool/options.py` & `dhcptool-2023.8.9/dhcptool/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # @File    : options.py
 # @Software: PyCharm
 # @desc    :
 import binascii
 from typing import Text
 
 from scapy.layers.dhcp6 import DHCP6OptVendorClass, VENDOR_CLASS_DATA, DHCP6OptIfaceId, DHCP6OptStatusCode, DHCP6OptRapidCommit, DHCP6OptOptReq, \
-    DHCP6OptIAAddress, DHCP6OptIAPrefix
+    DHCP6OptIAAddress, DHCP6OptIAPrefix, DHCP6OptClientFQDN
 from dhcptool.env_args import logs
 
 
 class Options:
     def __init__(self, args):
         self.args = args
 
@@ -40,26 +40,27 @@
         super(Dhcp4Options, self).__init__(args=self.args)
 
     def make_options_list(self) -> list:
         """
         制作 options
         :return:
         """
-        options = []
+        options,op_82_sub_key = [], 0
         options_list = self.parse_dhcp4_options()
         if options_list is not None:
             for index, i in enumerate(options_list):
                 if int(i[0]) == 12:
                     options.append(self.option_12(hostname=i[1]))
                 if int(i[0]) == 7:
                     options.append(self.option_7(log_server=i[1]))
                 if int(i[0]) == 60:
                     options.append(self.option_60(vendor_class_id=i[1]))
                 if int(i[0]) == 82:
-                    options.append(self.option_82(i[1], str(index + 1).rjust(2, '0')))
+                    op_82_sub_key +=1
+                    options.append(self.option_82(i[1], str(op_82_sub_key).rjust(2, '0')))
                 if int(i[0]) == 55:
                     options.append(self.option_55(param_req_list=i[1]))
                 if int(i[0]) == 50:
                     options.append(self.option_50(requested_addr=i[1]))
                 if int(i[0]) == 51:
                     options.append(self.option_51(lease_time=i[1]))
                 if int(i[0]) == 2:
@@ -126,75 +127,74 @@
         return 'param_req_list', param_req_list
 
     @staticmethod
     def option_50(requested_addr='192.168.0.1'):
         return 'requested_addr', requested_addr
 
     @staticmethod
-    def option_51(lease_time):
+    def option_51(lease_time: int=43200) -> tuple:
         """
 
         :param lease_time: 租约时间
         :return:
         """
-        pass
+        return 'lease_time', int(lease_time)
 
     @staticmethod
-    def option_2(time_zone):
+    def option_2(time_zone:int = 500):
         """
-
-        :param time_zone: 时区
+        :param times_zone: 时区
         :return:
         """
-        pass
+        return 'time_zone', int(time_zone)
 
     @staticmethod
-    def option_3(router):
+    def option_3(router='0.0.0.0'):
         """
 
-        :param router: 路由 接受IP数组
+        :param router: 路由
         :return:
         """
-        pass
+        return 'router', router
 
     @staticmethod
-    def option_13(boot_size):
+    def option_13(boot_size=1000):
         """
 
         :param boot_size:
         :return:
         """
-        pass
+        return 'boot-size', int(boot_size)
 
     @staticmethod
     def option_15(domain: Text):
         """
 
         :param domain: 域名
         :return:
         """
-        pass
+        return 'domain', domain
 
     @staticmethod
     def option_19(ip_forwarding: bool):
         """
 
         :param ip_forwarding: ip转发
         :return:
         """
-        pass
+        return 'ip_forwarding', bool(ip_forwarding)
 
     @staticmethod
-    def option_23(default_ip_ttl: bool):
+    def option_23(default_ttl: int):
         """
 
         :param default_ip_ttl: 默认ip ttl值
         :return:
         """
-        pass
+        return 'default_ttl', default_ttl
 
 
 class Dhcp6Options(Options):
 
     def __init__(self, args):
         self.args = args
         super(Dhcp6Options, self).__init__(args=self.args)
@@ -285,7 +285,17 @@
         """
         DHCP6OptIAPrefix  二级option,不能与 一级进行 option拼接
         :return:
         """
         prefix, prefix_len = prefix.split('/')[0], prefix.split('/')[1]
         option26_pkt = DHCP6OptIAPrefix(prefix=prefix, plen=int(prefix_len))
         return option26_pkt
+    
+
+    @staticmethod
+    def option_39():
+        """
+        DHCP6OptClientFQDN
+        :return:
+        """
+        option39_pkt = DHCP6OptClientFQDN(flags=0, fqdn="")
+        return option39_pkt
```

### Comparing `dhcptool-0.1.0/dhcptool/tools.py` & `dhcptool-2023.8.9/dhcptool/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from scapy.layers.dhcp import DHCPTypes, DHCP, BOOTP
 from scapy.layers.dhcp6 import dhcp6types, DHCP6OptIAAddress, DHCP6OptRelayMsg, DHCP6OptIAPrefix
 from scapy.layers.inet import IP, UDP
 from scapy.layers.inet6 import IPv6
 from scapy.layers.l2 import Ether
 from scapy.utils import mac2str, str2mac
 from scapy.volatile import RandMAC
-from dhcptool.env_args import pkt_result, logs, summary_result, global_var, response_filter_regex
+from dhcptool.env_args import pkt_result, logs, summary_result, global_var
 import time
 
 
 class Tools:
 
     @staticmethod
     def mac_self_incrementing(mac, num, offset=1):
@@ -115,16 +115,19 @@
 
         return local_ipv4
 
     @staticmethod
     def get_local_ipv6():
         # 获取本机ipv6
         local_ipv6 = socket.socket(socket.AF_INET6, socket.SOCK_DGRAM)
-        local_ipv6.connect(('2001:da8:ff:305:20c:29ff:fe1f:a92a', 80))
-        local_ipv6 = local_ipv6.getsockname()[0]
+        try:
+            local_ipv6.connect(('2001:da8:ff:305:20c:29ff:fe1f:a92a', 80))
+            local_ipv6 = local_ipv6.getsockname()[0]
+        except:
+            local_ipv6 = "1000:0:0:31::135"
         return local_ipv6
 
     @staticmethod
     def analysis_results(pkts_list, args: Namespace = None, call_name=None):
         """
         解析结果并存入队列
         :param args:
```

### Comparing `dhcptool-0.1.0/README.md` & `dhcptool-2023.8.9/README.md`

 * *Files identical despite different names*

### Comparing `dhcptool-0.1.0/PKG-INFO` & `dhcptool-2023.8.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: dhcptool
-Version: 0.1.0
+Version: 2023.8.9
 Summary: 
 Author: mf.liang
 Author-email: mf.liang@outlook.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.6.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: scapy (>=2.5.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 使用说明
```

