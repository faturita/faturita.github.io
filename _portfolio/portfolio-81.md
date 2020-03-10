---
title: "Liveness Detection"
excerpt: "This is currently a big deal in banking industry"
collection: portfolio
---

![Descriptor](/images/liveness.jpg){:height="450px" width="300px"}

* *Description*: Online Banks are claiming for this.  They want to be able to identify that an actual person is behind a mobile phone and is trying to register into a mobile app, to get a banking account, to issue a mortgage and so on.  It is not exactly recognizing who the person is against some previous record based on the picture of the face.  It is understaing that the picture is not fake, and that the person is not wearing a mask.  It is a anti-spoofing approach. 

* *Project*: The idea of this project is first to implement a desktop application that uses the camera from the computer to perform liveness detection.  It is also interesting to use the mobile camera to do the same.  The final scope is to perform all that using only javascript in a web app and do that offline withtout the intervention of any server side component.

* *Scope*:  the first steps towards the MVP is to have an application running either in a desktop app or in a mobile phone.

* Spanish: Los procesos de registro onboarding inicial, requieren un primer paso donde se realiza una identificación de la persona física contra los registros gubernamentales.  Se intenta verificar que quién está detrás del registro inicial es quien dice ser.  Para eso se busca realizar una validación contra los registros gubernamentales que suele ser mediante un chequeo y validación de consistencia de los datos, y una validación biométrica.

A su vez, el avance de los celulares así como también la ubicuidad de las cámaras en tablets y notebooks, empujó para que los mecanismos basados en reconocimiento faciales estén siendo ampliamente utilizados. Después de la identificación dactilar, el reconocimiento facial es el mecanismo actual más usado[1].

En este contexto, aparece el biometric spoofing: técnica que intenta confundir a los sistemas biométricos para reconocer a una identidad ilegítima como una genuina por medio de presentar al sistema alternativas sintéticas falsas basadas en el original, directamente sobre el sensor biométrico[1].

Esta es una área no resuelta, que suele ser categorizada en seguridad como side-channel attacks.  Son los escenarios más complejos de resolver.  Por esa razón, es a su vez intensamente investigada[3] tanto desde el mundo académico como desde la perspectiva tecnológica de desarrollar una solución comercial.

En los mecanismos de identificación o autenticación biométricos, 

* La información biométrica es pública y no es modificable.

* Los tipos de ataques que se pueden implementar requieren una low-bar de ingreso, convirtiendo muchos posibles usuarios en posibles atacantes del sistema.

* Al ser ataques side-channel los sistemas de protección digital son complementarios pero inherentemente insuficientes.

Por esta razón las alternativas de solución aparecen de la mano de implementaciones de inteligencia artificial, o machine-learning para inferir características del proceso de adquisición que permitan realizar la identificación de la falsificación sintética.

Los tipos de ataque que pueden realizarse son ataques directos o side-channel attacks, sobre el dispositivo de captura o directamente sobre el dato biométrico (biometric sample).


Los ataques sobre el dato biométrico requieren interceptar el dato una vez que la misma ya fue capturado.  Esto incluye alterar el pipeline de reconocimiento, alterar la transmisión de la información, alterar su almacenamiento, etc.


Los ataques sobre el dispositivo de captura incluyen el tampering del sensor puntual (e.g. cámaras CCD), o la  inyección de material biométrico que no sea fresco, implementando ataques de replay.


Sin embargo, tanto los dispositivos como los medios de almacenamiento y transmisión, suelen estar protegidos por mecanismos criptográficos, que un atacante debe vulnerar para tener acceso.  Por ello, como “la cadena de la seguridad se suele romper por el eslabón más débil”[6], los ataques directos de spoofing biométrico son la alternativa directa más simple de aplicar (hoy x hoy).

Los ataques directos de Biometric Face Spoofing suelen clasificarse[4] en:

* Photo Attack: se presenta una imagen 2D al sensor CCD, impresa en una hoja de papel, o desplegada en una tablet, y se intenta engañar al sistema con la foto del sujeto falsificado.

* Video Attack: se presenta la imagen 2D pero que permite implementar un escenario de validación dinámico, donde por ejemplo se pueden incluir pestañeos, movimientos de labio, movimientos de la cabeza.  Esto incluye los escenarios challenge-response, donde una aplicación simple le permite al atacante implementar los diferentes mecanismos que solicita la aplicación.

* Masks: muy populares recientemente en las protestas en Hong Kong, van desde hojas impresas con caras falsas que intentan ubicarse sobre el perfil de una cara real (abordan los chequeos de profundidad) hasta modelos en 3D con la textura de la cara a falsificar impresa.

