# Construcción de corpus para el análisis

## 1. Consecución de la información

La selección de tutelas por parte de la Corte Constitucional se efectúa sobre un cúmulo importante de sentencias de tutelas dictadas por los jueces en los juzgados y tribunales de todo el país. De acuerdo a la última estadística del Consejo Superior de la Judicatura llegan a la Corte mensualmente 40.000 expedientes al mes, de los cuales la mitad pueden ser radicados. No obstante, los fallos de la tutelas no pudieron obtenerse de la misma Corte Constitucional, que recibe todos los expedientes para su eventual revisión.

Así las cosas, para construir el corpus fue necesario acudir a las siguientes fuentes: 1), la *Gaceta* de la Corte Constitucional en físico (1992) para realizar una prueba a partir del análisis de las primeras 15 sentencias; 2), la relatoría de la Corte Constitucional para encontrar la base de datos que permitiera hacer el contraste con el corpus; 3), las secretarías de los Juzgados, en tanto puerta de entrada de las demandas de tutelas y, por ende, la fuente original a partir de la cual se produce el fallo que luego llega a la Corte; 4), las relatorías de los tres tribunales ―Superior de Bogotá, Contencioso Administrativo de Cundinamarca y Superior de Cundinamarca―; y v), dos tribunales fuera de Bogotá (Pereira y Medellín). 

Obtenida la información, se han encontrado las siguientes dificultades: 
* Los expedientes no son digitalizados por los juzgados. En consecuencia, la muestra que será objeto de análisis debe restringirse a los fallos, que sí se producen en formatos digitales. No obstante, aun estos constituyen un desafío puesto que, dada la ausencia de criterios unificados para producirlos, su naturaleza es variable: hasta el momento, se han encontrado documentos compuestos en 5 formatos distintos, algunos de los cuales no son editables. 
* Derivado de lo anterior, los textos originales de los expedientes en papel solo se encuentran en las secretarías de los juzgados. Ahora, si bien es posible, en teoría, buscar los fallos a través del Sistema Justicia Siglo XXI del Consejo Superior de la Judicatura, solo si se conociesen los datos de identificación del proceso y las partes sería posible recabar información, hecho que nos ha obligado a acudir directamente a las sedes judiciales para conseguirla. 
* Cada juzgado hace un manejo muy propio de la gestión documental: no se acata la Ley de Archivos (594 de 2000), existen distintas formas de registrar y almacenar la información, y no se cuenta con relatorías. Ha sido necesario, por tanto, acudir a contactos personales para obtener los fallos; en algunos casos, estos se obtuvieron mediante derecho de petición, mientras que en otros solo bastó acercarse a las secretarías con una unidad de almacenamiento masivo y firmar una planilla de control para acceder a los archivos. 
* Aun cuando la información de los fallos de tutela se encuentra en Internet y es de libre acceso, las búsquedas relativamente eficientes solamente operan para los fallos de la Corte Constitucional. En el caso de los tribunales, la información se encuentra en Boletines en PDF no editables.

## 2. Composición del corpus

### 2.1. Diseño de la muestra

Vista la envergadura del universo de información que se enfrenta en un ejercicio de investigación – creación como el propuesto, ha sido claro desde el inicio que el volumen de documentos que compondrían la muestra sería arbitrario. Así entonces, la representatividad de la muestra no estará dada por el valor numérico absoluto frente a la totalidad del universo de información, sino por la capacidad que esta tenga para reflejar las tendencias de uso de la lengua (de acuerdo con la conceptualización de Biber [1991]) que, a posterioridad, se evidenciarán a través del modelado de tópicos.

Nótese en este punto que la jurisprudencia emitida por la Corte Constitucional desde su creación (en 1991) asciende a 25.000 documentos, aproximadamente. Con esto, y para atender lo expresado en el párrafo anterior, se tomó la decisión de trabajar con el volumen total de información recabada en los archivos de los juzgados, que en este momento asciende a cerca de 8200 fallos de tutela, distribuidos en un periodo de 8 años (2010-2018). La muestra, entonces, ostenta hasta el momento una envergadura equivalente al 30 % del total de documentos que componen la jurisprudencia de la Corte. En este sentido, se aspira a conseguir fallos de años anteriores al periodo descrito en aras de enriquecer el análisis.

El hecho de que los fallos de tutela contengan secciones cuya construcción obedece a tipologías textuales disímiles (narrativa, descriptiva y argumentativa) hizo pensar, en principio, que los resultados del modelado de tópicos serían más precisos si estos se separaran en función de dichos componentes (*i. e.* consideraciones, hechos, pretensiones, decisiones). No obstante, la gran cantidad de archivos obtenidos hasta el momento excede la capacidad humana disponible para realizar dicha labor de segmentación (que debería realizarse manualmente, puesto que se trata  de texto no marcado). Se optó, en consecuencia, por realizar el análisis de todos los archivos de la muestra sin segmentarlos. 

### 2.2. Sistematización de la muestra

Tras haber establecido las características generales de la muestra, corresponde tomar decisiones respecto de la manera como se organizará el acervo de información para el análisis; a continuación, se describen con más detalle estos asuntos.

#### 2.2.1. Formato

El algoritmo que se empleará para construir el modelo de tópicos (Mallet) exige trabajar con archivos de texto plano y codificación Unicode (UTF-8). Ahora bien, dado el carácter desestructurado de la información de la muestra (archivos en formatos de texto enriquecido, en incluso de imagen), se ha hecho necesario buscar herramientas digitales que permitan convertirla de forma eficiente y confiable al formato requerido. En consecuencia, se decidió emplear para este menester la aplicación Textutil: se trata de un paquete de servicios para la conversión de archivos de texto que se ejecuta en la terminal del sistema operativo Mac OS X. Aparte de haber mostrado resultados satisfactorios en ejercicios preliminares (realizados con el corpus de prueba), se destaca de otras aplicaciones de su tipo en tanto permite convertir directorios completos [^1].  

#### 2.2.2. Gestión de archivos

Tomada la decisión de no separar los fallos por componentes, se estableció una nomenclatura para los archivos cuyo clasificador único ha de ser un número consecutivo asignado de forma automática al renombrar los archivos por volumen, así:

![nomenclatura-archivos](https://github.com/cmvaronc/lectura-distante-tutelas/blob/master/nomenclatura-archivos-v1.png)
 
La configuración de una estructura de carpetas para el almacenamiento de los archivos, por su parte, tampoco ha estado exenta de discusiones. Se resolvió dividir los archivos en carpetas por año, así:

![estructura-archivos](https://github.com/cmvaronc/lectura-distante-tutelas/blob/master/estructura-archivos.png)

## Notas

[^1]: Para el caso de los archivos dispuestos en formatos no editables, tales como PDF o TIF, será necesario recurrir a la tecnología de reconocimiento óptico de caracteres (OCR), tema que aun se encuentra en discusión.
 
## Referencias
Biber, D. (1993). Representativeness in Corpus Design. *Literary and Linguistic Computing, 8*(4), 243–257. https://doi.org/10.1093/llc/8.4.243

