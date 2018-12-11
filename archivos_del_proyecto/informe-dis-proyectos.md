# ¿Cómo la inteligencia artificial puede mejorar el proceso de selección de tutelas en la Corte Constitucional? (informe de investigación preliminar)

*Estudiantes: María Fernanda Guerrero Mateus y Carlos Manuel Varón Castañeda*

*Fecha: 11 de diciembre de 2018*

## Introducción

La tutela es el mecanismo procesal más utilizado por los ciudadanos para defender sus derechos fundamentales. Su reconocida popularidad hace que la selección de sentencias de tutela sea, para la Corte Constitucional, su mayor desafío, en razón de los más de 42.000 expedientes mensuales que recibe de todo el país para su eventual revisión (Corte Constitucional, s. f.; El País, 2014; El Espectador, s. f.; La Patria, 2018, s. f.). Queda entonces claro que, de no atenderse adecuadamente esta situación, la complejidad que reviste la gestión de tutelas en materia de procesamiento de información podrían llevar este mecanismo del éxito al mayor de los fracasos.

Con el panorama anterior,  y dada una circunstancia afortunada de conjunción de saberes y experiencias (propiciada por el desarrollo de la Maestría en Humanidades Digitales), surgió la idea de adelantar una iniciativa de investigación – creación colaborativa para tratar de responder un pregunta que, a la vez, sirve como pilar fundamental de dicho ejercicio académico: ¿un sistema automatizado podría asistir el proceso de revisión y selección de tutelas adelantado por los judicantes (estudiantes de Derecho) en la Corte Constitucional?

Teniendo en cuenta el anterior contexto el desarrollo del trabajo de investigación, colaborativo e interdisciplinario, propone un doble acercamiento: en primer lugar, desde las humanidades digitales, el proyecto busca técnicas de lectura distante para crear una metodología que apoye la selección y posterior revisión de sentencias de tutela. En segundo lugar, desde la informática jurídica de ayuda a la decisión, el proyecto implica el uso de la tópica digital como metodología de búsqueda del saber jurídico a partir de sus fuentes y su interpretación, de conformidad con las actuales exigencias del derecho global contemporáneo (Moro, 2015; Moro & Puppo, 2010). 

Así entonces, el proyecto de investigación al que nos abocamos ostenta dos frentes: de un lado, un ejercicio de carácter experimental, cuyo objetivo es emplear la técnica de modelado de tópicos para realizar una caracterización semántica de un corpus de fallos de tutela de primera y segunda instancias, con miras a probar si el algoritmo empleado para ello permite inferir la composición temática de documentos nuevos. Y segundo, un proceso de investigación y análisis cualitativo respecto de la manera como se llevan a cabo los procesos constitucional y de gestión documental en la Corte Constitucional en relación con las tutelas, de tal manera que sea posible plantear, a manera de producto final, una propuesta de aplicación que permita agilizar el proceso de lectura, interpretación y argumentación del caso realizado por los estudiantes de Derecho en esa dependencia, quienes tienen a su cargo elaborar las reseñas temáticas que luego serán insumo para la labor de selección que efectúa la Sala de revisión.

Con lo dicho, el informe que se presenta a continuación, realizado a manera de avance de este proceso de investigación conjunta, consta de tres partes: 1), una descripción sucinta de los aspectos metodológicos más destacables de los dos frentes de la investigación; 2), una presentación de los avances alcanzados hasta el momento en el desarrollo de dicho proceso; y 3) algunas reflexiones respecto de la labor adelantada y de las posibilidades que se abren torno del desarrollo del proyecto a futuro.

## Marco metodológico

Como se dijo antes, la naturaleza colaborativa del trabajo de investigación que nos ocupa consta de dos frentes y, por ende, se hace uso de dos herramientas metodológicas principales: de un lado, el modelado de tópicos como herramientas de la lingüística de corpus. Y de otro, la observación participante dirigida al proceso de gestión documental que la rama judicial realiza en torno de las tutelas; y, de modo particular, la labor de revisión y selección propia de la Corte Constitucional. A continuación se tratarán brevemente estos asuntos.

### Herramientas

#### Modelado de tópicos

