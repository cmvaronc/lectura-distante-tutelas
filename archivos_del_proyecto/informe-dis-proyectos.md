# ¿Cómo la inteligencia artificial puede mejorar el proceso de selección de tutelas en la Corte Constitucional? (informe de investigación preliminar)

*Estudiantes: María Fernanda Guerrero y Carlos Manuel Varón*

*Fecha: 11 de diciembre de 2018*

## Introducción

La tutela es el mecanismo procesal más utilizado por los ciudadanos para defender sus derechos fundamentales. Su reconocida popularidad hace que la selección de sentencias de tutela sea, para la Corte Constitucional, su mayor desafío, en razón de los más de 42.000 expedientes mensuales que recibe de todo el país para su eventual revisión. Así entonces, está claro que, de no atenderse adecuadamente esta situación, la complejidad que reviste la gestión de tutelas en materia de procesamiento de información podrían llevar este mecanismo del éxito al mayor de los fracasos.

Con el panorama anterior,  y dada una circunstancia afortunada de conjunción de saberes y experiencias (propiciada por el desarrollo de la Maestría en Humanidades Digitales), surgió la idea de adelantar una iniciativa de investigación – creación colaborativa para tratar de responder un pregunta que, a la vez, sirve como pilar fundamental de dicho ejercicio académico: ¿un sistema automatizado podría asistir el proceso de revisión y selección de tutelas adelantado por los judicantes (estudiantes de Derecho) en la Corte Constitucional?

Teniendo en cuenta el anterior contexto el desarrollo del trabajo de investigación, colaborativo e interdisciplinario, propone un doble acercamiento: en primer lugar, desde las humanidades digitales, el proyecto busca técnicas de lectura distante para crear una metodología que apoye la selección y posterior revisión de sentencias de tutela. En segundo lugar, desde la informática jurídica de ayuda a la decisión, el proyecto implica el uso de la tópica digital como metodología de búsqueda del saber jurídico a partir de sus fuentes y su interpretación, de conformidad con las actuales exigencias del derecho global contemporáneo. 

Así entonces, el proyecto de investigación al que nos abocamos ostenta dos frentes: de un lado, un ejercicio de carácter experimental, cuyo objetivo es emplear la técnica de modelado de tópicos para realizar una caracterización semántica de un corpus de fallos de tutela de primera y segunda instancias, con miras a probar si el algoritmo empleado para ello permite inferir la composición temática de documentos nuevos. Y segundo, un proceso de investigación y análisis cualitativo respecto de la manera como se lleva a cabo el proceso de gestión documental en la Corte Constitucional en relación con las tutelas, de tal manera que sea posible plantear, a manera de cierre, una propuesta de aplicación que permita agilizar el proceso de lectura realizado por los estudiantes de Derecho en ese espacio.

Con lo dicho, el informe que se presenta a continuación, realizado a manera de avance de este proceso de investigación conjunta, consta de tres partes: 1), una descripción sucinta de los aspectos metodológicos más destacables de los dos frentes de la investigación; 2), una presentación de los avances alcanzados hasta el momento en el desarrollo de dicho proceso; y 3) algunas reflexiones respecto de la labor adelantada y de las posibilidades que se abren torno del desarrollo del proyecto a futuro.

## Marco metodológico

Como se dijo antes, la naturaleza colaborativa del trabajo de investigación que nos ocupa consta de dos frentes y, por ende, se hace uso de dos herramientas metodológicas principales: de un lado, el modelado de tópicos como herramientas de la lingüística de corpus. Y de otro, la observación participante dirigida al proceso de gestión documental que la rama judicial realiza en torno de las tutelas; y, de modo particular, la labor de revisión y selección propia de la Corte Constitucional -esécíficamente, los judicantes (estudiantes de Derecho)-. A continuación se tratarán brevemente estos asuntos.

### Herramientas

#### Modelado de tópicos

Esta técnica de lectura distante (cuyos fundamentos se encuentran en la lingüística computacional aplicada) tiene por objetivo extraer, de corpus textuales de gran envergadura, unidades semánticas -tópicos- cuyos elementos constitutivos -*tokens*- tienen una alta probabilidad de estar relacionados entre sí (Templeton, s. f.). En términos ideales, cada tópico aludiría a una temática específica y, con esto, se asumiría que cada texto del corpus tiene origen en una mezcla de dichas unidades semánticas. 

