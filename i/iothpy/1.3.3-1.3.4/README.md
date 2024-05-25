# Comparing `tmp/iothpy-1.3.3.tar.gz` & `tmp/iothpy-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iothpy-1.3.3.tar", last modified: Thu May 16 10:02:35 2024, max compression
+gzip compressed data, was "iothpy-1.3.4.tar", last modified: Sat May 25 06:56:10 2024, max compression
```

## Comparing `iothpy-1.3.3.tar` & `iothpy-1.3.4.tar`

### file list

```diff
@@ -1,27 +1,37 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 10:02:35.001923 iothpy-1.3.3/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2024-05-16 07:43:54.000000 iothpy-1.3.3/CMakeLists.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    26526 2024-03-26 14:33:52.000000 iothpy-1.3.3/LICENSE
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      145 2024-03-26 14:33:52.000000 iothpy-1.3.3/MANIFEST.in
--rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-05-16 10:02:35.001923 iothpy-1.3.3/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6180 2024-03-26 14:33:52.000000 iothpy-1.3.3/README.md
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 10:02:35.001923 iothpy-1.3.3/iothpy/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2779 2024-05-04 06:34:10.000000 iothpy-1.3.3/iothpy/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    30003 2024-05-04 06:34:10.000000 iothpy-1.3.3/iothpy/const_linkadd.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7268 2024-05-04 06:34:10.000000 iothpy-1.3.3/iothpy/iothpy.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    78783 2024-03-26 14:33:52.000000 iothpy-1.3.3/iothpy/iothpy_socket.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      983 2024-03-26 14:33:52.000000 iothpy-1.3.3/iothpy/iothpy_socket.h
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    38819 2024-05-16 07:37:18.000000 iothpy-1.3.3/iothpy/iothpy_stack.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      260 2024-03-26 14:33:52.000000 iothpy-1.3.3/iothpy/iothpy_stack.h
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    14359 2024-03-26 14:33:52.000000 iothpy-1.3.3/iothpy/msocket.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2411 2024-03-26 14:33:52.000000 iothpy-1.3.3/iothpy/override.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4400 2024-04-04 11:20:54.000000 iothpy-1.3.3/iothpy/stack.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2892 2024-03-26 14:33:52.000000 iothpy-1.3.3/iothpy/utils.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      680 2024-03-26 14:33:52.000000 iothpy-1.3.3/iothpy/utils.h
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 10:02:35.001923 iothpy-1.3.3/iothpy.egg-info/
--rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-05-16 10:02:34.000000 iothpy-1.3.3/iothpy.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      419 2024-05-16 10:02:34.000000 iothpy-1.3.3/iothpy.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2024-05-16 10:02:34.000000 iothpy-1.3.3/iothpy.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        7 2024-05-16 10:02:34.000000 iothpy-1.3.3/iothpy.egg-info/top_level.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       75 2024-03-26 14:33:52.000000 iothpy-1.3.3/pyproject.toml
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2024-05-16 10:02:35.001923 iothpy-1.3.3/setup.cfg
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1592 2024-05-16 10:02:22.000000 iothpy-1.3.3/setup.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-25 06:56:10.899036 iothpy-1.3.4/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1068 2024-05-25 06:31:22.000000 iothpy-1.3.4/CMakeLists.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    26526 2024-03-26 14:33:52.000000 iothpy-1.3.4/LICENSE
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      145 2024-03-26 14:33:52.000000 iothpy-1.3.4/MANIFEST.in
+-rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-05-25 06:56:10.899036 iothpy-1.3.4/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6180 2024-03-26 14:33:52.000000 iothpy-1.3.4/README.md
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-25 06:56:10.883035 iothpy-1.3.4/_skbuild/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-25 06:56:10.883035 iothpy-1.3.4/_skbuild/linux-x86_64-3.12/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-25 06:56:10.883035 iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-25 06:56:10.891035 iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2779 2024-05-25 06:50:27.000000 iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/__init__.py
+-rw-r--r--   0 francesco  (1000) francesco  (1000)    87576 2024-05-25 06:50:27.000000 iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_const_linkadd.cpython-312-x86_64-linux-gnu.so
+-rw-r--r--   0 francesco  (1000) francesco  (1000)   193896 2024-05-25 06:50:26.000000 iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_iothpy.cpython-312-x86_64-linux-gnu.so
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    14359 2024-05-25 06:50:27.000000 iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/msocket.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2411 2024-05-25 06:50:27.000000 iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/override.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4400 2024-05-25 06:50:27.000000 iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/stack.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-25 06:56:10.895036 iothpy-1.3.4/iothpy/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2779 2024-05-04 06:34:10.000000 iothpy-1.3.4/iothpy/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    30409 2024-05-25 06:45:16.000000 iothpy-1.3.4/iothpy/const_linkadd.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7268 2024-05-04 06:34:10.000000 iothpy-1.3.4/iothpy/iothpy.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    78783 2024-03-26 14:33:52.000000 iothpy-1.3.4/iothpy/iothpy_socket.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      983 2024-03-26 14:33:52.000000 iothpy-1.3.4/iothpy/iothpy_socket.h
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    38819 2024-05-16 07:37:18.000000 iothpy-1.3.4/iothpy/iothpy_stack.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      260 2024-03-26 14:33:52.000000 iothpy-1.3.4/iothpy/iothpy_stack.h
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    14359 2024-03-26 14:33:52.000000 iothpy-1.3.4/iothpy/msocket.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2411 2024-03-26 14:33:52.000000 iothpy-1.3.4/iothpy/override.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4400 2024-04-04 11:20:54.000000 iothpy-1.3.4/iothpy/stack.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2892 2024-03-26 14:33:52.000000 iothpy-1.3.4/iothpy/utils.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      680 2024-03-26 14:33:52.000000 iothpy-1.3.4/iothpy/utils.h
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-25 06:56:10.899036 iothpy-1.3.4/iothpy.egg-info/
+-rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-05-25 06:56:10.000000 iothpy-1.3.4/iothpy.egg-info/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      838 2024-05-25 06:56:10.000000 iothpy-1.3.4/iothpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2024-05-25 06:56:10.000000 iothpy-1.3.4/iothpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        7 2024-05-25 06:56:10.000000 iothpy-1.3.4/iothpy.egg-info/top_level.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       75 2024-03-26 14:33:52.000000 iothpy-1.3.4/pyproject.toml
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2024-05-25 06:56:10.899036 iothpy-1.3.4/setup.cfg
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1592 2024-05-25 06:49:30.000000 iothpy-1.3.4/setup.py
```

### Comparing `iothpy-1.3.3/CMakeLists.txt` & `iothpy-1.3.4/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,14 @@
   if(NOT ${HEADER}_OK)
     message(FATAL_ERROR "header file ${HEADER} not found")
   endif()
 endforeach(HEADER)
 
 # Target for python extension module
 add_library(_iothpy MODULE iothpy/iothpy.c iothpy/iothpy_socket.c iothpy/iothpy_stack.c iothpy/utils.c)
