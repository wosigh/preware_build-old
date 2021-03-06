NAME = $(shell basename $(shell pwd))
TITLE = UberKernel (TouchPad)
DEVICE = touchpad
CATEGORY = Stable
VERSIONS = 3.0.2-93 3.0.4-93 3.0.5-93
APPINFO_DESCRIPTION = A collection of all the best kernel improvements for the HP TouchPad, rolled into a single OTA-safe installation package.<br>\
<b>Note that usage of this package is very likely to <a href=http://developer.palm.com/blog/2010/03/a-statement-on-the-overclocking-patches/>void your warranty</a> if things go wrong.</b><br>\
Current additions include:<ul>\
<li>New 1.8 GHz overclocking support, including voltage selection, ported to the TouchPad by uNiXpSyChO.</li>\
<li>An addition to the standard <b>ondemandtcl</b> governor (known as <b>ondemand-ng</b>) to support <b>screenstate</b> frequency limiting functionality when the screen is off.</li>\
<li>All standard Linux 2.6.35 <a href=http://www.ibm.com/developerworks/linux/library/l-cpufreq-1/index.html>cpufreq governors</a> made available for selection via the Govnah application.</li>\
<li>A new <a href=http://lwn.net/Articles/275978/><b>Budget Fair Queueing (BFQ)</b> IO scheduler</a> made available for selection via the Govnah application.</li>\
<li>New SIO and V(R) IO schedulers.</li>\
<li>Modification of the lowmemnotify threshold calculation to take into account free swap space. This reduces the occurrence of the Too Many Cards error.</li>\
<li>Support for EXT4 filesystems.</li>\
<li>Support for NFS and CIFS (Samba) network filesystems.</li>\
<li>Support for iSCSI and ATA over Ethernet storage network protocols.</li>\
<li>Support for USB Audio.</li>\
</ul><br>\
All additions are controlled by using the Govnah application.<br>\
For more information, visit <a href=${HOMEPAGE}>${HOMEPAGE}</a>
DESCRIPTION = ${APPINFO_DESCRIPTION}<br>${KERNEL_DISCLAIMER}
APPINFO_CHANGELOG = [ \
{ "version" : "${WEBOS_VERSION}-93", "log" : [ "Remove /boot/update-image file left over from OTA update" ] }, \
{ "version" : "${WEBOS_VERSION}-92", "log" : [ "Added USB Audio support" ] }, \
{ "version" : "${WEBOS_VERSION}-91", "log" : [ "Forward ported to webOS 3.0.5 kernel" ] }, \
{ "version" : "${WEBOS_VERSION}-89", "log" : [ "Added 1.8 GHz overclocking support" ] }, \
{ "version" : "${WEBOS_VERSION}-88", "log" : [ "Added EXT4, iSCSI and ATA over Ethernet support", "Added BFQ, SIO and V(R) I/O schedulers" ] }, \
{ "version" : "${WEBOS_VERSION}-68", "log" : [ "Added TMC error fix" ] }, \
{ "version" : "${WEBOS_VERSION}-52", "log" : [ "Added UTF8 support" ] }, \
{ "version" : "${WEBOS_VERSION}-36", "log" : [ "Added NFS and CIFS support" ] }, \
{ "version" : "${WEBOS_VERSION}-22", "log" : [ "Added BFQ IO scheduler support" ] }, \
{ "version" : "${WEBOS_VERSION}-20", "log" : [ "Added 1.5 GHz overclocking support" ] }, \
{ "version" : "${WEBOS_VERSION}-8", "log" : [ "Initial version" ] }, \
]
CHANGELOG = \
${WEBOS_VERSION}-93: Remove /boot/update-uimage file left over from OTA update.<br>\
${WEBOS_VERSION}-92: Added USB Audio support.<br>\
${WEBOS_VERSION}-91: Forward ported to webOS 3.0.5 kernel.<br>\
${WEBOS_VERSION}-89: Added 1.8 GHz overclocking support.<br>\
${WEBOS_VERSION}-88: Added EXT4, iSCSI and ATA over Ethernet support. Added BFQ, SIO and V(R) I/O schedulers. <br>\
${WEBOS_VERSION}-68: Added TMC error fix.<br>\
${WEBOS_VERSION}-52: Added UTF8 support.<br>\
${WEBOS_VERSION}-36: Added NFS and CIFS support.<br>\
${WEBOS_VERSION}-22: Added BFQ IO scheduler support.<br>\
${WEBOS_VERSION}-20: Added 1.5 GHz overclocking support.<br>\
${WEBOS_VERSION}-8: Initial version.

HOMEPAGE = http://www.webos-internals.org/wiki/Application:UberKernel

KERNEL_GIT = git://github.com/rwhitby/webos-uber-kernel.git
KERNEL_TAG = uber-${VERSION}

TYPE = Kernel

include ../../support/kernel.mk