Esta técnica de lectura distante (cuyos fundamentos se encuentran en la lingüística computacional aplicada) tiene por objetivo extraer, de corpus textuales de gran envergadura, unidades semánticas -tópicos- cuyos elementos constitutivos -*tokens*- tienen una alta probabilidad de estar relacionados entre sí (Templeton, s. f.). En términos ideales, cada tópico aludiría a una temática específica y, con esto, se asumiría que cada texto del corpus tiene origen en una mezcla de dichas unidades semánticas. 

Para el caso que nos ocupa, se tomó la decisión de emplear para esta labor un algoritmo de uso gratuito y gran aceptación en el ámbito académico, llamado Latent Dirichlet Allocation (LDA); de modo concreto, se empleó una herramienta que se sirve de LDA: Mallet, concebida por la Universidad De Massachussets. Nótese que, salvo ajustes básicos, esta realización del algoritmo es mayormente "no supervisada" (*unsupervised*), es decir, el usuario tiene poco control sobre los parámetros del análisis; no obstante, ostenta un rasgo que le confiere cierta ventaja frente a otras aplicaciones de su tipo (y que, en nuestro caso, fue determinante para su elección): permite configurar y emplear listas de palabras vacías (*stopwords*) personalizadas, condición necesaria en análisis de este tipo.

#### Trabajo en campo

Respecto de este punto, se emplearon herramientas propias de la investigación cualitativa para componer dos ejercicios: primero, dos mapas mentales, uno para conocer a los actores involucrados de forma directa en el proceso de selección de tutelas de la Corte Constitucional, y otro para describir el marco regulatorio aplicable al proceso de selección[^2]; y segundo, una caracterización tipológica del proceso constitucional de selección de la tutela mediante diagramas de flujo digitales de las instancias procesales, con sus correspondientes tareas en materia de gestión documental. Se hicieron entonces cuatro diagramas de flujo para mostrar el recorrido del expediente de tutela desde el momento en que se radica por primera vez (en el juzgado de origen) hasta que arriba y es radicado nuevamente en la Corte Constitucional. 

