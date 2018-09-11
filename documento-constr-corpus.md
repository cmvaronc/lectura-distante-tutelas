# Construcción de corpus para el análisis

## 1. Consecución de la información

La selección de tutelas por parte de la Corte Constitucional se efectúa sobre un cúmulo importante de sentencias de tutelas dictadas por los jueces en los juzgados y tribunales de todo el país. De acuerdo a la última estadística del Consejo Superior de la Judicatura llegan a la Corte mensualmente 40 mil expedientes al mes de los cuales 20 pueden ser radicados. No obstante los fallos de la tutelas no pudieron obtenerse de la misma Corte Constitucional, que recibe todos los expedientes para su eventual revisión.

Así las cosas para construir el Corpus tuvimos que acudir a las siguientes fuentes: i) La Gaceta de la Corte Constitucional en físico (1992) para realizar una prueba a partir del análisis de las primeras 15 sentencias. ii) La relatoría de la Corte Constitucional para encontrar la base de datos que nos permitiera hacer el contraste con el corpus. iii) Las secretarías de los Juzgados que son la puerta de entrada de las demandas de tutelas y, por ende, la fuente original que produce el fallo que luego llega a la Corte. iv) Las relatorías de los tres Tribunales (Superior de Bogotá, Contencioso administrativo de Cundinamarca y Superior de Cundinamarca). v) Dos Tribunales fuera de Bogotá ( Pereira y Medellín). 

5.- Obtenida la información encontramos las siguientes dificultades: 
i)	Los textos originales se encuentran en físico y en formatos no editables que tuvieron que depurarse y convertirlos en texto plano. 

ii)	Los textos originales en papel solamente se encuentran en las secretarias de los juzgados, donde reposan los expedientes de la tutela. La búsqueda de los fallos, a través del Sistema Justicia Siglo XXI del CSJ, se hace imposible debido a que se desconocen los datos que piden para hacer la búsqueda. Cada Juzgado hace un manejo muy propio de la gestión documental, no se acata la ley de archivos, existen distintas formas de registrar y almacenar la información y no se cuenta con relatorías por lo que requerimos de contactos personales para poder obtenerlas. En algunos casos se obtuvieron ejerciendo el derecho de petición, en otros simplemente acercándose a la secretaría con una USB y firmando una planilla. 

iii)	La información de los fallos de tutela se encuentra en Internet, pero la búsqueda relativamente eficiente solamente opera para los fallos de la Corte Constitucional. En el caso de los Tribunales, la información se encuentra en Boletines en PDF, no editables.

iv)	La posible incapacidad de hacer un modelo de tópicos por componentes debido a la gran cantidad de información obtenida(8247 archivos, 5 formatos distintos). 

## 2. Composición del corpus

### 2.1. Diseño de la muestra

Vista la envergadura del universo de información que se enfrenta en un ejercicio de investigación – creación como el propuesto, ha sido claro desde el inicio que el volumen de documentos que compondrían la muestra sería arbitrario. Así entonces, la representatividad de la muestra no estará dada por el valor numérico absoluto frente a la totalidad del universo de información, sino por la capacidad que esta tenga para reflejar las tendencias de uso de la lengua (de acuerdo con la conceptualización de Biber [1991]) que, a posterioridad, se evidenciarán mediante el modelado de tópicos.

Nótese en este punto que la jurisprudencia emitida por la Corte Constitucional desde su creación (en 1991) asciende a 25.000 documentos, aproximadamente. Con esto, y para atender lo expresado en el párrafo anterior, se tomó la decisión de componer una muestra aleatorizada de 250 expedientes, obtenidos de un conjunto de 500 que serán recabados de los archivos de los juzgados . La muestra, entonces, ostentará una envergadura equivalente al 1 % del total de documentos que componen la jurisprudencia de la Corte.

El hecho de que los expedientes de tutela ostenten secciones cuya construcción obedece a tipologías textuales disímiles (narrativa, descriptiva y argumentativa) podría sesgar los resultados del modelado de tópicos. Por tal motivo, se tomó la decisión de separarlos por componentes (i. e. consideraciones, hechos, provisiones, decisiones), de tal manera que se produzca un modelo de tópicos para cada uno.

### 2.2. Sistematización de la muestra

Tras haber establecido las características generales de la muestra, corresponde tomar decisiones respecto de la manera como se organizará el acervo de información para el análisis; a continuación, se describen con más detalle estos asuntos.

#### 2.2.1. Formato

El algoritmo que se empleará para construir el modelo de tópicos (Mallet) exige trabajar con archivos de texto plano y codificación Unicode (UTF-8). Ahora bien, dado el carácter desestructurado de la información de la muestra (archivos en formatos de texto enriquecido, en incluso de imagen), se ha hecho necesario buscar herramientas digitales que permitan convertirla de forma eficiente y confiable al formato requerido. En consecuencia, se decidió emplear para este menester la aplicación Textutil: se trata de un paquete de servicios para la conversión de archivos de texto que se ejecuta en la terminal del sistema operativo Mac OS X. Aparte de haber mostrado resultados satisfactorios en ejercicios preliminares (realizados con el corpus de prueba), se destaca de otras aplicaciones de su tipo en tanto permite convertir directorios completos.  

#### 2.2.2. Gestión de archivos

Encontrar un elemento que sirviese como clasificador único para nombrar los archivos ha resultado ser una tarea más complicada de lo que se pensó en principio, máxime si se toma en cuenta que cada expediente se dividirá en componentes (que a su turno constituirán archivos individuales). En este sentido, se creyó prudente recurrir a la clasificación dada desde los juzgados a los expedientes, con lo cual se tomarán los siguientes elementos para nombrar los archivos:

![nomenclatura-archivos](https://github.com/cmvaronc/lectura-distante-tutelas/blob/master/nomenclatura-archivos.png)
 
La configuración de una estructura de carpetas para el almacenamiento de los archivos, por su parte, tampoco ha estado exenta de discusiones. Se resolvió asignar una carpeta individual a cada expediente en la que se almacenen los archivos de cada uno de sus componentes, así:

![estructura-archivos](https://github.com/cmvaronc/lectura-distante-tutelas/blob/master/estructura-archivos.png)
 
## Referencias
Biber, D. (1993). Representativeness in Corpus Design. *Literary and Linguistic Computing, 8*(4), 243–257. https://doi.org/10.1093/llc/8.4.243

