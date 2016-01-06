Custom OpenWrt Designated Driver Patch For TL-WDR3500/3600/4300/4310/MW4350R
============================================================================

Dependencies
------------

* OpenWRT BuildRoot
* OpenWRT BuildRoot Dependencies
* Java Runtime

How to use
----------

* Install all the development packages required for OpenWrt BuildRoot
* Install Java Runtime
* Clone the Designated Driver Repository

    git clone git://git.openwrt.org/openwrt.git --depth 1

Clone this Repository and copy into the OpenWRT repository

    git clone https://github.com/gwlim/mips74k-designated-driver-patch.git temp --depth 1; mv temp/* openwrt/; rm -rf temp

Change directory into the OpenWrt Repository

    cd openwrt

Run the script

./patch_openwrt.sh

Make Menuconfig and select the Target Profile TP-LINK TL-WDR3500/3600/4300/4310/MW4350R (all the packages and config is inside except build target

    make menuconfig

Save and make

    make V=s
