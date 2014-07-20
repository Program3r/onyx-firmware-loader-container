Safecast Geiger - Container Devel Loader
==============================

A container that compiles the latest devel firmware.


CPU TARGETS: 64bit
OS: Linux




Windows / OSX
-------------------
* Run VirtualBox
* Install Ubuntu                            #Pre-built VM will be provided soon.
* Plug in Safecast geiger counter
* Forward USB device to Virtual Machine


Linux
-------------------
Install Docker

docker run -privileged -v=/dev/bus/usb:/dev/bus/usb -t -rm="true" program3r/safecastgeiger-containerloader
