---
title: "Epistemología a la carta"
excerpt: "Epistemología a la carta"
collection: portfolio
---

> Reglas para sacar valor a los Proyectos Finales de Carrera, los Trabajos Finales Integradores, las Tesinas de Especialización, las Tesis de Maestria y las Tesis de Doctorado.

## La Clave

* La clave está en definir un scope realista del proyecto lo más acotado posible. Lo que queda afuera no se hace, ni nos preocupa. Pero todo lo que queda adentro hay que hacerlo bien.

## Tips

* Las tesis se escriben en Latex.  [Date un tiempo para mirar este video si no tenés idea que es](https://youtu.be/KhWwuQ7qf5A?si=pdaq11w0ieBtnNqc&t=96).  Con las herramientas generativas hoy es mucho más simple de escribir documentos en Latex.
* El documento en Overleaf/Latex/OpenAI Prism tiene que estar desde el primer día y hay que usarlo como un repositorio de referencias, tirar texto ahí, poner enlaces.  Hay que ir acumulando y documentando todo el material que se va juntando, incluso aquel que no prospera.  Pueden arrancar con este [template](https://raw.githubusercontent.com/faturita/faturita.github.io/master/files/Template_PF_2024.zip).
* Prolijo con los datos:   Tiene que estar super claro como acceder a los datos, que es lo que contienen y el speech de como fueron tomados.  Esto puede incluir la solicitud al Comité de Etica del Departamento de Investigación y Doctorado de la Universidad, con la aprobación.
* Armar scripts basados en esos datos para poder regenerar todos los gráficos.
* Los gráficos tienen que tener los ejes bien marcados y en tamaños grandes bien visibles, generalmente sin títulos.  Todos los gráficos tienen que ser en formato EPS.
* Armar un apartado que resuma las contribuciones del trabajo, explicitadas una a una.
* Las fotos tienen que tener la cara tapada, buena iluminación, mostrar los elementos importantes destacados de forma que se visualicen de manera correcta.

## En relación a las Iteraciones
* No tiene sentido empezar todo de cero todo el tiempo.  Por eso, siempre es mejor **construir sobre los hombros de los gigantes** y avanzar en iteraciones trabajos previos haciendo aportes.
* Pero el trabajo realizado tiene que ser AUTOCONTENIDO.  Es decir, debe establecer claramente el objetivo y el alcance, dentro del marco de un proyecto más abarcativo y a largo plazo, y ofrecer todo lo necesario para que sea comprensible en sí mismo.  Esto siempre es posible.
* Por ejemplo, los trabajos no pueden tener como título "Proyecto 2", sino que tienen que centrarse en cuál fue el aporte implementado en esa iteración.  Esto jerarquiza además al trabajo y le da su justa medida en relación a los aportes, además de que lo focaliza y ayuda a que el informe, que es la evidencia de todo el trabajo realizado, tenga un estructura mucho más adecuada.

## En relación al Trabajo
* Cuatro palabras: Rigor, reliability, robustness, and transparency
* *Rigor*: Se refiere a que el trabajo no saltee paso, no corner-cut (o si lo hace que lo aclare como limitación).
* *Reliability*: Que los resultados o el funcionamiento se sostenga y que no sea producto de azar puro.
* *Robustness*: Que ese funcionamiento o resultados permitan tolerar argumentos que lo debatan, o en el caso de desarrollos que permitan tolerar pequeñas variaciones en su uso DENTRO del propio alcance.  Por ejemplo, un auto que se detiene repentinamente a los 20 km por hora no es robusto.
* *Transparency*: que toda la información esté visible, accesible.

## En relación a los Experimentos, los Datos y las Figuras
* El Informe es muchas veces la única evidencia que queda del trabajo realizado y del proyecto encarado.  Por lo tanto tiene que ofrecer evidencias abundantes para PROBAR que se trabajó, y además probar qué se obtuvo.
* Los **Experimentos** o las validaciones de funcionamiento, tienen que estar bien claros y determinados.  Tiene que detallarse con precisión quienes son los sujetos y qué y cómo se estudio algo del mundo real. Esto debe incluir la solicitud al Comité de Etica del Departamento de Investigación y Doctorado o similar de la Universidad o institución, con su aprobación.  Por ejemplo, "Los experimentos son el 1,2,3,4 y a continuacón se describen en detalle.". 
* Un entregable de valor en un PF es el/los dataset completo en un repositorio público de datos como Cloud Ocean o IEEE Dataport o Kaggle.
* Es importante poder tener no sólo los datos bien resguardados, sino también todos los datos de postcálculo posteriores y también el pipeline de procesamiento y todo el **setup** armado para poder regenerarlo en cualquier momento.  Esto hay que mantenerlo durante todo el proyecto (y después también si el proyecto continúa con una publicación posterior).
* Incluso en aras de mantener una alta reproducibilidad de los resultados, diferentes revistas científicas obligan a los autores a subir el código a una plataforma como Code Ocean o incluso github.
* Es importante tener resguardados todos los scripts y el pipeline para la generación de los gráficos que explotan justamente esos datos.
* Las figuras son clave, porque es la manera más concreta de transmitir información compleja.
* Tienen que poder leerse bien los ejes de la figuras, con un font grande que pueda leerse (ver principios de diseño de Amanda Heidt)

![Neurotronics](/images/designprinciples.png){:height="450px" width="300px"}

## En relación al Informe - ¿Qué cosas NO van?
* El informe NO ES el Research Proposal que es la propuesta de trabajo.  Es un documento totalmente independiente. Idealmente un buen informe, tiene un título, y el informe habla de ese título y del tema, y el hecho de que se haya usado como una tesis, proyecto final o similar apenas se menciona al principio y nunca más.  Los temas epistemológicos no tienen que estar en el Informe.
* En el Informe NO SE ESCRIBE SOBRE EL INFORME.  Por ejemplo, el informe no contiene informacion de los pasos que se dieron para construir el propio informe.  Dependiendo del trabajo, se pueden describir lecciones aprendidas, pero se escribe una historia y no el detalle punto a punto de lo que se se fue haciendo.  Por ejemplo, algo asi NO HAY QUE PONERLO: "Para el desarrollo de este informe, primero visitamos un investigador que lamentablemente no nos contestó.  Luego fuimos a ver otro investigador que nos contestó al principio, pero luego no nos contestó mas.  Finalmente hablamos con un tercero que sí nos contestó." 😖
* En el Informe NO SE HABLA SOBRE LOS ALUMNOS QUE CONSTRUYERON EL INFORME.  Por ejemplo, "Este trabajo me ayudó a comprender cómo llevar adelante un proyecto de investigación." 😒

## En relación al Informe - ¿De qué SI se trata?
* Como pensarlo:  una manera es pensar una pregunta e intentar que el informe la responda, en sus propios términos. Así entonces, al informe hay que considerarlo como lo que saldría en google cuando alguién hace esa pregunta.  El informe contesta esa pregunta.
* Secciones:
    * **Abstract**: El abstract se escribe AL FINAL y es un resumen en un párrafo chiquito (no más de 200 palabras) de lo que el trabajo hace, destacando el problema general (porque se hace esto), como se aborda resolver ese problema, y que se concluye al final.
    * **Introducción**: va desde lo general, desde los problemas de la humanidad, haciendose cada vez más específico hasta plantear el problema que existe, que no fue resuelto por nadie, y que este trabajo viene a solucionar.  Al final requiere poner contribuciones/objetivos.  Después un walkthrough que detalle que es lo que hay en cada parte del propio informe.
    * **Background**:  en esta parte se introduce al lector los temas necesarios para que pueda entender de que se trata el tema presentado.  Esto es explicar los temas de base, con citas y referencias, y por supuesto siempre alrededor del problema abordado en el trabajo.   ¿Qué hay que saber para entender esto?
    * **State-Of-The-Art**:  esto es el SOTA, el "literature review".  En esta parte se describen los trabajos de la literatura que quieren, más o menos, hacer lo mismo que se presenta en este trabajo.  Es la descripción de los trabajos que son competidores con este trabajo.
    * **Materials and Methods**: Esta sección, generalmente en capítulos describen el meollo de la solución.  Cómo se intenta responder a las preguntas establecidas en la introducción.  Si hay experimentos, se describen los mismos.  Cuanto más reproducible sea la descripción, en general se considera más formal.
    * **Results**: Se muestran los resultados obtenidos.
    * **Discussion**: Se discuten y se explican los resultados obtenidos.  Esta sección suele estar mezclada con la anterior en una sola.
    * **Conclussions**: Se detallan las conclusiones en base a información aportada por este trabajo.
    * **Future Work**: Se detalla como se continuaría el trabajo de contar con tiempo infinito.
* Cada vez que se pone un gráfico hay que explicarlo y tiene que tener una razón para estar ahí.  Gráficos de relleno no sirven para nada.  No está bueno poner capturas de salidas de pantalla, a no ser que sea estrictamente importante.
* Cada vez que se menciona algo que existe, hay que citarlo.
* En el informe no van las actividades que se hicieron para construir el informe.
* VERIFICAR la ortografía !!!!!!  Traten sobre todo de evitar los errores bestiales.
* Verificar bien las secciones.  Otra vez:  Intro, Materials and Methods, Results, Discussion, Conclussion, Future Work
* El siguiente gráfico muestra bien los pasos necesarios para escribir un paper, que son similares a los necesarios para el trabajo

![Neurotronics](/images/howtowritepaper.png){:height="450px" width="300px"}

![Neurotronics](/images/abstract.jpeg){:height="450px" width="300px"}

## En relación al Informe - La plataforma
Hay que usar Latex.  Cualquier otra cosa merece el quinto anillo.  Cuando arrancan el proyecto van a arrancar con un template básico en Latex sobre la plataforma de Overleaf.  La curva de aprendizaje es compleja, pero el documento sale perfecto y Latex fuerza a escribir de una manera particular.  Elimina más fácilmente vicios que en otra plataforma son naturales.  Pueden utilizar esta guía también excelente [Latex Paper Writing Tips](https://github.com/guanyingc/latex_paper_writing_tips).

## En relación al Informe - La búsqueda bibliográfica
La búsqueda bibliográfica o armado del SOTA, **State of the Art** implica recorrer las bases de datos bibliográficas buscando proyectos que sean COMPETIDORES del que se está construyendo, en menor o mayor medida.  Tratar de entender dónde está el mundo en relación a este problema, y en base a eso qué lugar ocupará esta investigación/informe.  Esta es una búsqueda compleja porque en el límite de la ciencia, que es justamente donde cualesquiera de estos trabajos idealmente gustaría ocupar, la nomeclatura no está acordada y las cosas se suelen llamar de muchas maneras diferentes.  La clave está en identificar buenos keywords que ayuden a ir acercando el concepto lo más posible.  La mejor herramienta actualmente es [Google Scholar](https://scholar.google.com).  Primero hay que tratar de buscar algún buen REVIEW del tema.  Estos son artículos especiales que justamente hacen una revisión del estado del arte en el tema.  Y desde ahí ir para atrás y para adelante en relación a las citas.  Google scholar permite ver los papers que son citados por un artículo así también los paper que cita, con lo cual de los review se pueden ir buscando los papers más importantes hacía atrás y lo más recientes hacia adelante (que por lo general van a referenciar algún buen review).  [PubMed](https://pubmed.ncbi.nlm.nih.gov/) es otra base de datos importante porque identifica aquellos trabajos científicos que tienen relevancia médica. Otras herramientas excelentes para buscar información bibliográfica es: Web of Science o Scopus (si tenés acceso), [ResearchGate](https://researchgate.net), [Semantic Scholar](https://www.semanticscholar.org/) ,[Undermind](https://www.undermind.ai/home/), [Consensus](https://consensus.app/),[OpenAlex](https://openalex.org/), con estas últimas haciendo uso de modelos de lenguaje de IA.  Si buscan papers de [ArXiv](https://arxiv.org/) fijense los comentarios en [AlphaXiv](https://alphaxiv.org).

En resumen,

* [Google Scholar](https://scholar.google.com): El buscador por default y además métrica más objetiva de credenciales científicas.
* [PubMed](https://pubmed.ncbi.nlm.nih.gov/): Si el paper está acá, tiene alguna conexión con salud.
* [ResearchGate](https://researchgate.net): la red social científica.
* [Semantic Scholar](https://www.semanticscholar.org/): Pre-LLM para una búsqueda más precisa de papers.
* [Undermind](https://www.undermind.ai/home/)
* [Consensus](https://consensus.app/)
* [Perplexity](https://www.perplexity.ai/): LLM que combina varios papers y permite seguir trazos de lineas apuntando las referencias.  Es excelente.
* [Open Alex](https://openalex.org): Base de datos de papers con sus métricas.
* [ArXiv](https://arxiv.org/): Repositorio de preprints. Muchos papers de IA y de tecnología.
* [AlphaXiv](https://alphaxiv.org): Muestra los papers de arxiv con comentarios agregados por la comunidad.
* [ResearchRabbit](https://app.researchrabbit.ai/):  Permite organizar la búsqueda de bibliografía con LLMs.



## En relación al Informe - La Escritura
El informe no tiene que ser ni largo ni corto.  Tiene que ser:
* *Consistente*: tiene que introducir adecuadamente los términos, conceptos que utiliza ANTES de utilizarlos.  Por ejemplo, si detalla un método de procesar señales, antes tiene que hablar de qué son esas señales.
* *Autocontenido*: que puede leerse de principio a fin dejando claro el mensaje que intenta transmitir sin tener que forzar al lector obligatoriamente a leer otra cosa.  Por ejemplo, si el mensaje es sobre un nuevo método para resolver un problema de optimización, entonces los problemas de optimización merecen bastante lugar dentro del informe, no se pueden explicar en una linea.
* *Reproducible*: que todo explicado con el detalle SUFICIENTE como para poder reproducirlo desde cero.  Cuánto es suficiente?  Una buena medida es en general hasta las librerías.  Si es algo de software y es una librería, puedo poner la referencia al paper y no explicar en super detalle el método que está explicado en la librería.
* *Resonante*: que se encuentre pertinente en el tiempo y en el espacio donde se crea, que aborde los problemas actuales y relevantes.
* *Estilo*: Todo esto lo pueden tener manteniendo el estilo que ustedes quieran: [Ye Olde Scientific Writing](https://www.lastwordonnothing.com/2015/02/05/ye-olde-scientific-writing/), o esto [Donald Duck](https://gjsd.gile-edu.org/index.php/home/article/view/7-donald-duck-141-145).

## En relación al Informe - El Proceso de Escritura

* Se llama *Síndrome de la Hoja en blanco*: es el efecto de bloquearse cuando hay que escribir todo lo que se hizo para el informe.
* Dos buenas ideas: (1) arranquen sobre el documento en latex directamente y vayan agregando todas las referencias que fueron encontrando y TIRAN en el texto sin ningún cuidado gramatical una breve oración de lo que esa referencia dice y la citan en el texto.  Lo (2) que pueden hacer es sobre esa hoja en blanco empezar a tirar las ideas directamente, una abajo de la otra, como si fuera un anotador sin sentido.  Lo que importa es empezar a tener la arcilla con la que luego se va a editar, iterar y refinar en pasos sucesivos hasta que se le va dando forma.
* Pueden encontrar muchos más tips acá: [Writing Tips Nature](https://www.nature.com/articles/d41586-024-02013-4)
* Excelente guía con 10 reglas para tener en cuenta: [10 Rules for Writing](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005619)


## En relación al Informe - El Contenido
En la cabeza del lector del Informe, van a aparecer estas preguntas, por lo que el informe tiene que en algún punto abordar alguna respuesta.
* ¿De qué se trata el trabajo? ¿Qué es lo que puntualmente quieren resolver, cuál es el problema principal?  Yo no sé NADA de este tema que presentan, denme una mini intro general para que entienda y denme referencias para aprender más o ver el detalle.
* ¿Cómo es lo que están presentando? ¿De qué se trata el método, algoritmo, solución, etc? ¿O qué es lo que quieren saber que hoy no se sabe?
* ¿Qué experimentos hicieron o cómo me van a demostrar que lo que hicieron funciona? ¿Qué métrica van a utilizar? ¿Contra que lo van a comparar?
* ¿Qué limitaciones tiene lo que presentan? ¿En qué casos no anda bien, o como van corrigiendo o aplicando mejoras para lidear con cada una de esas limitaciones?
* ¿Cómo sigue la cosa después? ¿Qué harían ustedes si tuviesen todo el dinero, tiempo, ganas del mundo para seguir con este proyecto?
* El título del trabajo, y el alcance, hacen referencia al tema principal que se presenta.  Eso justamente es lo principal y en general es lo que demanda del trabajo mayor atención, reflejada en por ejemplo, cuántas hojas se usan para esa parte.  El resto del contenido está POR Y PARA esa parte.  Por ejemplo, en un trabajo que involucra una implementación de rede neuronales recurrentes para predecir el valor de bitcoin, no tiene sentido en la intro poner 3 carillas de redes convolucionales !


![Ask Your Papers](/images/AskYourPapers.png){:height="450px" width="300px"}



## En relación al Informe - El ABSTRACT
El Abstract normalmente se escribe al final.  No es la introducción al tema, eso es justamente la **Introducción**.  El Abstract (o Resumen) es el resumen del trabajo, por lo tanto tiene que detallarle a un lector lo que el trabajo tiene de una manera concisa.  No tiene sentido que sea largo, debe ser corto porque es un TL;DR (Too Long, Don't Read). 

![¿Cómo escribir un Abstract?](/images/natureabstractwriting.jpeg){:height="450px" width="300px"}

El Abstract arranca describiendo el contexto general y de ahí la necesidad puntual **de la humanidad** que este trabajo aborda.  Luego se describe el objetivo que empujó el trabajo, y el detalle metodológico general, enfatizando el aspecto experimental (que experimento se hizo y cómo).  Luego se mencionan los resultados, la frutilla de lo que presenta este trabajo.  Finalmente se establece la conclusión ''che, con esto que hicimos probamos que si juntamos nitrato de potasio, carbón  y azufre la cosa explota'', para finalmente destacar eventualmente las implicancias de eso: ''tendremos fuegos artificiales''.


## En relación a cuando está terminado
Este es el trabajo final de todo el esfuerzo de toda la carrera.  Se lo quieren sacar de encima, pero que lo que quede en el documento los haga sentir orgullosos y sientan que refleja bien todos estos años de esfuerzo. Una buena manera de pensarlo es si se lo enviarías a un posible empleador en una entrevista, como muestra de cómo podés trabajar. Si esa respuesta es positiva, entonces es porque el trabajo está terminado.

## En relación a la entrega del informe
El informe *tiene que entregarse al menos un mes, es decir 30 días antes de la fecha estimada o requerida de defensa*.  Tengan en cuenta muy bien cuándo son las fechas limites que hay que defender para poder entrar en las colaciones correspondientes.  ESTA ES UNA RESPONSABILIDAD DE LOS ALUMNOS DE CONTROLAR, ya que son ellos los que tienen la necesidad.  El proceso es iterativo entre el tutor y el grupo de alumnos.  Las devoluciones pueden demorar entre una hora o una semana aproximadamente, y de haber una demora particular será comunicada.  Leer y corregir el proyecto requiere tiempo.

## En relación a las devoluciones de los jurados
Las devoluciones de los jurados/revisores hay que usarlas a favor, siempre, al igual que se hace en el Aikido donde la energia del contrincante se usa para nuestro propio beneficio.  Acá es igual, porque detrás de cualquier crítica siempre hay espacio para generar una mejora.
Para hacer el abordaje es necesario tener presente el scope del proyecto: que va y que no.  Las críticas sobre lo que está dentro son siempre las más jugosas.

En general se suele seguir un modelo de respuestas similar a [este](https://raw.githubusercontent.com/faturita/faturita.github.io/master/files/response.letter.sample.tex)


## En relación a algunas herramientas

* [PlotNeuralNet](https://github.com/HarisIqbal88/PlotNeuralNet): Para hacer gráficos de arquitecturas de redes neuronales.
* [MatchaIO](https://www.mathcha.io/): Excelente herramienta para generar gráficos simples, y suficientemente buenos en tikz para Latex.
* [IPE-Web](https://ipe-web.otfried.org/index.html) Excelente para edición de gráficos también para Latex.
* [Latex UI Elements](https://ipe-web.otfried.org/index.html): Creación de elementos gráficos para Latex
* [OpenArt](https://openart.ai/home): Buenísima herramienta generativa para imágenes, a buen precio.

## En relación a la DEFENSA 
Una vez entregado el Informe, aplicadas las devoluciones de los jurados, se hace una defensa, también llamada VIVA, donde los tesistas defienden su trabajo ante sus tutores, sus jurados, y el público eventualmente.  Para ello elaboran una presentación que luego culmina con un espacio de Q&A.

* La presentación es con slides y se muestra en el dia de la defensa.   
* Una presentación de 40 minutos es siempre más que suficiente.
* Es importante que sea concreta, acotada al tiempo (super importante), que sean claros con el mensaje que dan.  Que muestren el trabajo que hicieron, que muestre el esfuerzo.
* La base es académica y de ingenieria.  Esto implica que lo que se dice se sustenta (o se tiene que sustentar).
* Ahí es donde juega el OBJETIVO y el ALCANCE del proyecto (que están también plasmados en el informe).  Una vez que se define el objetivo, el alcance se elige, y es lo que limita.  Todo lo que queda adentro, hay que explicarlo, argumentarlo o estar listo para hacerlo.  Lo que queda afuera, no hay problema.  Esto es super importante de entenderlo porque es la clave para una buena defensa.  Por ejemplo, el nombre del proyecto es "Estudio de los métodos de clasificación basados en kNN para datos médicos de Córdoba".  El título implicitamente ya está limitando el alcance, entonces si alguien pregunta "Probaron con un método UMAP?", - "No la verdad que no probamos ese método, nos concentramos en kNN principalmente, pero sería interesante hacerlo en el futuro.".  Listo. 
* Todo lo que es SUBJETIVO no lo tienen que decir ni poner.   Por ejemplo, "Elegimos este método porque nos pareció el MEJOR", No.  Tiene que decir que eligieron ese método porque hicieron experimentos y en la tabla figura con los mejores resultados (decisiones informadas), o porque tienen una referencia de alguién que lo hizo así.   Todo lo superlativo tienen que eliminarlo (adjetivos como bueno, lindo, copado, etc).   Las decisiones que toman tienen que ser en base a los datos que tuvieron ustedes o que pueden soportarla con referencias.
* ¿Esto último quiere decir que siempre hay que hacer eso y nunca usar algo simplemente porque nos pareció y funcionó o porque probamos muchas opciones y funcionó?  La creación de algo requiere de cortar clavos y hacer cosas mundanas siempre, donde el método científico y la correctitud en el procedimiento no siempre pueden seguirse al pie de la letra (sino miren esto [Honest Truth](https://twitter.com/hashtag/overlyhonestmethods?src=hashtag_click) ).  Lo que sí hay que hacer es cuando la suerte aparece así, que es un componente válido aunque muchos lo nieguen, hay que construir para atrás y hacer todo lo posible para intentar entender y justificar por qué esa fue la mejor decisión, encontrar referencias o justificarla.
* Las referencias son un arma espectacular [Referencias](https://twitter.com/MemingPhD/status/1562516001006419969/photo/1)
* La presentación es una especie de show donde muestran su trabajo, es un "show educado".  Tiene que tener un nudo, donde plantean el problema mundial que motiva esto.  Luego plantean las soluciones existentes y van especificando la problemática hasta que llegan a un problema donde lo que ustedes hicieron es la solución.    Luego plantean el meollo de la cuestión, siempre jugando con que las cosas no salen no salen, hasta que cuentan cómo resolvieron algo, presentan la problemática y cómo lo resolvieron.   Tienen que incluir al principio muy bien lo que ustedes creen que son sus contribuciones.  Y esto enfatizarlo también en las conclusiones, similar al [Viaje del heroe](https://en.wikipedia.org/wiki/Hero%27s_journey).  Miren esto también explicado por un maestro total del *storytelling*, [Kurt Vonnegut](https://twitter.com/Rainmaker1973/status/1694013662837481609?s=20).
* El ESTILO de la presentación de la defensa es PROPIO de cada grup, de cada persona.  Es preferible algo que sale mal con el estilo propio que algo que sale más o menos con un estilo impuesto (que siempre es aburrido y pobre).
* Traten de hablar todos, pero estar todos al tanto de lo que resolvieron.  Es interesante que den su perspectiva sobre los problemas que tuvieron también y como le encontraron la vuelta desde el lado de la ingeniería.
* 3/4 del tiempo es contar los aportes, el nudo del trabajo. En el otro 1/4 hay que ofrecer a los interlocutores el material para que entiendan lo que se hizo.
* Gedankenexperiment:  consiste en lo siguiente: pensár que están en un bar de Berlin con una compañera de trabajo que es técnica, sabe de ciencia, sabe de ciencias de la computación, conoce algo BASICO del tema en cuestión.   Hay que contarle sobre sobre la tesis.  Toman una servilleta y empiezan a poner garabatos que ayudan a la explicación.  Se hace la explicación, utilizando esos garabatos.  Bueno, entonces los slides de la presentación de la defensa, se deberían arrancar desde ahí, desde esos garabatos.  Luego se va para atrás, cuando su compañera dice "¿Cuál es la diferencia entre este tema BASICO acá y este otro tema BASICO (que ustedes están usando)?", entonces se arma un slide para contestar eso, y para adelante cuándo pregunta "Todo muy lindo, ¿pero esto para que mierda sirve?".  Y así.  De hecho si tienen la oportunidad de realmente salir en estos días a un evento social, jueguen a este juego DE VERDAD. Fijense cómo ocurre la magia.
* Es importante que tengan bien en cuenta quienes son los jurados, a qué se dedican, qué hacen.  Stalkeenlos un poco para ver cuáles son sus especialidades porque justamente las preguntas que hagan van a girar alrededor de eso.
* Super importante: Demuestren confianza en su trabajo y en su conocimiento de la materia.  Siempre hay alguién que sabe más, siempre hay más tema para aprender.  Ustedes estudiaron y trabajaron muchísimo, y sobre ese tema, más que nadie en toda la defensa seguramente.   Por lo tanto, sientanse con total confianza en su conocimiento sobre el tema.  Si llegan a la defensa es porque ya son expertos.  Defiendanlo así.  Por ejemplo
    * Jurado malvado: "Creen ustedes que este método que están proponiendo puede llegar a utilizarse o que es relevante en el estado del arte sobre este tema?".
    * ❌: "El tema es muy complejo, nosotros no sabemos muchos, somos solo estudiantes, no sabemos si puede utilizarse o no, hay cosas muy avanzadas."
    * ✅: "Dentro del marco de las limitaciones que nosotros especificamos en nuestro informe y en esta defensa, este método puede utilizarse de manera adecuada y puede ser útil para solucionar el problema en cuestión."

![Neurotronics](/images/oralpresentations.jpeg){:height="450px" width="300px"}


![Bad Talks](/images/badtalk.jpeg){:height="450px" width="300px"}


## En relación al English
* Particularly when students are interested in broadcasting their work to international companies, it is advised to write their PF in English.
* Keep sentences simple, straightforward.  Try to avoid very complicated indirect speeches, or very complicated subjective sentences.
* Use synonyms extensively,
   * BUT: however, although, though, yet, nevertheless
   * ALSO: besides, likewise, moreover, as well as, furthermore
   * THEREFORE: hence, thus, as a result, subsequently, for this reason
   * ESPECIALLY: mainly, notably, above all, principally, exclusively
* In English, you always need a subject.
* Keep the same verb form throughout the entire text.
* Some common mistakes (From IEEE Class Template's handy guidelines)
   * The word "data" is plural, not singular.
   * A graph within a graph is an inset not an insert.
   * Alternatively not alternately
   * Do not confuse "imply" to "infer"
   * Non is not a word, then it should be joined to the word it modifies without a hyphen (because the hyphen is used to create words based on two or more already existing words).
   
## En relación al Disclaimer Final

Este tipo de proyectos requieren ciertas características en cuánto a las intenciones del equipo de trabajo que lo van a llevar adelante.

* Si lo que quieren es sacarse la materia de encima, NO HAGAN NI SE EMBARQUEN EN ESTOS PROYECTOS.
* Tienen que tener ganas de hacerlo, les tiene que copar.  Hay que aprender temas nuevos, quizás hasta incluso alejados del área específica de cada uno.  Por lo tanto, para que funcione eso, es importante que haya una buena motivación para encarar el tema.
* Es importante que el grupo de trabajo tenga una buena dinámica y empuje el tema por motus propia.  Las tesis o proyectos finales son proyectos de alumnos que requieren que los administren de manera adecuada ejecutandolos.  Tienen que tener el ownership del proyecto y hacerse cargo.

## En relación a las Referencias y a Ver Más

* Rocco S., Hatcher T., 2011, "The handbook of scholarly writing and publishing"
* Samaja J., 1999, "Epistemología y Metodología"
* Osmond A., 2013, "Academic Writing and Grammar for Students"
* Gastel B., Day R.A., 2019, "How to Write and Publish a Scientific Paper"
