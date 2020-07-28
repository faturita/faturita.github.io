---
title: "BCI Sift"
excerpt: "P300-Based BCI Speller based on the SIFT Method"
collection: portfolio
---

![Descriptor](/images/SignalWithFullDescriptors3.png){:height="450px" width="300px"}

* *Description*: This system is composed of two parts.  The first one is the platform on OpenVibe which generates stimulations for a P300-Based Speller using the standard 6x6 Farwell and Donchin spelling matrix.  The other part is a program in C++ which reads messages from LSL protocol, process each stimulus, averages signal and sends the selected letter back to the OpenVibe platform.  The C++ program uses OpenCV and VLFeat to generate the images, capture the P300 Wave, classify them using NNBN, and send back the signal to OpenVibe where a program running in Lua captures the message and highlight the selected letter.

* *Scope*: we need to change review the online speller for ALPI


Code 
* [Code Ocean Online Platform](https://codeocean.com/capsule/5299343/tree/v2)
* <https://github.com/faturita/BciSift>
* <https://github.com/faturita/GuessMe>






