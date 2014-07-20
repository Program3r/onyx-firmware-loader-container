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
* Plug in Onyx geiger counter
* Start Boot2Docker
* Open VirtualBox manager > boot2docker-vm > settings
* Network > Attached to > Bridged Adapter
* USB > Enable USB Controller

Linux
-------------------
* Install Docker
* Re-plug Onyx Devce
* docker run -privileged -v=/dev/bus/usb:/dev/bus/usb -t -rm="true" program3r/onyx-firmware-loader-container:latest



TROUBLESHOOTING
------------------

* Re-plug Onyx Devce
* Start new compiler container
