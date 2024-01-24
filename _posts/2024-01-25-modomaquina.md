---
title: 'Aprendizaje Modo Maquina'
date: 2024-01-25
permalink: /posts/2024/01/modomaquina/
tags:
  - mobile
---

* [El Drive de ML](https://drive.google.com/file/d/1sJvLQwxMyu89t2z4Zf9tD7O7efnbIUyB/view)


# Preliminares
* [Mathematics for Machine Learning de Garret Thomas](https://gwthomas.github.io/docs/math4ml.pdf): Excelente Resumen paso a paso de matemáticas para ML.  Esto sirve para aquellos que busquen un repaso de algebra lineal, calculo multivariado, proba, etc.
* [Mathematics for Machine Learning, Diesendorth](https://mml-book.github.io/): Idem anterior, un poco más formal.  Hiper actualizado.
* [Introduction to Applied Linear Algebra](https://www.amazon.com/Introduction-Applied-Linear-Algebra-Matrices/dp/1316518965):  algebra lineal aplicada, con foco en las técnicas que se usan en ML. 
* [A beginner guide to neural network mathematics](https://nms.kcl.ac.uk/ton.coolen/published/1998/summerschool98.pdf):  Detrás del aprendizaje en las redes neuronales, están las ténicas de optimizació.  Este libro tiene todo lo que hace falta para entender esas técnicas de optimización detrás de las redes neuronales.
* [Linear algebra for Computer Vision](https://www.seas.upenn.edu/~cis515/linalg-I.pdf): Extraordinario resumen de la matemática que se usa en CV.
* Linear algebra and optimization for machine learning(Charu Aggarwal): Buenísimo libro, el autor es hiper didáctico.



## Algunos temas de matemáticas específicos
* [Multiplicadores de Lagrange](https://www.alexirpan.com/2019/07/27/lagrange-multipliers.html): Resolución de sistemas de ecuaciones que se usa para Optimización.
* [Harmonic Analysis and Representation Theory](http://www.cis.upenn.edu/~jean/nc-harmonic.pdf): Generalización de análisis de fourier y resolución de ODEs con series armónicas.
* [Differential Theory and Lie Groups](https://www.seas.upenn.edu/~jean/diffgeom-spr-II.pdf)

# Deep Learning
* [2010 !](http://people.idsia.ch/~juergen/2010-breakthrough-supervised-deep-learning.html): 2010 Breakthrough of supervised learning
* https://arxiv.org/pdf/1906.01615.pdf   Automata representation
* https://blog.acolyer.org/2016/03/09/neural-turing-machines/   Turing Neural Networks


# Python ML
* **Python Crash Course**: Intro a programación en python.  Para el que no sabe nada, sirve.
* **Guide to Numpy**: Intro a programación con tensores.  Es un libro muy bueno, derivado de la propia documentación de Numpy.  Hay que estar más canchero con lo básico de python para sacarle más provecho.
* **SciPy and Numpy An Overview**: Intro a ML usando Python.  Este libro tiene ejemplos muy concretos de escenarios de soluciones de ML (por ejemplo, un detector de Spam).
* **Fluent Python 3**: Este libro es avanzado en python.  Es interesante para profundizar en el conocimiento del lenguaje y su aplicación a Data Science.
* **A Primer on Scientific Programming with Python**:  Intro a programación científica con Python, es un "Numerical Recipes" con python.
* **Learning Scientific Programming with python**:  Programación científica con Python, similar al anterior.
* **The Art of R programming**: recetas en R para ML
* **Python Machine Learning**: se puede descargar de [aca](https://github.com/rasbt/python-machine-learning-book-2nd-edition).  ML desde una perspectiva de un programador python.
* **Python Data Visualization**: Visualizaciónes con python
* **Practical Time Series Analysis**: Hands on, para trabajar con series de tiempo con keras.
* **Learning the Pandas Library**: Muy bueno para aprender los detalles de la cocina de datos con Pandas.
* **Python for Data Analysis**: Muy bueno también, actualizado y práctico.


# Libros de ML: 
* **Machine Learning in Action by Harrington**: Muy accesible, tipo cookbook. Bueno para empezar paso a paso.
* **Breaking Data Science Open**: Intro general a Data Science.  Este libro es bueno para tener letra para converser a un CEO de alocar presupuesto para el area.
* **Machine Learning, de Tom Mitchel**: Clásico de Ml.  Es el textbook sobre el tema (un poco outdated hoy por hoy).
* **Dive Into Deep Learning**, [aca](http://d2l.ai/).  Excelente libro sobre Deep Learning.
* **Generative Deep Learning Models, David Foster**: Este libro es muy nuevo, y tiene varias recetas y explicaciones sobre cómo implementar redes neuronales generativas.
* **The Elements of Statistical Learning**: Excelente libro para entender cuál es el ataque de Análisis Multivariado a ML.
* **Data Mining and Analysis: Fundamental Concepts and Algorithms, Zaki**: técnicas no supervisadas de clusterización.  Es un excelente libro compendio con muchos detalles de algoritmos de reducción de dimensionalidad.
* **Neural Networks and Deep Learning, Aggarwal**: Un exquisito compendio de Deep Learning con muy buenas bases matemáticas.

## Solid stuff

* **Good rules to remember while publishing ML info on other journals**: https://journals.aps.org/prfluids/pdf/10.1103/PhysRevFluids.6.070001
* **A guide to Convolution Arithmetic for CNN** *: Guía sobre las transposiciones de tensores en CNN.
* **Extracting knowledge from Time Series**: Modelado científico, específico para series de tiempo.  Uno de los mejores libros para entender la epistemología de todo esto. Es ruso.
* **Handbook of Blind Source Separation**: técnicas no supervisadas para separar diferentes fuentes.  Mejorar señal-ruido o separar señales que están mezcladas.
* **The Nature of Statistical Learning Theory**: introduce de una excelente manera, Learning Theory (SVM surgió acá).
* **Methods for Statistical Data Analysis of Multivariate Observations**: Análisis multivariado.
* **Practical Nonparametric and Semiparametric Bayesian Statistics**: Análisis estadístico de redes neuronales
* **Regularization**: https://towardsdatascience.com/understanding-the-scaling-of-l%C2%B2-regularization-in-the-context-of-neural-networks-e3d25f8b50db and http://bjlkeng.github.io/posts/probabilistic-interpretation-of-regularization/


# Papers: 

Estos papers son muy buenos para entender algunas ideas de ML que te permiten bajar un poco a la tierra del tema, desmitificarlo.

* https://people.idsia.ch/~juergen/scientific-integrity-turing-award-deep-learning.html
* Array programming with Numpy: Porque razón Numpy es tan importante https://www.nature.com/articles/s41586-020-2649-2
* Game of life is hard to learn for NN: https://arxiv.org/abs/2009.01398
* The Hardware Lottery:  Al final todo se somete a una suerte de que el hardware para realizar el procesamiento requerido finalmente estuvo disponible https://arxiv.org/abs/2009.06489
* Schmidhuber Paper Review de Deep Learning super completa: https://www.sciencedirect.com/science/article/abs/pii/S0893608014002135
* Anthony Zador, "A critique of pure learning" https://www.nature.com/articles/s41467-019-11786-6.  This paper is so great: contains many references, explain learning from a biological viewpoint, and has so many eastern eggs and jokes.
* LeCun, Yann, Yoshua Bengio, and Geoffrey Hinton. "Deep learning." nature 521.7553 (2015): 436.
* What does it mean to understand a neural network?, https://arxiv.org/abs/1907.06374
* A few useful things to know about Machine Learning, Pedro Domingos.
* On the Surprising Behaviour of Distance Metrics in High Dimensional Space, Aggarwal
* Do really Machine Learning machines learn, Bringsjord
* Este es el paper que introduce SVM: "Support Vector Networks" https://link.springer.com/content/pdf/10.1007/BF00994018.pdf
* Learning a Mahalanobis Distance Metric for Data Clustering and Classification, Xiang
* Ten quick tips for dimensionality reduction, https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006907
* Breaking the curse of dimensionality http://jmlr.org/papers/volume18/14-546/14-546.pdf
* Crítica de Deep Learning de Gary Marcus: https://arxiv.org/pdf/1801.00631.pdf
* Compendio, resumen, excelente paper de Terrence Sejnowski (presidiente de NIPS): https://www.pnas.org/content/early/2020/01/23/1907373117.short
* Estupendo: https://www.forbes.com/sites/robtoews/2021/06/01/what-artificial-intelligence-still-cant-do
* https://www.scientificamerican.com/article/will-artificial-intelligence-ever-live-up-to-its-hype/
* https://spectrum.ieee.org/the-institute/ieee-member-news/stop-calling-everything-ai-machinelearning-pioneer-says
* https://spectrum.ieee.org/view-from-the-valley/artificial-intelligence/machine-learning/andrew-ng-xrays-the-ai-hype
* https://arxiv.org/pdf/2104.12871.pdf
* https://www.nature.com/articles/s41467-019-11786-6
* https://www.technologyreview.com/2017/04/11/5113/the-dark-secret-at-the-heart-of-ai/
*  https://arxiv.org/abs/1911.01547
* https://www.forbes.com/sites/robtoews/2021/06/01/what-artificial-intelligence-still-cant-do
* A la AI le da el piné?: https://www.scientificamerican.com/article/will-artificial-intelligence-ever-live-up-to-its-hype/, "They will always remain mere machines [refiriéndose a los programas de IA]. That’s my guess, and my hope." ?
* Stop calling everything AI de Michael Jordan:  este autor que se llama como el famoso basquetbolista, es una figura de enorme renombre en Aprendizaje Automático.  Es uno de los creadores de "Inferencia Variacional", algo que vamos a ver brevemente en la parte de Deep Learning: https://spectrum.ieee.org/the-institute/ieee-member-news/stop-calling-everything-ai-machinelearning-pioneer-says
* Andrew Ng X-Rays the AI Hype:   Andrew Ng es uno de los dueños de Coursera, figura super reconocida en Deep Learning (fue alumno de doctorado de Michael Jordan): https://spectrum.ieee.org/view-from-the-valley/artificial-intelligence/machine-learning/andrew-ng-xrays-the-ai-hype
* Why AI is so difficult ?: de Melanie Mitchel, una referente en sistemas complejos y algoritmos genéticos: https://arxiv.org/pdf/2104.12871.pdf
* A critique of pure learning and what artificial neural networks can learn from animal brains. de Anthony Zador (biólogo neurocientista): https://www.nature.com/articles/s41467-019-11786-6
* The dark secret at the heart of AI: https://www.technologyreview.com/2017/04/11/5113/the-dark-secret-at-the-heart-of-ai/, El problema de la inteligibilidad en redes neuronales artificiales.
* Estupendo compendio de las limitaciones actuales de la IA:  https://www.forbes.com/sites/robtoews/2021/06/01/what-artificial-intelligence-still-cant-do

## Last mile

* https://arxiv.org/pdf/1808.01531v2.pdf GAN convergence
* Intro a Reinforcement Deep Learning: https://arxiv.org/pdf/1811.12560.pdf
* Deep Learning alternative framework http://caffe.berkeleyvision.org/

# Tips

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">A 1 hidden layer perceptron can approximate arbitrary continuous functions using a large enough number of neutrons (Cybenko&#39;s theorem). <a href="https://t.co/rS2X93GBib">https://t.co/rS2X93GBib</a> <a href="https://t.co/nCZDqgZV2g">https://t.co/nCZDqgZV2g</a> <a href="https://t.co/1hVRrgv6n5">pic.twitter.com/1hVRrgv6n5</a></p>&mdash; Gabriel Peyré (@gabrielpeyre) <a href="https://twitter.com/gabrielpeyre/status/1304645917648269312?ref_src=twsrc%5Etfw">September 12, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">covariance vs. mutual information <a href="https://t.co/k0DQaXVvvO">pic.twitter.com/k0DQaXVvvO</a></p>&mdash; Ari Seff (@ari_seff) <a href="https://twitter.com/ari_seff/status/1409296508634152964?ref_src=twsrc%5Etfw">June 27, 2021</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>


* Universal Theorem
* Visualización de Redes Neuronales: http://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=4,2&seed=0.91824&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false
* https://towardsdatascience.com/a-gentle-journey-from-linear-regression-to-neural-networks-68881590760e
* The measure of intelligence https://arxiv.org/abs/1911.01547
* https://arxiv.org/pdf/1906.07633.pdf Flor culstering to cluster explanation of neural networks
* https://arxiv.org/pdf/1904.01983.pdf One neuron is more informative than a network
* https://arxiv.org/abs/1907.06374
* https://github.com/bhavinjawade/Advanced-Data-Structures-with-Python: Excelente recurso con info de estructuras de datos en python.
* https://machinelearningmastery.com/tactics-to-combat-imbalanced-classes-in-your-machine-learning-dataset/: Como combatir los problemas de clases desbalanceadas.
* Buenas Práticas para ML Engineering: http://martin.zinkevich.org/rules_of_ml/rules_of_ml.pdf

# MOOCs

* Google Crash Course https://developers.google.com/machine-learning/crash-course/
* http://mjt.cs.illinois.edu/courses/dlt-f19/ NTK

# Tutoriales

* https://medium.com/@dhruvp/how-to-write-a-neural-network-to-play-pong-from-scratch-956b57d4f6e0
* Grokking Deep Learning https://github.com/iamtrask/Grokking-Deep-Learning
* Machine Learning Tokyo: https://github.com/Machine-Learning-Tokyo/Math_resources
* tSNE: https://towardsdatascience.com/t-sne-python-example-1ded9953f26
* Time Series Neural Networks https://www.datasciencecentral.com/profiles/blogs/time-series-classification-with-tensorflow
* https://medium.com/@tdietterich/what-does-it-mean-for-a-machine-to-understand-555485f3ad40
* https://deepai.org/publication/learning-by-abstraction-the-neural-state-machine
* https://medium.com/@devnag/generative-adversarial-networks-gans-in-50-lines-of-code-pytorch-e81b79659e3f
* https://medium.com/@ODSC/data-scientists-versus-statisticians-8ea146b7a47f
* Ejemplo de Regresión Logística: https://medium.com/@ODSC/logistic-regression-with-python-ede39f8573c7
* Intro a TensorFlow: https://medium.com/tensorflow/introducing-tensorflow-graphics-computer-graphics-meets-deep-learning-c8e3877b7668
* Redes Convolucionales: https://www.freecodecamp.org/news/everything-you-need-to-know-to-master-convolutional-neural-networks-ef98ca3c7655/
* Intro a Keras: https://adventuresinmachinelearning.com/keras-lstm-tutorial/
* Documentación Keras: https://keras.io/getting-started/sequential-model-guide/
* C++ Machine Learning: https://www.quora.com/I-want-to-use-C++-to-learn-Machine-Learning-instead-of-Python-or-R-is-it-fine
* Redes convolucionales de adversarios: https://towardsdatascience.com/dcgans-deep-convolutional-generative-adversarial-networks-c7f392c2c8f8
* https://blogs.princeton.edu/imabandit/2019/07/10/guest-post-by-julien-mairal-a-kernel-point-of-view-on-convolutional-neural-networks-part-i/

# Neural Networks and computing
* https://www.cs.montana.edu/~elser/turing%20papers/Schoolboy%20Ideas.pdf

# Challenges 

* AIcrowd https://www.aicrowd.com/

# Datasets

* https://physionet.org/content/mimic-cxr/2.0.0/

# NLP

* https://stanfordnlp.github.io/stanfordnlp/
* https://tabnine.com/blog/deep
* https://arxiv.org/abs/1810.04805 BERT
* http://jalammar.github.io/illustrated-bert/
* https://scientific-knowledge.github.io/

# Visualizations

* http://visualizationuniverse.com/tools/

#  Fallacies of Data Science
* Cherry Picking: Selecting results that fit your claim.
* Data Dredging: Results or correlation was due to CHANCE.
* Survivorship bias: Drawing conclusions from an incomplete set of data that survived.
* Perverse incentive: the incentive produces the opposite result ("this doesn't work")
* False causality: two things occur together, they are related (falsely)
* Sampling bias
* Gamblers fallacy: believing that when something happen the chance of happening again is reduced.
* Simpsons paradox: a trend is present in a group but dissapears when data is combined.
* Clever Hans Effect: https://arxiv.org/pdf/2006.10609.pdf

# Business

* https://hackernoon.com/why-businesses-fail-at-machine-learning-fbff41c4d5db

# Swift and Julia
* https://towardsdatascience.com/why-swift-may-be-the-next-big-thing-in-deep-learning-f3f6a638ca72
* https://medium.com/codex/is-julia-really-fast-12cd7caef96b

# Robotics

* https://www.robonet.wiki/

# Hype and News
* https://ai.googleblog.com/2019/08/exploring-weight-agnostic-neural.html

# Key people in Argentina

* Juliana Gambini, ML Computer Vision, SAR
* Micaela Mantegna, Abogamer.
* Luciana Benotti, NLP
* Juan Miguel Santos, DL/ML/RL/Robótica




# Conferencias
Do you have 2 or more publications in NeurIPS, ICML, COLT, UAI, AISTATS, AAAI, IJCAI, AAMAS, ICLR, ICRA, IROS, CVPR, ECCV, ICCV, ACL, EMNLP, EACL, NAACL, TACL, ICAPS, KDD, WSDM, WWW, JMLR, Ann Stats, JASA, TPAMI, IEEE Trans Image Proc, IEEE Trans Signal Proc, IEEE Trans Info Theory, Mathematical Programming, SIAM Journal on Optimization?