Para el caso que nos ocupa, se tomó la decisión de emplear para esta labor un algoritmo de uso gratuito y gran aceptación en el ámbito académico, llamado Latent Dirichlet Allocation (LDA); de modo concreto, se empleó una herramienta que se sirve de LDA: Mallet, concebida por la Universidad De Massachussets. Nótese que, salvo ajustes básicos, esta realización del algoritmo es mayormente "no supervisada" (*unsupervised*), es decir, el usuario tiene poco control sobre los parámetros del análisis; no obstante, ostenta un rasgo que le confiere cierta ventaja frente a otras aplicaciones de su tipo (y que, en nuestro caso, fue determinante para su elección): permite configurar y emplear listas de palabras vacías (*stopwords*) personalizadas, condición necesaria en análisis de este tipo.

#### Trabajo en campo

Respecto de este punto, se emplearon herramientas propias de la investigación cualitativa para componer dos ejercicios: primero, dos mapas mentales, uno para conocer a los actores involucrados de forma directa en el proceso de selección de tutelas de la Corte Constitucional, y otro para describir el marco regulatorio aplicable al proceso de selección; y segundo, una caracterización tipológica del proceso constitucional de selección de la tutela mediante diagramas de flujo digitales de las instancias procesales, con sus correspondientes tareas en materia de gestión documental. Se hicieron entonces cuatro diagramas de flujo para mostrar el recorrido del expediente de tutela desde el momento en que se radica por primera vez (en el juzgado de origen) hasta que arriba y es radicado nuevamente en la Corte Constitucional. 