-target_link_libraries(_iothpy -lioth -liothconf -liothdns -lpicoxnet)
+target_link_libraries(_iothpy -lioth -liothconf -liothdns)
 python_extension_module(_iothpy)
 
 add_library(_const_linkadd MODULE iothpy/const_linkadd.c)
 python_extension_module(_const_linkadd)
 
 install(TARGETS _iothpy _const_linkadd LIBRARY DESTINATION iothpy)
```

### Comparing `iothpy-1.3.3/LICENSE` & `iothpy-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/PKG-INFO` & `iothpy-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iothpy
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python library for internet of threads
 Home-page: https://github.com/ramenguy99/iothpy
 Author: Dario Mylonopoulos
 Author-email: dmylos@yahoo.it
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `iothpy-1.3.3/README.md` & `iothpy-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy/__init__.py` & `iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/__init__.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy/const_linkadd.c` & `iothpy-1.3.4/iothpy/const_linkadd.c`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
 #ifndef _GNU_SOURCE
 #define _GNU_SOURCE
 #endif
 
 #include <nlinline+.h>
 #include <linux/if_link.h>
+#include <linux/version.h>
+
+#define IS_DEBIAN_UNSTABLE_KERNEL LINUX_VERSION_CODE >= KERNEL_VERSION(6,2,0)
 
 #define ADD_INT(name, value) \
     do { \
         if (PyModule_AddIntConstant(module, name, value) < 0) { \
             return NULL; \
         } \
     } while (0)