Biometría de varios factores: al igual que ocurre con la autenticación en varios factores, los procesos biométricos que exploran a la vez diferentes factores, como pueden ser una huella dactilográfico junto con un reconocimiento facial, asumen el supuesto que el atacante requiere a la vez, sintetizar esa información biométrica que suele estar en canales diferentes.
Sensores especializados: el nombre “liveness detection” o “vitality detection” proviene justamente de intentar detectar información intrínseca o involuntaria, midiendo información de algún proceso biológico.  Por ejemplo, modificar el sensor para agregarle sensibilidad al infrarrojo para detectar la variación en la intensidad de rojos de una imágen que se corresponde con el pulso.
Digitales: o basados en el espacio de las características o los features.  Este es el más explorado, donde se aborda la problemática como un problema de clasificación en machine-learning.  Puede ser estático, dinámico o implementando un mecanismo de challenge-response, generando una interactividad con el sujeto (y una penalidad en usabilidad).
Scoring: mecanismos tradicionales de detección de fraude, muy populares en el mundo de transacciones de tarjeta de crédito o escenarios actuarios.  Visualizando cada proceso de identificación como una transacción que es scoreada y que suma a un corpus de datos que luego son abordados por análisis de datos globales (i.e. analytics o data science).

Existe un viejo adagio de seguridad informática que establece que es una mala idea desarrollar por cuenta propia un sistema de seguridad informática[8].  El aliciente a este planteo es cuando se piensa en un proceso a largo plazo, de evolución y mantenimiento continuo, o cuando se es consciente de las inherentes vulnerabilidades que un sistema así puede tener, y se aceptan como un riesgo válido y tolerable para el sistema en cuestión.

Adicionalmente, por el tipo de problema que se aborda, vemos en este desarrollo un componente de innovación que apunta a tener una solución técnica que hoy no existe, o no tiene el grado de madurez necesario.  Esto requiere inevitablemente de un proceso de iteración y un abordaje de la solución a largo plazo.

Aconsejamos la posibilidad de implementar una solución híbrida (offline/online) que justamente aproveche las capacidades de procesamiento server-side. Justamente la capacidad de poder poner recursos de hardware, accesibles para una entidad como un banco, es lo que permite mover la barra hacia arriba.

De este modo la implementación offline permite una solución factible que opera principalmente como un sistema de backup.  Desde el punto de vista de la propia programación el sistema puede estudiar e implementar un trade-off entre latencia vs. tiempo de procesamiento, y elegir la mejor opción de cara a ofrecerle al usuario la mejor experiencia en performance, velocidad, uso de datos, usabilidad.

Por otro lado, al implementar un mecanismos de seguridad, es necesario conocer qué es lo que se intenta evitar. En este caso, se hace necesario esbozar en una etapa inicial, un modelado de amenazas, un Threat Model para entender qué tipos de ataques, escalonados según el nivel del ataque.  


Para esto es necesario conocer cuál es la situación actual que tienen en los sistemas productivos: qué tipos de ataques son los que detectaron hasta el momento, bajo qué contextos, cuál fue el éxito actual del sistema en detectarlos.  


Consideramos que este punto es clave más allá de un resultado obtenido con un conjunto de datasets puntuales, y que permite hacer el abordaje a la seguridad desde una perspectiva más general, que suele ser la recomendada (ya que la seguridad es una propiedad global que se implementa con mecanismos de chequeos locales).



Some links
* [Servicio RENAPER](https://www.argentina.gob.ar/sid-sistema-de-identidad-digital)
* [Face++](https://www.faceplusplus.com/face-based-identification/)
* [Cognitive with Azure}(https://docs.microsoft.com/en-us/azure/cognitive-services/face/face-api-how-to-topics/how-to-use-headpose)
Papers 
* Abbas Ur Rehman, "LiveNet: Improving features generalization for face liveness detection using convolution neural networks", 2018
* Javier Galbally, "Biometric Antispoofing Methods: A Survey in Face Recognition", 2014
* Galbally, J., Marcel, S. and Fierrez, J., 2014. Biometric antispoofing methods: A survey in face recognition. IEEE Access, 2, pp.1530-1552.
* Mazzucato, M., 2019.Catch-up and Mission-oriented Innovation.How Nations Learn: Technological Learning,Industrial Policy,and Catch-Up, p.63
* https://fg2020.org/ 
* Marcel, S., Nixon, M.S. and Li, S.Z., 2014. Handbook of biometric anti-spoofing (Vol. 1). New York: Springer. 
* Chakraborty, S. and Das, D., 2014. An overview of face liveness detection. arXiv preprint arXiv:1405.2227.
* Li, K.C., Chen, X. and Susilo, W. eds., 2019. Advances in Cyber Security: Principles, Techniques, and Applications. Springer.
* https://fortune.com/2019/10/04/hong-kong-protests-mask-ban-surveillance-anonymity-facial-recognition/
* Ferguson, N. and Schneier, B., 2003. Practical cryptography (Vol. 141). New York: Wiley.
* Yallamandaiah, S. and Nalluri, P., 2019, September. Comprehensive analysis of face recognition techniques: A survey. In Computer-Aided Developments: Electronics and Communication: Proceeding of the First Annual Conference on Computer-Aided Developments in Electronics and Communication (CADEC-2019), Vellore Institute of Technology, Amaravati, India, 2-3 March 2019 (p. 149). CRC Press.





