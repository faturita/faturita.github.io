---
title: "Alignment Algorithm for EEG Signals"
excerpt: "Use Gambini algorithm to create an alignment algorithm for EEG segments"
collection: portfolio
---

* *Description*: La idea de esta propuesta es aplicar el método de Gambini para resolver el problema de la sincronización de los potenciales en EEG como el del P300.  Es algo copadísimo porque es un problema muy rico.  Por ejemplo, tenes tres microfonos que escuchan a tres personas hablar, entonces esas tres fuentes de cada persona se mezcla en cada micrófono.  Eso se puede separar con ICA que es una técnica de BSS.   Pero por el efecto de propagación del sonido, en realidad esas fuentes no están alineadas y haría falta encontrar un método para alinearlas temporalmente.  Ahí entraría otra vez el algoritmo de Gambini.  En el paper  https://www.mdpi.com/2076-3425/8/11/199/htm, este paper tiene el método para realizar la experimentación en base a los registros de EEG pseudo-reales y al armado de sham signals.  De hecho estaríamos usando datos de 3 sujetos (pasivos) de este dataset y la señal de P300 a inyectar es justamente la que surge de esto.

* https://www.frontiersin.org/articles/10.3389/fncom.2019.00043/full: Este paper por otor lado tiene la explicación muy detallada de cómo opera el Speller y cómo opera en ese sentido el averaging de las señales.  Incluso se señala en conclusiones el problema que justamente nosotros queremos abordar en esta propuesta.

* https://codeocean.com/capsule/5299343/tree/v2: este es todo el código que hace la extracción de la señal de P300 y la inyección de la señal en los streams de EEG.  Esto es lo que estoy migrando a python a este repo https://github.com/faturita/python-nerv

* Este sería un paper que estaría en esta linea: https://www.sciencedirect.com/science/article/abs/pii/S1053811910001503
* Este es otro paper que habla sobre el método más utilizado para esto, dynamic time warping: https://ieeexplore.ieee.org/abstract/document/7344551


* El proyecto donde está el código en Matlab que hacía el "drogado" de la señal está en la plataforma Code Ocean de código reproducible: https://codeocean.com/capsule/5299343/tree/v2.   Este sitio es el que corresponde al paper y el que disponibiliza todos los datos que se usan en ese paper, todo el código completo, así como también las salidas publicadas en ese paper.   El código DrugEEG.m es el que estoy tratando de migrar.

* Eso mismo está implementado en https://github.com/faturita/python-nerv/blob/master/DrugSignal.py

* Ese código en base a este registro basal, AGREGANDO la señal correspondiente al template en las localizaciones que corresponden a los momentos donde están los estímulos de las filas y las columnas que corresponden a cada letra.  Las 7 palabras son

TOKENMIRARJUJUYMANSOCINCOJUEGOQUESO

* La idea al final es usar 3 palabras para entrenar al clasificador, y usar 4 palabras para determinar cuán bien o no el clasificador acierta las letras.  Como el dataset lo estamos armando nosotros, la clasificación tiene que dar perfecta y debería generar exactamente esas 4 palabras perfecta (la idea después es distorsionar la inserción para justamente probar métodos que corrijan esa distorsión).


* 1-Arrancas con este algoritmo https://github.com/faturita/python-nerv/blob/master/DrugSignal.py
* 2- Una vez que lo entiendas bien, planteas un modelo de rúido sobre todo en latencia de la señal de ERP del P300.  Por ejemplo, ruído normal.
* 3- Implementás el algoritmo de Juliana para señales unidireccionales.  https://bibliotecadigital.exactas.uba.ar/download/tesis/tesis_n3966_Gambini.pdf
* 4- Corrés el algoritmo de Dynamic Time Warping como una referencia alternativa.
* 5- Ves y comparas cual de los dos te da mejor.
* 6- Probas eso sobre el dataset que te comenté de los pacientes de ALS y ves si aplicando el algoritmo de ajuste de Juliana obtenes una mejor performance en la identificación de las señales.

* *Technologies*: EEG, MNE








