Onyx Geiger Counter - Firmware Loader & Devel Compiler in a Container

==============================


REQUIREMENTS:
==========================

CPU: x64 + Virtualization

OS: Linux / Windows / OSX





INSTRUCTIONS:
==========================

Windows / OSX
-------------------
* Download Boot2Docker -- http://boot2docker.io/   (This will restart system after install)
* Install Boot2Docker -- Custom Installation > Boot2Docker + VirtualBox (if missing) > Install Devices > Restart
* Open VirtualBox manager
* Start Boot2Docker
* * Open VirtualBox manager > boot2docker-vm > STOP (if running)
* Open VirtualBox manager > boot2docker-vm > settings
* Network > Attached to > Bridged Adapter (optional)
* USB > Enable USB Controller > ADD (Green + Sign) > FTDI FT232R USB UART > OK
* Close Boot2Docker Application
* VirtualBox manager > boot2docker-vm > start
* Wait for boot
* Un-lock Onyx geiger counter (switch on back)
* Plug in Onyx geiger counter
* Open boot2docker-vm

Linux
-------------------
* Install Docker - https://docs.docker.com/installation/

Docker
-------------------
* Re-plug Onyx Devce
* docker run -privileged -v=/dev/bus/usb:/dev/bus/usb -t -rm="true" program3r/onyx-firmware-loader-container:latest

Afterward
-------------------
* Scream "It's Alive!"

UPDATING
==========================
* VirtualBox manager > boot2docker-vm > start
* Open boot2docker-vm
* Plug In Onyx Devce
* docker run -privileged -v=/dev/bus/usb:/dev/bus/usb -t -rm="true" program3r/onyx-firmware-loader-container:latest
* Scream "It's Alive!"

TROUBLESHOOTING
==========================

Won't Upload Firmware?
* Re-plug Onyx Devce
* Start new compiler container

Onyx not showing in VirtualBox?
* Download VirtualBox -- https://www.virtualbox.org/wiki/Downloads
* Shut off all programs
* Install VirtualBox

Too much radiation exposure?
* Get out of the immediate area quickly.
* Remove your outer layer of clothing.
* Place clothing in a plastic bag or away from others.
* Wash all exposed parts of your body.
* Internal contamination may call for medical attention.
#SOURCE - CDC     http://www.bt.cdc.gov/radiation/contamination.asp
