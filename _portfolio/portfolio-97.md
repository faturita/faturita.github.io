---
title: "MotorUnitBot"
excerpt: "Yet Another DIY basic 6-DOF Manipulator"
collection: portfolio
---

![Descriptor](/images/motorunit.jpg){:height="450px" width="300px"}


## Description

This is a very basic 6-DOF DIY manipulator.  It is currently prototyped with aluminium rods from Makeblock.  It has the typical configuration of the old PUMA manipulator. 

* 1st Joint: Vertical, axial with the whole arm. 12 V DC motor with a 20 step encoder.
* 2nd Joint: On X axis, 12 V DC motor with a 20 step encoder. 
* 3rd Joint: On X axis, 12 V Servo.
* 4th Joint: On X axis, 12 V Servo.
* 5th Joint: On Y axis, 6 V DC motor open loop.
* 6th Joint: Gripper, 6 V DC motor open loop.

## Goals

* Testbed
* Test RL scenarios, particularly Meta World Dataset tasks, implemented in the real world.

## Methodology

First complete the basic testbed.  There are several things missing from the manipulator.  For instance, current encoders are very coarse and should be improved in terms of precision.  There are also several aspects of the manipulator that can be improved like the connection between the first joint and the rest of the arm. 

## Scope

Improve the maniupulator, train any model on Meta World, and port that into the real manipulator.

## Links
* Repository: https://github.com/faturita/MotorUnitBot