En el marco de esta labor de investigación de campo, se han realizado visitas a nueve sedes judiciales y relatorías de Bogotá; a la Corte Constitucional (en 2 ocasiones); a la Defensoría del Pueblo; y a la Procuraduría General de la Nación.  Aparte de ser este el medio por el cual se acopiaron los documentos que componen el corpus analizado a través del modelado de tópicos, las visitas dieron lugar a la composición de los diagramas de flujo mencionados. En ellas se han empleado instrumentos básicos que son propios de la observación participante pasiva (Sandoval, 1996, pp. 118-127): entrevistas, fotografías (disponibles [aquí](http://mariafernandaguerreromateus.omeka.net/)) y diarios de campo (disponibles en [https://bit.ly/2QIHZIT](https://bit.ly/2QIHZIT))

#### Muestra

La colección de documentos acopiada para efectos del modelado de tópicos consta de xxxxx fallos de tutela de primera y segunda instancias, recogidos en las visitas a las sedes judiciales. Para efectos del análisis cuyos resultados se mostrarán en la siguiente sección, se empleó un corpus de prueba compuesto por 900 de esos fallos, que cubren el periodo 2010-2018, debidamente organizados de acuerdo con criterios establecidos por los suscritos investigadores.

Dado el carácter altamente desestructurado de esta colección de documentos (*i. e.* nomenclaturas confusas, multiplicidad de formatos), sumado al hecho de que el uso de Mallet hace necesario disponer los archivos por analizarse bajo parámetros específicos en materia de formato y codificación (archivos de texto plano con codificación Unicode UTF-8), se hizo necesario establecer algunas  pautas básicas de organización, entre las cuales cabe mencionar las siguientes:

* Dada la mencionada ausencia de unificación en materia de formato de los archivos que componen el corpus, se hizo necesario buscar una herramienta digital que permitiera convertirlos de forma eficiente y confiable al formato requerido. En consecuencia, se decidió emplear para este menester la  aplicación Textutil: se trata de un paquete de servicios para la  conversión de archivos de texto que se ejecuta en la terminal del sistema operativo Mac OS X. Aparte de haber mostrado resultados satisfactorios en ejercicios preliminares (realizados con un corpus de prueba), se destaca de otras aplicaciones de su tipo en tanto permite convertir directorios completos.
* El hecho de que los fallos de tutela contengan secciones cuya  construcción obedece a tipologías textuales disímiles (narrativa,  descriptiva y argumentativa) hizo pensar, en principio, que los  resultados del modelado de tópicos serían más precisos si estos se  separaran en función de dichos componentes (*i. e.*  consideraciones, hechos, pretensiones, decisiones). No obstante, la gran cantidad de archivos obtenidos hasta el momento excede la capacidad  humana disponible para realizar dicha labor de segmentación (que debería realizarse manualmente, puesto que se trata  de texto no marcado). Se  optó, en consecuencia, por realizar el análisis de todos los archivos de la muestra sin segmentarlos.
* Tras múltiples intentos y discusiones en torno de la nomenclatura que se adoptaría para el corpus, se tomó la determinación de emplear la siguiente: VA IMAGEN DE LA NOMENCLATURA. No obstante, es altamente probable que esta sea modificada nuevamente, toda vez que se espera enriquecer el análisis de tal manera que estén representados en igual volumen todos los meses de los años analizados.

Una descripción más detallada de la metodología empleada para la construcción del corpus puede consultarse en [https://bit.ly/2QopqdJ](https://bit.ly/2QopqdJ). 

## Resultados preliminares

### Primer esbozo de un modelo de tópicos para fallos de tutela

Hasta el momento se han realizado 52 pruebas, todas bajo los mismos parámetros básicos, a saber: 

Archivos analizados: 900

Periodo abarcado por el corpus de prueba: 2010-2018 (100 archivos por año)

Número de palabras vacías (*stopwords*): 1360[^1]

Tópicos que componen el modelo: 20

Se expone a continuación la versión más reciente del modelo de tópicos construido a través de las iteraciones sucesivas de las pruebas con los parámetros expuestos.

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

### Caracterización tipológica de procesos que componen el trámite de las tutelas en la rama judicial

A partir de lo recogido en las visitas de campo, y realizada una labor de contraste entre lo establecido en las normativas oficiales y lo visto *in situ*, se compusieron los siguientes diagramas de flujo y mapas mentales: estos dan cuenta del proceso adelantado en la rama judicial para dar trámite a todas las acciones de tutela, por un lado; y de los actores y la normativa oficial involucrados en el proceso de selección adelantado en la Corte Constitucional, por otro. Si bien nuestro interés se centra en la labor de la Corte Constitucional, componer el recorrido completo proporciona una visión de contexto de suma utilidad para componer una propuesta de aplicación como la que se pretende.

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

![d-flujo-corte2](F:\informe-avance-diseno-proyectos\imagenes\diagramas-flujo\diagrama-flujo-corte-const_2.jpg)Sobre este último proceso, y dado el objeto de interés para esta investigación, es necesario puntualizar algunos asuntos respecto de la labor de los estudiantes de Derecho en la Corte. En su quehacer, estos últimos componen documentos que reciben el nombre de reseñas esquemáticas, considerados por la Corte instrumentos de trabajo de carácter secundario para el proceso de selección. Las reseñas conforman el insumo cognitivo que condensa los aspectos más relevantes que deben tener en cuenta los magistrados encargados de la selección para tomar la decisión respecto a su relevancia como caso emblemático que debe someterse a revisión. 

Entre 1992 y 2006, las reseñas se elaboraron en papel; y desde 2006 a la fecha, se diligencian mediante una aplicación informática cuyo diseño estuvo a cargo de la dependencia de sistemas de la Corte[^3]. La reseña no se encuentra catalogada en la tabla de retención documental que relaciona los documentos relevantes procesalmente hablando. En años recientes, el Archivo Central de la Corte y la Secretaría General decidieron digitalizar las reseñas elaboradas en papel e integrarlas a la base de datos de gestión de la corporación. El formato para componerlas, que existe desde los inicios de la Corte Constitucional, está dividido de la siguiente manera: 

1. Datos de identificación del caso
   - Fecha
   - Número de expediente
   - Demandante
   - Demandado
   - Juez de primera instancia
   - Juez de segunda instancia
   - Derecho fundamental vulnerado
   - Datos del demandante (sexo, etnia, condición de vulnerabilidad, etc.)

2. Caracterización
   - Hechos de la demanda
   - Primera instancia
   - Segunda instancia
   - Impugnación
   - Segunda instancia
   - Datos del despacho del magistrado
   - Datos sobre la preselección para revisión

3. Criterios orientadores
   - Objetivos
   - Observaciones
   - Problema jurídico

4. Observaciones

### Primer intento de categorización del modelo de tópicos: clasificación en función de derechos

He aquí el puente entre los saberes lingüístico y jurisprudencial. Una vez obtenido el modelo de tópicos que se presentó anteriormente, y vistas otras experiencias académicas al respecto, surgió la idea de reemplazar los números con los que se identifican los tópicos por etiquetas asignadas con base en una interpretación de los mismos en función de su valor semántico y jurisprudencial. 

Con lo anterior, encontramos que los tópicos del modelo actual pueden dividirse, en principio: en dos grandes categorías: 

1. Tópicos de carácter **procesal**: comprenden información respecto del proceso judicial de la tutela y, por ende, su presencia y relevancia en todos los archivos del corpus analizado es constante, hecho que explica su mayor “peso” estadístico.
2. Tópicos de carácter **sustancial**: corresponden, en esencia, a derechos vulnerados, en tanto razón de ser de la acción de tutela como proceso judicial. Constituyen, pues, el “tema de fondo” en los documentos que son objeto de análisis y, por ende, el objeto de mayor interés en el proceso de revisión realizado en la Corte Constitucional.

Dada esta categorización inicial, se planteó la posibilidad de asignar etiquetas individuales a cada tópico para reemplazar los números con los que se identifican en Mallet. Por ello se optó por considerar la elaboración de una categorización que enriqueciera la lectura de los textos y, por ende, su búsqueda en un contexto de datos masivos como el que corresponde a las sentencias de tutela que integran el corpus analizado. Se pensó, entonces, en equiparar los tópicos que identificamos como sustanciales con derechos y deberes fundamentales.

Para elaborar la categorización se tomaron en cuenta clasificaciones que trae el texto de la misma Constitución y que han sido desarrolladas por la jurisprudencia y la doctrina constitucional sobre el tema de los derechos fundamentales, como objeto de protección a través de la acción de tutela. Como producto de ese análisis se esbozaron cuatro gráficos que contienen distintas clasificaciones. Después de un análisis más detenido optamos por considerar un listado que elaboramos a partir de una lista de temas organizada por la relatoría de la Corte Constitucional, a saber:

**Derechos fundamentales (de aplicación inmediata)**

* derecho a la vida
  * del bebe prematuro
  * del desplazado por la violencia
  * de docente
  * de ex soldado
  * del menor de edad
  * de mujeres defensoras de derechos humanos
  * de personas de la tercera edad
  * de personas discapacitadas
  * de persona incluida en el programa de protección de víctimas, testigos, intervinientes en proceso penal
  * del personal docente
  * de víctimas del conflicto armado;
  * de víctimas de violencia física a compañera permanente
  * de víctimas de violencia para devolución de dineros
  * del interno
  * del no nacido
  * del menor adulto
  * del menor
  * del nasciturus frente al aborto
  * del niño
  * del no nacido
  * del pensionado
  * del trabajador
  * del soldado bachiller
  * del disminuido psiquico
  * del menor discapacitado
  * de persona en condición de discapacidad
  * de la persona enferma
    * que requiere medicamentos para el corazón
    * que requiere medicamentos sustituto eficaz previa autorización del médico tratante
    * que requiere diagnóstico
    * que requiere tratamiento no incluido en el POS
    * que requiere tratamiento de aneurisma cerebral por la medicina 						prepagada
    * que requiere tratamiento de hemodiálisis
    * que requiere tratamiento sin condicionarlo al pago compartido
    * que requiere tratamiento sin cumplir periodo mínimo de cotización
    * que requiere tratamiento de diálisis sin cumplir periodo mínimo de cotización en personas de escasos recursos
    * que requiere tratamiento
    * que requiere traslado
* Derecho a la vida digna
  * del adulto mayor
  * del disminuido psíquico
  * del menor discapacitado
  * del menor
  * de la mujer embarazada cabeza de familia
  * de persona con discapacidad auditiva
  * de la persona de la tercera edad
  * de la persona en condición de discapacidad
  * de la persona inválida
  * de persona en situación de debilidad manifiesta
  * del adolescente
  * del disminuido físico
  * del enfermo mental
  * del menor con síndrome de Down
  * del recluso con discapacidad
  * del niño
  * del niño discapacitado
  * del interno
  * del pensionado
  * del trabajador
* Derecho a la integridad personal
  * de mujeres defensoras de derechos humanos
  * de mujeres desplazadas
  * del interno
  * del menor
  * de cónyuges
  * del menor de edad
  * del padre alcohólico   
  * de personas detenidas

**Deberes fundamentales**

- de las autoridades públicas frente a los derechos
- de los particulares en materia de orden público
- de los particulares frente a los derechos constitucionales
- de los municipios relacionados con el aprovisionamiento y servicio público de aseo
- asociados a la protección de los animales
- de los ciudadanos
- de los medios de comunicación
- de las autoridades en orden público y seguridad
- de asistencia y solidaridad de las comunidades religiosas
- del juez en el desarrollo del proceso penal
- de la administración de justicia
- de la administración pública
- de la empresa
- de la familia frente al derecho a la educación
- de la persona y el ciudadano
- de las autoridades de policía
- de las compañías aseguradoras
- de las partes procesales y el apoderado
- de los funcionarios de la rama judicial
- de los padres de familia
- del abogado
- del comerciante al expedir factura
- del conyuge
- del empleador
- del fondo de pensiones
- del estado en materia salarial
- del estado frente a las víctimas por el cambio climático
- del estado frente al derecho a la educación
- del estado frente al acceso a la justicia penal
- del estado frente a los desastres naturales
- del estado frente a los menores de edad
- del estudiante
- del extranjero en conmoción interior
- del funcionario público
- del funcionario judicial
- del médico
- del juez
- del servicio público
- del profesional


## Discusión

El proceso de análisis en los dos frentes de trabajo permite realizar algunas reflexiones preliminares, que nos permitimos compartir aquí.

* El problema planteado reviste un grado de complejidad que supera con creces lo previsto, tanto desde lo informacional y lingüístico como desde lo organizacional. Sumado a ello, las dificultades en la consecución de la información y el descubrimiento de prácticas poco transparentes son indicativas de formas de trabajo en las que imperan la discrecionalidad de juez y del personal del juzgado o tribunal.
* La insensibilidad frente a la memoria judicial, dada por la abrumadora cantidad de información, permea todas las instancias judiciales relacionadas con la tutela. Las oportunidades de mejora en relación con procesos de gestión documental en la rama judicial están a la espera de ser resueltas, a partir de un régimen especial que determine en qué consisten los principios de la autonomía e independencia y la cooperación armónica entre las ramas del poder público. A este respecto, la cultura organizacional que impera en las sedes judiciales necesita nuevos aires, que incentiven una cultura de la innovación desde los puntos de vista gerencial y de gestión del cambio.
* La clasificación misma de los derechos y deberes fundamentales ha probado ser otro desafío, en virtud de la multiplicidad de interpretaciones y lecturas que existen al respecto. Sobre este punto, considerar las instituciones (públicas y privadas) que vulneran los derechos y los principios y valores constitucionales permitirán ampliar el espectro de análisis del modelo de tópicos, e incidirá también en los métodos de  interpretación del derecho mismo. Es muy probable, por tanto, que tanto la lista mostrada como el modelo de tópicos propiamente dicho se expandan a futuro.
* La cultura jurídica se abre a nuevos paradigmas en lo que atañe a, de un lado, la enseñanza del Derecho a los futuros profesionales de esta disciplina; y de otro, a la formación judicial en materias de mecanismos de interpretación del derecho, hermenéutica jurídica, argumentación y razonamiento jurídico, inmersos todos ellos en formas nuevas de lectura. 
* las instancias judiciales de la tutela —y de modo más amplio, la rama judicial en su conjunto— no ostentan vínculos reales en términos operativos: la adopción y regulación de procesos obedece al criterio particular de cada sede judicial. El éxito de una estrategia como la que se pretende esbozar con esta iniciativa debería partir, en primer término, de propender a adoptar mejores prácticas de trabajo y cooperación y gestión judicial en este sentido. 
* Para las humanidades digitales es relevante estudiar la problemática que presenta la selección de tutelas desde el momento mismo en que un ciudadano interpone su demanda de tutela, porque supone una práctica interpretativa que tiene que ver con el significado que posee ese mecanismo procesal en el Estado Social de Derecho, más que con la eficiencia en términos del número de tutelas resueltas o seleccionadas. La interpretación del fenómeno problemático, que busca una solución en la práctica, tiene que ver con las narrativas (hechos y pretensiones ) de los ciudadanos en la vida cotidiana, esto es, sus necesidades, deseos y prioridades, traducidos en derechos fundamentales vulnerados por carencias generadas desde el mismo Estado. El ciudadano es, entonces, el gran artífice de la tutela; y el juez constitucional es el garante.  
* Hasta ahora, el algoritmo empleado en la composición del modelo de tópicos ha demostrado ser una herramienta útil para establecer las unidades temáticas que componen los documentos del corpus analizado. Ahora bien, no se ha probado aún su capacidad de inferencia, esto es, de establecer la composición de documentos nuevos con precisión a partir del modelo entrenado previamente. La tarea que se presenta ante nosotros consistirá, entonces, en efectuar dicha validación.

## Notas

[^1]: Para la construcción de la lista de palabras vacías se partió del listado de base proporcionado por [Ranks.nl](https://www.ranks.nl), de uso recomendado por los autores de Mallet. Se incluyeron, además, nombres de personas con base en las listas de nombres más comunes presentes en los registros civiles de nonatos, publicadas por la Registraduría Nacional del Estado Civil para los años 2014, 2015, 2016 y 2017. Asimismo, no se tomaron en cuenta los datos de personas y sujetos procesales. Conforme se realizaron sucesivas iteraciones de las pruebas para obtener el modelo de tópicos, la lista se enriqueció con nuevos términos (en su mayoría, inflexiones verbales y adverbios) hasta alcanzar la envergadura que ostenta actualmente.

[^2]: Sumados a los diagramas de flujo, se compusieron mapas mentales como estrategia para identificar de mejor manera a todos los actores del proceso. Estos se encuentran disponibles para ser consultados en [https://bit.ly/2EqbxFA](https://bit.ly/2EqbxFA)  

[^3]: Es importante tener en cuenta que las reseñas no están incluidas en las tablas de retención documental del proceso de revisión y selección de tutelas dado que, en términos formales, los estudiantes no son considerados actores directos en dicho proceso por la Corte; su labor se toma como secundaria y de asistencia, si bien la realidad deja en evidencia lo contrario. 



#### Referencias

Corte Constitucional (s. f.). Número de tutelas resueltas por la Corte desde el 2005. Recuperado de: http://www.corteconstitucional.gov.co/noticia.php?CORTE-LLEGA-A-REVISION-DEL-EXPEDIENTE-CINCO-MILLONES-2572

Corte Constitucional (s. f.). Se radica en la Corte Constitucional la tutela número 7 millones. Recuperado de: http://www.corteconstitucional.gov.co/inicio/Tutela%20numero%207%20millones.php

El Espectador (s. f.). La primera tutela tramitada digitalmente llega a la Corte Constitucional. Recuperado de https://www.elespectador.com/noticias/judicial/la-primera-tutela-tramitada-digitalmente-llega-la-corte-constitucional-articulo-726920

El País (2014, 15 de julio). El edificio de la Corte puede colapsar por cantidad de tutelas. Recuperado de: https://www.elpais.com.co/colombia/edificio-de-la-corte-constitucional-puede-colapsar-por-cantidad-de-tutelas.html

La Patria (2018, 30 de septiembre). 7 millones de tutelas, una alerta de violación de derechos. Recuperado de: http://www.lapatria.com/nacional/7-millones-de-tuteles-una-alerta-de-violacion-de-derechos-424131

Moro, P. (2015). *Topica digitale e ricerca del diritto. Metodologia e informatica giuridica nell’era dell’infosourcing*. Turín: G. Giappichelli Editore.

Moro P. & Puppo, F. (2010). Informatica giuridica y retorica forense. Recuperado de https://www.openstarts.units.it/bitstream/10077/3540/1/Tigor_3_moro_puppo.pdf

Sandoval, C. (1996). *Investigación cualitativa*. Bogotá: Icfes.

Templeton, C. (2011). Topic Modeling in the Humanities: An Overview. Recuperado de [https://mith.umd.edu/topic-modeling-in-the-humanities-an-overview/.](https://mith.umd.edu/topic-modeling-in-the-humanities-an-overview/.)
