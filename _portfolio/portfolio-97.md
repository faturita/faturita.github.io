---
title: "MotorUnitBot"
excerpt: "Yet Another DIY basic 7-DOF Manipulator"
collection: portfolio
---

![Descriptor](https://private-user-images.githubusercontent.com/4692882/373020063-8f4f3449-104d-4db6-9f6a-f1e19bf88006.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3Mjg0MzAyNjMsIm5iZiI6MTcyODQyOTk2MywicGF0aCI6Ii80NjkyODgyLzM3MzAyMDA2My04ZjRmMzQ0OS0xMDRkLTRkYjYtOWY2YS1mMWUxOWJmODgwMDYuanBnP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MTAwOCUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDEwMDhUMjMyNjAzWiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9MjRmNTNiZmU2MzA0N2U0Y2M0YzQ4MWQwODE0ZTE0ZjczNThiNmJmOTkyYTNhYjUxYzg5NjcwNmUxOGJlYTIzNSZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QifQ.rwwCbRFTKgAKzNQrAcO0R_OVwT3GaR0yfB714-poRQk){:height="450px" width="300px"}



## Description

This is a very basic 7-DOF DIY manipulator.  The idea is to test RL scenarios, particularly Meta World Dataset tasks, implemented in the real world.

## Methodology

First complete the basic test bed.  There are several things missing from the manipulator.  For instance, current encoders are very coarse and should be improved in terms of precision.  There are also several aspects of the manipulator that can be improved like the conection between the first joint and the rest of the arm.  The forward and inverse kinematic should be calculated.

## Scope

Improve the maniupulator, train any model on Meta World, and port that into the real manipulator.

## Links
* Repository: https://github.com/faturita/MotorUnitBot
