---
title: 'OpenCV Toolchain for Windows'
date: 2019-05-21
permalink: /posts/2019/05/opencvsetup/
tags:
  - OpenCV
  - CV
  - Windows
---

Guide to install OpenCV 4 toolchain on Windows

# Instalarse Visual Studio 2019 (VC16)

# Download

* Bajarse pkg-config-lite-0.28-1_bin-win32 [Link](https://sourceforge.net/projects/pkgconfiglite/)
* Bajarse GStreamer Developer package [Link](https://gstreamer.freedesktop.org/data/pkg/windows/1.16.0/)

Para GStreamer instalar tanto los MSI de los paquetes DEVEL como el Runtime (el que no se llama devel)

# Agregar los siguientes directorios al PATH (o similares dependiendo donde se hayan instalado)

* C:\path-to-pkg-config\bin
* C:\gstreamer\1.0\x86\lib\gstreamer-1.0 (for gstreamer 1.0)
* C:\gstreamer\1.0\x86\lib (for gstreamer 1.0)

# Agregar la siguiente variable de entorno

* PKG_CONFIG_PATH D:\gstreamer\1.0\x86_64\lib\pkgconfig

# Instalarse [CMake](https://cmake.org/download/)

# Bajarse opencv4.1.0

# Configuración

En este punto hay que levantar la consola de "Developer Command Prompt" de Visual Studio 2019.  Desde ahí puedo chequear que esté seteada la variable %PKG_CONFIG_PATH% para ver si está bien configurada (con "echo %PKG_CONFIG_PATH%).

Luego hay que ejecutar

 cmake-gui
 
que va a levantar la consola de instalación de CMAKE.  

![](https://cdn-images-1.medium.com/max/1600/1*TlmN_r7YOuEwPu5BN4sYcQ.png)

Hay que poner como source el directorio de opencv4 y como build el directorio build dentro de ese directorio (cmake lo crea nuevo).  Hay que poner que se usará "Visual Studio VC16" como entorno.  Hay que darle "Configure" y si todo está ok "Generate".  Es importnate chequear ahí que aparezcan las librerías de GSTREAMER marcadas para compilar.  Si no está marcado GSTREAMER hay que habilitarlo como una opción (WITH_GSTREAMER).

El "Generate" va a generar un archivo de Solution para VS 2019 que se llama "OpenCV".  Hay que abrirlo y darle BUILD_ALL tanto en DEBUG como en RELEASE.   Luego hay que ir al proyecto "CMAKETargets" y buildear también INSTALL.  Esto ejecuta la instalación final de todos los paquetes para poder linkearlos desde otros prosyectos.


# Pasos finales

Agregar todos los directorios al proyecto que uno quiere compilar.  Esto es el directorio de Includes (Additional Include Directories), algo así 

  D:/workspace/opencv-4.1.0/build/install/include/

y el directorio desde donde puede encontrar los libs para linkear (Additional Library Directories)

  D:/workspace/opencv-4.1.0/build/install/x64/vc16/lib

Luego hay que agregar las dependencias de librerías adicionales.  Es la siguiente lista:

opencv_calib3d410.lib
opencv_core410.lib
opencv_dnn410.lib
opencv_features2d410.lib
opencv_flann410.lib
opencv_gapi410.lib
opencv_highgui410.lib
opencv_imgcodecs410.lib
opencv_imgproc410.lib
opencv_ml410.lib
opencv_objdetect410.lib
opencv_photo410.lib
opencv_stitching410.lib
opencv_video410.lib
opencv_videoio410.lib

Finalmente, hay que agregar todas las DLL al directorio donde queda el ejecutable que uno quiere usar (una por cada .lib).   Por último, último, hay que agregar la DLL de gstreamer 1.0.

# Referencias

https://gstreamer.freedesktop.org/documentation/installing/on-windows.html
https://medium.com/@sourabhjigjinni/install-opencv-4-0-0-for-c-windows-7-10-code-blocks-tdm-gcc-64-dff65addf162
https://cvexplorare.wordpress.com/2016/11/15/opencv-gstreamer-windows/
https://stackoverflow.com/questions/29388518/libgstreamer-1-0-0-dll-not-found-gstreamer
https://docs.alfresco.com/4.2/tasks/fot-addpath.html
