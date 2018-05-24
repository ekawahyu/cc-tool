#cc-tool version 0.26
cc-tool provides support for Texas Instruments CC Debugger

# Project home:
http://sourceforge.net/projects/cctool/

# Building from source, dependencies:

* Ubuntu: `libusb-1.0`, `libboost-all-dev` 
* Fedora: `boost-devel`, `libusb1-devel`
* Mac OS 10.6.7, from ports: `libusb`, `boost`, `pkgconfig`

# Mac OS Build Guide

Install:

* Xcode (Mac App Store)
* [Homebrew](https://brew.sh/) 

Clone repo, `cd` to its folder then:

```
brew install boost
brew install libusb
./configure
./make
```

# User guide:
```
man cc-tool
```
# Additional:

File `udev/90-cc-debugger.rules` contains udev rules changing permissions 
for TI CC Debugger device and TI evolution boards so they can be used 
from non-privileged accounts. Copy it to `/etc/udev/rules.d`

# Support:

Send bug/build problem reports, new feature or new chip support suggestions 
to `george-u@yandex.com`  

If you found a bug try to reproduce it with command line option `--log` and
send the log file along with the problem description.
