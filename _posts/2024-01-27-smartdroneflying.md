---
title: 'Smart Drone Flying'
date: 2024-01-26
permalink: /posts/2024/01/smartdroneflying/
tags:
  - mobile
---

How to use and program AR Parrot 2 to impress your friends 😎.

# Smart Drone Flying

The Parrot ARDrone 2 is a piece of oustanding device.  However, its library sucks.

If we want to do smart flying we need to use an open source better python library.

# The probably-best library for ardrone.

Ardone-webflight is based on the nodecopter library:http://eschnou.github.io/ardrone-webflight/

This is an awesome library on nodejs.

You can install OpenCV for Node or you can also 
 
 https://www.npmjs.com/package/opencv

Or you can link node with python with:
 
 https://www.npmjs.com/package/node-python

# Streaming

Parrot Ar Drone streams in h.264, but not many libraries can deal with the video stream.

So, if you want to do it by hand:
 https://pypi.python.org/pypi/ffmpy/0.0.4
 https://github.com/Ch00k/ffmpy/blob/master/tests/test_all.py
 http://sourceforge.net/p/ps-drone/discussion/general/thread/dc620cd0/
 http://zulko.github.io/blog/2013/09/27/read-and-write-video-frames-in-python-using-ffmpeg/
 http://stackoverflow.com/questions/25782600/sending-video-stream-from-server-to-client-using-socket-programming-in-python
 http://www.renevolution.com/how-to-install-ffmpeg-on-mac-os-x/
 https://github.com/Sanderi44/AR-Drone-Fire-Detection/blob/master/videocontrol.py
 http://stackoverflow.com/questions/26691189/how-to-capture-video-stream-with-opencv-python

What in generally works is:

```bash
 ffmpeg -f rawvideo -i tcp://192.168.1.1:5555 -c:v h264
```

```bash
 ffplay -framedrop -infbuf -f h264 -i http://192.168.1.1:5555 -framerate 60
```

For IP Camera:

```bash
 ffmpeg -f mjpeg -i "http://192.168.0.3:80/cgi-bin/fwstream.cgi?.mjpg&FwModId=0&PortId=0&PauseTime=0&FwCgiVer=0x0001" output.mp4
```

## Ar Drone Fire Detection
Another very interesting project wich actually uses the python library:

 https://github.com/Sanderi44/AR-Drone-Fire-Detection

## Ardrone For Processing

 http://kougaku-navi.net/ARDroneForP5/index_en.html

## More libraries

 https://pervasive297.wikispaces.com/drone

## Paparazzi Project
Paparazzi is a project from DU Delft university to replace the firmware of the AR Drone Parrot with a new customized open source firmware.

 http://wiki.paparazziuav.org/wiki/AR_Drone_2/getting_started

## Build OpenCV 3 on MacOSX for python 2.7

So far, the best solution is to use OpenCV3 with Python 2.7, using the libardrone library.  The `VideoCapture('http...')` function can be used and it can analyze on real time the drone stream.

Activate your virtual environment: 
 source cv/bin/activate

Deactivate it 
 deactivate
 
Virtualenvironment wrapper
 source /usr/local/bin/virtualenvwrapper.sh
 workon cv

The procedure is described here:  http://www.pyimagesearch.com/2015/06/15/install-opencv-3-0-and-python-2-7-on-osx/

Remember to install FFMPEG before you compile OpenCV so that you can easily access to the drone stream.

```bash
export FFMPEG_INCLUDE_DIR=/usr/local/Cellar/ffmpeg/3.1.4/include/
export FFMPEG_LIB_DIR=/usr/local/Cellar/ffmpeg/3.1.4/lib/


cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local \
	-D PYTHON2_PACKAGES_PATH=~/.virtualenvs/cv/lib/python2.7/site-packages \
	-D PYTHON2_LIBRARY=/usr/local/Cellar/python/2.7.11/Frameworks/Python.framework/Versions/2.7/lib/ \
	-D PYTHON2_INCLUDE_DIR=/usr/local/Frameworks/Python.framework/Headers \
	-D INSTALL_C_EXAMPLES=OFF -D INSTALL_PYTHON_EXAMPLES=ON \
	-D FFMPEG_LIB_DIR=/usr/local/Cellar/ffmpeg/3.1.4/include/ \
	-D FFMPEG_INCLUDE_DIR=/usr/local/Cellar/ffmpeg/3.1.4/include/ \
	-D BUILD_EXAMPLES=ON \
	-D OPENCV_EXTRA_MODULES_PATH=~/work/opencv_contrib/modules ..
```

 http://www.marinamele.com/2014/07/install-python3-on-mac-os-x-and-use-virtualenv-and-virtualenvwrapper.html
 http://docs.python-guide.org/en/latest/dev/virtualenvs/
 http://www.bogotobogo.com/python/OpenCV_Python/python_opencv3.php
 http://www.bogotobogo.com/OpenCV/opencv_3_tutorial_ubuntu14_install_cmake.php
 http://www.pyimagesearch.com/2015/06/15/install-opencv-3-0-and-python-2-7-on-osx/