@@ -109,18 +112,20 @@
 	"IFLA_PROTO_DOWN_REASON",
 	"IFLA_PARENT_DEV_NAME",
 	"IFLA_PARENT_DEV_BUS_NAME",
 	"IFLA_GRO_MAX_SIZE",
 	"IFLA_TSO_MAX_SIZE",
 	"IFLA_TSO_MAX_SEGS",
 	"IFLA_ALLMULTI",		/* Allmulti count: > 0 means acts ALLMULTI */
+#if IS_DEBIAN_UNSTABLE_KERNEL
 	"IFLA_DEVLINK_PORT",
 	"IFLA_GSO_IPV4_MAX_SIZE",
 	"IFLA_GRO_IPV4_MAX_SIZE",
 	"IFLA_DPLL_PIN",
+#endif
 	"__IFLA_MAX"
 };
 static const char* IFLA_PROTO_DOWNREASON[] = {
 	"IFLA_PROTO_DOWN_REASON_UNSPEC",
 	"IFLA_PROTO_DOWN_REASON_MASK",	/* u32, mask for reason bits */
 	"IFLA_PROTO_DOWN_REASON_VALUE",   /* u32, reason bit value */
 	"__IFLA_PROTO_DOWN_REASON_CNT",
@@ -138,15 +143,16 @@
 	"IFLA_INET6_CACHEINFO",	/* time values and max reasm size */
 	"IFLA_INET6_ICMP6STATS",	/* statistics (icmpv6)		*/
 	"IFLA_INET6_TOKEN",	/* device token			*/
 	"IFLA_INET6_ADDR_GEN_MODE", /* implicit address generator mode */
 	"IFLA_INET6_RA_MTU",	/* mtu carried in the RA message */
 	"__IFLA_INET6_MAX"
 };
