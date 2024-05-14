---
title: "Alignment Algorithm for EEG Signals"
excerpt: "Use Gambini algorithm to create an alignment algorithm for EEG segments"
collection: portfolio
---

## Description

The idea of this proposal is to apply the Gambini method to solve the problem of synchronizing potentials in EEG, such as the P300. It's really exciting because it's a very complex problem. For example, you have three microphones listening to three people talking, so the sources from each person mix in each microphone. This can be separated with ICA, which is a BSS technique. However, due to the sound propagation effect, these sources are not aligned, and a method to align them temporally is needed. That's where the Gambini algorithm comes in. In the paper [MDPI](https://www.mdpi.com/2076-3425/8/11/199/htm), this method is used for experimentation based on pseudo-real EEG records and the creation of sham signals. In fact, we would be using data from 3 subjects (passive) from this dataset, and the P300 signal to inject is precisely derived from this.

* [Frontiers in Computational Neuroscience](https://www.frontiersin.org/articles/10.3389/fncom.2019.00043/full): This paper provides a very detailed explanation of how the Speller operates and how signal averaging works in this context. It even highlights in the conclusions the problem we want to address in this proposal.

* [Code Ocean](https://codeocean.com/capsule/5299343/tree/v2): This is all the code for extracting the P300 signal and injecting the signal into the EEG streams. This is what I am migrating to Python in this repo [Python Nerv](https://github.com/faturita/python-nerv).

* A relevant paper in this line: [ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S1053811910001503)
* Another paper discussing the most used method for this, dynamic time warping: [IEEE](https://ieeexplore.ieee.org/abstract/document/7344551)

* The project where the Matlab code for the "doping" of the signal is located is on the Code Ocean platform for reproducible code: [Code Ocean](https://codeocean.com/capsule/5299343/tree/v2). This site corresponds to the paper and provides all the data used in that paper, the complete code, as well as the published outputs. The DrugEEG.m code is what I am trying to migrate.

* This is implemented in [DrugSignal.py](https://github.com/faturita/python-nerv/blob/master/DrugSignal.py)

* This code, based on this baseline record, ADDS the corresponding signal to the template at the locations corresponding to the moments where the stimuli of the rows and columns corresponding to each letter are. The 7 words are

TOKENMIRARJUJUYMANSOCINCOJUEGOQUESO

* The final idea is to use 3 words to train the classifier and 4 words to determine how well the classifier identifies the letters. Since we are creating the dataset ourselves, the classification should be perfect and should generate exactly these 4 words perfectly (the idea then is to distort the insertion to test methods that correct this distortion).

* Steps:
** Start with this algorithm [DrugSignal.py](https://github.com/faturita/python-nerv/blob/master/DrugSignal.py)
** Once you understand it well, create a noise model, particularly in the latency of the ERP P300 signal. For example, normal noise.
** Implement Juliana's algorithm for unidirectional signals: [Gambini thesis](https://bibliotecadigital.exactas.uba.ar/download/tesis/tesis_n3966_Gambini.pdf)
** Run the Dynamic Time Warping algorithm as an alternative reference.
** See and compare which one gives better results.
** Test this on the ALS patient dataset and see if applying Juliana's adjustment algorithm improves signal identification performance.

* *Technologies*: EEG, MNE








