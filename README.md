# Backup of pirate loader

The Bus pirate is an amazing piece of software that I have used many times over the years. The main problem for me is the documentation and
website of http://dangerousprototypes.com. I get lost and confused. Back a few year ago I upgraded my bus pirate and again today. It is really
easy if you can find the pirate loader. It is hidden somwhere on https://code.google.com/archive/p/dangerous-prototypes-open-hardware/downloads.

Today (december 2018) I downloaded the whole source archive from there and "managed" to find the code "hidden" in trunk/Bus_Pirate/BPv4-bootloader/pirate-loader and was able to flash my bus pirate v3 with new firmware. 

* Get the lasted firmware from git@github.com:mikebdp2/Bus_Pirate.git (Bus_Pirate/package_latest)
* build the software in this directory (make) to get pirate-loader_lnx
* Put the device into bootloader mode ($) on "recent" firmware (else boot with the programming pins into bootloader mode)
* Flash ./pirate-loader_lnx --dev=/dev/ttyUSB0 --hex=~/projects/Bus_Pirate/package_latest/BPv3/bpv3_fw7.0_opt0_18092016.hex


http://dangerousprototypes.com/blog/2010/01/22/how-to-firmware-upgrades-with-the-linux-mac-windows-console/
http://dangerousprototypes.com/docs/Pirate-Loader_console_upgrade_application_%28Linux,_Mac,_Windows%29