-static const char* IFLA_INET6_GEN_MODE[] = {"IN6_ADDR_GEN_MODE_EUI64",
+static const char* IFLA_INET6_GEN_MODE[] = {
+	"IN6_ADDR_GEN_MODE_EUI64",
 	"IN6_ADDR_GEN_MODE_NONE", 
 	"IN6_ADDR_GEN_MODE_STABLE_PRIVACY",
 	"IN6_ADDR_GEN_MODE_RANDOM"
 };
 
 /* Bridge section */
 static const char* IFLA_BR[] = { 
@@ -194,16 +200,18 @@
 	"IFLA_BR_VLAN_STATS_ENABLED",
 	"IFLA_BR_MCAST_STATS_ENABLED",
 	"IFLA_BR_MCAST_IGMP_VERSION",
 	"IFLA_BR_MCAST_MLD_VERSION",
 	"IFLA_BR_VLAN_STATS_PER_PORT",
 	"IFLA_BR_MULTI_BOOLOPT",
 	"IFLA_BR_MCAST_QUERIER_STATE",
+#if IS_DEBIAN_UNSTABLE_KERNEL
 	"IFLA_BR_FDB_N_LEARNED",
 	"IFLA_BR_FDB_MAX_LEARNED",
+#endif
 	"__IFLA_BR_MAX",
 };
 
 static const char* BRIDGE_MODE[]={"BRIDGE_MODE_UNSPEC","BRIDGE_MODE_HAIRPIN"};
 
 static const char* IFLA_BRPORT[] = {
 	"IFLA_BRPORT_UNSPEC",
@@ -242,19 +250,21 @@
 	"IFLA_BRPORT_ISOLATED",
 	"IFLA_BRPORT_BACKUP_PORT",
 	"IFLA_BRPORT_MRP_RING_OPEN",
 	"IFLA_BRPORT_MRP_IN_OPEN",
 	"IFLA_BRPORT_MCAST_EHT_HOSTS_LIMIT",
 	"IFLA_BRPORT_MCAST_EHT_HOSTS_CNT",
 	"IFLA_BRPORT_LOCKED",
+#if IS_DEBIAN_UNSTABLE_KERNEL
 	"IFLA_BRPORT_MAB",
 	"IFLA_BRPORT_MCAST_N_GROUPS",
 	"IFLA_BRPORT_MCAST_MAX_GROUPS",
 	"IFLA_BRPORT_NEIGH_VLAN_SUPPRESS",
 	"IFLA_BRPORT_BACKUP_NHID",
+#endif
 	"__IFLA_BRPORT_MAX"
 };
 
 static const char* IFLA_INFO[] = {
 	"IFLA_INFO_UNSPEC",
 	"IFLA_INFO_KIND",
 	"IFLA_INFO_DATA",
@@ -287,15 +297,17 @@
 	"IFLA_MACVLAN_FLAGS",
 	"IFLA_MACVLAN_MACADDR_MODE",
 	"IFLA_MACVLAN_MACADDR",
 	"IFLA_MACVLAN_MACADDR_DATA",
 	"IFLA_MACVLAN_MACADDR_COUNT",
 	"IFLA_MACVLAN_BC_QUEUE_LEN",
 	"IFLA_MACVLAN_BC_QUEUE_LEN_USED",
+#if IS_DEBIAN_UNSTABLE_KERNEL
 	"IFLA_MACVLAN_BC_CUTOFF",
+#endif
 	"__IFLA_MACVLAN_MAX",
 };
 static const char* MACVLAN_MACADDR[] = {
 	"MACVLAN_MACADDR_ADD",
 	"MACVLAN_MACADDR_DEL",
 	"MACVLAN_MACADDR_FLUSH",
 	"MACVLAN_MACADDR_SET"
@@ -353,29 +365,33 @@
 static const char* IPVLAN_MODE[] = {
 	"IPVLAN_MODE_L2",
 	"IPVLAN_MODE_L3",
 	"IPVLAN_MODE_L3S",
 	"IPVLAN_MODE_MAX"
 };
 
+#if IS_DEBIAN_UNSTABLE_KERNEL
 static const char* NETKIT_MODE[] = {
 	"NETKIT_L2",
 	"NETKIT_L3",
 };
 
+
 static const char* IFLA_NETKIT[] = {
 	"IFLA_NETKIT_UNSPEC",
 	"IFLA_NETKIT_PEER_INFO",
 	"IFLA_NETKIT_PRIMARY",
 	"IFLA_NETKIT_POLICY",
 	"IFLA_NETKIT_PEER_POLICY",
 	"IFLA_NETKIT_MODE",
 	"__IFLA_NETKIT_MAX",
 };
 
+#endif
+
 /* VXLAN section */
 static const char* VNIFILTER_ENTRY[] = {
 	"VNIFILTER_ENTRY_STATS_UNSPEC",
 	"VNIFILTER_ENTRY_STATS_RX_BYTES",
 	"VNIFILTER_ENTRY_STATS_RX_PKTS",
 	"VNIFILTER_ENTRY_STATS_RX_DROPS",
 	"VNIFILTER_ENTRY_STATS_RX_ERRORS",
@@ -431,16 +447,18 @@
 	"IFLA_VXLAN_REMCSUM_NOPARTIAL",
 	"IFLA_VXLAN_COLLECT_METADATA",
 	"IFLA_VXLAN_LABEL",
 	"IFLA_VXLAN_GPE",
 	"IFLA_VXLAN_TTL_INHERIT",
 	"IFLA_VXLAN_DF",
 	"IFLA_VXLAN_VNIFILTER", /* only applicable with COLLECT_METADATA mode */
+#if IS_DEBIAN_UNSTABLE_KERNEL
 	"IFLA_VXLAN_LOCALBYPASS",
 	"IFLA_VXLAN_LABEL_POLICY", /* IPv6 flow label policy; ifla_vxlan_label_policy */
+#endif
 	"__IFLA_VXLAN_MAX"
 };
 
 static const char* IFLA_VXLANDF[] =  {
 	"VXLAN_DF_UNSET",
 	"VXLAN_DF_SET",
 	"VXLAN_DF_INHERIT",
@@ -549,15 +567,17 @@
 	"IFLA_BOND_AD_USER_PORT_KEY",
 	"IFLA_BOND_AD_ACTOR_SYSTEM",
 	"IFLA_BOND_TLB_DYNAMIC_LB",
 	"IFLA_BOND_PEER_NOTIF_DELAY",
 	"IFLA_BOND_AD_LACP_ACTIVE",
 	"IFLA_BOND_MISSED_MAX",
 	"IFLA_BOND_NS_IP6_TARGET",
+#if IS_DEBIAN_UNSTABLE_KERNEL
 	"IFLA_BOND_COUPLED_CONTROL",
+#endif
 	"__IFLA_BOND_MAX",
 };
 static const char* IFLA_BOND_ADINFO[] = {
 	"IFLA_BOND_AD_INFO_UNSPEC",
 	"IFLA_BOND_AD_INFO_AGGREGATOR",
 	"IFLA_BOND_AD_INFO_NUM_PORTS",
 	"IFLA_BOND_AD_INFO_ACTOR_KEY",
@@ -919,17 +939,19 @@
 	ADD_INT("IPVLAN_F_PRIVATE",IPVLAN_F_PRIVATE);
 	ADD_INT("IPVLAN_F_VEPA", IPVLAN_F_VEPA);
 
 	ADD_INT("NETKIT_NEXT",NETKIT_NEXT);
 	ADD_INT("NETKIT_PASS",NETKIT_PASS);
 	ADD_INT("NETKIT_DROP",NETKIT_DROP);
 	ADD_INT("NETKIT_REDIRECT",NETKIT_REDIRECT);
+#if IS_DEBIAN_UNSTABLE_KERNEL
 	ADD_ENUM(NETKIT_MODE, NETKIT_L3);
 	ADD_ENUM(IFLA_NETKIT, __IFLA_NETKIT_MAX);
 	ADD_INT("IFLA_NETKIT_MAX", IFLA_NETKIT_MAX);
+#endif
 
 	ADD_INT("TUNNEL_MSG_FLAG_STATS", TUNNEL_MSG_FLAG_STATS);
 	ADD_INT("TUNNEL_MSG_VALID_USER_FLAGS", TUNNEL_MSG_VALID_USER_FLAGS);
 	ADD_ENUM(VNIFILTER_ENTRY, __VNIFILTER_ENTRY_STATS_MAX);
 	ADD_INT("VNIFILTER_ENTRY_STATS_MAX", VNIFILTER_ENTRY_STATS_MAX);
 
 	ADD_ENUM(VXLAN_VNIFILTERENTRY, __VXLAN_VNIFILTER_ENTRY_MAX);
```

### Comparing `iothpy-1.3.3/iothpy/iothpy.c` & `iothpy-1.3.4/iothpy/iothpy.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy/iothpy_socket.c` & `iothpy-1.3.4/iothpy/iothpy_socket.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy/iothpy_socket.h` & `iothpy-1.3.4/iothpy/iothpy_socket.h`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy/iothpy_stack.c` & `iothpy-1.3.4/iothpy/iothpy_stack.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy/msocket.py` & `iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/msocket.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy/override.py` & `iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/override.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy/stack.py` & `iothpy-1.3.4/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/stack.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy/utils.c` & `iothpy-1.3.4/iothpy/utils.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy/utils.h` & `iothpy-1.3.4/iothpy/utils.h`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.3/iothpy.egg-info/PKG-INFO` & `iothpy-1.3.4/iothpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iothpy
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python library for internet of threads
 Home-page: https://github.com/ramenguy99/iothpy
 Author: Dario Mylonopoulos
 Author-email: dmylos@yahoo.it
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `iothpy-1.3.3/setup.py` & `iothpy-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 long_description = ""
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup (
        #setuptools options
        name = 'iothpy',
-       version = '1.3.3',
+       version = '1.3.4',
        author = 'Dario Mylonopoulos',
        author_email = 'dmylos@yahoo.it',
        url = 'https://github.com/ramenguy99/iothpy',
        description = 'Python library for internet of threads',
        long_description = long_description,
        long_description_content_type="text/markdown",
        packages = ["iothpy"],
```

