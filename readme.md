## Usage

run `/usr/lib/arm-linux-gnueabihf/qt5/examples/multimediawidgets/player/player`

## Introduction

stack:

vpu -> mpp -> gstreamer-rk -> qt video

sink:

eglglesisnk for 1080p  
rkximagesink(kms) for 4k

## Build
apt-get build-dep qtmultimedia-opensource-src
#### debug
qmake -r  
make install
#### deb
DEB_BUILD_OPTIONS=nocheck debuild -i -nc -us -uc -b -d  -aarmhf


###

![image](http://doc.qt.io/archives/qt-5.5/images/mediaplayerex.jpg)
