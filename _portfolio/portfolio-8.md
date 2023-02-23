---
title: "OpenGL/ODE Simulation Platform and Game"
excerpt: "Very old simulation platform"
collection: portfolio
---

![Descriptor](/images/waku.png){:height="450px" width="300px"}

## Description

Game and Simulation Engine based on OpenGL and Open Dynamics Engine (ODE).  This is the remake of an old game.  It is used as a platform to test AI algorithms, Robotics, Dynamics, and so on.

## Scope

A lot to do.

This game, and humble, simulation engine was creating on top of OpenGL 1.x (before Shaders).  The good think about this opengl version is that it is used, even currently, as basis of the visual interface of major operating systems like linux (Gnome and KDE) and Mac OSX.  Hence, it is still supported and, and the same time, it is super compatible for all the most important platforms.

Additionally, this version of opengl is super easy to use, and helps to understand better what is actually under the hood of graphics programming (if you want to go even deeper you can try https://machinethink.net/blog/3d-rendering-without-shaders/).

The other part of the engine is the open dynamics engine.  This allows to perform physical simulations of objects in 3D space.  This engine also has a very extensible collision engine and a fairly good library to process 3DS digital files that can be easily created in Blender.

### What can be done?

* Physics Simulation:  ODE is a physics simulation but there are others.  ODE solves one part of the problem, the rigid body dynamics, but there are much more things that can be fixed.  For instance, ODE has a limited set of connectors that can be extended to have more, and that sometimes are faulty.  Another thing that could be interested to work with is simulation of ballistic scenarios aiming to have something that what Kerbal does with rockets.

* Fluid Mechanics simulations:  It will be super nice to add a new layer to perform fluid dynamics simulations (for the ships, the speeders, the airplanes, everything).  These frameworks can be used to do so https://fluidenginedevelopment.org/ o http://www.lousodrome.net/opengl/index.html.en#water. 

* Robotics: this is an excellent platform to test any kind of robotics problem, like path planning, navigation, SLAM, walking robots, bipedal robots and so on. It can be linked with https://github.com/csiro-robotics/syropod_highlevel_controller.

* Artificial Intelligence:  this is an excellent platform to test artificial intelligence concepts like multiagents systems coordination that play in a controlled but real-like world. Something in the line of  https://robocode.sourceforge.io/ but extending it a little bit more (like two tanks that need to fight one against the other).

* Art: for instace how the water actually moves, how the wake of a boat is generated.  It can also include computer graphics problems like bounding boxes, colisions, 3D structures.


Project: https://github.com/faturita/wakuseibokan, 
Videos: https://www.youtube.com/watch?v=_LJj1x4orbU


# Requirements

OpenGL, CUDA, computer graphics, algebra, physics, numerical methods, fluid mechanics, navier-stokes equation (i am joking)

# Videos

* https://www.youtube.com/playlist?list=PLJHMIS4ekxNSLS422Nw7D2JlJW3En1Vul


# Code 
* https://github.com/faturita/Wakuseibokan






