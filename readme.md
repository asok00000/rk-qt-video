## Usage

run `/usr/lib/arm-linux-gnueabihf/qt5/examples/multimediawidgets/player/player`

You can click the bottom right corner to switch between eglglesisnk(gpu) and rkximagesink(drm)

## Introduction
This is qtmultimedia's rockchip version to support gstreamer-rk

The video stack is:
vpu -> mpp -> gstreamer-rk -> qtmultimedia -> player

## Build
apt-get build-dep qtmultimedia-opensource-src
#### debug
qmake -r  
make install
#### deb
DEB_BUILD_OPTIONS=nocheck debuild -i -nc -us -uc -b -d  -aarmhf