En el marco de esta labor de investigación de campo, se han realizado visitas a nueve sedes judiciales y relatorías de Bogotá; a la Corte Constitucional (en 2 ocasiones); a la Defensoría del Pueblo; y a la Procuraduría General de la Nación.  Aparte de ser este el medio por el cual se acopiaron los documentos que componen el corpus analizado a través del modelado de tópicos, las visitas dieron lugar a la composición de los diagramas de flujo mencionados. En ellas se han empleado instrumentos básicos, propios de la observación participante pasiva: entrevistas, fotografías (disponibles [aquí](http://mariafernandaguerreromateus.omeka.net/)) y diarios de campo (disponibles en [https://bit.ly/2QIHZIT](https://bit.ly/2QIHZIT))

#### Muestra

La colección de documentos acopiada para efectos del modelado de tópicos consta de xxxxx fallos de tutela de primera y segunda instancias, recogidos en las visitas a las sedes judiciales. Para efectos del análisis cuyos resultados se mostrarán en la siguiente sección, se empleó un corpus de prueba compuesto por 900 de esos fallos, que cubren el periodo 2010-2018, debidamente organizados de acuerdo con criterios establecidos por los suscritos investigadores.

Dado el carácter altamente desestructurado de esta colección de documentos (*i. e.* nomenclaturas confusas, multiplicidad de formatos), sumado al hecho de que el uso de Mallet hace necesario disponer los archivos por analizarse bajo parámetros específicos en materia de formato y codificación (archivos de texto plano con codificación Unicode UTF-8), se hizo necesario establecer algunas  pautas básicas de organización, entre las cuales cabe mencionar las siguientes:

* Dada la mencionada ausencia de unificación en materia de formato de los archivos que componen el corpus, se hizo necesario buscar una herramienta digital que permitiera convertirlos de forma eficiente y confiable al formato requerido. En consecuencia, se decidió emplear para este menester la  aplicación Textutil: se trata de un paquete de servicios para la  conversión de archivos de texto que se ejecuta en la terminal del sistema operativo Mac OS X. Aparte de haber mostrado resultados satisfactorios en ejercicios preliminares (realizados con un corpus de prueba), se destaca de otras aplicaciones de su tipo en tanto permite convertir directorios completos.
* El hecho de que los fallos de tutela contengan secciones cuya  construcción obedece a tipologías textuales disímiles (narrativa,  descriptiva y argumentativa) hizo pensar, en principio, que los  resultados del modelado de tópicos serían más precisos si estos se  separaran en función de dichos componentes (*i. e.*  consideraciones, hechos, pretensiones, decisiones). No obstante, la gran cantidad de archivos obtenidos hasta el momento excede la capacidad  humana disponible para realizar dicha labor de segmentación (que debería realizarse manualmente, puesto que se trata  de texto no marcado). Se  optó, en consecuencia, por realizar el análisis de todos los archivos de la muestra sin segmentarlos.
* Tras múltiples intentos y discusiones en torno de la nomenclatura que se adoptaría para el corpus, se tomó la determinación de emplear la siguiente: VA IMAGEN DE LA NOMENCLATURA. No obstante, es altamente probable que esta sea modificada nuevamente, toda vez que se espera enriquecer el análisis de tal manera que estén representados en igual volumen todos los meses de los años analizados.

Una descripción más detallada de la metodología empleada para la construcción del corpus puede consultarse en [https://bit.ly/2QopqdJ](https://bit.ly/2QopqdJ). 

## Resultados preliminares

### Primer esbozo de un modelo de tópicos para fallos de tutela

Encontramos 2 grandes categorías de tópicos: 1), procesal (que tiene que ver con el proceso constitucional); 2), sustancial (derechos y deberes fundamentales, instituciones, y principios y valores constitucionales).

Hasta el momento, se han realizado 52 pruebas, todas bajo los mismos parámetros básicos, a saber: 

Archivos analizados: 900

Periodo abarcado por el corpus de prueba: 2010-2018 (100 archivos por año)

Número de palabras vacías (*stopwords*): 1360[^1]

Tópicos que componen el modelo: 20

#### Modelo de tópicos

| N.° de tópico | “Peso” estadístico | Tokens (en orden de importancia)                             |
| ------------- | ------------------ | :----------------------------------------------------------- |
| 0             | 0,06327            | unidad víctimas reparación integral ayuda   humanitaria vivienda administrativa petición social accionada indemnización   derecho población fallo desplazada sentencia familiar desplazamiento   subsidio |
| 1             | 0,04173            | superintendencia sociedad comercio sociedades liquidación intervención   industria medida accionada artículo posesión personas empresa legal   accionantes cámara captación actividades financiera trabajo |
| 2             | 0,03947            | nacional información datos registraduría obligación cédula registro   artículo riesgo paz ciudadanía policía electoral congreso negativo refinancia   ciudadanos voto refrendación fuente |
| 3             | 0,43114            | petición derecho acción fondo fundamental solicitud accionada término   decisión artículo accionante autoridad amparo resolución obtener notificación   caso parte ministerio dar |
| 4             | 0,03359            | régimen pensiones transición artículo edad prima traslado derecho media   ahorro pensión social prestación individual sentencia personas vejez iss   pensional sistema |
| 5             | 0,10175            | juzgado inmueble proceso diligencia municipal judicial propiedad   secuestro registro predio medida accionado descongestión conciliación   artículo debido parte cautelar matrícula actuación |
| 6             | 0,04491            | penal proceso fiscalía artículo nación medida juez público libertad penas   ministerio investigación aseguramiento seguridad control pena fiscal   funciones víctima debido |
| 7             | 0,04596            | contrato artículo demandante vehículo pago demanda proceso promesa   compraventa demandado incumplimiento nulidad parte negocio resolución pública   escritura laboral disenso vendedor |
| 8             | 0,14492            | acción judicial juzgado fundamentales defensa amparo decisión trámite   protección persona término judiciales proceso inmediatez instancia juez causa   accionante hechos caso |
| 9             | 0,03939            | crédito fondo ahorro cuotas nacional proceso debido vivienda sentencia   sistema deudor pesos fna contrato plazo uvr hipotecario pactado   consentimiento modificación |
| 10            | 0,6356             | sala decisión acción accionante judicial amparo magistrado instancia   protección sentencia autoridad magistrada justicia proceso fallo juzgado   impugnación antecedentes nombre fundamentales |
| 11            | 0,0523             | nacional servicio educación militar convocatoria policía artículo   ejército profesional comisión concurso proceso universidad cnsc institución   programa retiro accionante laboral personal |
| 12            | 0,08859            | banco proceso remate crédito debido valor diligencia pago avalúo   hipotecario obligación dictamen acreedor dian inmueble liquidación garantía   cautelares objeción cobro |
| 13            | 0,12               | proceso sentencia juez juzgado prueba accionante decisión restitución   arrendamiento contrato debido derecho demandado valoración municipal   judiciales fallo demanda procesal justicia |
| 14            | 0,0503             | desacato incidente fallo trámite juez orden unidad sentencia providencia   reparación sanción nulidad consulta integral juzgado persona incumplimiento   responsabilidad sanciones responsable |
| 15            | 0,30215            | acción mecanismo defensa protección judicial perjuicio fundamentales   irremediable derecho amparo accionante evitar jurisdicción transitorio   administrativo juez decisión resolución decreto persona |
| 16            | 0,1786             | accionante sala fallo juez decisión demanda amparo juzgado accionado   impugnado impugnación magistrados decida solicitud nombre magistrado justicia   protección antecedentes autoridad |
| 17            | 0,06286            | salud eps servicio médico servicios tratamiento vida social paciente   tratante pos integral fosyga prestación accionada médicos sentencia   medicamentos parte seguridad |
| 18            | 0,09267            | pensión pago social reconocimiento laboral mínimo pensional sentencia   colpensiones invalidez vital artículo seguridad liquidación incapacidades   cajanal calificación prestaciones sociales nacional |
| 19            | 0,37653            | proceso juzgado decisión judicial sentencia juez acción artículo parte   recurso providencia derecho debido actuación municipal accionado judiciales   trámite defensa fundamentales |

#### Comportamiento de los tópicos

Las siguientes visualizaciones muestran, de un lado, la relevancia adquirida por cada tópico del modelo en cada uno de los archivos analizados —esto es, su *comportamiento* o relevancia y, con ello, su composición discursiva—; y de otro, una comparación entre los promedios de comportamiento calculados para cada tópico por año, organizada en orden ascendente (es decir, aquellos tópicos con comportamientos promedio más altos se ubican en la parte baja). 

##### Comportamientos promedio por año

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\promedio-topicos.jpg)

