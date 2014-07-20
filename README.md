Onyx Geiger Counter - Firmware Loader & Devel Compiler in a Container

==============================


CPU TARGETS: 64bit
OS: Linux

INSTRUCTIONS:


Windows / OSX
-------------------
* Run VirtualBox
* Install Ubuntu                            #Pre-built VM will be provided soon.
* Plug in Onyx geiger counter
* Forward USB device to Virtual Machine


Linux
-------------------
* Install Docker
* Re-plug Onyx Devce
* docker run -privileged -v=/dev/bus/usb:/dev/bus/usb -t -rm="true" program3r/onyx-firmware-loader-container



TROUBLESHOOTING
------------------

* Re-plug Onyx Devce
* Start new container
