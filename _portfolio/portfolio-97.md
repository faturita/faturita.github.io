---
title: "MotorUnitBot"
excerpt: "Yet Another DIY basic 6-DOF Manipulator"
collection: portfolio
---

![Descriptor](/images/motorunit.jpg){:height="450px" width="300px"}

<iframe width="560" height="315" src="https://youtube.com/shorts/53h3F6D1VVU?feature=shared" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## Description

This is a very basic prototype of a 6-DOF DIY manipulator.  It is currently prototyped with aluminium rods from Makeblock.  It has the typical configuration of the old PUMA manipulator. 

* 1st Joint: Vertical, axial with the whole arm. 12 V DC motor with a 20 step encoder.
* 2nd Joint: On X axis, 12 V DC motor with a 20 step encoder. 
* 3rd Joint: On X axis, 12 V Servo.
* 4th Joint: On X axis, 12 V Servo.
* 5th Joint: On Y axis, 6 V DC motor open loop.
* 6th Joint: Gripper, 6 V DC motor open loop.

## Goals

* Manipulator Testbed
* Test Eye-Hand coordination.
* Test RL scenarios, particularly Meta World Dataset tasks, transfered into the real world.

## Methodology

First complete the basic testbed.  There are several things missing from the manipulator.  For instance, current encoders are very coarse and should be improved in terms of precision.  There are also several aspects of the manipulator that can be improved like the connection between the first joint and the rest of the arm. 


## TODO List
* Improve the current motor driver to allow better handling of input messages.
* Improve the motor driver message protocol.
* Put in place the code to handle the frequency update and the reception of the state of the arm.
* Use trajectory planning to update the setpoint for each joint.
* Add IMUs on the end effector.
* Add sensors on the grip to allow better gripping.
* Calculate the forward kinematics and inverse kinematics.
* Build a power source.
* Change completely the mechanics.
* Soft robotics on the grip.
* Use CV from a RPi or Jetson Nano to identify the position of an object and handle the manipulator to pick it up (eye-hand coordination)


## Links
* Repository: https://github.com/faturita/MotorUnitBot
* MetaWorld Challenge: https://meta-world.github.io/
* Related paper: https://arxiv.org/abs/2407.21546