##### Comportamiento de cada tópico por año

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-0.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-1.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-2.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-3.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-4.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-5.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-6.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-7.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-8.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-9.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-10.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-11.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-12.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-13.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-14.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-15.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-16.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-17.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-18.JPG)

![](F:\informe-avance-diseno-proyectos\imagenes\visualizaciones-topicos\topico-19.JPG)

### Caracterización tipológica de procesos y actores involucrados en el trámite de las acciones de tutela en la rama judicial

A partir de lo recogido en las visitas de campo, y realizada una labor de contraste entre lo establecido en las normativas oficiales y lo visto *in situ*, se compusieron los siguientes diagramas de flujo; estos dan cuenta del proceso adelantado en la rama judicial para dar trámite a todas las acciones de tutela. Si bien nuestro interés se centra en la labor de la Corte Constitucional, componer el recorrido completo proporciona una visión de contexto de suma utilidad para componer una propuesta de aplicación como la que se pretende.

#### Ingreso de la tutela al sistema judicial

![d-flujo-reparto1](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-reparto_1.jpg)

![d-flujo-reparto2](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-reparto_2.jpg)

#### Proceso de tutela en primera instancia ante los juzgados

![diagrama-flujo-primera-instancia1](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-primera-instancia_1.jpg)

![diagrama-flujo-primera-instancia2](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-primera-instancia_2.jpg)

![diagrama-flujo-primera-instancia3](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-primera-instancia_3.jpg)

![diagrama-flujo-primera-instancia4](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-primera-instancia_4.jpg)

#### Apelación o segunda instancia

![d-flujo-segunda-instancia1](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-segunda-instancia_1.jpg)

![d-flujo-segunda-instancia2](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-segunda-instancia_2.jpg)

#### Proceso de revisión y selección en la Corte

![d-flujo-corte1](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-corte-const_1.jpg)

![d-flujo-corte2](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-corte-const_2.jpg)

### Primer intento de categorización del modelo de tópicos: clasificación en función de derechos

He aquí el puente entre los saberes lingüístico y jurisprudencial. Una vez obtenido el modelo de tópicos que se presentó anteriormente, y vistas otras experiencias académicas al respecto, surgió la idea de reemplazar los números con los que se identifican los tópicos por etiquetas asignadas con base en una interpretación de los mismos en función de su valor semántico y jurisprudencial. 

Con lo anterior, encontramos que los tópicos del modelo actual pueden dividirse, en principio: en dos grandes categorías: 

1. Tópicos de carácter **procesal**: comprenden información respecto del proceso judicial de la tutela y, por ende, su presencia y relevancia en todos los archivos del corpus analizado es constante, hecho que explica su mayor “peso” estadístico.
2. Tópicos de carácter **sustancial**: corresponden, en esencia, a derechos vulnerados, en tanto razón de ser de la acción de tutela como proceso judicial. Constituyen, pues, el “tema de fondo” en los documentos que son objeto de análisis y, por ende, el objeto de mayor interés en el proceso de revisión realizado en la Corte Constitucional.

