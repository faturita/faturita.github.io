---
title: "OpenGL/ODE Simulation Platform and Game"
excerpt: "Very old simulation platform"
collection: portfolio
---

![Descriptor](/images/waku.png){:height="450px" width="300px"}

* *Description*: Game and Simulation Engine based on OpenGL and Open Dynamics Engine.  This is the remake of an old game.  It is used as a platform to test AI algorithms.

* *Scope*: A lot to do.

El núcleo y base del proyecto consiste en un Motor Dinámico, es decir, un sistema que resuelve la física de cuerpos.  Esto está hecho con un proyecto que se llama ODE, Open Dynamics Engine, y es lo que permite realizar simulaciones físicas.  La segunda parte linkeada a esto es un motor de juegos básicos con OpenGL en C++: esto son las estructuras de datos para manejar el rendering y el modelo de objetos físicos sumados a un sistema de detección de colisiones. Además tiene un renderización de 3DS con lo cual pueden crear modelos con Blender por ejemplo y cargarlos directamente en el motor.

¿Qué es lo que se puede hacer con esto y hacia dónde se lo puede llevar?

Simulación de física: ODE es un proyecto de simulación física pero hay otros. Los resultados que se pueden obtener son realmente buenísimos, no sólo desde el lado del realismo sino también desde el lado artístico.  Por ejemplo, se puede mejorar el sistema para implementar un simulador de avión realista, por ejemplo, teniendo en cuenta temas de aeronáutica o por ejemplo temas balísticos para representar cómo viaja uno de los cohetes de SpaceX (tipo Kerbal).  

Simulación de fluidos:  En el juego que está montado hay un efecto de agua muy simple hecho con una Textura dibujada en un piso que es de 1000x1000 y que va dezplazando la textura según el movimiento de la cámara.  Hay que hacer un upgrade de eso, por ejemplo implementado esto: https://fluidenginedevelopment.org/ o http://www.lousodrome.net/opengl/index.html.en#water.  Estaría bárbaro implementar olas realistas.

Robótica: es una plataforma genial para probar cosas de robótica, como pueden ser algoritmos de navegación, de SLAM, robots bípedos.  Por ejemplo, vinculandola con esto https://github.com/csiro-robotics/syropod_highlevel_controller.

Inteligencia Artificial:  es una plataforma para hacer pruebas de sistemas multiagentes que operan en un mundo "Real" para probar algoritmos de IA adversariales o colaborativos (como esto pero más realista https://robocode.sourceforge.io/).   

Artístico: Por ejemplo se puede encarar por el lado de simular como es el movimiento del agua, como un barco deja estela. etc.  Abordar temas interesantes de computación gráfica e intentar atacarlos.  Diseños de estructuras 3D y navegación, bounding boxes, colisiones.

El proyecto actual lo pueden encontrar acá:  https://github.com/faturita/wakuseibokan, demo https://www.youtube.com/watch?v=_LJj1x4orbU
Yo lo estuve laburandolo durante la pandemia, ya que encontré algo de espacio para programar.

En concreto, algunas puntas por las que se pueden encarar proyectos con esto

Emprolijar y construir el motor:  optimizar el código, implementar la posibilidad de usar diferentes motores dinámicos (por ejemplo reemplazar ODE por Bullets).  Otra cosa que hay que hacer es actualizar a una versión más nueva de OpenGL porque está un poco vieja la que está, por ejemplo, hay que ponerle Shaders y mejorar el audio.  Acá hay infinito para hacer pero el proyecto puede ser el armado del motor.
Mejorar ODE:  ODE es un proyecto Open Source buenísimo que está un poco abandonado.  Pueden trabajar en ese proyecto implementando mejoras y contribuyendo.
Gaming: pueden usarla como base para construir un juego que quieran.  La base está y si bien hay que mejorarla (programar un juego eficiente es MUY complejo), es algo factible.

Etcetera, etcetera, etcetera....

Que necesitan saber o aprender: C++ y mucho. OpenGL, programación gráfica, algebra lineal aplicada.  Shaders, CUDA, Física, métodos numéricos.  Si eligieron esta carrera por temas de juegos, este es un buen proyecto. Creatividad y ganas de explotarla.

Vista previa del vídeo Wakuseibokan, https://github.com/faturita/wakuseibokan de YouTube


Code 
* <https://github.com/faturita/Wakuseibokan>






