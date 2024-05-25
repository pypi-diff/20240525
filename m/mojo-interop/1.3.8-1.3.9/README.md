# Comparing `tmp/mojo_interop-1.3.8.tar.gz` & `tmp/mojo_interop-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_interop-1.3.8.tar", max compression
+gzip compressed data, was "mojo_interop-1.3.9.tar", max compression
```

## Comparing `mojo_interop-1.3.8.tar` & `mojo_interop-1.3.9.tar`

### file list

```diff
@@ -1,369 +1,369 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:54:30.874907 mojo_interop-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0      434 2024-01-26 02:54:30.875015 mojo_interop-1.3.8/README.rst
--rw-r--r--   0        0        0     1098 2024-02-17 00:15:58.469082 mojo_interop-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     2347 2024-01-26 02:54:30.876839 mojo_interop-1.3.8/source/packages/mojo/factories/mojointeroplandscapingfactories.py
--rw-r--r--   0        0        0     1184 2024-01-26 02:54:30.876921 mojo_interop-1.3.8/source/packages/mojo/factories/mojointeroptestplusfactories.py
--rw-r--r--   0        0        0       88 2024-01-26 02:54:30.877045 mojo_interop-1.3.8/source/packages/mojo/interop/clients/clientroles.py
--rw-r--r--   0        0        0     9941 2024-01-26 02:54:30.877141 mojo_interop-1.3.8/source/packages/mojo/interop/clients/clientsourcepackager.py
--rw-r--r--   0        0        0      180 2024-01-26 02:54:30.877198 mojo_interop-1.3.8/source/packages/mojo/interop/clients/constants.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.877256 mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/__init__.py
--rw-r--r--   0        0        0     5849 2024-02-10 01:33:00.318937 mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/ext/commandsext.py
--rw-r--r--   0        0        0    18918 2024-01-26 02:54:30.877488 mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/ext/configureext.py
--rw-r--r--   0        0        0     1989 2024-01-26 02:54:30.877567 mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/linuxclient.py
--rw-r--r--   0        0        0     2081 2024-01-26 02:54:30.877667 mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py
--rw-r--r--   0        0        0     1450 2024-01-26 02:54:30.877735 mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.877798 mojo_interop-1.3.8/source/packages/mojo/interop/clients/osx/__init__.py
--rw-r--r--   0        0        0     1490 2024-01-26 02:54:30.877866 mojo_interop-1.3.8/source/packages/mojo/interop/clients/osx/osxclient.py
--rw-r--r--   0        0        0     2000 2024-01-26 02:54:30.877922 mojo_interop-1.3.8/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py
--rw-r--r--   0        0        0     1425 2024-01-26 02:54:30.877984 mojo_interop-1.3.8/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.878049 mojo_interop-1.3.8/source/packages/mojo/interop/clients/windows/__init__.py
--rw-r--r--   0        0        0     1502 2024-01-26 02:54:30.878117 mojo_interop-1.3.8/source/packages/mojo/interop/clients/windows/windowsclient.py
--rw-r--r--   0        0        0     2052 2024-01-26 02:54:30.878177 mojo_interop-1.3.8/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py
--rw-r--r--   0        0        0     1477 2024-01-26 02:54:30.878229 mojo_interop-1.3.8/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py
--rw-r--r--   0        0        0      527 2024-01-26 02:54:30.878358 mojo_interop-1.3.8/source/packages/mojo/interop/clusters/constants.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.878429 mojo_interop-1.3.8/source/packages/mojo/interop/clusters/raspberrypi/__init__.py
--rw-r--r--   0        0        0      941 2024-01-26 02:54:30.878495 mojo_interop-1.3.8/source/packages/mojo/interop/clusters/raspberrypi/picluster.py
--rw-r--r--   0        0        0     1477 2024-01-26 02:54:30.878547 mojo_interop-1.3.8/source/packages/mojo/interop/clusters/raspberrypi/pinode.py
--rw-r--r--   0        0        0     2138 2024-01-26 02:54:30.878609 mojo_interop-1.3.8/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinator.py
--rw-r--r--   0        0        0     1226 2024-01-26 02:54:30.878664 mojo_interop-1.3.8/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinatorcoupling.py
--rw-r--r--   0        0        0      519 2024-01-26 02:54:30.878937 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/__init__.py
--rw-r--r--   0        0        0     2272 2024-01-26 02:54:30.879019 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsaddress.py
--rw-r--r--   0        0        0      639 2024-01-26 02:54:30.879082 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsapi.py
--rw-r--r--   0        0        0     9720 2024-01-26 02:54:30.879191 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsconst.py
--rw-r--r--   0        0        0     2121 2024-01-26 02:54:30.879289 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnshostinfo.py
--rw-r--r--   0        0        0     9274 2024-01-26 02:54:30.879369 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py
--rw-r--r--   0        0        0    15537 2024-01-26 02:54:30.879475 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py
--rw-r--r--   0        0        0     1862 2024-01-26 02:54:30.879530 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnspointer.py
--rw-r--r--   0        0        0     2250 2024-01-26 02:54:30.879603 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsquestion.py
--rw-r--r--   0        0        0      832 2024-01-26 02:54:30.879691 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py
--rw-r--r--   0        0        0     6850 2024-01-26 02:54:30.879779 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsrecord.py
--rw-r--r--   0        0        0     3599 2024-01-26 02:54:30.879877 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsserver.py
--rw-r--r--   0        0        0     2719 2024-01-26 02:54:30.879979 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsservice.py
--rw-r--r--   0        0        0     2004 2024-01-26 02:54:30.880055 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnstext.py
--rw-r--r--   0        0        0     3750 2024-01-26 02:54:30.880128 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsutil.py
--rw-r--r--   0        0        0     2807 2024-01-26 02:54:30.880206 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsvalidation.py
--rw-r--r--   0        0        0     1056 2024-01-26 02:54:30.880306 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/exceptions.py
--rw-r--r--   0        0        0     2601 2024-01-26 02:54:30.880402 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/mdnsagent.py
--rw-r--r--   0        0        0     6279 2024-01-26 02:54:30.880476 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py
--rw-r--r--   0        0        0     2505 2024-01-26 02:54:30.880540 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py
--rw-r--r--   0        0        0     1294 2024-01-26 02:54:30.880599 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/testmessages.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.880691 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/power/dlipower/__init__.py
--rw-r--r--   0        0        0      894 2024-01-26 02:54:30.880765 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py
--rw-r--r--   0        0        0     3743 2024-01-26 02:54:30.880817 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py
--rw-r--r--   0        0        0     6143 2024-01-26 02:54:30.880942 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py
--rw-r--r--   0        0        0     8246 2024-01-26 02:54:30.881064 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/serial/tcpserialagent.py
--rw-r--r--   0        0        0     4883 2024-01-26 02:54:30.881167 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py
--rw-r--r--   0        0        0     6075 2024-01-26 02:54:30.881247 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py
--rw-r--r--   0        0        0     1834 2024-01-26 02:54:30.881324 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.881387 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/__init__.py
--rw-r--r--   0        0        0    12854 2024-02-16 08:23:54.257584 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshagent.py
--rw-r--r--   0        0        0      713 2024-01-26 02:54:30.881545 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshaspects.py
--rw-r--r--   0        0        0    27684 2024-02-16 08:47:43.623057 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshbase.py
--rw-r--r--   0        0        0     1495 2024-01-26 02:54:30.881758 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshconst.py
--rw-r--r--   0        0        0     7000 2024-01-26 02:54:30.881818 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py
--rw-r--r--   0        0        0     6004 2024-01-26 02:54:30.881892 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py
--rw-r--r--   0        0        0     1698 2024-01-26 02:54:30.881955 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshdevice.py
--rw-r--r--   0        0        0    22453 2024-01-26 02:54:30.882091 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshhelpers.py
--rw-r--r--   0        0        0    13083 2024-02-16 08:24:15.689075 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshsession.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.882309 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/__init__.py
--rw-r--r--   0        0        0      991 2024-01-26 02:54:30.882418 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/examples/helloworldtasking.py
--rw-r--r--   0        0        0     1038 2024-01-26 02:54:30.882484 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/itaskingsequencer.py
--rw-r--r--   0        0        0      366 2024-01-26 02:54:30.882595 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/linux/tasker-service.template
--rw-r--r--   0        0        0      818 2024-01-26 02:54:30.882658 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/linux/taskerservice
--rw-r--r--   0        0        0     1316 2024-01-26 02:54:30.882725 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskeraspects.py
--rw-r--r--   0        0        0     8956 2024-01-26 02:54:30.882802 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskercontroller.py
--rw-r--r--   0        0        0    13350 2024-01-26 02:54:30.882908 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskerdaemon.py
--rw-r--r--   0        0        0      184 2024-01-26 02:54:30.882961 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskerexceptions.py
--rw-r--r--   0        0        0     7208 2024-02-17 00:16:01.897060 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskernode.py
--rw-r--r--   0        0        0     4307 2024-01-26 02:54:30.883116 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskerserver.py
--rw-r--r--   0        0        0     1431 2024-01-26 02:54:30.883181 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskerservermanager.py
--rw-r--r--   0        0        0    14561 2024-01-26 02:54:30.883307 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskerservice.py
--rw-r--r--   0        0        0    13035 2024-02-15 02:44:39.225881 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskersession.py
--rw-r--r--   0        0        0     1107 2024-02-16 22:36:14.559996 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskersessionref.py
--rw-r--r--   0        0        0    21237 2024-01-26 02:54:30.883551 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/tasking.py
--rw-r--r--   0        0        0     3253 2024-01-26 02:54:30.883633 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskingadapter.py
--rw-r--r--   0        0        0     4044 2024-01-26 02:54:30.883701 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskinggroupscope.py
--rw-r--r--   0        0        0      190 2024-02-15 03:30:13.623445 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskingprogresscallback.py
--rw-r--r--   0        0        0     4500 2024-02-16 23:47:44.560620 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskingresultpromise.py
--rw-r--r--   0        0        0      540 2024-01-26 02:54:30.883869 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/__init__.py
--rw-r--r--   0        0        0      319 2024-01-26 02:54:30.883920 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/aliases.py
--rw-r--r--   0        0        0     2431 2024-01-26 02:54:30.883976 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/aspects.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884028 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/content/__init__.py
--rw-r--r--   0        0        0    15564 2024-01-26 02:54:30.884129 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/content/didllite.py
--rw-r--r--   0        0        0      557 2024-01-26 02:54:30.884239 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/devices/__init__.py
--rw-r--r--   0        0        0    14091 2024-01-26 02:54:30.884343 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py
--rw-r--r--   0        0        0     1762 2024-01-26 02:54:30.884396 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py
--rw-r--r--   0        0        0    44945 2024-01-26 02:54:30.884504 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py
--rw-r--r--   0        0        0      494 2024-01-26 02:54:30.884595 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884654 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884718 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/embeddeddevices/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884778 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/rootdevices/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884853 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/services/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884980 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/embeddeddevices/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.885056 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/rootdevices/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.885170 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/__init__.py
--rw-r--r--   0        0        0     3546 2024-01-26 02:54:30.885328 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py
--rw-r--r--   0        0        0     6256 2024-01-26 02:54:30.885455 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py
--rw-r--r--   0        0        0    11235 2024-01-26 02:54:30.885595 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py
--rw-r--r--   0        0        0    11630 2024-01-26 02:54:30.885695 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py
--rw-r--r--   0        0        0    14967 2024-01-26 02:54:30.885756 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py
--rw-r--r--   0        0        0    20235 2024-01-26 02:54:30.885824 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py
--rw-r--r--   0        0        0    13617 2024-01-26 02:54:30.885914 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py
--rw-r--r--   0        0        0    16810 2024-01-26 02:54:30.885979 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py
--rw-r--r--   0        0        0     6154 2024-01-26 02:54:30.886055 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py
--rw-r--r--   0        0        0    12602 2024-01-26 02:54:30.886131 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py
--rw-r--r--   0        0        0    17054 2024-01-26 02:54:30.886215 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py
--rw-r--r--   0        0        0     4608 2024-01-26 02:54:30.886307 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py
--rw-r--r--   0        0        0      664 2024-01-26 02:54:30.886378 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py
--rw-r--r--   0        0        0     4143 2024-01-26 02:54:30.886443 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py
--rw-r--r--   0        0        0    11364 2024-01-26 02:54:30.886498 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py
--rw-r--r--   0        0        0    12982 2024-01-26 02:54:30.886559 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py
--rw-r--r--   0        0        0     4195 2024-01-26 02:54:30.886621 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py
--rw-r--r--   0        0        0     4195 2024-01-26 02:54:30.886679 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py
--rw-r--r--   0        0        0     5753 2024-01-26 02:54:30.886744 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py
--rw-r--r--   0        0        0     9487 2024-01-26 02:54:30.886815 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py
--rw-r--r--   0        0        0    11483 2024-01-26 02:54:30.886891 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py
--rw-r--r--   0        0        0    13568 2024-01-26 02:54:30.886947 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py
--rw-r--r--   0        0        0    23778 2024-01-26 02:54:30.887055 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py
--rw-r--r--   0        0        0     4463 2024-01-26 02:54:30.887133 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py
--rw-r--r--   0        0        0     7496 2024-01-26 02:54:30.887202 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py
--rw-r--r--   0        0        0    10904 2024-01-26 02:54:30.887271 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py
--rw-r--r--   0        0        0     7765 2024-01-26 02:54:30.887357 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py
--rw-r--r--   0        0        0     8862 2024-01-26 02:54:30.887415 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py
--rw-r--r--   0        0        0    10040 2024-01-26 02:54:30.887483 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py
--rw-r--r--   0        0        0     2077 2024-01-26 02:54:30.887546 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py
--rw-r--r--   0        0        0     4026 2024-01-26 02:54:30.887601 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py
--rw-r--r--   0        0        0     4993 2024-01-26 02:54:30.887665 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py
--rw-r--r--   0        0        0     3862 2024-01-26 02:54:30.887728 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py
--rw-r--r--   0        0        0     3200 2024-01-26 02:54:30.887790 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py
--rw-r--r--   0        0        0     2073 2024-01-26 02:54:30.887852 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py
--rw-r--r--   0        0        0     3611 2024-01-26 02:54:30.887916 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py
--rw-r--r--   0        0        0     3105 2024-01-26 02:54:30.887976 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py
--rw-r--r--   0        0        0     4720 2024-01-26 02:54:30.888052 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py
--rw-r--r--   0        0        0     9985 2024-01-26 02:54:30.888138 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py
--rw-r--r--   0        0        0     1816 2024-01-26 02:54:30.888196 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py
--rw-r--r--   0        0        0     8105 2024-01-26 02:54:30.888294 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py
--rw-r--r--   0        0        0     3965 2024-01-26 02:54:30.888358 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py
--rw-r--r--   0        0        0     3965 2024-01-26 02:54:30.888424 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py
--rw-r--r--   0        0        0    10274 2024-01-26 02:54:30.888484 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py
--rw-r--r--   0        0        0    10274 2024-01-26 02:54:30.888546 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py
--rw-r--r--   0        0        0     4709 2024-01-26 02:54:30.888610 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py
--rw-r--r--   0        0        0     5835 2024-01-26 02:54:30.888672 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py
--rw-r--r--   0        0        0    11150 2024-01-26 02:54:30.888757 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py
--rw-r--r--   0        0        0     1725 2024-01-26 02:54:30.888820 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py
--rw-r--r--   0        0        0     3322 2024-01-26 02:54:30.888877 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py
--rw-r--r--   0        0        0     2141 2024-01-26 02:54:30.888937 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py
--rw-r--r--   0        0        0     2746 2024-01-26 02:54:30.888994 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py
--rw-r--r--   0        0        0     4752 2024-01-26 02:54:30.889069 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py
--rw-r--r--   0        0        0     5248 2024-01-26 02:54:30.889135 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py
--rw-r--r--   0        0        0     5767 2024-01-26 02:54:30.889198 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py
--rw-r--r--   0        0        0     1785 2024-01-26 02:54:30.889260 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py
--rw-r--r--   0        0        0    20981 2024-01-26 02:54:30.889331 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py
--rw-r--r--   0        0        0    22594 2024-01-26 02:54:30.889411 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py
--rw-r--r--   0        0        0    26986 2024-01-26 02:54:30.889490 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py
--rw-r--r--   0        0        0     7370 2024-01-26 02:54:30.889577 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py
--rw-r--r--   0        0        0    11192 2024-01-26 02:54:30.889656 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py
--rw-r--r--   0        0        0    11192 2024-01-26 02:54:30.889729 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py
--rw-r--r--   0        0        0     9838 2024-01-26 02:54:30.889804 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py
--rw-r--r--   0        0        0    10359 2024-01-26 02:54:30.889877 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py
--rw-r--r--   0        0        0     2233 2024-01-26 02:54:30.889939 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py
--rw-r--r--   0        0        0     3291 2024-01-26 02:54:30.890005 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py
--rw-r--r--   0        0        0     4268 2024-01-26 02:54:30.890077 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py
--rw-r--r--   0        0        0     7820 2024-01-26 02:54:30.890153 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py
--rw-r--r--   0        0        0     8166 2024-01-26 02:54:30.890218 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py
--rw-r--r--   0        0        0     6212 2024-01-26 02:54:30.890292 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py
--rw-r--r--   0        0        0     1385 2024-01-26 02:54:30.890355 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py
--rw-r--r--   0        0        0    12448 2024-01-26 02:54:30.890442 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py
--rw-r--r--   0        0        0    15248 2024-01-26 02:54:30.890516 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py
--rw-r--r--   0        0        0     5167 2024-01-26 02:54:30.890589 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py
--rw-r--r--   0        0        0     6634 2024-01-26 02:54:30.890656 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py
--rw-r--r--   0        0        0    17165 2024-01-26 02:54:30.890723 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py
--rw-r--r--   0        0        0    31025 2024-01-26 02:54:30.890799 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.890841 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/__init__.py
--rw-r--r--   0        0        0      479 2024-01-26 02:54:30.890945 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.891016 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/dynamic/__init__.py
--rw-r--r--   0        0        0      247 2024-01-26 02:54:30.891210 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:BinaryLight:1.xml
--rw-r--r--   0        0        0      280 2024-01-26 02:54:30.891288 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DigitalSecurityCamera:1.xml
--rw-r--r--   0        0        0      420 2024-01-26 02:54:30.891349 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DimmableLight:1.xml
--rw-r--r--   0        0        0     1159 2024-01-26 02:54:30.891416 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml
--rw-r--r--   0        0        0     1865 2024-01-26 02:54:30.891479 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml
--rw-r--r--   0        0        0      459 2024-01-26 02:54:30.891537 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:1.xml
--rw-r--r--   0        0        0      604 2024-01-26 02:54:30.891597 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml
--rw-r--r--   0        0        0      208 2024-01-26 02:54:30.891653 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:LANDevice:1.xml
--rw-r--r--   0        0        0      408 2024-01-26 02:54:30.891714 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:1.xml
--rw-r--r--   0        0        0      408 2024-01-26 02:54:30.891775 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:2.xml
--rw-r--r--   0        0        0      580 2024-01-26 02:54:30.891847 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml
--rw-r--r--   0        0        0      999 2024-01-26 02:54:30.891913 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml
--rw-r--r--   0        0        0      999 2024-01-26 02:54:30.891982 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml
--rw-r--r--   0        0        0      580 2024-01-26 02:54:30.892037 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml
--rw-r--r--   0        0        0     1170 2024-01-26 02:54:30.892095 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml
--rw-r--r--   0        0        0     1170 2024-01-26 02:54:30.892153 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml
--rw-r--r--   0        0        0     1170 2024-01-26 02:54:30.892204 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml
--rw-r--r--   0        0        0      294 2024-01-26 02:54:30.892265 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Printer:1.xml
--rw-r--r--   0        0        0      187 2024-01-26 02:54:30.892327 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAClient:1.xml
--rw-r--r--   0        0        0      183 2024-01-26 02:54:30.892380 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:1.xml
--rw-r--r--   0        0        0      183 2024-01-26 02:54:30.892433 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:2.xml
--rw-r--r--   0        0        0      499 2024-01-26 02:54:30.892491 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:1.xml
--rw-r--r--   0        0        0      499 2024-01-26 02:54:30.892547 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:2.xml
--rw-r--r--   0        0        0      300 2024-01-26 02:54:30.892611 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIClientDevice:1.xml
--rw-r--r--   0        0        0      294 2024-01-26 02:54:30.892674 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIServerDevice:1.xml
--rw-r--r--   0        0        0      561 2024-01-26 02:54:30.892726 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml
--rw-r--r--   0        0        0      380 2024-01-26 02:54:30.892774 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:1.xml
--rw-r--r--   0        0        0      380 2024-01-26 02:54:30.892823 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:2.xml
--rw-r--r--   0        0        0      419 2024-01-26 02:54:30.892880 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:1.xml
--rw-r--r--   0        0        0      622 2024-01-26 02:54:30.892936 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml
--rw-r--r--   0        0        0      416 2024-01-26 02:54:30.892989 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:1.xml
--rw-r--r--   0        0        0      936 2024-01-26 02:54:30.893053 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml
--rw-r--r--   0        0        0     1090 2024-01-26 02:54:30.893109 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml
--rw-r--r--   0        0        0     1244 2024-01-26 02:54:30.893168 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml
--rw-r--r--   0        0        0      338 2024-01-26 02:54:30.893229 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:1.xml
--rw-r--r--   0        0        0      340 2024-01-26 02:54:30.893286 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:2.xml
--rw-r--r--   0        0        0      490 2024-01-26 02:54:30.893341 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WLANAccessPointDevice:1.xml
--rw-r--r--   0        0        0    21478 2024-01-26 02:54:30.893530 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml
--rw-r--r--   0        0        0    22506 2024-01-26 02:54:30.893679 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml
--rw-r--r--   0        0        0    32819 2024-01-26 02:54:30.893768 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml
--rw-r--r--   0        0        0     3894 2024-01-26 02:54:30.893850 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml
--rw-r--r--   0        0        0     5779 2024-01-26 02:54:30.893959 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml
--rw-r--r--   0        0        0    10054 2024-01-26 02:54:30.894058 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml
--rw-r--r--   0        0        0    22061 2024-01-26 02:54:30.894152 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml
--rw-r--r--   0        0        0    27823 2024-01-26 02:54:30.894247 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml
--rw-r--r--   0        0        0     5740 2024-01-26 02:54:30.894313 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml
--rw-r--r--   0        0        0    15507 2024-01-26 02:54:30.894392 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml
--rw-r--r--   0        0        0    22397 2024-01-26 02:54:30.894454 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml
--rw-r--r--   0        0        0     4082 2024-01-26 02:54:30.894523 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml
--rw-r--r--   0        0        0     2151 2024-01-26 02:54:30.894582 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml
--rw-r--r--   0        0        0     5359 2024-01-26 02:54:30.894648 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml
--rw-r--r--   0        0        0    11356 2024-01-26 02:54:30.894744 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml
--rw-r--r--   0        0        0    12959 2024-01-26 02:54:30.894847 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml
--rw-r--r--   0        0        0     7870 2024-01-26 02:54:30.894909 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml
--rw-r--r--   0        0        0     6485 2024-01-26 02:54:30.894971 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml
--rw-r--r--   0        0        0     8455 2024-01-26 02:54:30.895036 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml
--rw-r--r--   0        0        0    14206 2024-01-26 02:54:30.895114 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml
--rw-r--r--   0        0        0    15034 2024-01-26 02:54:30.895166 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml
--rw-r--r--   0        0        0    17600 2024-01-26 02:54:30.895217 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml
--rw-r--r--   0        0        0    27620 2024-01-26 02:54:30.895279 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml
--rw-r--r--   0        0        0     4821 2024-01-26 02:54:30.895427 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml
--rw-r--r--   0        0        0     7808 2024-01-26 02:54:30.895487 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml
--rw-r--r--   0        0        0     8486 2024-01-26 02:54:30.895563 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml
--rw-r--r--   0        0        0     4783 2024-01-26 02:54:30.895625 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml
--rw-r--r--   0        0        0     6607 2024-01-26 02:54:30.895687 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml
--rw-r--r--   0        0        0     8457 2024-01-26 02:54:30.895739 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml
--rw-r--r--   0        0        0     2249 2024-01-26 02:54:30.895792 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml
--rw-r--r--   0        0        0     3447 2024-01-26 02:54:30.895858 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml
--rw-r--r--   0        0        0     5176 2024-01-26 02:54:30.895905 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml
--rw-r--r--   0        0        0     2637 2024-01-26 02:54:30.895973 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml
--rw-r--r--   0        0        0     4564 2024-01-26 02:54:30.896029 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml
--rw-r--r--   0        0        0     3751 2024-01-26 02:54:30.896081 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml
--rw-r--r--   0        0        0     3673 2024-01-26 02:54:30.896173 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml
--rw-r--r--   0        0        0     2461 2024-01-26 02:54:30.896258 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml
--rw-r--r--   0        0        0     4528 2024-01-26 02:54:30.896337 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml
--rw-r--r--   0        0        0     7628 2024-01-26 02:54:30.896400 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml
--rw-r--r--   0        0        0     1045 2024-01-26 02:54:30.896448 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml
--rw-r--r--   0        0        0    15694 2024-01-26 02:54:30.896514 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml
--rw-r--r--   0        0        0     3331 2024-01-26 02:54:30.896581 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml
--rw-r--r--   0        0        0     3234 2024-01-26 02:54:30.896630 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml
--rw-r--r--   0        0        0    12147 2024-01-26 02:54:30.896683 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml
--rw-r--r--   0        0        0    12076 2024-01-26 02:54:30.896738 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml
--rw-r--r--   0        0        0     4682 2024-01-26 02:54:30.896810 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml
--rw-r--r--   0        0        0    13539 2024-01-26 02:54:30.896862 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml
--rw-r--r--   0        0        0    25446 2024-01-26 02:54:30.896941 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml
--rw-r--r--   0        0        0     1919 2024-01-26 02:54:30.896999 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml
--rw-r--r--   0        0        0     3445 2024-01-26 02:54:30.897048 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml
--rw-r--r--   0        0        0     2800 2024-01-26 02:54:30.897097 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml
--rw-r--r--   0        0        0     3264 2024-01-26 02:54:30.897151 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml
--rw-r--r--   0        0        0     4324 2024-01-26 02:54:30.897217 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml
--rw-r--r--   0        0        0     4744 2024-01-26 02:54:30.897278 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml
--rw-r--r--   0        0        0     6642 2024-01-26 02:54:30.897351 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml
--rw-r--r--   0        0        0     2399 2024-01-26 02:54:30.897425 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml
--rw-r--r--   0        0        0    24162 2024-01-26 02:54:30.897508 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml
--rw-r--r--   0        0        0    25624 2024-01-26 02:54:30.897576 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml
--rw-r--r--   0        0        0    29018 2024-01-26 02:54:30.897690 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml
--rw-r--r--   0        0        0    13767 2024-01-26 02:54:30.897747 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml
--rw-r--r--   0        0        0    13651 2024-01-26 02:54:30.897807 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml
--rw-r--r--   0        0        0    13651 2024-01-26 02:54:30.897865 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml
--rw-r--r--   0        0        0    13686 2024-01-26 02:54:30.897943 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml
--rw-r--r--   0        0        0    14103 2024-01-26 02:54:30.898010 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml
--rw-r--r--   0        0        0     1285 2024-01-26 02:54:30.898070 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml
--rw-r--r--   0        0        0     2951 2024-01-26 02:54:30.898153 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml
--rw-r--r--   0        0        0     3412 2024-01-26 02:54:30.898226 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml
--rw-r--r--   0        0        0     7592 2024-01-26 02:54:30.898302 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml
--rw-r--r--   0        0        0     8319 2024-01-26 02:54:30.898368 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml
--rw-r--r--   0        0        0     4926 2024-01-26 02:54:30.898426 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml
--rw-r--r--   0        0        0      754 2024-01-26 02:54:30.898498 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml
--rw-r--r--   0        0        0    14359 2024-01-26 02:54:30.898553 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml
--rw-r--r--   0        0        0    19829 2024-01-26 02:54:30.898606 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml
--rw-r--r--   0        0        0     7097 2024-01-26 02:54:30.898680 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml
--rw-r--r--   0        0        0     6730 2024-01-26 02:54:30.898738 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml
--rw-r--r--   0        0        0    18555 2024-01-26 02:54:30.898797 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml
--rw-r--r--   0        0        0    39224 2024-01-26 02:54:30.898882 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml
--rw-r--r--   0        0        0    16892 2024-01-26 02:54:30.898996 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py
--rw-r--r--   0        0        0     2823 2024-01-26 02:54:30.899067 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/paths.py
--rw-r--r--   0        0        0      481 2024-01-26 02:54:30.899145 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/services/__init__.py
--rw-r--r--   0        0        0     5518 2024-01-26 02:54:30.899210 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py
--rw-r--r--   0        0        0    26073 2024-01-26 02:54:30.899328 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py
--rw-r--r--   0        0        0    11691 2024-01-26 02:54:30.899411 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/soap.py
--rw-r--r--   0        0        0      939 2024-01-26 02:54:30.899466 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnpconstants.py
--rw-r--r--   0        0        0    56002 2024-01-26 02:54:30.899666 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py
--rw-r--r--   0        0        0     7467 2024-01-26 02:54:30.899723 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py
--rw-r--r--   0        0        0     2628 2024-01-26 02:54:30.899768 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnperrors.py
--rw-r--r--   0        0        0    11247 2024-01-26 02:54:30.899861 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnpfactory.py
--rw-r--r--   0        0        0    21613 2024-01-26 02:54:30.899968 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py
--rw-r--r--   0        0        0      494 2024-01-26 02:54:30.900051 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/xml/__init__.py
--rw-r--r--   0        0        0    20710 2024-01-26 02:54:30.900155 mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py
--rw-r--r--   0        0        0       67 2024-01-26 02:54:30.900259 mojo_interop-1.3.8/source/packages/mojo/interop/services/common.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.900322 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/__init__.py
--rw-r--r--   0        0        0        1 2024-01-26 02:54:30.900417 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.900478 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/model/__init__.py
--rw-r--r--   0        0        0      464 2024-01-26 02:54:30.900540 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/model/summary.py
--rw-r--r--   0        0        0    13344 2024-01-26 02:54:30.900625 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/model/vm.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.900683 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/specs/__init__.py
--rw-r--r--   0        0        0     2226 2024-01-26 02:54:30.900746 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/specs/vmcreate.py
--rw-r--r--   0        0        0     5889 2024-01-26 02:54:30.900827 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/specs/vmhardware.py
--rw-r--r--   0        0        0      481 2024-01-26 02:54:30.900880 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/specs/vmplacement.py
--rw-r--r--   0        0        0      314 2024-01-26 02:54:30.900947 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/specs/vmstorage.py
--rw-r--r--   0        0        0      262 2024-01-26 02:54:30.900997 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/vcenter.py
--rw-r--r--   0        0        0        1 2024-01-26 02:54:30.901070 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/metasphere/__init__.py
--rw-r--r--   0        0        0      315 2024-01-26 02:54:30.901117 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/metasphere/vcenter.py
--rw-r--r--   0        0        0    11195 2024-01-26 02:54:30.901191 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/metasphere/vmguestos.py
--rw-r--r--   0        0        0     3287 2024-01-26 02:54:30.901262 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/metasphere/vmhardware.py
--rw-r--r--   0        0        0     2149 2024-01-26 02:54:30.901319 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vmworkstationagent.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.901365 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:54:30.901424 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/__init__.py
--rw-r--r--   0        0        0      873 2024-01-26 02:54:30.901492 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/baseext.py
--rw-r--r--   0        0        0      849 2024-01-26 02:54:30.901556 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/certificatemanagementext.py
--rw-r--r--   0        0        0      806 2024-01-26 02:54:30.901601 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/clusterext.py
--rw-r--r--   0        0        0      806 2024-01-26 02:54:30.901647 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/computeext.py
--rw-r--r--   0        0        0      806 2024-01-26 02:54:30.901688 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/contentext.py
--rw-r--r--   0        0        0      824 2024-01-26 02:54:30.901735 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/cryptomanagerext.py
--rw-r--r--   0        0        0     2416 2024-01-26 02:54:30.901795 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/datacenterext.py
--rw-r--r--   0        0        0     1512 2024-01-26 02:54:30.901838 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/datastoreext.py
--rw-r--r--   0        0        0      815 2024-01-26 02:54:30.901893 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/deploymentext.py
--rw-r--r--   0        0        0     3028 2024-01-26 02:54:30.901956 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/folderext.py
--rw-r--r--   0        0        0      800 2024-01-26 02:54:30.902034 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/guestext.py
--rw-r--r--   0        0        0     2005 2024-01-26 02:54:30.902084 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/hostext.py
--rw-r--r--   0        0        0      794 2024-01-26 02:54:30.902127 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/hvcext.py
--rw-r--r--   0        0        0      809 2024-01-26 02:54:30.902174 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/identityext.py
--rw-r--r--   0        0        0      812 2024-01-26 02:54:30.902227 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/inventoryext.py
--rw-r--r--   0        0        0     1734 2024-01-26 02:54:30.902290 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/isoext.py
--rw-r--r--   0        0        0      794 2024-01-26 02:54:30.902354 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/lcmext.py
--rw-r--r--   0        0        0      842 2024-01-26 02:54:30.902407 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/namespacemanagementext.py
--rw-r--r--   0        0        0      815 2024-01-26 02:54:30.902455 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/namespacesext.py
--rw-r--r--   0        0        0     1152 2024-01-26 02:54:30.902513 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/networkext.py
--rw-r--r--   0        0        0      794 2024-01-26 02:54:30.902564 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/ovfext.py
--rw-r--r--   0        0        0      821 2024-01-26 02:54:30.902630 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/resourcepoolext.py
--rw-r--r--   0        0        0      809 2024-01-26 02:54:30.902681 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/servicesext.py
--rw-r--r--   0        0        0      806 2024-01-26 02:54:30.902732 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/storageext.py
--rw-r--r--   0        0        0      821 2024-01-26 02:54:30.902789 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/systemconfigext.py
--rw-r--r--   0        0        0      805 2024-01-26 02:54:30.902869 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/taggingext.py
--rw-r--r--   0        0        0      820 2024-01-26 02:54:30.902923 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/tokenserviceext.py
--rw-r--r--   0        0        0      808 2024-01-26 02:54:30.902978 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/topologyext.py
--rw-r--r--   0        0        0      847 2024-01-26 02:54:30.903029 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/trustedinfrastructureext.py
--rw-r--r--   0        0        0     9272 2024-01-26 02:54:30.903080 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/vmext.py
--rw-r--r--   0        0        0    10881 2024-01-26 02:54:30.903164 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/vsphereagent.py
--rw-r--r--   0        0        0      781 2024-01-26 02:54:30.903218 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/vspherecoordinator.py
--rw-r--r--   0        0        0      562 2024-01-26 02:54:30.903282 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/vspherecoordinatorcoupling.py
--rw-r--r--   0        0        0     1505 2024-01-26 02:54:30.903341 mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/vsphereservice.py
--rw-r--r--   0        0        0     3605 2024-01-26 02:54:30.903437 mojo_interop-1.3.8/source/packages/mojo/interop/testing/interoptestjob.py
--rw-r--r--   0        0        0     3849 2024-01-26 02:54:30.903512 mojo_interop-1.3.8/source/packages/mojo/interop/testing/interoptestsequencer.py
--rw-r--r--   0        0        0     3318 1970-01-01 00:00:00.000000 mojo_interop-1.3.8/setup.py
--rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 mojo_interop-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:54:30.874907 mojo_interop-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0      434 2024-01-26 02:54:30.875015 mojo_interop-1.3.9/README.rst
+-rw-r--r--   0        0        0     1098 2024-02-17 00:25:22.610947 mojo_interop-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2347 2024-01-26 02:54:30.876839 mojo_interop-1.3.9/source/packages/mojo/factories/mojointeroplandscapingfactories.py
+-rw-r--r--   0        0        0     1184 2024-01-26 02:54:30.876921 mojo_interop-1.3.9/source/packages/mojo/factories/mojointeroptestplusfactories.py
+-rw-r--r--   0        0        0       88 2024-01-26 02:54:30.877045 mojo_interop-1.3.9/source/packages/mojo/interop/clients/clientroles.py
+-rw-r--r--   0        0        0     9941 2024-01-26 02:54:30.877141 mojo_interop-1.3.9/source/packages/mojo/interop/clients/clientsourcepackager.py
+-rw-r--r--   0        0        0      180 2024-01-26 02:54:30.877198 mojo_interop-1.3.9/source/packages/mojo/interop/clients/constants.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.877256 mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/__init__.py
+-rw-r--r--   0        0        0     5849 2024-02-10 01:33:00.318937 mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/ext/commandsext.py
+-rw-r--r--   0        0        0    18918 2024-01-26 02:54:30.877488 mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/ext/configureext.py
+-rw-r--r--   0        0        0     1989 2024-01-26 02:54:30.877567 mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/linuxclient.py
+-rw-r--r--   0        0        0     2081 2024-01-26 02:54:30.877667 mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py
+-rw-r--r--   0        0        0     1450 2024-01-26 02:54:30.877735 mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.877798 mojo_interop-1.3.9/source/packages/mojo/interop/clients/osx/__init__.py
+-rw-r--r--   0        0        0     1490 2024-01-26 02:54:30.877866 mojo_interop-1.3.9/source/packages/mojo/interop/clients/osx/osxclient.py
+-rw-r--r--   0        0        0     2000 2024-01-26 02:54:30.877922 mojo_interop-1.3.9/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py
+-rw-r--r--   0        0        0     1425 2024-01-26 02:54:30.877984 mojo_interop-1.3.9/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.878049 mojo_interop-1.3.9/source/packages/mojo/interop/clients/windows/__init__.py
+-rw-r--r--   0        0        0     1502 2024-01-26 02:54:30.878117 mojo_interop-1.3.9/source/packages/mojo/interop/clients/windows/windowsclient.py
+-rw-r--r--   0        0        0     2052 2024-01-26 02:54:30.878177 mojo_interop-1.3.9/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py
+-rw-r--r--   0        0        0     1477 2024-01-26 02:54:30.878229 mojo_interop-1.3.9/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py
+-rw-r--r--   0        0        0      527 2024-01-26 02:54:30.878358 mojo_interop-1.3.9/source/packages/mojo/interop/clusters/constants.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.878429 mojo_interop-1.3.9/source/packages/mojo/interop/clusters/raspberrypi/__init__.py
+-rw-r--r--   0        0        0      941 2024-01-26 02:54:30.878495 mojo_interop-1.3.9/source/packages/mojo/interop/clusters/raspberrypi/picluster.py
+-rw-r--r--   0        0        0     1477 2024-01-26 02:54:30.878547 mojo_interop-1.3.9/source/packages/mojo/interop/clusters/raspberrypi/pinode.py
+-rw-r--r--   0        0        0     2138 2024-01-26 02:54:30.878609 mojo_interop-1.3.9/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinator.py
+-rw-r--r--   0        0        0     1226 2024-01-26 02:54:30.878664 mojo_interop-1.3.9/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinatorcoupling.py
+-rw-r--r--   0        0        0      519 2024-01-26 02:54:30.878937 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/__init__.py
+-rw-r--r--   0        0        0     2272 2024-01-26 02:54:30.879019 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsaddress.py
+-rw-r--r--   0        0        0      639 2024-01-26 02:54:30.879082 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsapi.py
+-rw-r--r--   0        0        0     9720 2024-01-26 02:54:30.879191 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsconst.py
+-rw-r--r--   0        0        0     2121 2024-01-26 02:54:30.879289 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnshostinfo.py
+-rw-r--r--   0        0        0     9274 2024-01-26 02:54:30.879369 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py
+-rw-r--r--   0        0        0    15537 2024-01-26 02:54:30.879475 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py
+-rw-r--r--   0        0        0     1862 2024-01-26 02:54:30.879530 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnspointer.py
+-rw-r--r--   0        0        0     2250 2024-01-26 02:54:30.879603 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsquestion.py
+-rw-r--r--   0        0        0      832 2024-01-26 02:54:30.879691 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py
+-rw-r--r--   0        0        0     6850 2024-01-26 02:54:30.879779 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsrecord.py
+-rw-r--r--   0        0        0     3599 2024-01-26 02:54:30.879877 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsserver.py
+-rw-r--r--   0        0        0     2719 2024-01-26 02:54:30.879979 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsservice.py
+-rw-r--r--   0        0        0     2004 2024-01-26 02:54:30.880055 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnstext.py
+-rw-r--r--   0        0        0     3750 2024-01-26 02:54:30.880128 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsutil.py
+-rw-r--r--   0        0        0     2807 2024-01-26 02:54:30.880206 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsvalidation.py
+-rw-r--r--   0        0        0     1056 2024-01-26 02:54:30.880306 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/exceptions.py
+-rw-r--r--   0        0        0     2601 2024-01-26 02:54:30.880402 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/mdnsagent.py
+-rw-r--r--   0        0        0     6279 2024-01-26 02:54:30.880476 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py
+-rw-r--r--   0        0        0     2505 2024-01-26 02:54:30.880540 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py
+-rw-r--r--   0        0        0     1294 2024-01-26 02:54:30.880599 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/testmessages.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.880691 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/power/dlipower/__init__.py
+-rw-r--r--   0        0        0      894 2024-01-26 02:54:30.880765 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py
+-rw-r--r--   0        0        0     3743 2024-01-26 02:54:30.880817 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py
+-rw-r--r--   0        0        0     6143 2024-01-26 02:54:30.880942 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py
+-rw-r--r--   0        0        0     8246 2024-01-26 02:54:30.881064 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/serial/tcpserialagent.py
+-rw-r--r--   0        0        0     4883 2024-01-26 02:54:30.881167 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py
+-rw-r--r--   0        0        0     6075 2024-01-26 02:54:30.881247 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py
+-rw-r--r--   0        0        0     1834 2024-01-26 02:54:30.881324 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.881387 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/__init__.py
+-rw-r--r--   0        0        0    12854 2024-02-16 08:23:54.257584 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshagent.py
+-rw-r--r--   0        0        0      713 2024-01-26 02:54:30.881545 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshaspects.py
+-rw-r--r--   0        0        0    27684 2024-02-16 08:47:43.623057 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshbase.py
+-rw-r--r--   0        0        0     1495 2024-01-26 02:54:30.881758 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshconst.py
+-rw-r--r--   0        0        0     7000 2024-01-26 02:54:30.881818 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py
+-rw-r--r--   0        0        0     6004 2024-01-26 02:54:30.881892 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py
+-rw-r--r--   0        0        0     1698 2024-01-26 02:54:30.881955 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshdevice.py
+-rw-r--r--   0        0        0    22453 2024-01-26 02:54:30.882091 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshhelpers.py
+-rw-r--r--   0        0        0    13083 2024-02-16 08:24:15.689075 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshsession.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.882309 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/__init__.py
+-rw-r--r--   0        0        0      991 2024-01-26 02:54:30.882418 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/examples/helloworldtasking.py
+-rw-r--r--   0        0        0     1038 2024-01-26 02:54:30.882484 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/itaskingsequencer.py
+-rw-r--r--   0        0        0      366 2024-01-26 02:54:30.882595 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/linux/tasker-service.template
+-rw-r--r--   0        0        0      818 2024-01-26 02:54:30.882658 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/linux/taskerservice
+-rw-r--r--   0        0        0     1316 2024-01-26 02:54:30.882725 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskeraspects.py
+-rw-r--r--   0        0        0     8956 2024-01-26 02:54:30.882802 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskercontroller.py
+-rw-r--r--   0        0        0    13350 2024-01-26 02:54:30.882908 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskerdaemon.py
+-rw-r--r--   0        0        0      184 2024-01-26 02:54:30.882961 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskerexceptions.py
+-rw-r--r--   0        0        0     7208 2024-02-17 00:16:01.897060 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskernode.py
+-rw-r--r--   0        0        0     4307 2024-01-26 02:54:30.883116 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskerserver.py
+-rw-r--r--   0        0        0     1431 2024-01-26 02:54:30.883181 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskerservermanager.py
+-rw-r--r--   0        0        0    15359 2024-02-17 00:25:12.251907 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskerservice.py
+-rw-r--r--   0        0        0    13035 2024-02-15 02:44:39.225881 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskersession.py
+-rw-r--r--   0        0        0     1107 2024-02-16 22:36:14.559996 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskersessionref.py
+-rw-r--r--   0        0        0    21237 2024-01-26 02:54:30.883551 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/tasking.py
+-rw-r--r--   0        0        0     3253 2024-01-26 02:54:30.883633 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskingadapter.py
+-rw-r--r--   0        0        0     4044 2024-01-26 02:54:30.883701 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskinggroupscope.py
+-rw-r--r--   0        0        0      190 2024-02-15 03:30:13.623445 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskingprogresscallback.py
+-rw-r--r--   0        0        0     4500 2024-02-16 23:47:44.560620 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskingresultpromise.py
+-rw-r--r--   0        0        0      540 2024-01-26 02:54:30.883869 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/__init__.py
+-rw-r--r--   0        0        0      319 2024-01-26 02:54:30.883920 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/aliases.py
+-rw-r--r--   0        0        0     2431 2024-01-26 02:54:30.883976 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/aspects.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884028 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/content/__init__.py
+-rw-r--r--   0        0        0    15564 2024-01-26 02:54:30.884129 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/content/didllite.py
+-rw-r--r--   0        0        0      557 2024-01-26 02:54:30.884239 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/devices/__init__.py
+-rw-r--r--   0        0        0    14091 2024-01-26 02:54:30.884343 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py
+-rw-r--r--   0        0        0     1762 2024-01-26 02:54:30.884396 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py
+-rw-r--r--   0        0        0    44945 2024-01-26 02:54:30.884504 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py
+-rw-r--r--   0        0        0      494 2024-01-26 02:54:30.884595 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884654 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884718 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/embeddeddevices/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884778 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/rootdevices/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884853 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.884980 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/embeddeddevices/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.885056 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/rootdevices/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.885170 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/__init__.py
+-rw-r--r--   0        0        0     3546 2024-01-26 02:54:30.885328 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py
+-rw-r--r--   0        0        0     6256 2024-01-26 02:54:30.885455 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    11235 2024-01-26 02:54:30.885595 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py
+-rw-r--r--   0        0        0    11630 2024-01-26 02:54:30.885695 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py
+-rw-r--r--   0        0        0    14967 2024-01-26 02:54:30.885756 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py
+-rw-r--r--   0        0        0    20235 2024-01-26 02:54:30.885824 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py
+-rw-r--r--   0        0        0    13617 2024-01-26 02:54:30.885914 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    16810 2024-01-26 02:54:30.885979 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     6154 2024-01-26 02:54:30.886055 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py
+-rw-r--r--   0        0        0    12602 2024-01-26 02:54:30.886131 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    17054 2024-01-26 02:54:30.886215 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     4608 2024-01-26 02:54:30.886307 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py
+-rw-r--r--   0        0        0      664 2024-01-26 02:54:30.886378 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py
+-rw-r--r--   0        0        0     4143 2024-01-26 02:54:30.886443 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py
+-rw-r--r--   0        0        0    11364 2024-01-26 02:54:30.886498 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    12982 2024-01-26 02:54:30.886559 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     4195 2024-01-26 02:54:30.886621 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py
+-rw-r--r--   0        0        0     4195 2024-01-26 02:54:30.886679 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py
+-rw-r--r--   0        0        0     5753 2024-01-26 02:54:30.886744 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py
+-rw-r--r--   0        0        0     9487 2024-01-26 02:54:30.886815 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py
+-rw-r--r--   0        0        0    11483 2024-01-26 02:54:30.886891 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py
+-rw-r--r--   0        0        0    13568 2024-01-26 02:54:30.886947 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py
+-rw-r--r--   0        0        0    23778 2024-01-26 02:54:30.887055 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py
+-rw-r--r--   0        0        0     4463 2024-01-26 02:54:30.887133 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py
+-rw-r--r--   0        0        0     7496 2024-01-26 02:54:30.887202 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py
+-rw-r--r--   0        0        0    10904 2024-01-26 02:54:30.887271 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py
+-rw-r--r--   0        0        0     7765 2024-01-26 02:54:30.887357 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py
+-rw-r--r--   0        0        0     8862 2024-01-26 02:54:30.887415 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py
+-rw-r--r--   0        0        0    10040 2024-01-26 02:54:30.887483 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py
+-rw-r--r--   0        0        0     2077 2024-01-26 02:54:30.887546 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py
+-rw-r--r--   0        0        0     4026 2024-01-26 02:54:30.887601 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py
+-rw-r--r--   0        0        0     4993 2024-01-26 02:54:30.887665 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py
+-rw-r--r--   0        0        0     3862 2024-01-26 02:54:30.887728 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py
+-rw-r--r--   0        0        0     3200 2024-01-26 02:54:30.887790 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py
+-rw-r--r--   0        0        0     2073 2024-01-26 02:54:30.887852 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py
+-rw-r--r--   0        0        0     3611 2024-01-26 02:54:30.887916 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py
+-rw-r--r--   0        0        0     3105 2024-01-26 02:54:30.887976 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py
+-rw-r--r--   0        0        0     4720 2024-01-26 02:54:30.888052 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py
+-rw-r--r--   0        0        0     9985 2024-01-26 02:54:30.888138 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py
+-rw-r--r--   0        0        0     1816 2024-01-26 02:54:30.888196 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py
+-rw-r--r--   0        0        0     8105 2024-01-26 02:54:30.888294 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py
+-rw-r--r--   0        0        0     3965 2024-01-26 02:54:30.888358 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py
+-rw-r--r--   0        0        0     3965 2024-01-26 02:54:30.888424 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py
+-rw-r--r--   0        0        0    10274 2024-01-26 02:54:30.888484 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py
+-rw-r--r--   0        0        0    10274 2024-01-26 02:54:30.888546 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py
+-rw-r--r--   0        0        0     4709 2024-01-26 02:54:30.888610 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py
+-rw-r--r--   0        0        0     5835 2024-01-26 02:54:30.888672 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py
+-rw-r--r--   0        0        0    11150 2024-01-26 02:54:30.888757 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py
+-rw-r--r--   0        0        0     1725 2024-01-26 02:54:30.888820 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py
+-rw-r--r--   0        0        0     3322 2024-01-26 02:54:30.888877 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py
+-rw-r--r--   0        0        0     2141 2024-01-26 02:54:30.888937 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py
+-rw-r--r--   0        0        0     2746 2024-01-26 02:54:30.888994 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py
+-rw-r--r--   0        0        0     4752 2024-01-26 02:54:30.889069 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py
+-rw-r--r--   0        0        0     5248 2024-01-26 02:54:30.889135 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py
+-rw-r--r--   0        0        0     5767 2024-01-26 02:54:30.889198 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py
+-rw-r--r--   0        0        0     1785 2024-01-26 02:54:30.889260 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py
+-rw-r--r--   0        0        0    20981 2024-01-26 02:54:30.889331 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py
+-rw-r--r--   0        0        0    22594 2024-01-26 02:54:30.889411 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py
+-rw-r--r--   0        0        0    26986 2024-01-26 02:54:30.889490 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py
+-rw-r--r--   0        0        0     7370 2024-01-26 02:54:30.889577 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py
+-rw-r--r--   0        0        0    11192 2024-01-26 02:54:30.889656 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py
+-rw-r--r--   0        0        0    11192 2024-01-26 02:54:30.889729 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py
+-rw-r--r--   0        0        0     9838 2024-01-26 02:54:30.889804 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py
+-rw-r--r--   0        0        0    10359 2024-01-26 02:54:30.889877 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py
+-rw-r--r--   0        0        0     2233 2024-01-26 02:54:30.889939 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py
+-rw-r--r--   0        0        0     3291 2024-01-26 02:54:30.890005 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py
+-rw-r--r--   0        0        0     4268 2024-01-26 02:54:30.890077 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py
+-rw-r--r--   0        0        0     7820 2024-01-26 02:54:30.890153 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0     8166 2024-01-26 02:54:30.890218 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py
+-rw-r--r--   0        0        0     6212 2024-01-26 02:54:30.890292 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0     1385 2024-01-26 02:54:30.890355 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0    12448 2024-01-26 02:54:30.890442 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py
+-rw-r--r--   0        0        0    15248 2024-01-26 02:54:30.890516 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py
+-rw-r--r--   0        0        0     5167 2024-01-26 02:54:30.890589 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py
+-rw-r--r--   0        0        0     6634 2024-01-26 02:54:30.890656 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0    17165 2024-01-26 02:54:30.890723 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py
+-rw-r--r--   0        0        0    31025 2024-01-26 02:54:30.890799 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.890841 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/__init__.py
+-rw-r--r--   0        0        0      479 2024-01-26 02:54:30.890945 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.891016 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/dynamic/__init__.py
+-rw-r--r--   0        0        0      247 2024-01-26 02:54:30.891210 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:BinaryLight:1.xml
+-rw-r--r--   0        0        0      280 2024-01-26 02:54:30.891288 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DigitalSecurityCamera:1.xml
+-rw-r--r--   0        0        0      420 2024-01-26 02:54:30.891349 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DimmableLight:1.xml
+-rw-r--r--   0        0        0     1159 2024-01-26 02:54:30.891416 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml
+-rw-r--r--   0        0        0     1865 2024-01-26 02:54:30.891479 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml
+-rw-r--r--   0        0        0      459 2024-01-26 02:54:30.891537 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:1.xml
+-rw-r--r--   0        0        0      604 2024-01-26 02:54:30.891597 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml
+-rw-r--r--   0        0        0      208 2024-01-26 02:54:30.891653 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:LANDevice:1.xml
+-rw-r--r--   0        0        0      408 2024-01-26 02:54:30.891714 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:1.xml
+-rw-r--r--   0        0        0      408 2024-01-26 02:54:30.891775 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:2.xml
+-rw-r--r--   0        0        0      580 2024-01-26 02:54:30.891847 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml
+-rw-r--r--   0        0        0      999 2024-01-26 02:54:30.891913 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml
+-rw-r--r--   0        0        0      999 2024-01-26 02:54:30.891982 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml
+-rw-r--r--   0        0        0      580 2024-01-26 02:54:30.892037 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml
+-rw-r--r--   0        0        0     1170 2024-01-26 02:54:30.892095 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml
+-rw-r--r--   0        0        0     1170 2024-01-26 02:54:30.892153 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml
+-rw-r--r--   0        0        0     1170 2024-01-26 02:54:30.892204 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml
+-rw-r--r--   0        0        0      294 2024-01-26 02:54:30.892265 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Printer:1.xml
+-rw-r--r--   0        0        0      187 2024-01-26 02:54:30.892327 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAClient:1.xml
+-rw-r--r--   0        0        0      183 2024-01-26 02:54:30.892380 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:1.xml
+-rw-r--r--   0        0        0      183 2024-01-26 02:54:30.892433 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:2.xml
+-rw-r--r--   0        0        0      499 2024-01-26 02:54:30.892491 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:1.xml
+-rw-r--r--   0        0        0      499 2024-01-26 02:54:30.892547 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:2.xml
+-rw-r--r--   0        0        0      300 2024-01-26 02:54:30.892611 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIClientDevice:1.xml
+-rw-r--r--   0        0        0      294 2024-01-26 02:54:30.892674 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIServerDevice:1.xml
+-rw-r--r--   0        0        0      561 2024-01-26 02:54:30.892726 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml
+-rw-r--r--   0        0        0      380 2024-01-26 02:54:30.892774 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:1.xml
+-rw-r--r--   0        0        0      380 2024-01-26 02:54:30.892823 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:2.xml
+-rw-r--r--   0        0        0      419 2024-01-26 02:54:30.892880 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:1.xml
+-rw-r--r--   0        0        0      622 2024-01-26 02:54:30.892936 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml
+-rw-r--r--   0        0        0      416 2024-01-26 02:54:30.892989 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:1.xml
+-rw-r--r--   0        0        0      936 2024-01-26 02:54:30.893053 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml
+-rw-r--r--   0        0        0     1090 2024-01-26 02:54:30.893109 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml
+-rw-r--r--   0        0        0     1244 2024-01-26 02:54:30.893168 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml
+-rw-r--r--   0        0        0      338 2024-01-26 02:54:30.893229 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:1.xml
+-rw-r--r--   0        0        0      340 2024-01-26 02:54:30.893286 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:2.xml
+-rw-r--r--   0        0        0      490 2024-01-26 02:54:30.893341 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WLANAccessPointDevice:1.xml
+-rw-r--r--   0        0        0    21478 2024-01-26 02:54:30.893530 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml
+-rw-r--r--   0        0        0    22506 2024-01-26 02:54:30.893679 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml
+-rw-r--r--   0        0        0    32819 2024-01-26 02:54:30.893768 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml
+-rw-r--r--   0        0        0     3894 2024-01-26 02:54:30.893850 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml
+-rw-r--r--   0        0        0     5779 2024-01-26 02:54:30.893959 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml
+-rw-r--r--   0        0        0    10054 2024-01-26 02:54:30.894058 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml
+-rw-r--r--   0        0        0    22061 2024-01-26 02:54:30.894152 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml
+-rw-r--r--   0        0        0    27823 2024-01-26 02:54:30.894247 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml
+-rw-r--r--   0        0        0     5740 2024-01-26 02:54:30.894313 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml
+-rw-r--r--   0        0        0    15507 2024-01-26 02:54:30.894392 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml
+-rw-r--r--   0        0        0    22397 2024-01-26 02:54:30.894454 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml
+-rw-r--r--   0        0        0     4082 2024-01-26 02:54:30.894523 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml
+-rw-r--r--   0        0        0     2151 2024-01-26 02:54:30.894582 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml
+-rw-r--r--   0        0        0     5359 2024-01-26 02:54:30.894648 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml
+-rw-r--r--   0        0        0    11356 2024-01-26 02:54:30.894744 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml
+-rw-r--r--   0        0        0    12959 2024-01-26 02:54:30.894847 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml
+-rw-r--r--   0        0        0     7870 2024-01-26 02:54:30.894909 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml
+-rw-r--r--   0        0        0     6485 2024-01-26 02:54:30.894971 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml
+-rw-r--r--   0        0        0     8455 2024-01-26 02:54:30.895036 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml
+-rw-r--r--   0        0        0    14206 2024-01-26 02:54:30.895114 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml
+-rw-r--r--   0        0        0    15034 2024-01-26 02:54:30.895166 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml
+-rw-r--r--   0        0        0    17600 2024-01-26 02:54:30.895217 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml
+-rw-r--r--   0        0        0    27620 2024-01-26 02:54:30.895279 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml
+-rw-r--r--   0        0        0     4821 2024-01-26 02:54:30.895427 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml
+-rw-r--r--   0        0        0     7808 2024-01-26 02:54:30.895487 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml
+-rw-r--r--   0        0        0     8486 2024-01-26 02:54:30.895563 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml
+-rw-r--r--   0        0        0     4783 2024-01-26 02:54:30.895625 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml
+-rw-r--r--   0        0        0     6607 2024-01-26 02:54:30.895687 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml
+-rw-r--r--   0        0        0     8457 2024-01-26 02:54:30.895739 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml
+-rw-r--r--   0        0        0     2249 2024-01-26 02:54:30.895792 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml
+-rw-r--r--   0        0        0     3447 2024-01-26 02:54:30.895858 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml
+-rw-r--r--   0        0        0     5176 2024-01-26 02:54:30.895905 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml
+-rw-r--r--   0        0        0     2637 2024-01-26 02:54:30.895973 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml
+-rw-r--r--   0        0        0     4564 2024-01-26 02:54:30.896029 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml
+-rw-r--r--   0        0        0     3751 2024-01-26 02:54:30.896081 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml
+-rw-r--r--   0        0        0     3673 2024-01-26 02:54:30.896173 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml
+-rw-r--r--   0        0        0     2461 2024-01-26 02:54:30.896258 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml
+-rw-r--r--   0        0        0     4528 2024-01-26 02:54:30.896337 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml
+-rw-r--r--   0        0        0     7628 2024-01-26 02:54:30.896400 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml
+-rw-r--r--   0        0        0     1045 2024-01-26 02:54:30.896448 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml
+-rw-r--r--   0        0        0    15694 2024-01-26 02:54:30.896514 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml
+-rw-r--r--   0        0        0     3331 2024-01-26 02:54:30.896581 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml
+-rw-r--r--   0        0        0     3234 2024-01-26 02:54:30.896630 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml
+-rw-r--r--   0        0        0    12147 2024-01-26 02:54:30.896683 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml
+-rw-r--r--   0        0        0    12076 2024-01-26 02:54:30.896738 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml
+-rw-r--r--   0        0        0     4682 2024-01-26 02:54:30.896810 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml
+-rw-r--r--   0        0        0    13539 2024-01-26 02:54:30.896862 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml
+-rw-r--r--   0        0        0    25446 2024-01-26 02:54:30.896941 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml
+-rw-r--r--   0        0        0     1919 2024-01-26 02:54:30.896999 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml
+-rw-r--r--   0        0        0     3445 2024-01-26 02:54:30.897048 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml
+-rw-r--r--   0        0        0     2800 2024-01-26 02:54:30.897097 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml
+-rw-r--r--   0        0        0     3264 2024-01-26 02:54:30.897151 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml
+-rw-r--r--   0        0        0     4324 2024-01-26 02:54:30.897217 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml
+-rw-r--r--   0        0        0     4744 2024-01-26 02:54:30.897278 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml
+-rw-r--r--   0        0        0     6642 2024-01-26 02:54:30.897351 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml
+-rw-r--r--   0        0        0     2399 2024-01-26 02:54:30.897425 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml
+-rw-r--r--   0        0        0    24162 2024-01-26 02:54:30.897508 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml
+-rw-r--r--   0        0        0    25624 2024-01-26 02:54:30.897576 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml
+-rw-r--r--   0        0        0    29018 2024-01-26 02:54:30.897690 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml
+-rw-r--r--   0        0        0    13767 2024-01-26 02:54:30.897747 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml
+-rw-r--r--   0        0        0    13651 2024-01-26 02:54:30.897807 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml
+-rw-r--r--   0        0        0    13651 2024-01-26 02:54:30.897865 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml
+-rw-r--r--   0        0        0    13686 2024-01-26 02:54:30.897943 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml
+-rw-r--r--   0        0        0    14103 2024-01-26 02:54:30.898010 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml
+-rw-r--r--   0        0        0     1285 2024-01-26 02:54:30.898070 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml
+-rw-r--r--   0        0        0     2951 2024-01-26 02:54:30.898153 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml
+-rw-r--r--   0        0        0     3412 2024-01-26 02:54:30.898226 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml
+-rw-r--r--   0        0        0     7592 2024-01-26 02:54:30.898302 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml
+-rw-r--r--   0        0        0     8319 2024-01-26 02:54:30.898368 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml
+-rw-r--r--   0        0        0     4926 2024-01-26 02:54:30.898426 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml
+-rw-r--r--   0        0        0      754 2024-01-26 02:54:30.898498 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml
+-rw-r--r--   0        0        0    14359 2024-01-26 02:54:30.898553 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml
+-rw-r--r--   0        0        0    19829 2024-01-26 02:54:30.898606 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml
+-rw-r--r--   0        0        0     7097 2024-01-26 02:54:30.898680 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml
+-rw-r--r--   0        0        0     6730 2024-01-26 02:54:30.898738 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml
+-rw-r--r--   0        0        0    18555 2024-01-26 02:54:30.898797 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml
+-rw-r--r--   0        0        0    39224 2024-01-26 02:54:30.898882 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml
+-rw-r--r--   0        0        0    16892 2024-01-26 02:54:30.898996 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py
+-rw-r--r--   0        0        0     2823 2024-01-26 02:54:30.899067 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/paths.py
+-rw-r--r--   0        0        0      481 2024-01-26 02:54:30.899145 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/services/__init__.py
+-rw-r--r--   0        0        0     5518 2024-01-26 02:54:30.899210 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py
+-rw-r--r--   0        0        0    26073 2024-01-26 02:54:30.899328 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py
+-rw-r--r--   0        0        0    11691 2024-01-26 02:54:30.899411 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/soap.py
+-rw-r--r--   0        0        0      939 2024-01-26 02:54:30.899466 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnpconstants.py
+-rw-r--r--   0        0        0    56002 2024-01-26 02:54:30.899666 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py
+-rw-r--r--   0        0        0     7467 2024-01-26 02:54:30.899723 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py
+-rw-r--r--   0        0        0     2628 2024-01-26 02:54:30.899768 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnperrors.py
+-rw-r--r--   0        0        0    11247 2024-01-26 02:54:30.899861 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnpfactory.py
+-rw-r--r--   0        0        0    21613 2024-01-26 02:54:30.899968 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py
+-rw-r--r--   0        0        0      494 2024-01-26 02:54:30.900051 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/xml/__init__.py
+-rw-r--r--   0        0        0    20710 2024-01-26 02:54:30.900155 mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py
+-rw-r--r--   0        0        0       67 2024-01-26 02:54:30.900259 mojo_interop-1.3.9/source/packages/mojo/interop/services/common.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.900322 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/__init__.py
+-rw-r--r--   0        0        0        1 2024-01-26 02:54:30.900417 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.900478 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/model/__init__.py
+-rw-r--r--   0        0        0      464 2024-01-26 02:54:30.900540 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/model/summary.py
+-rw-r--r--   0        0        0    13344 2024-01-26 02:54:30.900625 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/model/vm.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.900683 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/specs/__init__.py
+-rw-r--r--   0        0        0     2226 2024-01-26 02:54:30.900746 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/specs/vmcreate.py
+-rw-r--r--   0        0        0     5889 2024-01-26 02:54:30.900827 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/specs/vmhardware.py
+-rw-r--r--   0        0        0      481 2024-01-26 02:54:30.900880 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/specs/vmplacement.py
+-rw-r--r--   0        0        0      314 2024-01-26 02:54:30.900947 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/specs/vmstorage.py
+-rw-r--r--   0        0        0      262 2024-01-26 02:54:30.900997 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/vcenter.py
+-rw-r--r--   0        0        0        1 2024-01-26 02:54:30.901070 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/metasphere/__init__.py
+-rw-r--r--   0        0        0      315 2024-01-26 02:54:30.901117 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/metasphere/vcenter.py
+-rw-r--r--   0        0        0    11195 2024-01-26 02:54:30.901191 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/metasphere/vmguestos.py
+-rw-r--r--   0        0        0     3287 2024-01-26 02:54:30.901262 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/metasphere/vmhardware.py
+-rw-r--r--   0        0        0     2149 2024-01-26 02:54:30.901319 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vmworkstationagent.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.901365 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:30.901424 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/__init__.py
+-rw-r--r--   0        0        0      873 2024-01-26 02:54:30.901492 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/baseext.py
+-rw-r--r--   0        0        0      849 2024-01-26 02:54:30.901556 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/certificatemanagementext.py
+-rw-r--r--   0        0        0      806 2024-01-26 02:54:30.901601 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/clusterext.py
+-rw-r--r--   0        0        0      806 2024-01-26 02:54:30.901647 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/computeext.py
+-rw-r--r--   0        0        0      806 2024-01-26 02:54:30.901688 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/contentext.py
+-rw-r--r--   0        0        0      824 2024-01-26 02:54:30.901735 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/cryptomanagerext.py
+-rw-r--r--   0        0        0     2416 2024-01-26 02:54:30.901795 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/datacenterext.py
+-rw-r--r--   0        0        0     1512 2024-01-26 02:54:30.901838 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/datastoreext.py
+-rw-r--r--   0        0        0      815 2024-01-26 02:54:30.901893 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/deploymentext.py
+-rw-r--r--   0        0        0     3028 2024-01-26 02:54:30.901956 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/folderext.py
+-rw-r--r--   0        0        0      800 2024-01-26 02:54:30.902034 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/guestext.py
+-rw-r--r--   0        0        0     2005 2024-01-26 02:54:30.902084 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/hostext.py
+-rw-r--r--   0        0        0      794 2024-01-26 02:54:30.902127 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/hvcext.py
+-rw-r--r--   0        0        0      809 2024-01-26 02:54:30.902174 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/identityext.py
+-rw-r--r--   0        0        0      812 2024-01-26 02:54:30.902227 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/inventoryext.py
+-rw-r--r--   0        0        0     1734 2024-01-26 02:54:30.902290 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/isoext.py
+-rw-r--r--   0        0        0      794 2024-01-26 02:54:30.902354 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/lcmext.py
+-rw-r--r--   0        0        0      842 2024-01-26 02:54:30.902407 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/namespacemanagementext.py
+-rw-r--r--   0        0        0      815 2024-01-26 02:54:30.902455 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/namespacesext.py
+-rw-r--r--   0        0        0     1152 2024-01-26 02:54:30.902513 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/networkext.py
+-rw-r--r--   0        0        0      794 2024-01-26 02:54:30.902564 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/ovfext.py
+-rw-r--r--   0        0        0      821 2024-01-26 02:54:30.902630 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/resourcepoolext.py
+-rw-r--r--   0        0        0      809 2024-01-26 02:54:30.902681 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/servicesext.py
+-rw-r--r--   0        0        0      806 2024-01-26 02:54:30.902732 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/storageext.py
+-rw-r--r--   0        0        0      821 2024-01-26 02:54:30.902789 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/systemconfigext.py
+-rw-r--r--   0        0        0      805 2024-01-26 02:54:30.902869 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/taggingext.py
+-rw-r--r--   0        0        0      820 2024-01-26 02:54:30.902923 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/tokenserviceext.py
+-rw-r--r--   0        0        0      808 2024-01-26 02:54:30.902978 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/topologyext.py
+-rw-r--r--   0        0        0      847 2024-01-26 02:54:30.903029 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/trustedinfrastructureext.py
+-rw-r--r--   0        0        0     9272 2024-01-26 02:54:30.903080 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/vmext.py
+-rw-r--r--   0        0        0    10881 2024-01-26 02:54:30.903164 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/vsphereagent.py
+-rw-r--r--   0        0        0      781 2024-01-26 02:54:30.903218 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/vspherecoordinator.py
+-rw-r--r--   0        0        0      562 2024-01-26 02:54:30.903282 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/vspherecoordinatorcoupling.py
+-rw-r--r--   0        0        0     1505 2024-01-26 02:54:30.903341 mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/vsphereservice.py
+-rw-r--r--   0        0        0     3605 2024-01-26 02:54:30.903437 mojo_interop-1.3.9/source/packages/mojo/interop/testing/interoptestjob.py
+-rw-r--r--   0        0        0     3849 2024-01-26 02:54:30.903512 mojo_interop-1.3.9/source/packages/mojo/interop/testing/interoptestsequencer.py
+-rw-r--r--   0        0        0     3318 1970-01-01 00:00:00.000000 mojo_interop-1.3.9/setup.py
+-rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 mojo_interop-1.3.9/PKG-INFO
```

### Comparing `mojo_interop-1.3.8/LICENSE.txt` & `mojo_interop-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/pyproject.toml` & `mojo_interop-1.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-interop"
 description = "Automation Mojo Interop Extensions"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
     "Myron Walker <myron.walker@gmail.com>"
 ]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `mojo_interop-1.3.8/source/packages/mojo/factories/mojointeroplandscapingfactories.py` & `mojo_interop-1.3.9/source/packages/mojo/factories/mojointeroplandscapingfactories.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/factories/mojointeroptestplusfactories.py` & `mojo_interop-1.3.9/source/packages/mojo/factories/mojointeroptestplusfactories.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/clientsourcepackager.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/clientsourcepackager.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/ext/commandsext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/ext/commandsext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/ext/configureext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/ext/configureext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/linuxclient.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/linuxclient.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/osx/osxclient.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/osx/osxclient.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/windows/windowsclient.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/windows/windowsclient.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clusters/constants.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clusters/constants.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clusters/raspberrypi/picluster.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clusters/raspberrypi/picluster.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clusters/raspberrypi/pinode.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clusters/raspberrypi/pinode.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinator.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinatorcoupling.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/__init__.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsaddress.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsaddress.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsapi.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsapi.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsconst.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsconst.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnshostinfo.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnshostinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnspointer.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnspointer.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsquestion.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsquestion.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsrecord.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsrecord.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsserver.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsserver.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsservice.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsservice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnstext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnstext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsutil.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsutil.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/dnsvalidation.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/dnsvalidation.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/exceptions.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/mdnsagent.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/mdnsagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/dns/testmessages.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/dns/testmessages.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/serial/tcpserialagent.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/serial/tcpserialagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshagent.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshaspects.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshaspects.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshbase.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshbase.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshconst.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshconst.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshdevice.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshdevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshhelpers.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshhelpers.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/ssh/sshsession.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/ssh/sshsession.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/examples/helloworldtasking.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/examples/helloworldtasking.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/itaskingsequencer.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/itaskingsequencer.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/linux/taskerservice` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/linux/taskerservice`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskeraspects.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskeraspects.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskercontroller.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskercontroller.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskerdaemon.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskerdaemon.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskernode.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskernode.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskerserver.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskerserver.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskerservermanager.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskerservermanager.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskerservice.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskerservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,20 +196,49 @@
             if os.path.exists(folder) and os.path.isdir(folder):
                 exists = True
         finally:
             this_type.service_lock.release()
 
         return exists
 
+    def exposed_get_tasking_progress(self, *, session_id: str, tasking_id: str) -> TaskingResult:
+
+        this_type = type(self)
+
+        progress_str = None
+
+        this_type.service_lock.acquire()
+        try:
+
+            this_type.logger.info("Method 'exposed_get_tasking_progress' was called.")
+
+            session = self._locked_get_session(session_id)
+            
+            this_type.service_lock.release()
+            try:
+                progress_str = session.get_tasking_progress(tasking_id)
+            finally:
+                this_type.service_lock.acquire()
+
+        except:
+            errmsg = traceback.format_exc()
+            this_type.logger.error(errmsg)
+            raise
+
+        finally:
+            this_type.service_lock.release()
+
+        return progress_str
+
 
     def exposed_get_tasking_result(self, *, session_id: str, tasking_id: str) -> TaskingResult:
 
         this_type = type(self)
 
-        result = None
+        result_str = None
 
         this_type.service_lock.acquire()
         try:
 
             this_type.logger.info("Method 'exposed_get_tasking_result' was called.")
 
             session = self._locked_get_session(session_id)
```

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskersession.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskersession.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskersessionref.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskersessionref.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/tasking.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/tasking.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskingadapter.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskingadapter.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskinggroupscope.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskinggroupscope.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/tasker/taskingresultpromise.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/tasker/taskingresultpromise.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/__init__.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/aspects.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/aspects.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/content/didllite.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/content/didllite.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/devices/__init__.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/paths.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/paths.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/soap.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/soap.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnpconstants.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnpconstants.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnperrors.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnperrors.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnpfactory.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnpfactory.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/model/vm.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/model/vm.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/specs/vmcreate.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/specs/vmcreate.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/datastructures/specs/vmhardware.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/datastructures/specs/vmhardware.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/metasphere/vmguestos.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/metasphere/vmguestos.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/metasphere/vmhardware.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/metasphere/vmhardware.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vmworkstationagent.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vmworkstationagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/baseext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/baseext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/certificatemanagementext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/certificatemanagementext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/clusterext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/clusterext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/computeext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/computeext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/contentext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/contentext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/cryptomanagerext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/cryptomanagerext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/datacenterext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/datacenterext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/datastoreext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/datastoreext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/deploymentext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/deploymentext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/folderext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/folderext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/guestext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/guestext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/hostext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/hostext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/hvcext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/hvcext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/identityext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/identityext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/inventoryext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/inventoryext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/isoext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/isoext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/lcmext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/lcmext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/namespacemanagementext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/namespacemanagementext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/namespacesext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/namespacesext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/networkext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/networkext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/ovfext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/ovfext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/resourcepoolext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/resourcepoolext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/servicesext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/servicesext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/storageext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/storageext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/systemconfigext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/systemconfigext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/taggingext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/taggingext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/tokenserviceext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/tokenserviceext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/topologyext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/topologyext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/trustedinfrastructureext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/trustedinfrastructureext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/ext/vmext.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/ext/vmext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/vsphereagent.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/vsphereagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/vspherecoordinator.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/vspherecoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/vspherecoordinatorcoupling.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/vspherecoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/services/vmware/vsphere/vsphereservice.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/services/vmware/vsphere/vsphereservice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/testing/interoptestjob.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/testing/interoptestjob.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/source/packages/mojo/interop/testing/interoptestsequencer.py` & `mojo_interop-1.3.9/source/packages/mojo/interop/testing/interoptestsequencer.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-1.3.8/setup.py` & `mojo_interop-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
  'mojo-xmodules>=1.3.0,<1.4.0',
  'pexpect>=4.8.0,<5.0.0',
  'psutil>=5.9.6,<6.0.0',
  'rpyc>=5.3.1,<6.0.0']
 
 setup_kwargs = {
     'name': 'mojo-interop',
-    'version': '1.3.8',
+    'version': '1.3.9',
     'description': 'Automation Mojo Interop Extensions',
     'long_description': '===============================\nAutomation Mojo Interop Package\n===============================\n\nThis *Automation Mojo Interop Package* contains interop extensions that add interop functionality to\nthe test environment *Landscape* object for a variety of platform clients, clusters, and protocols.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'Myron Walker',
     'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://automationmojo.com',
```

### Comparing `mojo_interop-1.3.8/PKG-INFO` & `mojo_interop-1.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-interop
-Version: 1.3.8
+Version: 1.3.9
 Summary: Automation Mojo Interop Extensions
 Home-page: http://automationmojo.com
 License: LICENSE.txt
 Keywords: python
 Author: Myron Walker
 Author-email: myron.walker@gmail.com
 Requires-Python: >=3.8,<4.0
```

