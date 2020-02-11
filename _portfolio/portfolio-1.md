---
title: "BCI Sift"
excerpt: "P300-Based BCI Speller based on the SIFT Method"
collection: portfolio
---

![Descriptor](images/SignalWithFullDescriptors3.png){:height="450px" width="300px"}

* Description: The system is composed of two parts.  The first on is the platform on OpenVibe which generates stimulations for a P300-Based Speller using the standard 6x6 Farwell and Donchin spelling matrix.  The other part is a program in C++ which reads messages from LSL protocol, process each stimulus, averages signal and sends the selected letter back to the OpenVibe platform.

* Scope: we need to change the spelling matrix to RSVP paradigm.

Code 
* https://github.com/faturita/BciSift
* https://github.com/faturita/GuessMe