Dada esta categorización inicial, se planteó la posibilidad de asignar etiquetas individuales a cada tópico para reemplazar los números con los que se identifican en Mallet. Para ello, y luego de hacer una lectura inicial tanto del modelo de tópicos como de información teórica, se compuso un campo semántico referido a derechos fundamentales como primer insumo para, a posteriori, equiparar los elementos del mismo con los tópicos.



 (VA LA LISTA DE DERECHOS)

## Discusión

La investigación, hasta ahora realizada, arroja las siguientes conclusiones preliminares:

* El problema inicialmente planteado desborda los límites dentro de los cuales se planteo lo que ha significado que las expectativas en su análisis se ha hecho mucho más grandes de lo que se esperaba. Las dificultades en la consecución de la información y el descubrimiento de prácticas poco transparentes son indicativas de formas de trabajo en el que impera la discrecionalidad de juez y del personal del juzgado o tribunal.
* La insensibilidad frente a la memoria judicial, por la abrumadora cantidad de información, permea todas las instancias judiciales relacionadas con la tutela. Las oportunidades de mejora en relación con procesos de gestión documental en la rama judicial están a la espera de ser resueltas a partir de un régimen especial que claramente determine en que consisten los principios de la autonomía e independencia y la cooperación armónica entre las ramas del poder público
* Las posibilidades que se abren en relación con los campos semánticos permitirá realizar otras categorizaciones que complementen la establecida para los derechos y deberes fundamentales. Considerar las instituciones (públicas y privadas) que vulneran los derechos y los principios y valores constitucionales permitirán ampliar el espectro de análisis del modelo de tópicos e incidirá también en los métodos de  interpretación del derecho;
* La cultura organizacional que impera en las sedes judiciales necesitan nuevos aires que incentiven una cultura de la innovación desde el punto de vista gerencial como de gestión del cambio.
* La cultura jurídica se abre a nuevos paradigmas en la pedagogía de la enseñanza de los potenciales profesionales del derecho como de la formación judicial en los mecanismos de interpretación del derecho, la hermenéutica jurídica, la argumentación y razonamiento jurídico que están inmersos en formas nuevas de lectura. 
* Una armonización y adopción de buenas prácticas de gestión judicial que vincule las instancias judiciales de la tutela, desde la entrada de la información, su procesamiento y un resultado útil puede Una interoperabilidad nos está presente en el sistema de justicia
* Para las humanidades digitales es relevante estudiar la problemática que presenta la selección de tutelas, desde el momento mismo en que un ciudadano interpone su demanda de tutela, porque supone una práctica interpretativa que tiene que ver más con el significado que posee ese mecanismo procesal en el Estado Social de Derecho, que con la eficiencia en términos del número de tutelas resueltas o de tutelas seleccionadas. La interpretación del fenómeno problemático, que busca una solución en la práctica, tiene que ver con las narrativas (hechos y pretensiones ) de los ciudadanos en la vida cotidiana, sus necesidades, deseos y prioridades traducidos en derechos fundamentales vulnerados por carencias generadas por el mismo estado. Finalmente, el ciudadano es el gran artífice de la tutela y el juez constitucional es el garante.  
* El acceso a la información judicial, la anonimización de información con el propósito de proteger datos personales de acuerdo a la ley vigente.

## Notas

[^1]: Para la construcción de la lista de palabras vacías se partió del listado de base proporcionado por [Ranks.nl](https://www.ranks.nl), de uso recomendado por los autores de Mallet. Se incluyeron, además, nombres de personas con base en las listas de nombres más comunes presentes en los registros civiles de nonatos, publicadas por la Registraduría Nacional del Estado Civil para los años 2014, 2015, 2016 y 2017. Conforme se realizaron sucesivas iteraciones de las pruebas para obtener el modelo de tópicos, la lista se enriqueció con nuevos términos (en su mayoría, inflexiones verbales y adverbios) hasta alcanzar la envergadura que ostenta actualmente.
[^2]: Sumados a los diagramas de flujo, se compusieron mapas mentales como estrategia para identificar de mejor manera a todos los actores del proceso. Estos se encuentran disponibles para ser consultados en [https://bit.ly/2EqbxFA](https://bit.ly/2EqbxFA)  



#### Modelado de tópicos

Templeton, C. (2011). Topic Modeling in the Humanities: An Overview. Recuperado de [https://mith.umd.edu/topic-modeling-in-the-humanities-an-overview/.](https://mith.umd.edu/topic-modeling-in-the-humanities-an-overview/.)
